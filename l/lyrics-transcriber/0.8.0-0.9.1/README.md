# Comparing `tmp/lyrics_transcriber-0.8.0.tar.gz` & `tmp/lyrics_transcriber-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.8.0.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.9.1.tar", max compression
```

## Comparing `lyrics_transcriber-0.8.0.tar` & `lyrics_transcriber-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-10-10 05:22:20.821172 lyrics_transcriber-0.8.0/LICENSE
--rw-r--r--   0        0        0     3618 2023-10-10 05:22:20.821172 lyrics_transcriber-0.8.0/README.md
--rw-r--r--   0        0        0       94 2023-10-10 05:22:20.821172 lyrics_transcriber-0.8.0/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0    20568 2023-10-10 05:22:20.821172 lyrics_transcriber-0.8.0/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-10-10 05:22:20.821172 lyrics_transcriber-0.8.0/lyrics_transcriber/tuul_utils/__init__.py
--rw-r--r--   0        0        0    90376 2023-10-10 05:22:20.821172 lyrics_transcriber-0.8.0/lyrics_transcriber/tuul_utils/ass.py
--rw-r--r--   0        0        0     8887 2023-10-10 05:22:20.825173 lyrics_transcriber-0.8.0/lyrics_transcriber/tuul_utils/subtitles.py
--rw-r--r--   0        0        0      699 2023-10-10 05:22:20.825173 lyrics_transcriber-0.8.0/lyrics_transcriber/tuul_utils/timing_data.py
--rw-r--r--   0        0        0        0 2023-10-10 05:22:20.825173 lyrics_transcriber-0.8.0/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     4443 2023-10-10 05:22:20.825173 lyrics_transcriber-0.8.0/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0     1661 2023-10-10 05:22:20.825173 lyrics_transcriber-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4968 1970-01-01 00:00:00.000000 lyrics_transcriber-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3618 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/README.md
+-rw-r--r--   0        0        0       94 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0    22413 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/lyrics_transcriber/tuul_utils/__init__.py
+-rw-r--r--   0        0        0    90122 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/lyrics_transcriber/tuul_utils/ass.py
+-rw-r--r--   0        0        0    11213 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/lyrics_transcriber/tuul_utils/subtitles.py
+-rw-r--r--   0        0        0      699 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/lyrics_transcriber/tuul_utils/timing_data.py
+-rw-r--r--   0        0        0        0 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     4657 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0     1661 2023-11-15 05:04:59.975007 lyrics_transcriber-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5019 1970-01-01 00:00:00.000000 lyrics_transcriber-0.9.1/PKG-INFO
```

### Comparing `lyrics_transcriber-0.8.0/LICENSE` & `lyrics_transcriber-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.8.0/README.md` & `lyrics_transcriber-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.8.0/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.9.1/lyrics_transcriber/transcriber.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         title=None,
         genius_api_token=None,
         spotify_cookie=None,
         output_dir=None,
         cache_dir="/tmp/lyrics-transcriber-cache/",
         log_level=logging.DEBUG,
         log_formatter=None,
+        background=None,
     ):
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)
         self.log_level = log_level
         self.log_formatter = log_formatter
 
         self.log_handler = logging.StreamHandler()
@@ -42,14 +43,16 @@
 
         self.logger.debug(f"LyricsTranscriber instantiating with input file: {audio_filepath}")
 
         self.cache_dir = cache_dir
         self.output_dir = output_dir
         self.audio_filepath = audio_filepath
 
+        self.background = background
+
         self.artist = artist
         self.title = title
         self.song_known = self.artist is not None and self.title is not None
 
         self.genius_api_token = os.getenv("GENIUS_API_TOKEN", default=genius_api_token)
         self.spotify_cookie = os.getenv("SPOTIFY_COOKIE_SP_DC", default=spotify_cookie)
 
@@ -337,28 +340,15 @@
     def write_ass_file(self):
         ass_filepath = self.result_metadata["ass_subtitles_filepath"]
         self.logger.debug(f"writing ASS formatted subtitle file: {ass_filepath}")
 
         intial_screens = self.create_screens()
         screens = subtitles.set_segment_end_times(intial_screens, int(self.result_metadata["song_duration"]))
         screens = subtitles.set_screen_start_times(screens)
