# Comparing `tmp/qsharp-1.4.1.dev0-cp37-abi3-win_arm64.whl.zip` & `tmp/qsharp-1.4.2.dev0-cp37-abi3-win_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 1635517 bytes, number of entries: 14
--rw-r--r--  4.6 unx     2098 b- defN 24-May-06 21:41 qsharp-1.4.1.dev0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-06 21:41 qsharp-1.4.1.dev0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3090 b- defN 24-May-06 21:41 qsharp/.data/qsharp_codemirror.js
--rw-r--r--  4.6 unx    38836 b- defN 24-May-06 21:41 qsharp/estimator/_estimator.py
--rw-r--r--  4.6 unx      859 b- defN 24-May-06 21:41 qsharp/estimator/__init__.py
--rw-r--r--  4.6 unx     1706 b- defN 24-May-06 21:41 qsharp/utils/_utils.py
--rw-r--r--  4.6 unx      146 b- defN 24-May-06 21:41 qsharp/utils/__init__.py
--rw-r--r--  4.6 unx      864 b- defN 24-May-06 21:41 qsharp/_fs.py
--rw-r--r--  4.6 unx     1848 b- defN 24-May-06 21:41 qsharp/_ipython.py
--rw-r--r--  4.6 unx     6436 b- defN 24-May-06 21:41 qsharp/_native.pyi
--rw-r--r--  4.6 unx    12818 b- defN 24-May-06 21:41 qsharp/_qsharp.py
--rw-r--r--  4.6 unx      902 b- defN 24-May-06 21:41 qsharp/__init__.py
--rwxr-xr-x  4.6 unx  3973120 b- defN 24-May-06 21:41 qsharp/_native.pyd
--rw-r--r--  4.6 unx     1085 b- defN 24-May-06 21:41 qsharp-1.4.1.dev0.dist-info/RECORD
-14 files, 4043902 bytes uncompressed, 1633747 bytes compressed:  59.6%
+Zip file size: 1650322 bytes, number of entries: 14
+-rw-r--r--  4.6 unx     2098 b- defN 24-May-14 22:45 qsharp-1.4.2.dev0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-14 22:45 qsharp-1.4.2.dev0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3090 b- defN 24-May-14 22:45 qsharp/.data/qsharp_codemirror.js
+-rw-r--r--  4.6 unx    38836 b- defN 24-May-14 22:45 qsharp/estimator/_estimator.py
+-rw-r--r--  4.6 unx      859 b- defN 24-May-14 22:45 qsharp/estimator/__init__.py
+-rw-r--r--  4.6 unx     1706 b- defN 24-May-14 22:45 qsharp/utils/_utils.py
+-rw-r--r--  4.6 unx      146 b- defN 24-May-14 22:45 qsharp/utils/__init__.py
+-rw-r--r--  4.6 unx      864 b- defN 24-May-14 22:45 qsharp/_fs.py
+-rw-r--r--  4.6 unx     1848 b- defN 24-May-14 22:45 qsharp/_ipython.py
+-rw-r--r--  4.6 unx     6534 b- defN 24-May-14 22:45 qsharp/_native.pyi
+-rw-r--r--  4.6 unx    12906 b- defN 24-May-14 22:45 qsharp/_qsharp.py
+-rw-r--r--  4.6 unx      902 b- defN 24-May-14 22:45 qsharp/__init__.py
+-rwxr-xr-x  4.6 unx  4007424 b- defN 24-May-14 22:45 qsharp/_native.pyd
+-rw-r--r--  4.6 unx     1085 b- defN 24-May-14 22:45 qsharp-1.4.2.dev0.dist-info/RECORD
+14 files, 4078392 bytes uncompressed, 1648552 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: qsharp-1.4.1.dev0.dist-info/METADATA
+Filename: qsharp-1.4.2.dev0.dist-info/METADATA
 Comment: 
 
-Filename: qsharp-1.4.1.dev0.dist-info/WHEEL
+Filename: qsharp-1.4.2.dev0.dist-info/WHEEL
 Comment: 
 
 Filename: qsharp/.data/qsharp_codemirror.js
 Comment: 
 
 Filename: qsharp/estimator/_estimator.py
 Comment: 
@@ -33,11 +33,11 @@
 
 Filename: qsharp/__init__.py
 Comment: 
 
 Filename: qsharp/_native.pyd
 Comment: 
 
-Filename: qsharp-1.4.1.dev0.dist-info/RECORD
+Filename: qsharp-1.4.2.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qsharp/_native.pyi

