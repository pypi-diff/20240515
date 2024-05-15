# Comparing `tmp/pydglab-0.2.0.tar.gz` & `tmp/pydglab-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydglab-0.2.0.tar", max compression
+gzip compressed data, was "pydglab-0.3.0.tar", max compression
```

## Comparing `pydglab-0.2.0.tar` & `pydglab-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35823 2024-05-10 07:01:10.429022 pydglab-0.2.0/LICENSE
--rw-r--r--   0        0        0      424 2024-05-11 16:46:11.750274 pydglab-0.2.0/pydglab/__init__.py
--rw-r--r--   0        0        0     3636 2024-05-11 16:49:38.159328 pydglab-0.2.0/pydglab/bthandler.py
--rw-r--r--   0        0        0     1224 2024-05-11 16:30:14.340564 pydglab-0.2.0/pydglab/model.py
--rw-r--r--   0        0        0    12188 2024-05-11 16:30:14.340564 pydglab-0.2.0/pydglab/service.py
--rw-r--r--   0        0        0     1176 2024-05-11 16:30:14.341563 pydglab-0.2.0/pydglab/uuid.py
--rw-r--r--   0        0        0      431 2024-05-11 16:53:16.930360 pydglab-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      633 2024-05-10 07:01:10.429022 pydglab-0.2.0/README.md
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 pydglab-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-05-10 07:01:10.429022 pydglab-0.3.0/LICENSE
+-rw-r--r--   0        0        0      420 2024-05-15 09:18:56.663975 pydglab-0.3.0/pydglab/__init__.py
+-rw-r--r--   0        0        0     3542 2024-05-15 20:11:54.267964 pydglab-0.3.0/pydglab/bthandler.py
+-rw-r--r--   0        0        0     1256 2024-05-15 09:18:56.664975 pydglab-0.3.0/pydglab/model.py
+-rw-r--r--   0        0        0    12397 2024-05-15 19:16:22.938779 pydglab-0.3.0/pydglab/service.py
+-rw-r--r--   0        0        0     1290 2024-05-15 08:07:06.030694 pydglab-0.3.0/pydglab/uuid.py
+-rw-r--r--   0        0        0      431 2024-05-15 20:11:33.689174 pydglab-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 2024-05-15 20:10:26.869349 pydglab-0.3.0/README.md
+-rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 pydglab-0.3.0/PKG-INFO
```

### Comparing `pydglab-0.2.0/LICENSE` & `pydglab-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydglab-0.2.0/pydglab/bthandler.py` & `pydglab-0.3.0/pydglab/bthandler.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,40 +41,66 @@
 async def get_batterylevel_(client: BleakClient, characteristics: CoyoteV2 | CoyoteV3):
     r = await client.read_gatt_char(characteristics.characteristicBattery)
     return r
 
 
 async def get_strength_(client: BleakClient, characteristics: CoyoteV2 | CoyoteV3):
     r = await client.read_gatt_char(characteristics.characteristicEStimPower)
+    # logger.debug(f"Received strenth bytes: {r.hex()} , which is {r}")
+    r.reverse()
     r = BitArray(r).bin
-    return int(r[-11:], 2) / 7, int(r[-22:-11], 2) / 7
+    # logger.debug(f"Received strenth bytes after decoding: {r}")
+    return int(r[-22:-11], 2) / 7, int(r[-11:], 2) / 7
 
 
-async def set_strength_(client: BleakClient, value: Coyote, characteristics: CoyoteV2 | CoyoteV3):
+async def set_strength_(
+    client: BleakClient, value: Coyote, characteristics: CoyoteV2 | CoyoteV3
+):
     # Create a byte array with the strength values.
     # The values are multiplied by 7 to convert them to the correct range.
