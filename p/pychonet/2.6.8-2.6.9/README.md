# Comparing `tmp/pychonet-2.6.8.tar.gz` & `tmp/pychonet-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pychonet-2.6.8.tar", last modified: Fri Mar 22 12:37:43 2024, max compression
+gzip compressed data, was "dist/pychonet-2.6.9.tar", last modified: Wed May 15 10:52:26 2024, max compression
```

## Comparing `pychonet-2.6.8.tar` & `pychonet-2.6.9.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2024-03-22 12:37:43.841785 pychonet-2.6.8/
--rw-r--r--   0 vaio       (500) vaio       (500)     5404 2024-03-22 12:24:57.000000 pychonet-2.6.8/CHANGES.txt
--rw-r--r--   0 vaio       (500) vaio       (500)    34494 2024-01-24 04:56:31.000000 pychonet-2.6.8/LICENSE-GPL
--rw-r--r--   0 vaio       (500) vaio       (500)     1075 2024-01-24 04:56:31.000000 pychonet-2.6.8/LICENSE-MIT
--rw-r--r--   0 vaio       (500) vaio       (500)       56 2024-01-24 04:56:31.000000 pychonet-2.6.8/MANIFEST.in
--rw-r--r--   0 vaio       (500) vaio       (500)     6284 2024-03-22 12:37:43.841785 pychonet-2.6.8/PKG-INFO
--rw-r--r--   0 vaio       (500) vaio       (500)     5913 2024-01-24 04:56:31.000000 pychonet-2.6.8/README.md
-drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2024-03-22 12:37:43.838785 pychonet-2.6.8/pychonet/
--rwxr--r--   0 vaio       (500) vaio       (500)      179 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/AutomaticEntranceDoor.py
--rwxr--r--   0 vaio       (500) vaio       (500)     4297 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/CeilingFan.py
--rwxr--r--   0 vaio       (500) vaio       (500)     6488 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/DistributionPanelMeter.py
--rwxr--r--   0 vaio       (500) vaio       (500)    10830 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/EchonetInstance.py
--rw-r--r--   0 vaio       (500) vaio       (500)     3553 2024-03-22 12:20:40.000000 pychonet-2.6.8/pychonet/ElectricBlind.py
--rwxr--r--   0 vaio       (500) vaio       (500)      153 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricCurtain.py
--rwxr--r--   0 vaio       (500) vaio       (500)      702 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricEnergyMeter.py
--rwxr--r--   0 vaio       (500) vaio       (500)      147 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricGate.py
--rwxr--r--   0 vaio       (500) vaio       (500)     2916 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricHeater.py
--rwxr--r--   0 vaio       (500) vaio       (500)     2379 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricLock.py
--rwxr--r--   0 vaio       (500) vaio       (500)      179 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricRainSlidingDoor.py
--rwxr--r--   0 vaio       (500) vaio       (500)      153 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricShutter.py
--rwxr--r--   0 vaio       (500) vaio       (500)     6938 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricStorageHeater.py
--rwxr--r--   0 vaio       (500) vaio       (500)      471 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricVehicleCharger.py
--rwxr--r--   0 vaio       (500) vaio       (500)     8215 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricWaterHeater.py
--rwxr--r--   0 vaio       (500) vaio       (500)      157 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/ElectricWindow.py
--rwxr--r--   0 vaio       (500) vaio       (500)     4076 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/FanHeater.py
--rwxr--r--   0 vaio       (500) vaio       (500)     2485 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/FloorHeater.py
--rwxr--r--   0 vaio       (500) vaio       (500)     2694 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/FuelCell.py
--rwxr--r--   0 vaio       (500) vaio       (500)      733 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/GasMeter.py
--rwxr--r--   0 vaio       (500) vaio       (500)     3290 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/GeneralLighting.py
--rwxr--r--   0 vaio       (500) vaio       (500)     3347 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/HomeAirCleaner.py
--rwxr--r--   0 vaio       (500) vaio       (500)    14221 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/HomeAirConditioner.py
--rwxr--r--   0 vaio       (500) vaio       (500)     2262 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/HomeSolarPower.py
--rwxr--r--   0 vaio       (500) vaio       (500)     4836 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/HotWaterGenerator.py
--rwxr--r--   0 vaio       (500) vaio       (500)     3356 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/HybridWaterHeater.py
--rwxr--r--   0 vaio       (500) vaio       (500)      650 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/LightingSystem.py
--rwxr--r--   0 vaio       (500) vaio       (500)     6107 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/LowVoltageSmartElectricEnergyMeter.py
--rwxr--r--   0 vaio       (500) vaio       (500)     2796 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/RiceCooker.py
--rwxr--r--   0 vaio       (500) vaio       (500)     1121 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/SingleFunctionLighting.py
--rwxr--r--   0 vaio       (500) vaio       (500)     8072 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/StorageBattery.py
--rwxr--r--   0 vaio       (500) vaio       (500)      599 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/TemperatureSensor.py
--rwxr--r--   0 vaio       (500) vaio       (500)     2821 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/WaterFlowMeter.py
--rwxr--r--   0 vaio       (500) vaio       (500)     3206 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/__init__.py
--rwxr--r--   0 vaio       (500) vaio       (500)    17675 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/echonetapiclient.py
-drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2024-03-22 12:37:43.840785 pychonet-2.6.8/pychonet/lib/
--rwxr--r--   0 vaio       (500) vaio       (500)        0 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/lib/__init__.py
--rwxr--r--   0 vaio       (500) vaio       (500)    11153 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/lib/const.py
--rwxr--r--   0 vaio       (500) vaio       (500)     8031 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/lib/eojx.py
--rwxr--r--   0 vaio       (500) vaio       (500)    70266 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/lib/epc.py
--rw-r--r--   0 vaio       (500) vaio       (500)     4776 2024-03-22 12:20:40.000000 pychonet-2.6.8/pychonet/lib/epc_functions.py
--rwxr--r--   0 vaio       (500) vaio       (500)     3686 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/lib/functions.py
--rwxr--r--   0 vaio       (500) vaio       (500)     4865 2024-03-19 15:13:04.000000 pychonet-2.6.8/pychonet/lib/udpserver.py
--rw-r--r--   0 vaio       (500) vaio       (500)       80 2024-03-22 12:31:38.000000 pychonet-2.6.8/pychonet/version.py
-drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2024-03-22 12:37:43.841785 pychonet-2.6.8/pychonet.egg-info/
--rw-r--r--   0 vaio       (500) vaio       (500)     6284 2024-03-22 12:37:43.000000 pychonet-2.6.8/pychonet.egg-info/PKG-INFO
--rw-r--r--   0 vaio       (500) vaio       (500)     1427 2024-03-22 12:37:43.000000 pychonet-2.6.8/pychonet.egg-info/SOURCES.txt
--rw-r--r--   0 vaio       (500) vaio       (500)        1 2024-03-22 12:37:43.000000 pychonet-2.6.8/pychonet.egg-info/dependency_links.txt
--rw-r--r--   0 vaio       (500) vaio       (500)       11 2024-03-22 12:37:43.000000 pychonet-2.6.8/pychonet.egg-info/requires.txt
--rw-r--r--   0 vaio       (500) vaio       (500)        9 2024-03-22 12:37:43.000000 pychonet-2.6.8/pychonet.egg-info/top_level.txt
--rw-r--r--   0 vaio       (500) vaio       (500)      265 2024-03-22 12:37:43.843785 pychonet-2.6.8/setup.cfg
--rw-r--r--   0 vaio       (500) vaio       (500)      662 2024-02-12 14:35:16.000000 pychonet-2.6.8/setup.py
+drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2024-05-15 10:52:26.495545 pychonet-2.6.9/
+-rwxr--r--   0 vaio       (500) vaio       (500)     5461 2024-05-15 10:46:29.000000 pychonet-2.6.9/CHANGES.txt
+-rw-r--r--   0 vaio       (500) vaio       (500)    34494 2024-01-24 04:56:31.000000 pychonet-2.6.9/LICENSE-GPL
+-rw-r--r--   0 vaio       (500) vaio       (500)     1075 2024-01-24 04:56:31.000000 pychonet-2.6.9/LICENSE-MIT
+-rw-r--r--   0 vaio       (500) vaio       (500)       56 2024-01-24 04:56:31.000000 pychonet-2.6.9/MANIFEST.in
+-rw-r--r--   0 vaio       (500) vaio       (500)     6284 2024-05-15 10:52:26.495545 pychonet-2.6.9/PKG-INFO
+-rw-r--r--   0 vaio       (500) vaio       (500)     5913 2024-01-24 04:56:31.000000 pychonet-2.6.9/README.md
+drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2024-05-15 10:52:26.492545 pychonet-2.6.9/pychonet/
+-rwxr--r--   0 vaio       (500) vaio       (500)      179 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/AutomaticEntranceDoor.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     4297 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/CeilingFan.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     6488 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/DistributionPanelMeter.py
+-rwxr--r--   0 vaio       (500) vaio       (500)    10830 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/EchonetInstance.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     3553 2024-03-22 12:20:40.000000 pychonet-2.6.9/pychonet/ElectricBlind.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      153 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricCurtain.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      702 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricEnergyMeter.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      147 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricGate.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     2916 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricHeater.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     2379 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricLock.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      179 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricRainSlidingDoor.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      153 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricShutter.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     6938 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricStorageHeater.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      471 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricVehicleCharger.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     8215 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricWaterHeater.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      157 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/ElectricWindow.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     4076 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/FanHeater.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     2485 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/FloorHeater.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     2694 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/FuelCell.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      733 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/GasMeter.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     3290 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/GeneralLighting.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     3347 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/HomeAirCleaner.py
+-rwxr--r--   0 vaio       (500) vaio       (500)    14221 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/HomeAirConditioner.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     2262 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/HomeSolarPower.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     4836 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/HotWaterGenerator.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     3356 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/HybridWaterHeater.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      650 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/LightingSystem.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     6107 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/LowVoltageSmartElectricEnergyMeter.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     4689 2024-05-14 08:24:39.000000 pychonet-2.6.9/pychonet/Refrigerator.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     2796 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/RiceCooker.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     1121 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/SingleFunctionLighting.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     8072 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/StorageBattery.py
+-rwxr--r--   0 vaio       (500) vaio       (500)      599 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/TemperatureSensor.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     2821 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/WaterFlowMeter.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     3285 2024-05-12 11:48:44.000000 pychonet-2.6.9/pychonet/__init__.py
+-rwxr--r--   0 vaio       (500) vaio       (500)    17675 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/echonetapiclient.py
+drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2024-05-15 10:52:26.495545 pychonet-2.6.9/pychonet/lib/
+-rwxr--r--   0 vaio       (500) vaio       (500)        0 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/lib/__init__.py
+-rwxr--r--   0 vaio       (500) vaio       (500)    11153 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/lib/const.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     8031 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/lib/eojx.py
+-rwxr--r--   0 vaio       (500) vaio       (500)    70266 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/lib/epc.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     5052 2024-05-14 08:24:39.000000 pychonet-2.6.9/pychonet/lib/epc_functions.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     3686 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/lib/functions.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     4865 2024-03-19 15:13:04.000000 pychonet-2.6.9/pychonet/lib/udpserver.py
+-rwxr--r--   0 vaio       (500) vaio       (500)       80 2024-05-15 10:47:22.000000 pychonet-2.6.9/pychonet/version.py
+drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2024-05-15 10:52:26.495545 pychonet-2.6.9/pychonet.egg-info/
+-rw-r--r--   0 vaio       (500) vaio       (500)     6284 2024-05-15 10:52:26.000000 pychonet-2.6.9/pychonet.egg-info/PKG-INFO
+-rw-r--r--   0 vaio       (500) vaio       (500)     1452 2024-05-15 10:52:26.000000 pychonet-2.6.9/pychonet.egg-info/SOURCES.txt
+-rw-r--r--   0 vaio       (500) vaio       (500)        1 2024-05-15 10:52:26.000000 pychonet-2.6.9/pychonet.egg-info/dependency_links.txt
+-rw-r--r--   0 vaio       (500) vaio       (500)       11 2024-05-15 10:52:26.000000 pychonet-2.6.9/pychonet.egg-info/requires.txt
+-rw-r--r--   0 vaio       (500) vaio       (500)        9 2024-05-15 10:52:26.000000 pychonet-2.6.9/pychonet.egg-info/top_level.txt
+-rw-r--r--   0 vaio       (500) vaio       (500)      265 2024-05-15 10:52:26.496545 pychonet-2.6.9/setup.cfg
+-rw-r--r--   0 vaio       (500) vaio       (500)      662 2024-02-12 14:35:16.000000 pychonet-2.6.9/setup.py
```

### Comparing `pychonet-2.6.8/CHANGES.txt` & `pychonet-2.6.9/CHANGES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,7 +67,8 @@
                     -- Complement EPC_CODE of Electric water heater
 v2.6.5, 19 Feb 2024 -- Fix syntax error in ElectricWaterHeater _026BCC()
 v2.6.6, 23 Feb 2024 -- Add 0x97: _hh_mm to EPC_SUPER_FUNCTIONS
                     -- Don't call update callback functions in discover()
                     -- Property value in the EPC_SUPER_FUNCTIONS constant
 v2.6.7, 19 Mar 2024 -- Eliminate the possibility of communication loss
 V2.6.8, 22 Mar 2024 -- Maintenance of ElectricBlind Class
