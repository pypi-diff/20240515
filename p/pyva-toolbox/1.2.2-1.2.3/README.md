# Comparing `tmp/pyva-toolbox-1.2.2.tar.gz` & `tmp/pyva_toolbox-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyva-toolbox-1.2.2.tar", last modified: Tue Jan  9 22:38:01 2024, max compression
+gzip compressed data, was "pyva_toolbox-1.2.3.tar", last modified: Wed May 15 19:57:08 2024, max compression
```

## Comparing `pyva-toolbox-1.2.2.tar` & `pyva_toolbox-1.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.452154 pyva-toolbox-1.2.2/
--rw-rw-rw-   0        0        0    27030 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     3029 2024-01-09 22:38:01.450951 pyva-toolbox-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2266 2023-10-23 19:40:36.000000 pyva-toolbox-1.2.2/README.md
--rw-rw-rw-   0        0        0      788 2024-01-09 22:33:16.000000 pyva-toolbox-1.2.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.385836 pyva-toolbox-1.2.2/pyva/
--rw-rw-rw-   0        0        0      555 2022-12-11 12:00:56.000000 pyva-toolbox-1.2.2/pyva/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.391073 pyva-toolbox-1.2.2/pyva/coupling/
--rw-rw-rw-   0        0        0      309 2022-06-30 20:36:33.000000 pyva-toolbox-1.2.2/pyva/coupling/__init__.py
--rw-rw-rw-   0        0        0      977 2022-07-01 16:25:41.000000 pyva-toolbox-1.2.2/pyva/coupling/connections.py
--rw-rw-rw-   0        0        0    83903 2023-10-28 16:42:15.000000 pyva-toolbox-1.2.2/pyva/coupling/junctions.py
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.395075 pyva-toolbox-1.2.2/pyva/data/
--rw-rw-rw-   0        0        0      504 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/data/__init__.py
--rw-rw-rw-   0        0        0    39586 2023-06-28 19:05:18.000000 pyva-toolbox-1.2.2/pyva/data/dof.py
--rw-rw-rw-   0        0        0    80918 2023-10-04 19:29:27.000000 pyva-toolbox-1.2.2/pyva/data/matrixClasses.py
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.397076 pyva-toolbox-1.2.2/pyva/geometry/
--rw-rw-rw-   0        0        0      109 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/geometry/__init__.py
--rw-rw-rw-   0        0        0    13731 2022-09-15 19:10:27.000000 pyva-toolbox-1.2.2/pyva/geometry/meshClasses.py
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.400074 pyva-toolbox-1.2.2/pyva/loads/
--rw-rw-rw-   0        0        0      176 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/loads/__init__.py
--rw-rw-rw-   0        0        0     1472 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/loads/loadCase.py
--rw-rw-rw-   0        0        0    81724 2023-10-06 21:04:03.000000 pyva-toolbox-1.2.2/pyva/models.py
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.407831 pyva-toolbox-1.2.2/pyva/properties/
--rw-rw-rw-   0        0        0      391 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/properties/__init__.py
--rw-rw-rw-   0        0        0     3223 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/properties/geometricalPropertyClasses.py
--rw-rw-rw-   0        0        0    43598 2023-09-15 12:35:52.000000 pyva-toolbox-1.2.2/pyva/properties/materialClasses.py
--rw-rw-rw-   0        0        0    55570 2023-11-15 21:33:08.000000 pyva-toolbox-1.2.2/pyva/properties/structuralPropertyClasses.py
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.421944 pyva-toolbox-1.2.2/pyva/systems/
--rw-rw-rw-   0        0        0     6225 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/systems/SEA_system.py
--rw-rw-rw-   0        0        0      546 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/systems/__init__.py
--rw-rw-rw-   0        0        0    38317 2023-11-15 19:46:59.000000 pyva-toolbox-1.2.2/pyva/systems/acoustic1Dsystems.py
--rw-rw-rw-   0        0        0    17746 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/systems/acoustic3Dsystems.py
--rw-rw-rw-   0        0        0    31041 2023-10-04 19:57:42.000000 pyva-toolbox-1.2.2/pyva/systems/acousticRadiators.py
--rw-rw-rw-   0        0        0    59801 2023-12-20 16:17:41.000000 pyva-toolbox-1.2.2/pyva/systems/infiniteLayers.py
--rw-rw-rw-   0        0        0     9566 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/systems/lumpedSystems.py
--rw-rw-rw-   0        0        0     4777 2022-04-02 16:26:38.000000 pyva-toolbox-1.2.2/pyva/systems/structure1Dsystems.py
--rw-rw-rw-   0        0        0    50157 2022-12-06 20:52:45.000000 pyva-toolbox-1.2.2/pyva/systems/structure2Dsystems.py
--rw-rw-rw-   0        0        0     3881 2022-10-10 19:11:01.000000 pyva-toolbox-1.2.2/pyva/useful.py
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.449629 pyva-toolbox-1.2.2/pyva_toolbox.egg-info/
--rw-rw-rw-   0        0        0     3029 2024-01-09 22:38:01.000000 pyva-toolbox-1.2.2/pyva_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2024-01-09 22:38:01.000000 pyva-toolbox-1.2.2/pyva_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-09 22:38:01.000000 pyva-toolbox-1.2.2/pyva_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-01-09 22:38:01.000000 pyva-toolbox-1.2.2/pyva_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-01-09 22:38:01.000000 pyva-toolbox-1.2.2/pyva_toolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-09 22:38:01.452154 pyva-toolbox-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      351 2024-01-09 22:36:17.000000 pyva-toolbox-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-09 22:38:01.447634 pyva-toolbox-1.2.2/tests/
--rw-rw-rw-   0        0        0      153 2022-03-21 22:45:17.000000 pyva-toolbox-1.2.2/tests/testbuffer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.735735 pyva_toolbox-1.2.3/
+-rw-rw-rw-   0        0        0    27030 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3029 2024-05-15 19:57:08.735735 pyva_toolbox-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2266 2023-10-23 19:40:36.000000 pyva_toolbox-1.2.3/README.md
+-rw-rw-rw-   0        0        0      788 2024-04-24 17:19:41.000000 pyva_toolbox-1.2.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.330271 pyva_toolbox-1.2.3/pyva/
+-rw-rw-rw-   0        0        0      555 2022-12-11 12:00:56.000000 pyva_toolbox-1.2.3/pyva/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.360920 pyva_toolbox-1.2.3/pyva/coupling/
+-rw-rw-rw-   0        0        0      309 2022-06-30 20:36:33.000000 pyva_toolbox-1.2.3/pyva/coupling/__init__.py
+-rw-rw-rw-   0        0        0      977 2022-07-01 16:25:41.000000 pyva_toolbox-1.2.3/pyva/coupling/connections.py
+-rw-rw-rw-   0        0        0    85148 2024-05-12 19:52:26.000000 pyva_toolbox-1.2.3/pyva/coupling/junctions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.395350 pyva_toolbox-1.2.3/pyva/data/
+-rw-rw-rw-   0        0        0      504 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/data/__init__.py
+-rw-rw-rw-   0        0        0    39586 2023-06-28 19:05:18.000000 pyva_toolbox-1.2.3/pyva/data/dof.py
+-rw-rw-rw-   0        0        0    80918 2023-10-04 19:29:27.000000 pyva_toolbox-1.2.3/pyva/data/matrixClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.411937 pyva_toolbox-1.2.3/pyva/geometry/
+-rw-rw-rw-   0        0        0      109 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/geometry/__init__.py
+-rw-rw-rw-   0        0        0    13731 2022-09-15 19:10:27.000000 pyva_toolbox-1.2.3/pyva/geometry/meshClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.426020 pyva_toolbox-1.2.3/pyva/loads/
+-rw-rw-rw-   0        0        0      176 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/loads/__init__.py
+-rw-rw-rw-   0        0        0     1472 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/loads/loadCase.py
+-rw-rw-rw-   0        0        0    81724 2024-05-10 08:09:13.000000 pyva_toolbox-1.2.3/pyva/models.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.473750 pyva_toolbox-1.2.3/pyva/properties/
+-rw-rw-rw-   0        0        0      391 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/properties/__init__.py
+-rw-rw-rw-   0        0        0     3223 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/properties/geometricalPropertyClasses.py
+-rw-rw-rw-   0        0        0    51311 2024-05-02 19:28:49.000000 pyva_toolbox-1.2.3/pyva/properties/materialClasses.py
+-rw-rw-rw-   0        0        0    55570 2023-11-15 21:33:08.000000 pyva_toolbox-1.2.3/pyva/properties/structuralPropertyClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.671615 pyva_toolbox-1.2.3/pyva/systems/
+-rw-rw-rw-   0        0        0     6225 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/systems/SEA_system.py
+-rw-rw-rw-   0        0        0      546 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/systems/__init__.py
+-rw-rw-rw-   0        0        0    38317 2023-11-15 19:46:59.000000 pyva_toolbox-1.2.3/pyva/systems/acoustic1Dsystems.py
+-rw-rw-rw-   0        0        0    17746 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/systems/acoustic3Dsystems.py
+-rw-rw-rw-   0        0        0    33683 2024-05-01 11:20:17.000000 pyva_toolbox-1.2.3/pyva/systems/acousticRadiators.py
+-rw-rw-rw-   0        0        0    59795 2024-01-12 18:04:57.000000 pyva_toolbox-1.2.3/pyva/systems/infiniteLayers.py
+-rw-rw-rw-   0        0        0     9566 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/systems/lumpedSystems.py
+-rw-rw-rw-   0        0        0     4777 2022-04-02 16:26:38.000000 pyva_toolbox-1.2.3/pyva/systems/structure1Dsystems.py
+-rw-rw-rw-   0        0        0    50157 2022-12-06 20:52:45.000000 pyva_toolbox-1.2.3/pyva/systems/structure2Dsystems.py
+-rw-rw-rw-   0        0        0     5941 2024-04-24 17:35:04.000000 pyva_toolbox-1.2.3/pyva/useful.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.735735 pyva_toolbox-1.2.3/pyva_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     3029 2024-05-15 19:57:06.000000 pyva_toolbox-1.2.3/pyva_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2024-05-15 19:57:06.000000 pyva_toolbox-1.2.3/pyva_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:57:06.000000 pyva_toolbox-1.2.3/pyva_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-15 19:57:06.000000 pyva_toolbox-1.2.3/pyva_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-15 19:57:06.000000 pyva_toolbox-1.2.3/pyva_toolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:57:08.735735 pyva_toolbox-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      351 2024-04-24 16:35:04.000000 pyva_toolbox-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:57:08.732226 pyva_toolbox-1.2.3/tests/
+-rw-rw-rw-   0        0        0      153 2022-03-21 22:45:17.000000 pyva_toolbox-1.2.3/tests/testbuffer.py
```

### Comparing `pyva-toolbox-1.2.2/LICENSE` & `pyva_toolbox-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/PKG-INFO` & `pyva_toolbox-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyva-toolbox
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python toolbox for vibroacoustic simulation
 Author: Dr. Alexander Peiffer
 Author-email: Alexander Peiffer <author@alexanderpeiffer.de>
 Project-URL: Homepage, https://github.com/minipief/pyva
 Project-URL: Bug Tracker, https://github.com/minipief/pyva/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `pyva-toolbox-1.2.2/README.md` & `pyva_toolbox-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyproject.toml` & `pyva_toolbox-1.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyva-toolbox"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Alexander Peiffer", email="author@alexanderpeiffer.de" },
 ]
 description = "Python toolbox for vibroacoustic simulation"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `pyva-toolbox-1.2.2/pyva/__init__.py` & `pyva_toolbox-1.2.3/pyva/__init__.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/coupling/connections.py` & `pyva_toolbox-1.2.3/pyva/coupling/connections.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/coupling/junctions.py` & `pyva_toolbox-1.2.3/pyva/coupling/junctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1154,59 +1154,69 @@
     
         if Signal:
             return mC.Signal(xdata,_ydata,dof.DOF(i_out_wave,np.zeros((1,Nsig)),_tdof))
         else:
             return _ydata
     
     
-    def transmission_wavenumber_diffuse(self,omega,i_sys = (0,1),i_in_wave = (5,5),i_out_wave = (5,3), N_step = 100,method = 'diffuse',Signal = True):
+    def transmission_wavenumber_diffuse(self,omega,i_sys = (0,1),i_in_wave = (5,5),i_out_wave = (5,3), \
+                                        N_step = 100,CLF_sw = False, method = 'diffuse',Signal = True):
         """
-        diffuse transmission coefficient for line junctions
+        Diffuse transmission coefficient for line junctions.
+        
+        When this method is used for calculating Equation (8.160) we don't need the diffuse field transmission coeffcient
+        <tau> but the pure wavenumber integral that is NOT divided by k_v^(m). For this purpose a switch in intgrated 
+        that sets k_in = 1.
         
 
         Parameters
         ----------
         omega : float or ndarray
             angular frequency.
         i_sys : tuple or list, optional
             incident and radiating system index vector. The default is (0,1).
         i_in_wave : tuple or list, optional
             incident wave_DOF. The default is (5,5).
         i_out_wave : tuple or list, optional
             transmissted wave_DOF. The default is (5,3).
         N_step : int, optional
             Number of wavenumber integration steps. The default is 100.
+        CLF_sw : bool, otional
+            Sets the incoming wavenumber to 1 if True for use in line junctin matrix Eq. (8.160). The default is False.
         method : str, optional
             Mewthod seclector 'diffuse' for diffuse field reciprocity, 'langley' for wave transmission. The default is 'diffuse'.
         Signal : bool, optional
             Swith for return datatype. The default is True.
 
         Returns
         -------
         ndarray (Signal = False) or Signal
             diffuse field transmission coefficient.
-        """
-
-                
+        """       
         # convert to np.array to become independent from tupels
         i_sys,i_in_wave,i_out_wave = all2array(i_sys,i_in_wave,i_out_wave)
 
         tau = np.zeros((len(i_out_wave),omega.size))
 
 
         
         for ifreq,om in enumerate(omega):
             
-            kx   = self.kx(om,i_sys,i_in_wave[0],i_out_wave,N_step,method = 'in-plane')     
-            k_in = self.systems[i_sys[0]].plate_wavenumber(om,i_in_wave[0])
+            kx   = self.kx(om,i_sys,i_in_wave[0],i_out_wave,N_step,method = 'in-plane')
+            if CLF_sw:
+                k_in = 1
+            else: 
+                k_in = self.systems[i_sys[0]].plate_wavenumber(om,i_in_wave[0])
+                
             if method == 'diffuse':
                 taus = self.transmission_wavenumber(om,kx,i_sys,i_in_wave,i_out_wave,Signal=False)#.ydata # check late with Signal option
             elif method == 'langley':
                 taus = self.transmission_wavenumber_langley(om,kx,i_sys,i_in_wave,i_out_wave,Signal=False)#.ydata
             
+            #Integral in wavenumber space instead of angle requires the division be the in-field wavenumber
             for i_wave,i_type in enumerate(i_out_wave):
                 tau[i_wave,ifreq] = integrate.trapz(taus[i_wave,:],kx)/k_in
 
         if Signal:
                         
             xdata = mC.DataAxis(omega,typestr='angular frequency')
             tdof = dof.DOFtype(typestr='transmission')
@@ -1367,15 +1377,16 @@
             # smaller for in-plane waves. So we need special treatment of both regimes1
 
             #k_in = self.systems[i_sys[0]].plate_wavenumber(om,i_in_wave[0])
             
             kx   = self.kx(om,i_sys,i_in_wave[0],i_out_wave,N_step,method = 'in-plane')
             
             if method == 'diffuse':
-                taus = self.transmission_wavenumber_LM(om,kx,i_sys,i_in_wave,i_out_wave,Signal=False) # check late with Signal option
+                taus = self.transmission_wavenumber(om,kx,i_sys,i_in_wave,i_out_wave,Signal=False) # check late with Signal option
+                #taus = self.transmission_wavenumber_LM(om,kx,i_sys,i_in_wave,i_out_wave,Signal=False) # check late with Signal option
             elif method == 'langley':
                 taus = self.transmission_wavenumber_langley(om,kx,i_sys,i_in_wave,i_out_wave,Signal=False)
                         
             for i_o_wave,i_type in enumerate(i_out_wave):
                 etas[i_o_wave,ifreq] = fak1[ifreq]/modal_dens*integrate.trapz(taus[i_o_wave,:],kx)
                 
                 
@@ -1461,15 +1472,15 @@
             
         if Signal:
             xdata = mC.DataAxis(omega,typestr = 'angular frequency')
             return mC.Signal(xdata,etas,dof.DOF(i_out_wave,np.zeros((1,Nsig)),_tdof))
         else:
             return etas
         
-    def junction_matrix(self,omega,N_step = 90, method = 'diffuse'):
+    def junction_matrix(self,omega,N_step = 200, method = 'diffuse'):
         """
         Creates junction matrix for LineJunction (all upper triangular)
         
         This method calculates the all CLF of junction matric [J] 
         The wavefields that are considered ar either the pressure wave or the bending wave
         The CLF is calculated running through through both indexes
 
@@ -1485,73 +1496,74 @@
         Returns
         -------
         JM : DynamiMatrix
             JunctionMatrix.
 
         """
                 
-        mod_dens = self.modal_density(omega)
+        #mod_dens = self.modal_density(omega)
 
         # prepare relevant wave_DOFs of junction only 3,4 couples to the fluid!          
-        j_wave_DOF = self.wave_DOF
-        Nw         = self.N_wave
+        j_wave_DOF = self.wave_DOF # DOF of this junction 
+        Nw         = self.N_wave   
 
     
         # .. indexes into upper triangular
         i_row,i_col = np.triu_indices(self.N_wave,1)    
  
         # initialise
         JM  = super().junction_matrix(omega)
         fak = self.length/2/np.pi**2/omega
         
         
-        #buffer for h_buf
+        # Buffer for column of CLFs
         h_buf = np.zeros((Nw-1,len(omega)))
         
 
         
-        # loop over upper triangular
-        # For plates it is better to use the lower triangulat coefficient, because in this
+        # loop over lower triangular matrix !!!!!
+        # For plates it is better to use the lower triangular coefficients, because in this
         # case the exciting wave field remains constant and the total stiffness matrix can be reused much better
         # ir_start = 0
            
         for ic in range(Nw-1): # loop over coloums
 
            # irows = i_row[ir_start:ir_start+self.N-ixc]  # take all row indexes of this coloums
-           irows = np.arange(ic+1,Nw)         # take all row indexes of this coloums
+           irows = np.arange(ic+1,Nw)          # the row indexes of current column ic
            sys_ = self.wave_sys[ic]
-           i_in_sys = self.systems.index(sys_)
-           Nr = Nw-1-ic # number of rows
+           i_in_sys = self.systems.index(sys_) # physical system index (not wave system)
+           Nr = Nw-1-ic                        # number of rows in current column
            
            # transmission call must be seperated into case of two same systems and
            # different systmes
            
-           # get list of respose systems
+           # get list of respose systems (not wave index)
            sys_IDs = self.wave_DOF[irows].ID
            # prepare input arguments of transmission_wavenumber for each system ID configuraiion
            out_IDs,ix_out,Ns_out= np.unique(sys_IDs, return_index = True,return_counts=True)
            
            #i0 = 0       
-           # loop over system configurations
+           # loop over physical system index
            for ii,ix_sys in enumerate(ix_out):
-               Nr = Ns_out[ii]
-               i0 = ix_out[ii] # the sort option requires this i0 may be jumping
+               Nr = Ns_out[ii] # Number of rows (output wave systems) for this phsysical system
+               i0 = ix_sys # the sort option requires this i0 may be jumping
                irows_ = np.arange(i0,(i0+Nr)) # row index with unique system combination
-               i_out_sys=self.systems.index(self.wave_sys[ix_sys])
+               i_out_sys=self.index(sys_IDs[ix_sys]) # self.index(self.wave_sys[ix_sys]) # gives wrong output system in secon loop
+               # Old index irows_
                h_buf[irows_,:] = -fak*self.transmission_wavenumber_diffuse(omega, (i_in_sys,i_out_sys), \
                                                                       np.tile(self.wave_DOF[ic].dof,(Nr,)), \
-                                                                      self.wave_DOF[irows[irows_]].dof,Signal=False)
+                                                                      self.wave_DOF[irows[irows_]].dof, CLF_sw=True, \
+                                                                      N_step=N_step, Signal=False)
                #i0 += Nr
            
            # And fill the lower tri and diagonal entries
            for ix,ir in enumerate(irows):
                JM[ir,ic,:] = h_buf[ix,:]    
-               JM[ir,ir,:] = JM[ir,ir,:].data - JM[ir,ic,:].data
-               JM[ic,ic,:] = JM[ic,ic,:].data - JM[ir,ic,:].data
-        
+               JM[ir,ir,:] = JM[ir,ir,:].data - h_buf[ix,:] # JM[ir,ic,:].data
+               JM[ic,ic,:] = JM[ic,ic,:].data - h_buf[ix,:] # JM[ir,ic,:].data
             
         # diagonal!
         return JM
         
 class AreaJunction(Junction):
     """ 
     Class for Area Junctions between plates and cavities
```