-    binArray = '0b00'+'{0:011b}'.format(value.ChannelB.strength * 7)+'{0:011b}'.format(value.ChannelA.strength * 7)
-    array = bytearray(BitArray(bin=binArray).tobytes())
-    
-    r = await client.write_gatt_char(characteristics.characteristicEStimPower, array)
-    return value.ChannelB.strength * 7, value.ChannelA.strength * 7
-
-
-async def set_wave_(client: BleakClient, value: ChannelA | ChannelB, characteristics: CoyoteV2 | CoyoteV3):
+    strengthA = int(value.ChannelA.strength) * 7
+    strengthB = int(value.ChannelB.strength) * 7
+    if (
+        value.ChannelA.strength is None
+        or value.ChannelA.strength < 0
+        or value.ChannelA.strength > 2047
+    ):
+        value.ChannelA.strength = 0
+    if (
+        value.ChannelB.strength is None
+        or value.ChannelB.strength < 0
+        or value.ChannelB.strength > 2047
+    ):
+        value.ChannelB.strength = 0
+
+    array = ((strengthA << 11) + strengthB).to_bytes(3, byteorder="little")
+
+    # logger.debug(f"Sending bytes: {array.hex()} , which is {array}")
+
+    r = await client.write_gatt_char(
+        characteristics.characteristicEStimPower, bytearray(array), response=False
+    )
+    return value.ChannelA.strength, value.ChannelB.strength
+
+
+async def set_wave_(
+    client: BleakClient,
+    value: ChannelA | ChannelB,
+    characteristics: CoyoteV2 | CoyoteV3,
+):
     # Create a byte array with the wave values.
-    binArray = '0b0000'+'{0:05b}'.format(value.waveZ)+'{0:010b}'.format(value.waveY)+'{0:05b}'.format(value.waveX)
-    array = bytearray(BitArray(bin=binArray).tobytes())
-
-    r = await client.write_gatt_char(characteristics.characteristicEStimA if type(value) is ChannelA else characteristics.characteristicEStimB, array)
+    array = ((value.waveX << 15) + (value.waveY << 5) + value.waveX).to_bytes(
+        3, byteorder="little"
+    )
+
+    # logger.debug(f"Sending bytes: {array.hex()} , which is {array}")
+
+    r = await client.write_gatt_char(
+        (
+            characteristics.characteristicEStimA
+            if type(value) is ChannelA
+            else characteristics.characteristicEStimB
+        ),
+        bytearray(array),
+        response=False,
+    )
     return value.waveX, value.waveY, value.waveZ
-
-
-async def set_wave_sync_(client: BleakClient, value: Coyote, characteristics: CoyoteV2 | CoyoteV3):
-    # Create a byte array with the wave values.
-    binArrayA = '0b0000'+'{0:05b}'.format(value.ChannelA.waveZ)+'{0:010b}'.format(value.ChannelA.waveY)+'{0:05b}'.format(value.ChannelA.waveX)
-    arrayA = bytearray(BitArray(bin=binArrayA).tobytes())
-    
-    binArrayB = '0b0000'+'{0:05b}'.format(value.ChannelB.waveZ)+'{0:010b}'.format(value.ChannelB.waveY)+'{0:05b}'.format(value.ChannelB.waveX)
-    arrayB = bytearray(BitArray(bin=binArrayB).tobytes())
-    
-    r = await client.write_gatt_char(characteristics.characteristicEStimA, arrayA), await client.write_gatt_char(characteristics.characteristicEStimB, arrayB)
-    return (value.ChannelA.waveX, value.ChannelA.waveY, value.ChannelA.waveZ), (value.ChannelB.waveX, value.ChannelB.waveY, value.ChannelB.waveZ)
```

### Comparing `pydglab-0.2.0/pydglab/model.py` & `pydglab-0.3.0/pydglab/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 from typing import Optional
 
+
 class ChannelA(object):
     def __init__(self):
         self.strength: Optional[int] = None
         self.wave: Optional[bytearray[int]] = bytearray((0, 0, 0))
         self.waveX: Optional[int] = self.wave[0]
         self.waveY: Optional[int] = self.wave[1]
         self.waveZ: Optional[int] = self.wave[2]
 
+
 class ChannelB(object):
     def __init__(self):
         self.strength: Optional[int] = None
         self.wave: Optional[bytearray[int]] = bytearray((0, 0, 0))
         self.waveX: Optional[int] = self.wave[0]
         self.waveY: Optional[int] = self.wave[1]
         self.waveZ: Optional[int] = self.wave[2]
 