+V2.6.9, 15 May 2024 -- Supports Refrigerator (0x03-0xB7)
```

### Comparing `pychonet-2.6.8/LICENSE-GPL` & `pychonet-2.6.9/LICENSE-GPL`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/LICENSE-MIT` & `pychonet-2.6.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/PKG-INFO` & `pychonet-2.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychonet
-Version: 2.6.8
+Version: 2.6.9
 Summary: A library for interfacing via the ECHONETlite protocol.
 Home-page: http://pypi.python.org/pypi/pychonet/
 Author: Scott Phillips
 Author-email: scotty.phillips@hotmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE-GPL
```

### Comparing `pychonet-2.6.8/README.md` & `pychonet-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/CeilingFan.py` & `pychonet-2.6.9/pychonet/CeilingFan.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/DistributionPanelMeter.py` & `pychonet-2.6.9/pychonet/DistributionPanelMeter.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/EchonetInstance.py` & `pychonet-2.6.9/pychonet/EchonetInstance.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/ElectricBlind.py` & `pychonet-2.6.9/pychonet/ElectricBlind.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/ElectricEnergyMeter.py` & `pychonet-2.6.9/pychonet/ElectricEnergyMeter.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/ElectricHeater.py` & `pychonet-2.6.9/pychonet/ElectricHeater.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/ElectricLock.py` & `pychonet-2.6.9/pychonet/ElectricLock.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/ElectricStorageHeater.py` & `pychonet-2.6.9/pychonet/ElectricStorageHeater.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/ElectricWaterHeater.py` & `pychonet-2.6.9/pychonet/ElectricWaterHeater.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/FanHeater.py` & `pychonet-2.6.9/pychonet/FanHeater.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/FloorHeater.py` & `pychonet-2.6.9/pychonet/FloorHeater.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/FuelCell.py` & `pychonet-2.6.9/pychonet/FuelCell.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/GasMeter.py` & `pychonet-2.6.9/pychonet/GasMeter.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/GeneralLighting.py` & `pychonet-2.6.9/pychonet/GeneralLighting.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/HomeAirCleaner.py` & `pychonet-2.6.9/pychonet/HomeAirCleaner.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/HomeAirConditioner.py` & `pychonet-2.6.9/pychonet/HomeAirConditioner.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/HomeSolarPower.py` & `pychonet-2.6.9/pychonet/HomeSolarPower.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/HotWaterGenerator.py` & `pychonet-2.6.9/pychonet/HotWaterGenerator.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/HybridWaterHeater.py` & `pychonet-2.6.9/pychonet/HybridWaterHeater.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/LightingSystem.py` & `pychonet-2.6.9/pychonet/LightingSystem.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/LowVoltageSmartElectricEnergyMeter.py` & `pychonet-2.6.9/pychonet/LowVoltageSmartElectricEnergyMeter.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/RiceCooker.py` & `pychonet-2.6.9/pychonet/RiceCooker.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/SingleFunctionLighting.py` & `pychonet-2.6.9/pychonet/SingleFunctionLighting.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/StorageBattery.py` & `pychonet-2.6.9/pychonet/StorageBattery.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/TemperatureSensor.py` & `pychonet-2.6.9/pychonet/TemperatureSensor.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/WaterFlowMeter.py` & `pychonet-2.6.9/pychonet/WaterFlowMeter.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/__init__.py` & `pychonet-2.6.9/pychonet/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .FloorHeater import FloorHeater
 from .FuelCell import FuelCell
 from .GasMeter import GasMeter
 from .ElectricEnergyMeter import ElectricEnergyMeter
 from .WaterFlowMeter import WaterFlowMeter
 from .CeilingFan import CeilingFan
 from .ElectricWaterHeater import ElectricWaterHeater