### Comparing `pyva-toolbox-1.2.2/pyva/data/dof.py` & `pyva_toolbox-1.2.3/pyva/data/dof.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/data/matrixClasses.py` & `pyva_toolbox-1.2.3/pyva/data/matrixClasses.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/geometry/meshClasses.py` & `pyva_toolbox-1.2.3/pyva/geometry/meshClasses.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/loads/loadCase.py` & `pyva_toolbox-1.2.3/pyva/loads/loadCase.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/models.py` & `pyva_toolbox-1.2.3/pyva/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3899,16 +3899,16 @@
 0000f3a0: 2020 2020 2020 2020 2020 2046 6f72 6365             Force
 0000f3b0: 206c 6f61 6473 206f 6e20 4645 7379 7374   loads on FEsyst
 0000f3c0: 656d 732e 2054 6865 2064 6566 6175 6c74  ems. The default
 0000f3d0: 2069 7320 4e6f 6e65 2e0d 0a0d 0a20 2020   is None.....   
 0000f3e0: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
 0000f3f0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
 0000f400: 2020 2020 2020 2069 6e74 0d0a 2020 2020         int..    
-0000f410: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
-0000f420: 494f 4e2e 0d0a 0d0a 2020 2020 2020 2020  ION.....        
+0000f410: 2020 2020 2020 2020 5374 6174 7573 2063          Status c
+0000f420: 6f64 652e 0d0a 0d0a 2020 2020 2020 2020  ode.....        
 0000f430: 2222 220d 0a20 2020 2020 2020 200d 0a20  """..        .. 
 0000f440: 2020 2020 2020 204e 5f73 6561 2020 3d20         N_sea  = 
 0000f450: 7365 6c66 2e4e 5f73 6561 200d 0a20 2020  self.N_sea ..   
 0000f460: 2020 2020 204e 5f66 7265 7120 3d20 6c65       N_freq = le
 0000f470: 6e28 7365 6c66 2e78 6461 7461 290d 0a20  n(self.xdata).. 
 0000f480: 2020 2020 2020 206f 6d65 6761 203d 2073         omega = s
 0000f490: 656c 662e 7864 6174 612e 616e 6775 6c61  elf.xdata.angula
```

### Comparing `pyva-toolbox-1.2.2/pyva/properties/geometricalPropertyClasses.py` & `pyva_toolbox-1.2.3/pyva/properties/geometricalPropertyClasses.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/properties/materialClasses.py` & `pyva_toolbox-1.2.3/pyva/properties/materialClasses.py`

 * *Files 8% similar despite different names*

```diff
@@ -884,14 +884,16 @@
     porosity: volume porosity
     tortuosity: tortuosity (alpha_inf)
     rho_bulk: apearant density of fluid and matrix
     length_visc: viscous characteristic length
     length_therm:  thermal characteristic length
     limp: Switch for use of limp model, false means rigid frame
     
+    all original attributes of fluid
+    
     See [All2005]_ for details of the theory
 
     """
     
     def __init__(self,flow_res,porosity,tortuosity,rho_bulk,length_visc,length_therm,limp = True,\
                      c0=343.,rho0=1.23,eta=0.0,dynamic_viscosity=1.84e-5,kappa = 1.4, \
                      Cp=1005.1, heat_conductivity = 0.0257673):