+
 class Coyote(object):
     def __init__(self):
         self.ChannelA: Optional[ChannelA] = ChannelA()
         self.ChannelB: Optional[ChannelB] = ChannelB()
         self.Battery: Optional[int] = None
 
 
 Wave_set = {
     "Going_Faster": [
-        (5,135,20),
-        (5,125,20),
-        (5,115,20),
-        (5,105,20),
-        (5,95,20),
-        (4,86,20),
-        (4,76,20),
-        (4,66,20),
-        (3,57,20),
-        (3,47,20),
-        (3,37,20),
-        (2,28,20),
-        (2,18,20),
-        (1,14,20),
-        (1,9,20),
+        (5, 135, 20),
+        (5, 125, 20),
+        (5, 115, 20),
+        (5, 105, 20),
+        (5, 95, 20),
+        (4, 86, 20),
+        (4, 76, 20),
+        (4, 66, 20),
+        (3, 57, 20),
+        (3, 47, 20),
+        (3, 37, 20),
+        (2, 28, 20),
+        (2, 18, 20),
+        (1, 14, 20),
+        (1, 9, 20),
     ],
-    
-}
+}
```

### Comparing `pydglab-0.2.0/pydglab/service.py` & `pydglab-0.3.0/pydglab/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,157 +3,162 @@
 from typing import Tuple
 from pydglab.model import *
 from pydglab.uuid import *
 from pydglab.bthandler import *
 
 logger = logging.getLogger(__name__)
 
+
 class dglab(object):
     coyote = Coyote()
 
     def __init__(self, address: str = None) -> None:
         self.address = address
         return None
 
-
-    async def create(self) -> 'dglab':
+    async def create(self) -> "dglab":
         """
         建立郊狼连接并初始化。
         Creates a connection to the DGLAB device and initialize.
 
         Returns:
             dglab: The initialized DGLAB object.
 
         Raises:
             Exception: If the device is not supported or if an unknown device is connected.
         """
-        
-        if self.address is None: 
+
+        if self.address is None:
             # If address is not provided, scan for it.
             self.address = await scan_()
-        
+
         # Connect to the device.
         logger.debug(f"Connecting to {self.address}")
         self.client = BleakClient(self.address, timeout=20.0)
         await self.client.connect()
-        
+
         # Wait for a second to allow service discovery to complete
         await asyncio.sleep(1)
-        
+
         # Check if the device is valid.
         services = self.client.services
         service = [service.uuid for service in services]
         logger.debug(f"Got services: {str(service)}")
         if CoyoteV2.serviceBattery in service and CoyoteV2.serviceEStim in service:
             logger.info("Connected to DGLAB v2.0")
-            
+
             # Update BleakGATTCharacteristic into characteristics list, to optimize performence.
             self.characteristics = CoyoteV2
             logger.debug(f"Got characteristics: {str(self.characteristics)}")
             for i in self.client.services.characteristics.values():
                 if i.uuid == self.characteristics.characteristicBattery:
                     self.characteristics.characteristicBattery = i
                 elif i.uuid == self.characteristics.characteristicEStimPower:
                     self.characteristics.characteristicEStimPower = i
                 elif i.uuid == self.characteristics.characteristicEStimA:
                     self.characteristics.characteristicEStimA = i
                 elif i.uuid == self.characteristics.characteristicEStimB:
                     self.characteristics.characteristicEStimB = i
-            
+
         elif CoyoteV3.serviceWrite in service and CoyoteV3.serviceNotify in service:
             raise Exception("DGLAB v3.0 is not supported")
         else:
-            raise Exception("Unknown device (你自己看看你连的是什么jb设备)") # Sorry for my language.
-        
+            raise Exception(
+                "Unknown device (你自己看看你连的是什么jb设备)"
+            )  # Sorry for my language.
+
         self.channelA_wave_set: list[tuple[int, int, int]] = []
         self.channelB_wave_set: list[tuple[int, int, int]] = []
-        
+
         # Initialize self.coyote
         await self.get_batterylevel()
         await self.get_strength()