+from .Refrigerator import Refrigerator
 
 
 def Factory(host, server, eojgc, eojcc, eojci=0x01):
     instance = None
     if eojgc in EOJX_CLASS:
         if eojcc in EOJX_CLASS[eojgc]:
             instance = f"{eojgc}-{eojcc}"
@@ -65,14 +66,15 @@
         f"{0x02}-{0x82}": GasMeter,
         f"{0x02}-{0x87}": DistributionPanelMeter,
         f"{0x02}-{0x88}": LowVoltageSmartElectricEnergyMeter,
         f"{0x02}-{0x90}": GeneralLighting,
         f"{0x02}-{0x91}": SingleFunctionLighting,
         f"{0x02}-{0xA3}": LightingSystem,
         f"{0x02}-{0xA6}": HybridWaterHeater,
+        f"{0x03}-{0xB7}": Refrigerator,
         None: None,
     }
     instance_object = instances.get(instance, None)
     if instance_object is not None:
         return instance_object(host, server, eojci)
 
     return EchonetInstance(host, eojgc, eojcc, eojci, server)
```

### Comparing `pychonet-2.6.8/pychonet/echonetapiclient.py` & `pychonet-2.6.9/pychonet/echonetapiclient.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/lib/const.py` & `pychonet-2.6.9/pychonet/lib/const.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/lib/eojx.py` & `pychonet-2.6.9/pychonet/lib/eojx.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/lib/epc.py` & `pychonet-2.6.9/pychonet/lib/epc.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/lib/epc_functions.py` & `pychonet-2.6.9/pychonet/lib/epc_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 DICT_41_AUTO_NONAUTO = {0x41: "auto", 0x42: "non-auto"}
 DICT_41_UNLOCK_LOCK = {0x42: DATA_STATE_UNLOCK, 0x41: DATA_STATE_LOCK}
 DICT_41_OPEN_CLOSED = {0x41: DATA_STATE_OPEN, 0x42: DATA_STATE_CLOSE}
 DICT_41_ENABLED_DISABLED = {0x41: "enabled", 0x42: "disabled"}
 DICT_41_AVAILABLE_NOT_AVAILABLE = {0x41: "available", 0x42: "not available"}
 DICT_41_HEATING_NOT_HEATING = {0x41: "heating", 0x42: "not heating"}
 DICT_41_PERMITTED_PROHIBITED = {0x41: "permitted", 0x42: "prohibited"}