@@ -947,26 +949,26 @@
         self.rho_bulk   = rho_bulk
         self.length_visc = length_visc
         self.length_therm = length_therm
         self.limp       = limp
         
     def __repr__(self):
         _str = 'EquivalentFluid(flow_res={0},porosity={1},tortuosity={2},rho_bulk={3},length_visc={4},length_visc={5},limp={6},'.\
-            format(self.flow_res, self.porosity,self.tortuosity,self.rho_bulk,self.length_visc,self.length_visc,self.limp)
+            format(self.flow_res, self.porosity,self.tortuosity,self.rho_bulk,self.length_visc,self.length_therm,self.limp)
         _str += 'c0={0},rho0={1},eta={2})'.format(self.c0, self.rho0,self.eta)
         return _str
-   
+    
     def __str__(self):
         """
-        str for EquivalentFluids
+        str for EquivalentFluid
 
         Returns
         -------
         _str : str
-            Fluid description.
+            EquivalentFluid description.
 
         """
         _str  = super().__str__()
         _str += "flow_res          : {0}\n".format(self.flow_res)
         _str += "porosity          : {0}\n".format(self.porosity)
         _str += "tortuosity        : {0}\n".format(self.tortuosity)
         _str += "rho_bulk          : {0}\n".format(self.rho_bulk)