-        
+
         await self.set_wave_sync(0, 0, 0, 0, 0, 0)
         await self.set_strength(0, 0)
-        
+
         # Start the wave tasks, to keep the device functioning.
-        self.wave_tasks = asyncio.gather(self._keep_wave(), self._channelA_wave_set_handler(), self._channelB_wave_set_handler())
-        
-        return self
+        self.wave_tasks = asyncio.gather(
+            self._keep_wave(),
+            self._channelA_wave_set_handler(),
+            self._channelB_wave_set_handler(),
+        )
 
+        return self
 
     @classmethod
-    async def from_address(cls, address: str) -> 'dglab':
+    async def from_address(cls, address: str) -> "dglab":
         """
         从指定的地址创建一个新的郊狼实例，在需要同时连接多个设备时格外好用。
         Creates a new instance of the 'dglab' class using the specified address.
 
         Args:
             address (str): The address to connect to.
 
         Returns:
             dglab: An instance of the 'dglab' class.
 
         """
-        
-        return cls(address)
 
+        return cls(address)
 
     async def get_batterylevel(self) -> int:
         """
         读取郊狼设备剩余电量，小心没电导致的寸止哦：）
         Retrieves the battery level from the device.
 
         Returns:
             int: The battery level as an integer value.
         """
-        
+
         value = await get_batterylevel_(self.client, self.characteristics)
         value = value[0]
         logger.debug(f"Received battery level: {value}")
         self.coyote.Battery = int(value)
         return self.coyote.Battery
 
-
     async def get_strength(self) -> Tuple[int, int]:
         """
         读取郊狼当前强度。
         Retrieves the strength of the device.
 
         Returns:
             Tuple[int, int]: 通道A强度，通道B强度
         """
         value = await get_strength_(self.client, self.characteristics)
         logger.debug(f"Received strength: A: {value[0]}, B: {value[1]}")
         self.coyote.ChannelA.strength = int(value[0])
         self.coyote.ChannelB.strength = int(value[1])
         return self.coyote.ChannelA.strength, self.coyote.ChannelB.strength
 
-
     async def set_strength(self, strength: int, channel: ChannelA | ChannelB) -> None:
         """
         设置电压强度。
         额外设置这个函数用于单独调整强度只是为了和设置波形的函数保持一致罢了。
         Set the strength of the device.
 
         Args:
             strength (int): 电压强度
             channel (ChannelA | ChannelB): 对手频道
 
         Returns:
             int: 电压强度
         """
-        
+
         if channel is ChannelA:
             self.coyote.ChannelA.strength = strength
         elif channel is ChannelB:
             self.coyote.ChannelB.strength = strength
         r = await set_strength_(self.client, self.coyote, self.characteristics)
         logger.debug(f"Set strength response: {r}")
-        return self.coyote.ChannelA.strength if channel is ChannelA else self.coyote.ChannelB.strength
-
+        return (
+            self.coyote.ChannelA.strength
+            if channel is ChannelA
+            else self.coyote.ChannelB.strength
+        )
 
     async def set_strength_sync(self, strengthA: int, strengthB: int) -> None:
         """
         同步设置电流强度。
         这是正道。
         Set the strength of the device synchronously.
 
@@ -166,25 +171,25 @@
         """
         self.coyote.ChannelA.strength = strengthA
         self.coyote.ChannelB.strength = strengthB
         r = await set_strength_(self.client, self.coyote, self.characteristics)
         logger.debug(f"Set strength response: {r}")
         return self.coyote.ChannelA.strength, self.coyote.ChannelB.strength
 
-
     """
     How wave set works:
     1. Set the wave set for channel A and channel B.
     2. The wave set will be looped indefinitely by
     wave_set_handler, and change the value in 
     self.coyote.ChannelN.waveN.
     """
 
-
-    async def set_wave_set(self, wave_set: list[tuple[int, int, int]], channel: ChannelA | ChannelB) -> None:
+    async def set_wave_set(
+        self, wave_set: list[tuple[int, int, int]], channel: ChannelA | ChannelB
+    ) -> None:
         """
         设置波形组，也就是所谓“不断变化的波形”。
         Set the wave set for the device.
 
         Args:
             wave_set (list[tuple[int, int, int]]): 波形组
             channel (ChannelA | ChannelB): 对手通道
@@ -194,16 +199,19 @@
         """
         if channel is ChannelA:
             self.channelA_wave_set = wave_set
         elif channel is ChannelB:
             self.channelB_wave_set = wave_set
         return None
 