```diff
@@ -180,14 +180,15 @@
     An output returned from the Q# interpreter.
     Outputs can be a state dumps or messages. These are normally printed to the console.
     """
 
     def __repr__(self) -> str: ...
     def __str__(self) -> str: ...
     def _repr_html_(self) -> str: ...
+    def _repr_latex_(self) -> Optional[str]: ...
     def state_dump(self) -> Optional[StateDumpData]: ...
 
 class StateDumpData:
     """
     A state dump returned from the Q# interpreter.
     """
 
@@ -200,14 +201,15 @@
     Get the amplitudes of the state vector as a dictionary from state integer to
     complex amplitudes.
     """
     def get_dict(self) -> dict: ...
     def __repr__(self) -> str: ...
     def __str__(self) -> str: ...
     def _repr_html_(self) -> str: ...
+    def _repr_latex_(self) -> Optional[str]: ...
 
 class Circuit:
     def json(self) -> str: ...
     def __repr__(self) -> str: ...
     def __str__(self) -> str: ...
 
 class QSharpError(BaseException):
```

## qsharp/_qsharp.py

```diff
@@ -339,14 +339,17 @@
 
     def __str__(self) -> str:
         return self.__data.__str__()
 
     def _repr_html_(self) -> str:
         return self.__data._repr_html_()
 
+    def _repr_latex_(self) -> Optional[str]:
+        return self.__data._repr_latex_()
+
     def check_eq(
         self, state: Union[Dict[int, complex], List[complex]], tolerance: float = 1e-10
     ) -> bool:
         """
         Checks if the state dump is equal to the given state. This is not mathematical equality,
         as the check ignores global phase.
```

## Comparing `qsharp-1.4.1.dev0.dist-info/METADATA` & `qsharp-1.4.2.dev0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp
-Version: 1.4.1.dev0
+Version: 1.4.2.dev0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `qsharp-1.4.1.dev0.dist-info/RECORD` & `qsharp-1.4.2.dev0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-qsharp-1.4.1.dev0.dist-info/METADATA,sha256=Q6w9fa-VldVCe4qGp50ayWtIHcBBLbm-k2YOMUF1tPg,2098
-qsharp-1.4.1.dev0.dist-info/WHEEL,sha256=xsrEGIMmQ1avWDJ2-RvHLDam8haXzwGnBhrUlFUsLAc,94
+qsharp-1.4.2.dev0.dist-info/METADATA,sha256=WvWiDBS2jxDrUAvvL3EtTCfdv1zB1u4g2EKc_HF17G8,2098
+qsharp-1.4.2.dev0.dist-info/WHEEL,sha256=xsrEGIMmQ1avWDJ2-RvHLDam8haXzwGnBhrUlFUsLAc,94
 qsharp/.data/qsharp_codemirror.js,sha256=72E3fTxGxfBe_bBhPD5-8ul_S61MLVA_JmMJwOXgmhc,3090
 qsharp/estimator/_estimator.py,sha256=LMTJg2xPwhvswlc0ts0zsjRPd82mF5KzYgmHyFFl2PE,38836
 qsharp/estimator/__init__.py,sha256=JK6oDnNX_rgsPnfyFsK0yxMBRinmW8jlc8183BydxXA,859
 qsharp/utils/_utils.py,sha256=s3ausLf4wp08rgRDrcdzSXOYPRQ63isX0umCA9MIq7M,1706
 qsharp/utils/__init__.py,sha256=ejBPCXRttEGKCDehjldx8SryqQfNHXsgsRFK5O-zRU8,146
 qsharp/_fs.py,sha256=RGhwMRUwfxGoPVEPaP39FxyRcPeZoyhB0kb4MwzxE54,864
 qsharp/_ipython.py,sha256=x8J7HatTw15xTg9Ppd-yRmhNz9eY8cBAhruRiHo46bQ,1848
-qsharp/_native.pyi,sha256=dC3H1V_TpWMVTfDjViMQtWhRELrbMOVFyLzkH1yUN7Q,6436
-qsharp/_qsharp.py,sha256=J-qEF-D2x54NLHdEfnc3GU4FgsLSFF7jplVDiiF-Kkg,12818
+qsharp/_native.pyi,sha256=pv1ZcI3tlKuOzxs2AdHTJi4odEGVXkz5-QVyXJfHtNo,6534
+qsharp/_qsharp.py,sha256=EIF8aqniTs5rFp736izdhg-yAY_A57sq4JVGjGFvwhI,12906
 qsharp/__init__.py,sha256=-KmJgZV8ZRqWSIOENAhyE39vYF5eZ_p4W04XZ29YKfs,902
-qsharp/_native.pyd,sha256=LMpQEicy3E8am90H_4tRc2xGTvc1-brcPVNVkdyANsg,3973120
-qsharp-1.4.1.dev0.dist-info/RECORD,,
+qsharp/_native.pyd,sha256=ayWixrDZg0LPbW_p13E9_A52gIWv9aiutErleDuyPvY,4007424
+qsharp-1.4.2.dev0.dist-info/RECORD,,
```