@@ -1110,14 +1112,262 @@
         -------
         complex
             speed of sound.
 
         """
          
         return 1j*omega/self.propagation_constant(omega)
+    
+    @staticmethod
+    def inverse_parameter_derivation(flow_res,porosity,rho_bulk,fluid,rho_eq,K_eq,omega,limp=True):
+        """
+        Create EquivalentFluid object from test paramters
+ 
+        Parameters
+        ----------
+        flow_res : float
+            flow resistivity
+        porosity : float
+            volume porosity.
+        rho_bulk : float
+            apearant density of fluid and matrix.
+        fluid : Fluid
+            fluid during test in the fluid phase of the absorber.
+        rho_eq : complex nd.array of size (N,) or complex
+            Equivalent density of absorber material under test.
+        K_eq : complex nd.array of size (N,) or complex
+            Equivalent bulk modulus of absorber material under test.
+        omega : ndarray of size (N,) or float
+            Upper and lower limit for averaging
+        limp : bool, optional
+            Switch for use of limp model. The default is True.
+ 
+ 
+        Returns
+        -------
+        EquivalentFluid
+            LMS extimation of the materail due to test results.
+ 
+        """
+ 
+        # Helpers
+        kappa_P0 = fluid.rho0*fluid.c0**2
+        buf_ = ((kappa_P0-porosity*K_eq)/(kappa_P0-fluid.kappa*porosity*K_eq))**2
+ 
+        # Tortuosity Eq (23) of PV3982 #*
+        tortuosity = porosity/fluid.rho0*\
+            (np.real(rho_eq)-np.sqrt(np.imag(rho_eq)**2-flow_res**2/omega**2))
+ 
+        # Characteristic viscous lenght Eq (24) of PV3982
+        length_visc = tortuosity/porosity*np.sqrt(2*fluid.dynamic_viscosity*fluid.rho0/omega/np.imag(rho_eq)/(tortuosity*fluid.rho0/porosity-np.real(rho_eq)))
+ 
+ 
+        # Static thermal permeability Eq (25) of PV9382
+        # not used because it is not part of the JCA Modell
+        static_thermal_permeability = porosity*fluid.heat_conductivity/fluid.Cp/fluid.rho0/omega/\
+            np.sqrt(-np.real(buf_))
+ 
+        # Static thermal permeability Eq (26) of PV9382
+        length_therm = 2*np.sqrt(fluid.heat_conductivity/fluid.Cp/fluid.rho0/omega/(-np.imag(buf_)))
+ 
+ 
+        return EquivalentFluid(flow_res, porosity, tortuosity, rho_bulk, length_visc, length_therm,
+                               limp = limp,c0=fluid.c0,rho0=fluid.rho0,
+                               dynamic_viscosity=fluid.dynamic_viscosity,kappa = fluid.kappa,
+                               Cp=fluid.Cp,heat_conductivity=fluid.heat_conductivity)
+    
+class DelanyBazley(Fluid):
+    """
+    This class implements the empirical model of DelanyBazly or the revised Miki expressions
+    
+    This class is a doughter class of fluid.
+    
+    Attributes
+    ----------
+    flow_res: flow resistivity
+    miki: Switch for use Delaney Bazley or Miki model. True means Miki model
+    
+    """
+    def __init__(self,flow_res,c0=343.,rho0=1.23,eta=0.0,dynamic_viscosity=1.84e-5,kappa = 1.4, \
+                     Cp=1005.1, heat_conductivity = 0.0257673,miki=False):
+        """
+        Construcutor of DelanyBazely class
+        
+        The Delany Bazely model is an empirical model for fibre material, further 
+        refined and modified by Miki.
+    
+        Parameters
+        ----------
+        flow_res : float
+            flow resistivity
+        miki : bool, optional
+            Switch for use of Miki model. The default is False.
+        c0 : complex, optional
+            Speed of sound. The default is 343..
+        rho0 : complex, optional
+            density. The default is 1.23.
+        eta : float, optional
+            Damping loss. The default is 0.01.
+        dynamic_viscosity : float, optional
+            Dynamic viscosity. The default is 1.84e-5.
+        kappa : float, optional
+            ratio of specific heat capacities. The default is 1.4.
+        Pr : float, optional
+            Prandtl number. The default is 0.71.
+
+        Returns
+        -------
+        None.
+
+        """
+    
+        super().__init__(c0,rho0,eta,dynamic_viscosity,kappa,Cp,heat_conductivity)
+    
+        self.flow_res   = flow_res
+        self.miki       = miki
+        
+    def __repr__(self):
+        _str = 'DelaneyBazley(flow_res={0},miki={1},'.\
+            format(self.flow_res, self.miki)
+        _str += 'c0={0},rho0={1},eta={2})'.format(self.c0, self.rho0,self.eta)
+        return _str
+   
+    def __str__(self):
+        """
+        str for DelanyBazley
+
+        Returns
+        -------
+        _str : str
+            DelanyBazley description.
+
+        """
+        _str  = super().__str__()
+        _str += "flow_res          : {0}\n".format(self.flow_res)
+        
+        return _str
+    
+    def impedance(self,omega):
+        """
+        Complex characteristic impedance including damping
+        
+
+        Parameters
+        ----------
+        omega : float or ndarray
+            angular frequency.
+
+        Returns
+        -------
+        complex
+            characteristic impedance.
+
+        """
+        
+        f = omega/2/np.pi
+        X = f/self.flow_res
+        f_min = 0.01*self.flow_res
+        f_max = 1.00*self.flow_res
+        
+        if np.min(f)<f_min or np.max(f)>f_max:
+            Warning("frequency out of range of the DelanyBazley model")
+            
+        if self.miki:
+            Z = self.rho0*self.c0*( 1 + 5.50*(X*1000)**(-0.632)
+                            - 8.43j*(X*1000)**(-0.632) )
+        else:
+            Z = self.rho0*self.c0*( 1 + 9.08*(X*1000)**(-0.75) 
+                     - 11.9j*(X*1000)**(-0.73) )
+            
+        return Z
+    
+    def wavenumber(self,omega):
+        """
+        Wavenumber including damping
+        
+        Parameters
+        ----------
+        omega : TYPE
+            DESCRIPTION.
+
+        Returns
+        -------
+        complex
+            Complex wavenumber
+            
+        """
+
+        f = omega/2/np.pi
+        X = f/self.flow_res
+        f_min,f_max = self.frequency_limits
+        
+        if np.min(f)<f_min or np.max(f)>f_max:
+            Warning("frequency out of range of the DelanyBazley model")
+            
+        if self.miki:
+            k = omega/self.c0 * (-1j) * ( 11.41*(X*1000)**(-0.618)
+                                      + 1j* (1 + 7.81*(X*1000)**(-0.618) ) )
+        else:
+            k = omega/self.c0 * (-1j) * ( 10.3*(X*1000)**(-0.59)
+                                            + 1j* ( 1 + 10.8*(X*1000)**(-0.70) ) )
+            
+        return k
+    
+    @property
+    def frequency_limits(self):
+        """
+        Frequency limits of Delany validity range.
+
+        Returns
+        -------
+        f_min : float
+            minimum allowed frequency.
+        f_max : float
+            maximum allowed frequency.
+
+        """
+        f_min = 0.01*self.flow_res
+        f_max = 1.00*self.flow_res
+        return (f_min,f_max)
+        
+    def c_freq(self,omega = 0.):
+        """
+        Complex, frequency dependent speed of sound
+
+        Parameters
+        ----------
+        omega : float
+            Angular frequency.
+
+        Returns
+        -------
+        complex
+            speed of sound.
+
+        """
+        
+        return omega/self.wavenumber(omega)
+        
+    def rho_freq(self,omega):
+        """
+        frequency dependend density of fluid
+                
+        Parameters
+        ----------
+        omega : float
+            Angular frequency.         
+        
+        Returns
+        -------
+        complex
+            density
+            
+        """
+        
+        return self.impedance(omega)*self.wavenumber(omega)/omega
 
 class PoroElasticMat(EquivalentFluid):
     """
     The PoroElasticMat class deals porous and elastic material
 
     The material model is implemented according to Allard [All2009]_ and requires a geometry information 
     of the frame given by the EquivalentFlluid attributes and the bulk properties elastic frame matrial.
