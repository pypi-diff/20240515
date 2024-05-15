# Comparing `tmp/xmlstore-0.9.8-py2.py3-none-any.whl.zip` & `tmp/xmlstore-0.9.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 77959 bytes, number of entries: 14
+Zip file size: 77944 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat        0 b- defN 19-May-29 07:59 xmlstore/__init__.py
 -rw-rw-rw-  2.0 fat     2659 b- defN 19-May-29 07:59 xmlstore/converter-1.0.xsd
--rw-rw-rw-  2.0 fat    64425 b- defN 20-Oct-01 16:42 xmlstore/datatypes.py
--rw-rw-rw-  2.0 fat    91580 b- defN 20-Oct-01 10:55 xmlstore/gui_qt4.py
+-rw-rw-rw-  2.0 fat    64400 b- defN 20-Oct-03 16:50 xmlstore/datatypes.py
+-rw-rw-rw-  2.0 fat    91548 b- defN 20-Oct-03 08:29 xmlstore/gui_qt4.py
 -rw-rw-rw-  2.0 fat     2311 b- defN 19-Jul-07 14:17 xmlstore/qt_compat.py
 -rw-rw-rw-  2.0 fat    15948 b- defN 19-Jun-19 10:34 xmlstore/util.py
 -rw-rw-rw-  2.0 fat    12280 b- defN 20-Sep-29 20:47 xmlstore/versioning.py
 -rw-rw-rw-  2.0 fat      562 b- defN 19-May-29 07:59 xmlstore/xmlstore-1.0.xsd
 -rw-rw-rw-  2.0 fat     9224 b- defN 19-May-29 07:59 xmlstore/xmlstore-base-1.0.xsd
 -rw-rw-rw-  2.0 fat   132314 b- defN 20-Sep-30 20:52 xmlstore/xmlstore.py
--rw-rw-rw-  2.0 fat      547 b- defN 20-Oct-01 17:20 xmlstore-0.9.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      116 b- defN 20-Oct-01 17:20 xmlstore-0.9.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 20-Oct-01 17:20 xmlstore-0.9.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1093 b- defN 20-Oct-01 17:20 xmlstore-0.9.8.dist-info/RECORD
-14 files, 333068 bytes uncompressed, 76169 bytes compressed:  77.1%
+-rw-rw-rw-  2.0 fat      547 b- defN 20-Oct-04 14:48 xmlstore-0.9.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      116 b- defN 20-Oct-04 14:48 xmlstore-0.9.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 20-Oct-04 14:48 xmlstore-0.9.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1093 b- defN 20-Oct-04 14:48 xmlstore-0.9.9.dist-info/RECORD
+14 files, 333011 bytes uncompressed, 76154 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: xmlstore/xmlstore-base-1.0.xsd
 Comment: 
 
 Filename: xmlstore/xmlstore.py
 Comment: 
 
-Filename: xmlstore-0.9.8.dist-info/METADATA
+Filename: xmlstore-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: xmlstore-0.9.8.dist-info/WHEEL
+Filename: xmlstore-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: xmlstore-0.9.8.dist-info/top_level.txt
+Filename: xmlstore-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xmlstore-0.9.8.dist-info/RECORD
+Filename: xmlstore-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xmlstore/datatypes.py

```diff
@@ -452,33 +452,33 @@
                 if match is None: raise Exception('Cannot parse "%s" as datetime object.' % args[0])
                 args = map(int,match.groups())
                 kwargs['tzinfo'] = util.getUTC()
         return super(DateTime,cls).__new__(cls,*args,**kwargs)
 
     def __init__(self,*args,**kwargs):
         DataTypeSimple.__init__(self)
-        
+
     @classmethod
     def fromNamelistString(cls,string,context,template=None):
         string = String.fromNamelistString(string,context,template)
         datetimematch = DateTime.reDateTime2.match(string)
         if datetimematch is None:
             raise Exception('Cannot convert namelist string "%s" to a datetime object.' % string)
         refvals = map(int,datetimematch.group(1,2,3,4,5,6)) # Convert matched strings into integers
-        return util.dateTimeFromTuple(refvals)
-        
+        return util.dateTimeFromTuple(tuple(refvals))
+
     def toXmlString(self,context):
         return util.formatDateTime(self,iso=True)
-        
+
     def toNamelistString(self,context,template=None):
         return String(util.formatDateTime(self,iso=True)).toNamelistString(context,template)
 
     def toPrettyString(self):
         return util.formatDateTime(self)
-        
+
 register('datetime',DateTime)
 
 class TimeDelta(DataTypeSimple,datetime.timedelta):
     """Class representing a time span, capable of being stored in/loaded from
     an XML store. Time spans are stored using the ISO 8601 duration data type format.
     """
```