-
-    async def set_wave_set_sync(self, wave_setA: list[tuple[int, int, int]], wave_setB: list[tuple[int, int, int]]) -> None:
+    async def set_wave_set_sync(
+        self,
+        wave_setA: list[tuple[int, int, int]],
+        wave_setB: list[tuple[int, int, int]],
+    ) -> None:
         """
         同步设置波形组。
         Set the wave set for the device synchronously.
 
         Args:
             wave_setA (list[tuple[int, int, int]]): 通道A波形组
             wave_setB (list[tuple[int, int, int]]): 通道B波形组
@@ -211,60 +219,58 @@
         Returns:
             None: None
         """
         self.channelA_wave_set = wave_setA
         self.channelB_wave_set = wave_setB
         return None
 
-
     async def _channelA_wave_set_handler(self) -> None:
         """
         Do not use this function directly.
-        
+
         Yep this is how wave set works :)
         PR if you have a better solution.
         """
         try:
             while True:
                 for wave in self.channelA_wave_set:
                     self.coyote.ChannelA.waveX = wave[0]
                     self.coyote.ChannelA.waveY = wave[1]
                     self.coyote.ChannelA.waveZ = wave[2]
                     await asyncio.sleep(0.1)
         except asyncio.exceptions.CancelledError:
             pass
 
-
     async def _channelB_wave_set_handler(self) -> None:
         """
         Do not use this function directly.
-        
+
         Yep this is how wave set works :)
         PR if you have a better solution.
         """
         try:
             while True:
                 for wave in self.channelB_wave_set:
                     self.coyote.ChannelB.waveX = wave[0]
                     self.coyote.ChannelB.waveY = wave[1]
                     self.coyote.ChannelB.waveZ = wave[2]
                     await asyncio.sleep(0.1)
         except asyncio.exceptions.CancelledError:
             pass
 
-
     """
     How set_wave works:
     Basically, it will generate a wave set with only one wave,
     and changes the value in self.hannelN_wave_set.
     All the wave changes will be applied to the device by wave_set.
     """
 
-
-    async def set_wave(self, waveX: int, waveY: int, waveZ: int, channel: ChannelA | ChannelB) -> Tuple[int, int, int]:
+    async def set_wave(
+        self, waveX: int, waveY: int, waveZ: int, channel: ChannelA | ChannelB
+    ) -> Tuple[int, int, int]:
         """
         设置波形。
         枯燥，乏味，感觉不如。。。
         Set the wave for the device.
 
         Args:
             waveX (int): 连续发出X个脉冲，每个脉冲持续1ms
@@ -277,20 +283,27 @@
         """
         if channel is ChannelA:
             self.channelA_wave_set = [(waveX, waveY, waveZ)]
         elif channel is ChannelB:
             self.channelB_wave_set = [(waveX, waveY, waveZ)]
         return waveX, waveY, waveZ
 
-
-    async def set_wave_sync(self, waveX_A: int, waveY_A: int, waveZ_A: int, waveX_B: int, waveY_B: int, waveZ_B: int) -> Tuple[int, int, int, int, int, int]:
+    async def set_wave_sync(
+        self,
+        waveX_A: int,
+        waveY_A: int,
+        waveZ_A: int,
+        waveX_B: int,
+        waveY_B: int,
+        waveZ_B: int,
+    ) -> Tuple[int, int, int, int, int, int]:
         """
         同步设置波形。
         Set the wave for the device synchronously.
-        
+
         Args:
             waveX_A (int): 通道A，连续发出X个脉冲，每个脉冲持续1ms
             waveY_A (int): 通道A，发出脉冲后停止Y个周期，每个周期持续1ms
             waveZ_A (int): 通道A，每个脉冲的宽度为Z
             waveX_B (int): 通道B，连续发出X个脉冲，每个脉冲持续1ms
             waveY_B (int): 通道B，发出脉冲后停止Y个周期，每个周期持续1ms
             waveZ_B (int): 通道B，每个脉冲的宽度为Z
@@ -298,29 +311,29 @@
         Returns:
             Tuple[Tuple[int, int, int], Tuple[int, int, int]]: A通道波形，B通道波形
         """
         self.channelA_wave_set = [(waveX_A, waveY_A, waveZ_A)]
         self.channelB_wave_set = [(waveX_B, waveY_B, waveZ_B)]
         return (waveX_A, waveY_A, waveZ_A), (waveX_B, waveY_B, waveZ_B)
 