```

### Comparing `pyva-toolbox-1.2.2/pyva/properties/structuralPropertyClasses.py` & `pyva_toolbox-1.2.3/pyva/properties/structuralPropertyClasses.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/systems/SEA_system.py` & `pyva_toolbox-1.2.3/pyva/systems/SEA_system.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/systems/__init__.py` & `pyva_toolbox-1.2.3/pyva/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/systems/acoustic1Dsystems.py` & `pyva_toolbox-1.2.3/pyva/systems/acoustic1Dsystems.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/systems/acoustic3Dsystems.py` & `pyva_toolbox-1.2.3/pyva/systems/acoustic3Dsystems.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/systems/acousticRadiators.py` & `pyva_toolbox-1.2.3/pyva/systems/acousticRadiators.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,17 +248,115 @@
         omega : float
             angular frequency
                                
         Returns:
             radiation impedance of sphere         
         
         """
-        kr = self.fluid.wavenumber(omega)*self.radius
-        return 1j*self.fluid.impedance(omega)*kr/(1+1j*kr)
+        area = 4*np.pi*self.radius**2
+        return self.acoustic_impedance(omega,self.radius)/area
     
+    def velocity_potential(self,omega,dist,Q=1.):
+        """
+        Velocity potential of breathing sphere
+
+        Parameters
+        ----------
+        omega : float
+            angular frequency.
+        dist : float
+            distance to sphere center.
+        Q : complex or nd.array of complex, optional
+            Source streng in volume flow rate, volume per time. The default is 1. .
+
+        Returns
+        -------
+        complex or nd.array of complex
+            velocity potential.
+
+        """
+
+        k = self.fluid.wavenumber(omega)
+        c_1 = -Q/4/np.pi/dist / (1 + 1j*k*self.radius)
+        
+        return c_1*np.exp(-1j*k*(dist-self.radius)) 
+    
+    
+    def pressure(self,omega,dist,Q=1.):
+        """
+        Pressure of breathing sphere
+
+        Parameters
+        ----------
+        omega : float
+            angular frequency.
+        dist : float
+            distance to sphere center.
+        Q : complex or nd.array of complex, optional
+            Source streng in volume flow rate, volume per time. The default is 1. .
+
+        Returns
+        -------
+        complex or nd.array of complex
+            pressure of breathing sphere.
+
+        """
+        
+        k = self.fluid.wavenumber(omega)
+        z0 = self.fluid.impedance(omega)
+        return -1j*k*z0*self.velocity_potential(omega,dist)
+    
+    def velocity(self,omega,dist,Q=1.):
+        """
+        Velocity of breathing sphere
+
+        Parameters
+        ----------
+        omega : float
+            angular frequency.
+        dist : float
+            distance to sphere center.
+        Q : complex or nd.array of complex, optional
+            Source streng in volume flow rate, volume per time. The default is 1. .
+
+        Returns
+        -------
+        complex or nd.array of complex
+            velocity of breathing sphere.
+
+        """
+        
+        k   = self.fluid.wavenumber(omega)
+        c_1 = -(1+1j*k*dist)/dist
+        return c_1*self.velocity_potential(omega,dist)
+    
+    def acoustic_impedance(self,omega,dist):
+        """
+        Acoustic impedance of breathing sphere
+
+        Parameters
+        ----------
+        omega : float
+            angular frequency.
+        dist : float
+            distance to sphere center.
+
+        Returns
+        -------
+        complex or nd.array of complex
+            acoustic impedance of sphere soud field.
+
+        """
+        kr = self.fluid.wavenumber(omega)*dist
+        z0 = self.fluid.impedance(omega)
+        
+        return 1j*z0*kr/(1+1j*kr)
+        
+        
+                
 class Monopole:
     """
     The Monopole class defines an acoustic momopole
     
     Attributes:
             Q:   Source strength in volume flow rate amplitude Q = dV/dt
         fluid:   fluid of free space