## xmlstore/gui_qt4.py

```diff
@@ -528,15 +528,14 @@
         try:
             v = float(input[:len(input)-len(self.suffix)])
         except ValueError:
             return input
 
         if self.minimum is not None and v<self.minimum: input = u'%s%s' % (self.minimum,self.suffix)
         if self.maximum is not None and v>self.maximum: input = u'%s%s' % (self.maximum,self.suffix)
-        print(u'"%s"' % input)
         return input
 
     def setSuffix(self,suffix):
         self.suffix = suffix
 
 class ScientificDoubleEditor(AbstractPropertyEditor,QtWidgets.QLineEdit):
     """Editor for a floating point value.
```

## Comparing `xmlstore-0.9.8.dist-info/METADATA` & `xmlstore-0.9.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlstore
-Version: 0.9.8
+Version: 0.9.9
 Summary: --- update - 
 Home-page: http://github.com/BoldingBruggeman/xmlstore
 Author: Jorn Bruggeman
 Author-email: jorn@bolding-bruggeman.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `xmlstore-0.9.8.dist-info/RECORD` & `xmlstore-0.9.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 xmlstore/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 xmlstore/converter-1.0.xsd,sha256=I2wEYZjOgs8pG5vxdR_w-DL1TUjTvgwh8FrW4awYfy8,2659
-xmlstore/datatypes.py,sha256=GFKLtmjzCzq25PqKTPB6fcHHRcDreZ_64NE3P73Too0,64425
-xmlstore/gui_qt4.py,sha256=uBmGrhcEk8wX0cZQy1VYX5266p9ylkhcNMXMZt-4T98,91580
+xmlstore/datatypes.py,sha256=Bv2EMKOU9dEzPoAvZPHC8lUwsXDP61Jdd-siKT8B0Ek,64400
+xmlstore/gui_qt4.py,sha256=BMlfin-9u6ucTE37AJPpQrObOlBnvfnEng_HNbDoKGs,91548
 xmlstore/qt_compat.py,sha256=3PeCuyz6qJZNfVUcDpQp61j9DSJKcL-bIub3uUjHDjI,2311
 xmlstore/util.py,sha256=-g1PB-ZhwY8fIeVl3dDM9Va5a9qOthNKwaUtylCyOWk,15948
 xmlstore/versioning.py,sha256=pALfJl1wAkDEK0WmB0a4ycYbXMIuA_tc2oioXJIZ-Es,12280
 xmlstore/xmlstore-1.0.xsd,sha256=WZi0sC9BOgmumV0DgaT80-j-IQRvEr8YWuehCM9VgFc,562
 xmlstore/xmlstore-base-1.0.xsd,sha256=mY38joUsBN7GDuB6GpJXMpsqlQMg0M57IJeadYdKMTY,9224
 xmlstore/xmlstore.py,sha256=QooRfsRyyp9eGVINh86WMQVM4712COWhaunmfpQqkEQ,132314
-xmlstore-0.9.8.dist-info/METADATA,sha256=vNVLEoUfHp6yJ1wv1bgie_U1I9K30rujx5Nou5p2xlo,547
-xmlstore-0.9.8.dist-info/WHEEL,sha256=gxPaqcqKPLUXaSAKwmfHO7_iAOlVvmp33DewnUluBB8,116
-xmlstore-0.9.8.dist-info/top_level.txt,sha256=1n6pUpKZcdtOaMo0LKCVzuM8dBctoS7spCefQvK1R7g,9
-xmlstore-0.9.8.dist-info/RECORD,,
+xmlstore-0.9.9.dist-info/METADATA,sha256=_bwvfHaJMSyr9WWjlifZBZLbUHrIVDLjTRJrwkqOGZQ,547
+xmlstore-0.9.9.dist-info/WHEEL,sha256=gxPaqcqKPLUXaSAKwmfHO7_iAOlVvmp33DewnUluBB8,116
+xmlstore-0.9.9.dist-info/top_level.txt,sha256=1n6pUpKZcdtOaMo0LKCVzuM8dBctoS7spCefQvK1R7g,9
+xmlstore-0.9.9.dist-info/RECORD,,
```