-
     async def _keep_wave(self) -> None:
         """
         Don't use this function directly.
         """
         while True:
-            r = await set_wave_sync_(self.client, self.coyote, self.characteristics)
+            r = await set_wave_(
+                self.client, self.coyote.ChannelA, self.characteristics
+            ), await set_wave_(self.client, self.coyote.ChannelB, self.characteristics)
             logger.debug(f"Set wave response: {r}")
             try:
                 await asyncio.sleep(0.1)
             except asyncio.exceptions.CancelledError:
                 break
         return None
 
-
     async def close(self):
         """
         郊狼虽好，可不要贪杯哦。
         Close the connection to the device.
 
         Returns:
             None: None
```

### Comparing `pydglab-0.2.0/pydglab/uuid.py` & `pydglab-0.3.0/pydglab/uuid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 # This file contains the UUIDs for the D-LAB ESTIM01 device
 
 from typing import Union
 from bleak import BleakGATTCharacteristic
 
+
 class CoyoteV2(object):
     name: str = "D-LAB ESTIM01"
     serviceBattery: str = "955a180a-0fe2-f5aa-a094-84b8d4f3e8ad"
-    characteristicBattery: Union[str, BleakGATTCharacteristic] = "955a1500-0fe2-f5aa-a094-84b8d4f3e8ad"
+    characteristicBattery: Union[str, BleakGATTCharacteristic] = (
+        "955a1500-0fe2-f5aa-a094-84b8d4f3e8ad"
+    )
     serviceEStim: str = "955a180b-0fe2-f5aa-a094-84b8d4f3e8ad"
-    characteristicEStimPower: Union[str, BleakGATTCharacteristic] = "955a1504-0fe2-f5aa-a094-84b8d4f3e8ad"
-    characteristicEStimA: Union[str, BleakGATTCharacteristic] = "955a1505-0fe2-f5aa-a094-84b8d4f3e8ad"
-    characteristicEStimB: Union[str, BleakGATTCharacteristic] = "955a1506-0fe2-f5aa-a094-84b8d4f3e8ad"
+    characteristicEStimPower: Union[str, BleakGATTCharacteristic] = (
+        "955a1504-0fe2-f5aa-a094-84b8d4f3e8ad"
+    )
+    characteristicEStimA: Union[str, BleakGATTCharacteristic] = (
+        "955a1505-0fe2-f5aa-a094-84b8d4f3e8ad"
+    )
+    characteristicEStimB: Union[str, BleakGATTCharacteristic] = (
+        "955a1506-0fe2-f5aa-a094-84b8d4f3e8ad"
+    )
+
 
 class CoyoteV3(object):
     name: str = "47L121000"
     wirelessSensorName: str = "47L120100"
     serviceWrite: str = "0000180c-0000-1000-8000-00805f9b34fb"
     serviceNotify: str = "0000180c-0000-1000-8000-00805f9b34fb"
-    characteristicWrite: Union[str, BleakGATTCharacteristic] = "0000150A-0000-1000-8000-00805f9b34fb"
-    characteristicNotify: Union[str, BleakGATTCharacteristic] = "0000150B-0000-1000-8000-00805f9b34fb"
+    characteristicWrite: Union[str, BleakGATTCharacteristic] = (
+        "0000150A-0000-1000-8000-00805f9b34fb"
+    )
+    characteristicNotify: Union[str, BleakGATTCharacteristic] = (
+        "0000150B-0000-1000-8000-00805f9b34fb"
+    )
```