```

### Comparing `pyva-toolbox-1.2.2/pyva/systems/infiniteLayers.py` & `pyva_toolbox-1.2.3/pyva/systems/infiniteLayers.py`

 * *Files 0% similar despite different names*

```diff
@@ -940,15 +940,15 @@
     
     Attributes
     ----------
     thickness : float
         thickness of the layer
     rho : float
         Density.
-    perforation : PerforatedLayer
+    perforation : ResistiveLayer
         optional additional perforation of the plate 
     
     ID : list of int
         [left ID, right ID] of MassLayer
     """
     
     def __init__(self,thickness,rho,perforation=None):
@@ -957,15 +957,15 @@
 
         Parameters
         ----------
         thickness : float
             thickness of the layer.
         rho : float
             Density.
-        perforation : PerforatedLayer
+        perforation : ResistiveLayer
             optional additional perforation of the plate 
 
         Returns
         -------
         None.
 
         """
@@ -1081,28 +1081,28 @@
     """
     The PlateLayer class represents the infinite plate layer 
     
     Attributes
     ----------
         plate_prop : PlateProp
             plate property of layer
-        perforation : PerforatedLayer
+        perforation : ResistiveLayer
             optional additional perforation of the plate 
 
     """
     
     def __init__(self,plate_prop,perforation = None):
         """
         Class constructor for PlateLayer objects
         
         Parameters
         ----------
         plate_prop : PlateProp
             plate property of layer
-        perforation : PerforatedLayer
+        perforation : ResistiveLayer
             optional additional perforation of the plate 
         """                
         # set DOF according to ID and natural DOF of the layer
         Tdof = ('pressure','velocity')
         _left_dof = dof.DOF([0,0],[0,3],Tdof)
         _right_dof = dof.DOF([1,1],[0,3],Tdof)
                        