-        lyric_subtitles_ass = subtitles.create_subtitles(
-            screens,
-            {
-                # "FontName": "Arial Narrow",
-                # "FontSize": 20,
-                # "PrimaryColor": (255, 0, 255, 255),
-                # "SecondaryColor": (0, 255, 255, 255),
-                "FontName": "Avenir Next",
-                "FontSize": 30,
-                "PrimaryColor": (4, 51, 255, 255),
-                "SecondaryColor": (255, 255, 255, 255),
-            },
-        )
-
+        lyric_subtitles_ass = subtitles.create_styled_subtitles(screens)
         lyric_subtitles_ass.write(ass_filepath)
 
     def create_video(self):
         self.logger.debug(f"create_video attempting to generate video file: {self.result_metadata['karaoke_video_filepath']}")
 
         audio_delay = 0
         audio_delay_ms = int(audio_delay * 1000)  # milliseconds
@@ -369,42 +359,87 @@
             video_metadata.append(f"artist={self.artist}")
         if self.title:
             video_metadata.append("-metadata")
             video_metadata.append(f"title={self.title}")
 
         ffmpeg_cmd = [
             "ffmpeg",
-            # Describe a video stream that is a black background
-            "-f",
-            "lavfi",
-            "-i",
-            # "color=c=black:s=1280x720:r=20",
-            "color=c=black:s=1920x1080:r=20",
-            # "color=c=black:s=3840x2160:r=30",
+            "-r", "30",  # Set frame rate to 30 fps for the following input
+        ]
+
+        background = False
+
+        # Check if a background image is provided, else use black background
+        if self.background:
+            self.logger.debug(f"self.background set to path: {self.background}")
+            if os.path.isfile(self.background):
+                self.logger.debug(f"background is valid file path: {self.background}")
+                background = self.background
+            else:
+                self.logger.error(f"background_image is NOT valid file path, falling back to black")
+
+        # fmt: off
+        if background:
+            self.logger.debug(f"background set: {background}")
+            ffmpeg_cmd += [
+                # Use provided image as background
+                "-loop", "1",  # Loop the image
+                "-i", self.background,  # Input image file
+            ]
+        else:
+            self.logger.debug(f"background not set, using solid black background")
+            ffmpeg_cmd += [
+                # Use black color as background
+                "-f", "lavfi",
+                # "-i", "color=c=black:s=1280x720:r=20",
+                # "-i", "color=c=black:s=1920x1080:r=20",
+                "-i", "color=c=black:s=3840x2160:r=30",
+            ]
+
+        video_codec = "libx264"
+        ffmpeg_codes = subprocess.getoutput("ffmpeg -codecs")
+
+        if "h264_videotoolbox" in ffmpeg_codes:
+            video_codec = "h264_videotoolbox"
+            self.logger.info(f"video codec set to hardware accelerated h264_videotoolbox")
+        elif "h264_qsv" in ffmpeg_codes:
+            video_codec = "h264_qsv"
+            self.logger.info(f"video codec set to hardware accelerated h264_qsv")
+
+        ffmpeg_cmd += [
             # Use accompaniment track as audio
-            "-i",
-            self.audio_filepath,
+            "-i", self.audio_filepath,
             # Set audio delay if needed
             # https://ffmpeg.org/ffmpeg-filters.html#adelay
             # "-af",
             # f"adelay=delays={audio_delay_ms}:all=1",
             # Re-encode audio as mp3
-            "-c:a",
-            "aac",
+            "-c:a", "aac",
             # Add subtitles
-            "-vf",
-            "ass=" + self.result_metadata["ass_subtitles_filepath"],
+            "-vf", "ass=" + self.result_metadata["ass_subtitles_filepath"],
+            # Encode as H264 using hardware acceleration if available
+            "-c:v", video_codec,
+            # Increase output video quality
+            "-preset", "slow",  # Use a slower preset for better compression efficiency
+            # "-crf", "1",  # Lower CRF for higher quality. Adjust as needed, lower is better quality
+            "-b:v", "5000k",  # Set the video bitrate, for example, 5000 kbps
+            "-minrate", "5000k",  # Minimum bitrate
+            "-maxrate", "20000k",  # Maximum bitrate
+            "-bufsize", "10000k",  # Set the buffer size, typically 2x maxrate
             # End encoding after the shortest stream
             "-shortest",
             # Overwrite files without asking
             "-y",
+            # Only encode the first 30 seconds (for testing, fast iteration when editing this)
+            # "-t", "30",
             *video_metadata,
             # Output path of video
             self.result_metadata["karaoke_video_filepath"],
         ]