+DICT_41_EMPTY_OR_NOT = {0x41: "not empty", 0x42: "empty"}
 DICT_30_TRUE_FALSE = {0x30: True, 0x31: False}
 DICT_30_ON_OFF = {0x30: DATA_STATE_ON, 0x31: DATA_STATE_OFF}
 DICT_30_OPEN_CLOSED = {0x30: DATA_STATE_OPEN, 0x31: DATA_STATE_CLOSE}
 
 # Like select type
 DICT_41_AUTO_8_SPEEDS = {
     0x41: "auto",
@@ -42,14 +43,26 @@
 
 DICT_41_LOW_MID_HIGH = {
     0x41: "low",
     0x42: "medium",
     0x43: "high",
 }
 
+DICT_41_NORMAL_QUICK_STANDBY = {
+    0x41: "normal",
+    0x42: "quick",
+    0x43: "standby",
+}
+
+DICT_41_ENABLED_DISABLED_TEMPDISABLED = {
+    0x41: "enabled",
+    0x42: "disabled",
+    0x43: "temporarily_disabled",
+}
+
 
 def _swap_dict(d: dict):
     return {v: k for k, v in d.items()}
 
 
 # ------------ EPC GENERIC FUNCTIONS -------
 def _int(edt, values: dict = {}, non_value: Any = "Invalid setting"):  # unsigned int
```

### Comparing `pychonet-2.6.8/pychonet/lib/functions.py` & `pychonet-2.6.9/pychonet/lib/functions.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet/lib/udpserver.py` & `pychonet-2.6.9/pychonet/lib/udpserver.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.6.8/pychonet.egg-info/PKG-INFO` & `pychonet-2.6.9/pychonet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychonet
-Version: 2.6.8
+Version: 2.6.9
 Summary: A library for interfacing via the ECHONETlite protocol.
 Home-page: http://pypi.python.org/pypi/pychonet/
 Author: Scott Phillips
 Author-email: scotty.phillips@hotmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE-GPL
```

### Comparing `pychonet-2.6.8/pychonet.egg-info/SOURCES.txt` & `pychonet-2.6.9/pychonet.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 pychonet/HomeAirCleaner.py
 pychonet/HomeAirConditioner.py
 pychonet/HomeSolarPower.py
 pychonet/HotWaterGenerator.py
 pychonet/HybridWaterHeater.py
 pychonet/LightingSystem.py
 pychonet/LowVoltageSmartElectricEnergyMeter.py
+pychonet/Refrigerator.py
 pychonet/RiceCooker.py
 pychonet/SingleFunctionLighting.py
 pychonet/StorageBattery.py
 pychonet/TemperatureSensor.py
 pychonet/WaterFlowMeter.py
 pychonet/__init__.py
 pychonet/echonetapiclient.py
```

### Comparing `pychonet-2.6.8/setup.py` & `pychonet-2.6.9/setup.py`

 * *Files identical despite different names*

