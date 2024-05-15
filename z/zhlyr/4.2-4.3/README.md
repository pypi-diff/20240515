# Comparing `tmp/zhlyr-4.2.tar.gz` & `tmp/zhlyr-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhlyr-4.2.tar", last modified: Wed May 15 15:06:32 2024, max compression
+gzip compressed data, was "zhlyr-4.3.tar", last modified: Wed May 15 16:42:06 2024, max compression
```

## Comparing `zhlyr-4.2.tar` & `zhlyr-4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 15:06:32.310210 zhlyr-4.2/
--rw-rw-rw-   0        0        0     4226 2024-05-15 15:06:32.309210 zhlyr-4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3411 2024-05-13 08:54:58.000000 zhlyr-4.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 15:06:32.311210 zhlyr-4.2/setup.cfg
--rw-rw-rw-   0        0        0     1151 2024-05-15 15:05:02.000000 zhlyr-4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:06:32.294545 zhlyr-4.2/zhlyr/
--rw-rw-rw-   0        0        0       92 2024-05-10 14:01:33.000000 zhlyr-4.2/zhlyr/__init__.py
--rw-rw-rw-   0        0        0     1847 2024-05-13 08:30:55.000000 zhlyr-4.2/zhlyr/recosnize.py
--rw-rw-rw-   0        0        0   486120 2024-05-15 15:06:31.000000 zhlyr-4.2/zhlyr/serialize.c
--rw-rw-rw-   0        0        0     2179 2024-05-10 18:26:37.000000 zhlyr-4.2/zhlyr/zhlyr.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:06:32.306700 zhlyr-4.2/zhlyr.egg-info/
--rw-rw-rw-   0        0        0     4226 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/top_level.txt
+drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-15 16:42:06.428885 zhlyr-4.3/
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     4083 2024-05-15 16:42:06.421884 zhlyr-4.3/PKG-INFO
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     3411 2024-05-13 08:54:58.000000 zhlyr-4.3/README.md
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)       38 2024-05-15 16:42:06.430396 zhlyr-4.3/setup.cfg
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1146 2024-05-15 16:42:04.000000 zhlyr-4.3/setup.py
+drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-15 16:42:06.322035 zhlyr-4.3/zhlyr/
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)      134 2024-05-15 16:36:48.000000 zhlyr-4.3/zhlyr/__init__.py
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1847 2024-05-13 08:30:55.000000 zhlyr-4.3/zhlyr/recosnize.py
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1931 2024-05-15 14:38:07.000000 zhlyr-4.3/zhlyr/serialize.pyx
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     2179 2024-05-10 18:26:37.000000 zhlyr-4.3/zhlyr/zhlyr.py
+drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-15 16:42:06.414858 zhlyr-4.3/zhlyr.egg-info/
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     4083 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/PKG-INFO
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)      234 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)        1 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)       32 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/requires.txt
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)        6 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/top_level.txt
```

### Comparing `zhlyr-4.2/PKG-INFO` & `zhlyr-4.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-Metadata-Version: 2.1
-Name: zhlyr
-Version: 4.2
-Summary: Python library for music handling
-Home-page: https://gaoc3.github.io/zhlyr/
-Author: Mtsky
-Author-email: secon2636@gmail.com
-License: MIT
-Keywords: lyrics,music,shazam,serialize,serializer,recognize
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: shazamio
-Requires-Dist: shazam
-Requires-Dist: cython
-
-- ## What is zhlyr?
-- **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
-
-- ## Code Area :
-
-  <details> 
-  <summary>
-  <i>⏬Install Zhlyr</i>
-  </summary>
-    
-  ```python3
-  💲pip install zhlyr
-  ```
-  ------
-  </details>
-  
-  <details>
-    <summary>
-    <i>🎵 Recognize track</i>
-    </summary>
-    <br>Recognize a track based on a file</br>
-  
-    ```python3
-    # Get full track json response object info
-  
-    import asynico
-    from zhlyr import Reconize
-    data = '/root/user/dir/simple.mp3'
-    async def get_info():
-      reco = await Reconize(data)
-      print(reco.json())
-    loop = asynico.new_event_loop()
-    loop.run_until_complete(get_info)
-  
-    # You can get respnose info as string response 
-    reco = Reconize(data)
-    print(reco.text)
-    ```
-  ------
-  
-  </details>
-  
-  <details>
-    <summary>
-    <i>🔍🎼 Get the lyrics of the track </i>
-    </summary>
-    <br>
-    
-    Get lyrics from title of the track
-    </br>
-    
-    ```python3
-    from zhlyr import ZhLyr
-    lyrics = ZhLyr.GetByTitle(title='save your trears',srt=false)
-    # :GetByTitle: `title`: str : title of the track to get trrack from it.
-    # :GetByTitle: `srt`: bool : if `true` he will return time as `srt` format.
-    # :GetByTitle: return json object
-    
-    for time , lyric in lyrics.items():
-      print(f'time {time} >>> lyric : {lyric}')
-    ```
-    
-    <br>
-    
-    Get lyrics from details of track
-    </br>
-    ```python3
-    lyrics = ZhLyr.GetByDetails(title='save your trears',artist='the weeknd',duration='3:35',srt=false)
-    # :GetByDetails: `title`: str : title of the track to get trrack from it.
-    # :GetByDetails: `artist`: str : artist of the track to get lyrics from it.
-    # :GetByDetails: `duration` : Optional[str]=None : duration of the track to get lyrics from it.
-    # :GetByDetails: `srt`: bool : if `true` he will return time as `srt` format.
-    # :GetByDetails: return json object
-    
-    for time , lyric in lyrics.items():
-      print(f'time {time} >>> lyric : {lyric}')
-    ```
-  ------
-  </details>
-  
-  <details>
-    
-  
-  
-    <summary>
-      <i>ℹ️ How to use data serialization </i>
-    </summary>
-    <br>
-    
-    Serialized data from response.
-    </br>
-    
-    ```python3
-    from zhlyr import Serializer
-    data = your_json_data
-    serialize = Serializer(data)
-    print(serialize)
-    ```
-    <br>
-    
-    Get vlue from key with serialized data.
-    </br>
-  
-    ```python3
-    data = {'key1':'hello world!'}
-    serialize = Serializer(data)
-    print(serialize.key1)
-    ```
-  ------
-  
-  </details>
-
-
-## My Accounts
-- [GitHub](https://github.com/Gaoc3/) [<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub" width="20" height="20">](https://github.com/)
-- [Instagram](https://www.instagram.com/mtsky.sensei/) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" width="20" height="20">](https://www.instagram.com/)
-- [Telegram](https://nar4nar.t.me) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram" width="20" height="20">](https://web.telegram.org/)
-  
-------
+Metadata-Version: 2.1
+Name: zhlyr
+Version: 4.3
+Summary: Python library for music handling
+Home-page: https://gaoc3.github.io/zhlyr/
+Author: Mtsky
+Author-email: secon2636@gmail.com
+License: MIT
+Keywords: lyrics,music,shazam,serialize,serializer,recognize
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: shazamio
+Requires-Dist: shazam
+Requires-Dist: cython
+
+- ## What is zhlyr?
+- **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
+
+- ## Code Area :
+
+  <details> 
+  <summary>
+  <i>⏬Install Zhlyr</i>
+  </summary>
+    
+  ```python3
+  💲pip install zhlyr
+  ```
+  ------
+  </details>
+  
+  <details>
+    <summary>
+    <i>🎵 Recognize track</i>
+    </summary>
+    <br>Recognize a track based on a file</br>
+  
+    ```python3
+    # Get full track json response object info
+  
+    import asynico
+    from zhlyr import Reconize
+    data = '/root/user/dir/simple.mp3'
+    async def get_info():
+      reco = await Reconize(data)
+      print(reco.json())
+    loop = asynico.new_event_loop()
+    loop.run_until_complete(get_info)
+  
+    # You can get respnose info as string response 
+    reco = Reconize(data)
+    print(reco.text)
+    ```
+  ------
+  
+  </details>
+  
+  <details>
+    <summary>
+    <i>🔍🎼 Get the lyrics of the track </i>
+    </summary>
+    <br>
+    
+    Get lyrics from title of the track
+    </br>
+    
+    ```python3
+    from zhlyr import ZhLyr
+    lyrics = ZhLyr.GetByTitle(title='save your trears',srt=false)
+    # :GetByTitle: `title`: str : title of the track to get trrack from it.
+    # :GetByTitle: `srt`: bool : if `true` he will return time as `srt` format.
+    # :GetByTitle: return json object
+    
+    for time , lyric in lyrics.items():
+      print(f'time {time} >>> lyric : {lyric}')
+    ```
+    
+    <br>
+    
+    Get lyrics from details of track
+    </br>
+    ```python3
+    lyrics = ZhLyr.GetByDetails(title='save your trears',artist='the weeknd',duration='3:35',srt=false)
+    # :GetByDetails: `title`: str : title of the track to get trrack from it.
+    # :GetByDetails: `artist`: str : artist of the track to get lyrics from it.
+    # :GetByDetails: `duration` : Optional[str]=None : duration of the track to get lyrics from it.
+    # :GetByDetails: `srt`: bool : if `true` he will return time as `srt` format.
+    # :GetByDetails: return json object
+    
+    for time , lyric in lyrics.items():
+      print(f'time {time} >>> lyric : {lyric}')
+    ```
+  ------
+  </details>
+  
+  <details>
+    
+  
+  
+    <summary>
+      <i>ℹ️ How to use data serialization </i>
+    </summary>
+    <br>
+    
+    Serialized data from response.
+    </br>
+    
+    ```python3
+    from zhlyr import Serializer
+    data = your_json_data
+    serialize = Serializer(data)
+    print(serialize)
+    ```
+    <br>
+    
+    Get vlue from key with serialized data.
+    </br>
+  
+    ```python3
+    data = {'key1':'hello world!'}
+    serialize = Serializer(data)
+    print(serialize.key1)
+    ```
+  ------
+  
+  </details>
+
+
+## My Accounts
+- [GitHub](https://github.com/Gaoc3/) [<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub" width="20" height="20">](https://github.com/)
+- [Instagram](https://www.instagram.com/mtsky.sensei/) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" width="20" height="20">](https://www.instagram.com/)
+- [Telegram](https://nar4nar.t.me) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram" width="20" height="20">](https://web.telegram.org/)
+  
+------
```

### Comparing `zhlyr-4.2/README.md` & `zhlyr-4.3/README.md`

 * *Files identical despite different names*

### Comparing `zhlyr-4.2/setup.py` & `zhlyr-4.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from Cython.Build import cythonize
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setup(
     name='zhlyr',
-    version='4.2',
+    version='4.3',
     packages=find_packages(),
     install_requires=['requests', 'shazamio', 'shazam', 'cython'],
-    ext_modules=cythonize('zhlyr/serialize.pyx'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='Python library for music handling',
     author='Mtsky',
     author_email='secon2636@gmail.com',
     url='https://gaoc3.github.io/zhlyr/',
     license='MIT',
@@ -25,8 +24,9 @@
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     keywords=['lyrics', 'music', 'shazam', 'serialize', 'serializer', 'recognize'],
     python_requires=">=3.9",
+    package_data={"zhlyr":['serialize.pyx']}
 )
```

### Comparing `zhlyr-4.2/zhlyr/recosnize.py` & `zhlyr-4.3/zhlyr/recosnize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-4.2/zhlyr/zhlyr.py` & `zhlyr-4.3/zhlyr/zhlyr.py`

 * *Files identical despite different names*

### Comparing `zhlyr-4.2/zhlyr.egg-info/PKG-INFO` & `zhlyr-4.3/zhlyr.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-Metadata-Version: 2.1
-Name: zhlyr
-Version: 4.2
-Summary: Python library for music handling
-Home-page: https://gaoc3.github.io/zhlyr/
-Author: Mtsky
-Author-email: secon2636@gmail.com
-License: MIT
-Keywords: lyrics,music,shazam,serialize,serializer,recognize
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: shazamio
-Requires-Dist: shazam
-Requires-Dist: cython
-
-- ## What is zhlyr?
-- **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
-
-- ## Code Area :
-
-  <details> 
-  <summary>
-  <i>⏬Install Zhlyr</i>
-  </summary>
-    
-  ```python3
-  💲pip install zhlyr
-  ```
-  ------
-  </details>
-  
-  <details>
-    <summary>
-    <i>🎵 Recognize track</i>
-    </summary>
-    <br>Recognize a track based on a file</br>
-  
-    ```python3
-    # Get full track json response object info
-  
-    import asynico
-    from zhlyr import Reconize
-    data = '/root/user/dir/simple.mp3'
-    async def get_info():
-      reco = await Reconize(data)
-      print(reco.json())
-    loop = asynico.new_event_loop()
-    loop.run_until_complete(get_info)
-  
-    # You can get respnose info as string response 
-    reco = Reconize(data)
-    print(reco.text)
-    ```
-  ------
-  
-  </details>
-  
-  <details>
-    <summary>
-    <i>🔍🎼 Get the lyrics of the track </i>
-    </summary>
-    <br>
-    
-    Get lyrics from title of the track
-    </br>
-    
-    ```python3
-    from zhlyr import ZhLyr
-    lyrics = ZhLyr.GetByTitle(title='save your trears',srt=false)
-    # :GetByTitle: `title`: str : title of the track to get trrack from it.
-    # :GetByTitle: `srt`: bool : if `true` he will return time as `srt` format.
-    # :GetByTitle: return json object
-    
-    for time , lyric in lyrics.items():
-      print(f'time {time} >>> lyric : {lyric}')
-    ```
-    
-    <br>
-    
-    Get lyrics from details of track
-    </br>
-    ```python3
-    lyrics = ZhLyr.GetByDetails(title='save your trears',artist='the weeknd',duration='3:35',srt=false)
-    # :GetByDetails: `title`: str : title of the track to get trrack from it.
-    # :GetByDetails: `artist`: str : artist of the track to get lyrics from it.
-    # :GetByDetails: `duration` : Optional[str]=None : duration of the track to get lyrics from it.
-    # :GetByDetails: `srt`: bool : if `true` he will return time as `srt` format.
-    # :GetByDetails: return json object
-    
-    for time , lyric in lyrics.items():
-      print(f'time {time} >>> lyric : {lyric}')
-    ```
-  ------
-  </details>
-  
-  <details>
-    
-  
-  
-    <summary>
-      <i>ℹ️ How to use data serialization </i>
-    </summary>
-    <br>
-    
-    Serialized data from response.
-    </br>
-    
-    ```python3
-    from zhlyr import Serializer
-    data = your_json_data
-    serialize = Serializer(data)
-    print(serialize)
-    ```
-    <br>
-    
-    Get vlue from key with serialized data.
-    </br>
-  
-    ```python3
-    data = {'key1':'hello world!'}
-    serialize = Serializer(data)
-    print(serialize.key1)
-    ```
-  ------
-  
-  </details>
-
-
-## My Accounts
-- [GitHub](https://github.com/Gaoc3/) [<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub" width="20" height="20">](https://github.com/)
-- [Instagram](https://www.instagram.com/mtsky.sensei/) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" width="20" height="20">](https://www.instagram.com/)
-- [Telegram](https://nar4nar.t.me) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram" width="20" height="20">](https://web.telegram.org/)
-  
-------
+Metadata-Version: 2.1
+Name: zhlyr
+Version: 4.3
+Summary: Python library for music handling
+Home-page: https://gaoc3.github.io/zhlyr/
+Author: Mtsky
+Author-email: secon2636@gmail.com
+License: MIT
+Keywords: lyrics,music,shazam,serialize,serializer,recognize
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: shazamio
+Requires-Dist: shazam
+Requires-Dist: cython
+
+- ## What is zhlyr?
+- **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
+
+- ## Code Area :
+
+  <details> 
+  <summary>
+  <i>⏬Install Zhlyr</i>
+  </summary>
+    
+  ```python3
+  💲pip install zhlyr
+  ```
+  ------
+  </details>
+  
+  <details>
+    <summary>
+    <i>🎵 Recognize track</i>
+    </summary>
+    <br>Recognize a track based on a file</br>
+  
+    ```python3
+    # Get full track json response object info
+  
+    import asynico
+    from zhlyr import Reconize
+    data = '/root/user/dir/simple.mp3'
+    async def get_info():
+      reco = await Reconize(data)
+      print(reco.json())
+    loop = asynico.new_event_loop()
+    loop.run_until_complete(get_info)
+  
+    # You can get respnose info as string response 
+    reco = Reconize(data)
+    print(reco.text)
+    ```
+  ------
+  
+  </details>
+  
+  <details>
+    <summary>
+    <i>🔍🎼 Get the lyrics of the track </i>
+    </summary>
+    <br>
+    
+    Get lyrics from title of the track
+    </br>
+    
+    ```python3
+    from zhlyr import ZhLyr
+    lyrics = ZhLyr.GetByTitle(title='save your trears',srt=false)
+    # :GetByTitle: `title`: str : title of the track to get trrack from it.
+    # :GetByTitle: `srt`: bool : if `true` he will return time as `srt` format.
+    # :GetByTitle: return json object
+    
+    for time , lyric in lyrics.items():
+      print(f'time {time} >>> lyric : {lyric}')
+    ```
+    
+    <br>
+    
+    Get lyrics from details of track
+    </br>
+    ```python3
+    lyrics = ZhLyr.GetByDetails(title='save your trears',artist='the weeknd',duration='3:35',srt=false)
+    # :GetByDetails: `title`: str : title of the track to get trrack from it.
+    # :GetByDetails: `artist`: str : artist of the track to get lyrics from it.
+    # :GetByDetails: `duration` : Optional[str]=None : duration of the track to get lyrics from it.
+    # :GetByDetails: `srt`: bool : if `true` he will return time as `srt` format.
+    # :GetByDetails: return json object
+    
+    for time , lyric in lyrics.items():
+      print(f'time {time} >>> lyric : {lyric}')
+    ```
+  ------
+  </details>
+  
+  <details>
+    
+  
+  
+    <summary>
+      <i>ℹ️ How to use data serialization </i>
+    </summary>
+    <br>
+    
+    Serialized data from response.
+    </br>
+    
+    ```python3
+    from zhlyr import Serializer
+    data = your_json_data
+    serialize = Serializer(data)
+    print(serialize)
+    ```
+    <br>
+    
+    Get vlue from key with serialized data.
+    </br>
+  
+    ```python3
+    data = {'key1':'hello world!'}
+    serialize = Serializer(data)
+    print(serialize.key1)
+    ```
+  ------
+  
+  </details>
+
+
+## My Accounts
+- [GitHub](https://github.com/Gaoc3/) [<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub" width="20" height="20">](https://github.com/)
+- [Instagram](https://www.instagram.com/mtsky.sensei/) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" width="20" height="20">](https://www.instagram.com/)
+- [Telegram](https://nar4nar.t.me) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram" width="20" height="20">](https://web.telegram.org/)
+  
+------
```