@@ -1616,28 +1616,28 @@
     
     Attributes
     ----------
     thickness: float
         thickness of the perforted layer
     prop: PlateProp
         property of plate modelled as 3D layer
-    perforation : PerforatedLayer
+    perforation : ResistiveLayer
         optional additional perforation of the plate 
 
     """
     
     def __init__(self,plate_prop,perforation = None):
         """
         Class contructor for ImperviousScreenLayer objects.
 
         Parameters
         ----------
         plate_prop : PlateProp
             plate property of layer
-        perforation : PerforatedLayer
+        perforation : ResistiveLayer
             optional additional perforation of the plate 
         """
                 
         # set DOF according to ID and natural DOF of the layer
         Tdof = ('velocity','velocity','stress','stress')
         _left_dof = dof.DOF([0,0,0,0],[1,3,3,5],Tdof)
         _right_dof = dof.DOF([1,1,1,1],[1,3,3,5],Tdof)
```

### Comparing `pyva-toolbox-1.2.2/pyva/systems/lumpedSystems.py` & `pyva_toolbox-1.2.3/pyva/systems/lumpedSystems.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/systems/structure1Dsystems.py` & `pyva_toolbox-1.2.3/pyva/systems/structure1Dsystems.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva/systems/structure2Dsystems.py` & `pyva_toolbox-1.2.3/pyva/systems/structure2Dsystems.py`

 * *Files identical despite different names*

### Comparing `pyva-toolbox-1.2.2/pyva_toolbox.egg-info/PKG-INFO` & `pyva_toolbox-1.2.3/pyva_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyva-toolbox
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python toolbox for vibroacoustic simulation
 Author: Dr. Alexander Peiffer
 Author-email: Alexander Peiffer <author@alexanderpeiffer.de>
 Project-URL: Homepage, https://github.com/minipief/pyva
 Project-URL: Bug Tracker, https://github.com/minipief/pyva/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `pyva-toolbox-1.2.2/pyva_toolbox.egg-info/SOURCES.txt` & `pyva_toolbox-1.2.3/pyva_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