+        # fmt: on
 
         self.logger.debug(f"running ffmpeg command to generate video: {ffmpeg_cmd}")
         ffmpeg_output = subprocess.check_output(ffmpeg_cmd, universal_newlines=True)
         return ffmpeg_output
 
     def format_time_lrc(self, duration):
         minutes = int(duration // 60)
```

### Comparing `lyrics_transcriber-0.8.0/lyrics_transcriber/tuul_utils/ass.py` & `lyrics_transcriber-0.9.1/lyrics_transcriber/tuul_utils/ass.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,22 +141,15 @@
         def tag_argument_to_number(cls, arg, default_value=None):
             match = cls.__re_tag_number.match(arg)
             if match is None:
                 return default_value
             return float(match.group(1))
 
     class Style:
-        aliases = {
-            "PrimaryColour": "PrimaryColor",
-            "SecondaryColour": "SecondaryColor",
-            "TertiaryColor": "OutlineColor",
-            "TertiaryColour": "OutlineColor",
-            "OutlineColour": "OutlineColor",
-            "BackColour": "BackColor",
-        }
+        aliases = {}
         formatters = None
         order = [
             "Name",
             "Fontname",
             "Fontsize",
             "PrimaryColour",
             "SecondaryColour",
@@ -184,18 +177,18 @@
         def __init__(self):
             self.type = None
             self.fake = False
 
             self.Name = ""
             self.Fontname = ""
             self.Fontsize = 1.0
-            self.PrimaryColor = (255, 255, 255, 255)
-            self.SecondaryColor = (255, 255, 255, 255)
-            self.OutlineColor = (255, 255, 255, 255)
-            self.BackColor = (255, 255, 255, 255)
+            self.PrimaryColour = (255, 255, 255, 255)
+            self.SecondaryColour = (255, 255, 255, 255)
+            self.OutlineColour = (255, 255, 255, 255)
+            self.BackColour = (255, 255, 255, 255)
             self.Bold = False
             self.Italic = False
             self.Underline = False
             self.StrikeOut = False
             self.ScaleX = 100
             self.ScaleY = 100
             self.Spacing = 0
@@ -245,18 +238,18 @@
                 obj2 = other
 
             obj1.type = obj2.type
 
             obj1.Name = obj2.Name
             obj1.Fontname = obj2.Fontname
             obj1.Fontsize = obj2.Fontsize
-            obj1.PrimaryColor = obj2.PrimaryColor
-            obj1.SecondaryColor = obj2.SecondaryColor
-            obj1.OutlineColor = obj2.OutlineColor
-            obj1.BackColor = obj2.BackColor
+            obj1.PrimaryColour = obj2.PrimaryColour
+            obj1.SecondaryColour = obj2.SecondaryColour
+            obj1.OutlineColour = obj2.OutlineColour
+            obj1.BackColour = obj2.BackColour
             obj1.Bold = obj2.Bold
             obj1.Italic = obj2.Italic
             obj1.Underline = obj2.Underline
             obj1.StrikeOut = obj2.StrikeOut
             obj1.ScaleX = obj2.ScaleX
             obj1.ScaleY = obj2.ScaleY
             obj1.Spacing = obj2.Spacing
@@ -277,18 +270,18 @@
                 self.type == other.type
                 and not self.fake
                 and not other.fake
                 and not other.fake
                 and (names_can_differ or self.Name == other.Name)
                 and self.Fontname == other.Fontname
                 and self.Fontsize == other.Fontsize
-                and self.PrimaryColor == other.PrimaryColor
-                and self.SecondaryColor == other.SecondaryColor
-                and self.OutlineColor == other.OutlineColor
-                and self.BackColor == other.BackColor
+                and self.PrimaryColour == other.PrimaryColour
+                and self.SecondaryColour == other.SecondaryColour
+                and self.OutlineColour == other.OutlineColour
+                and self.BackColour == other.BackColour
                 and self.Bold == other.Bold
                 and self.Italic == other.Italic
                 and self.Underline == other.Underline
                 and self.StrikeOut == other.StrikeOut
                 and self.ScaleX == other.ScaleX
                 and self.ScaleY == other.ScaleY
                 and self.Spacing == other.Spacing
@@ -303,18 +296,18 @@
                 and self.Encoding == other.Encoding
             )
 
     Style.formatters = {
         "Name": (Formatters.same, Formatters.same),
         "Fontname": (Formatters.same, Formatters.same),
         "Fontsize": (Formatters.str_to_number, Formatters.number_to_str),
-        "PrimaryColor": (Formatters.str_to_color, Formatters.color_to_str),
-        "SecondaryColor": (Formatters.str_to_color, Formatters.color_to_str),
-        "OutlineColor": (Formatters.str_to_color, Formatters.color_to_str),
-        "BackColor": (Formatters.str_to_color, Formatters.color_to_str),
+        "PrimaryColour": (Formatters.str_to_color, Formatters.color_to_str),
+        "SecondaryColour": (Formatters.str_to_color, Formatters.color_to_str),
+        "OutlineColour": (Formatters.str_to_color, Formatters.color_to_str),
+        "BackColour": (Formatters.str_to_color, Formatters.color_to_str),
         "Bold": (Formatters.str_to_n1bool, Formatters.n1bool_to_str),
         "Italic": (Formatters.str_to_n1bool, Formatters.n1bool_to_str),
         "Underline": (Formatters.str_to_n1bool, Formatters.n1bool_to_str),
         "StrikeOut": (Formatters.str_to_n1bool, Formatters.n1bool_to_str),
         "ScaleX": (Formatters.str_to_integer, Formatters.integer_to_str),
         "ScaleY": (Formatters.str_to_integer, Formatters.integer_to_str),
         "Spacing": (Formatters.str_to_integer, Formatters.integer_to_str),
```

### Comparing `lyrics_transcriber-0.8.0/lyrics_transcriber/tuul_utils/timing_data.py` & `lyrics_transcriber-0.9.1/lyrics_transcriber/tuul_utils/timing_data.py`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.8.0/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.9.1/lyrics_transcriber/utils/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 
     parser.add_argument(
         "--output_dir",
         default=None,
         help="Optional: directory where the output lyrics files will be saved. Default: current directory",
     )
 
+    parser.add_argument(
+        "--background",
+        default=None,
+        help="Optional: image file path to use for karaoke video background. Default: solid black",
+    )
+
     args = parser.parse_args()
 
     log_level = getattr(logging, args.log_level.upper())
     logger.setLevel(log_level)
 
     if not hasattr(args, "audio_filepath"):
         parser.print_help()
@@ -80,14 +86,15 @@
         spotify_cookie=args.spotify_cookie,
         artist=args.artist,
         title=args.title,
         output_dir=args.output_dir,
         cache_dir=args.cache_dir,
         log_formatter=log_formatter,
         log_level=log_level,
+        background=args.background,
     )
 
     result_metadata = transcriber.generate()
 
     logger.info(f"*** Success! ***")
 
     formatted_duration = f'{int(result_metadata["song_duration"] // 60):02d}:{int(result_metadata["song_duration"] % 60):02d}'
```

### Comparing `lyrics_transcriber-0.8.0/pyproject.toml` & `lyrics_transcriber-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.8.0"
+version = "0.9.1"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lyrics_transcriber" }]
 homepage = "https://github.com/karaokenerds/python-lyrics-transcriber"
 repository = "https://github.com/karaokenerds/python-lyrics-transcriber"
@@ -21,15 +21,15 @@
 onnx = "^1"
 onnxruntime = "^1"
 torch = ">1"
 tqdm = "^4"
 lyricsgenius = "^3"
 python-slugify = "^8"
 syrics = "^0"
-openai-whisper = "20230918"
+openai-whisper = "20231106"
 whisper-timestamped = "^1"
 # Note: after adding openai-whisper and whisper-timestamped with poetry lock, I then removed all traces of triton
 # from poetry.lock before running poetry install, as triton doesn't support macOS but isn't actually needed for whisper.
 # This was the only way I was able to get a working cross-platform build published to PyPI.
 # To update the lockfile and install/upgrade dependencies, modify the dependency list above then run:
 # poetry lock; patch -p0 poetry.lock <.github/removetriton.patch; poetry install
```

### Comparing `lyrics_transcriber-0.8.0/PKG-INFO` & `lyrics_transcriber-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.8.0
+Version: 0.9.1
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 Home-page: https://github.com/karaokenerds/python-lyrics-transcriber
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Cython (>=0,<1)
 Requires-Dist: dtw-python (>=1,<2)
 Requires-Dist: llvmlite (>=0,<1)
 Requires-Dist: lyricsgenius (>=3,<4)
 Requires-Dist: numba (>=0.57,<0.58)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: onnx (>=1,<2)
 Requires-Dist: onnxruntime (>=1,<2)
-Requires-Dist: openai-whisper (==20230918)
+Requires-Dist: openai-whisper (==20231106)
 Requires-Dist: python-slugify (>=8,<9)
 Requires-Dist: syrics (>=0,<1)
 Requires-Dist: torch (>1)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: whisper-timestamped (>=1,<2)
 Project-URL: Documentation, https://github.com/karaokenerds/python-lyrics-transcriber/blob/main/README.md
 Project-URL: Repository, https://github.com/karaokenerds/python-lyrics-transcriber
```

