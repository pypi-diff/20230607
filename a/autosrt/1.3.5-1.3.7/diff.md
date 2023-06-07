# Comparing `tmp/autosrt-1.3.5.tar.gz` & `tmp/autosrt-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.3.5.tar", last modified: Tue Jun  6 21:19:03 2023, max compression
+gzip compressed data, was "autosrt-1.3.7.tar", last modified: Wed Jun  7 14:09:16 2023, max compression
```

## Comparing `autosrt-1.3.5.tar` & `autosrt-1.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 21:19:03.197996 autosrt-1.3.5/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.5/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-06 21:19:03.198746 autosrt-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 21:19:03.161617 autosrt-1.3.5/autosrt/
--rw-rw-rw-   0        0        0   116952 2023-06-06 21:18:37.000000 autosrt-1.3.5/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:19:03.186008 autosrt-1.3.5/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-06 21:19:03.000000 autosrt-1.3.5/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-06 21:19:03.201744 autosrt-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:19:03.196498 autosrt-1.3.5/test/
--rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.3.5/test/test1.py
--rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.3.5/test/test2.py
--rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.3.5/test/test3.py
--rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.5/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:09:16.054965 autosrt-1.3.7/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.7/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-06-07 14:09:16.055714 autosrt-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 14:09:15.537890 autosrt-1.3.7/autosrt/
+-rw-rw-rw-   0        0        0   117283 2023-06-07 14:06:40.000000 autosrt-1.3.7/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:09:15.850084 autosrt-1.3.7/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-07 14:09:14.000000 autosrt-1.3.7/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-07 14:09:14.000000 autosrt-1.3.7/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:09:14.000000 autosrt-1.3.7/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-07 14:09:14.000000 autosrt-1.3.7/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-07 14:09:14.000000 autosrt-1.3.7/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 14:09:14.000000 autosrt-1.3.7/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-07 14:09:16.109657 autosrt-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:09:16.051967 autosrt-1.3.7/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.3.7/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.3.7/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.3.7/test/test3.py
+-rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.7/test/test4.py
```

### Comparing `autosrt-1.3.5/LICENSE` & `autosrt-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.5/PKG-INFO` & `autosrt-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.5
+Version: 1.3.7
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.5/README.md` & `autosrt-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.5/autosrt/__init__.py` & `autosrt-1.3.7/autosrt/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,281 +23,15 @@
 from glob import glob, escape
 import time
 from datetime import datetime, timedelta
 from pathlib import Path
 import shlex
 import shutil
 
-VERSION = "1.3.5"
-
-
-#======================================================== ffmpeg_progress_yield ========================================================#
-
-
-import re
-#import subprocess
-from typing import Any, Callable, Iterator, List, Optional, Union
-
-
-def to_ms(**kwargs: Union[float, int, str]) -> int:
-    hour = int(kwargs.get("hour", 0))
-    minute = int(kwargs.get("min", 0))
-    sec = int(kwargs.get("sec", 0))
-    ms = int(kwargs.get("ms", 0))
-
-    return (hour * 60 * 60 * 1000) + (minute * 60 * 1000) + (sec * 1000) + ms
-
-
-def _probe_duration(cmd: List[str]) -> Optional[int]:
-    '''
-    Get the duration via ffprobe from input media file
-    in case ffmpeg was run with loglevel=error.
-
-    Args:
-        cmd (List[str]): A list of command line elements, e.g. ["ffmpeg", "-i", ...]
-
-    Returns:
-        Optional[int]: The duration in milliseconds.
-    '''
-
-    def _get_file_name(cmd: List[str]) -> Optional[str]:
-        try:
-            idx = cmd.index("-i")
-            return cmd[idx + 1]
-        except ValueError:
-            return None
-
-    file_name = _get_file_name(cmd)
-    if file_name is None:
-        return None
-
-    try:
-        if sys.platform == "win32":
-            output = subprocess.check_output(
-                [
-                    "ffprobe",
-                    "-loglevel",
-                    "-1",
-                    "-hide_banner",
-                    "-show_entries",
-                    "format=duration",
-                    "-of",
-                    "default=noprint_wrappers=1:nokey=1",
-                    file_name,
-                ],
-                universal_newlines=True,
-                creationflags=subprocess.CREATE_NO_WINDOW,
-            )
-        else:
-            output = subprocess.check_output(
-                [
-                    "ffprobe",
-                    "-loglevel",
-                    "-1",
-                    "-hide_banner",
-                    "-show_entries",
-                    "format=duration",
-                    "-of",
-                    "default=noprint_wrappers=1:nokey=1",
-                    file_name,
-                ],
-                universal_newlines=True,
-            )
-
-        return int(float(output.strip()) * 1000)
-    except Exception:
-        # TODO: add logging
-        return None
-
-
-def _uses_error_loglevel(cmd: List[str]) -> bool:
-    try:
-        idx = cmd.index("-loglevel")
-        if cmd[idx + 1] == "error":
-            return True
-        else:
-            return False
-    except ValueError:
-        return False
-
-
-class FfmpegProgress:
-    DUR_REGEX = re.compile(
-        r"Duration: (?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
-    )
-    TIME_REGEX = re.compile(
-        r"out_time=(?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
-    )
-
-    def __init__(self, cmd: List[str], dry_run: bool = False) -> None:
-        '''Initialize the FfmpegProgress class.
-
-        Args:
-            cmd (List[str]): A list of command line elements, e.g. ["ffmpeg", "-i", ...]
-            dry_run (bool, optional): Only show what would be done. Defaults to False.
-        '''
-        self.cmd = cmd
-        self.stderr: Union[str, None] = None
-        self.dry_run = dry_run
-        self.process: Any = None
-        self.stderr_callback: Union[Callable[[str], None], None] = None
-        if sys.platform == "win32":
-            self.base_popen_kwargs = {
-                "stdin": subprocess.PIPE,  # Apply stdin isolation by creating separate pipe.
-                "stdout": subprocess.PIPE,
-                "stderr": subprocess.STDOUT,
-                "universal_newlines": False,
-                "shell": True,
-            }
-        else:
-            self.base_popen_kwargs = {
-                "stdin": subprocess.PIPE,  # Apply stdin isolation by creating separate pipe.
-                "stdout": subprocess.PIPE,
-                "stderr": subprocess.STDOUT,
-                "universal_newlines": False,
-            }
-
-    def set_stderr_callback(self, callback: Callable[[str], None]) -> None:
-        '''
-        Set a callback function to be called on stderr output.
-        The callback function must accept a single string argument.
-        Note that this is called on every line of stderr output, so it can be called a lot.
-        Also note that stdout/stderr are joined into one stream, so you might get stdout output in the callback.
-
-        Args:
-            callback (Callable[[str], None]): A callback function that accepts a single string argument.
-        '''
-        if not callable(callback) or len(callback.__code__.co_varnames) != 1:
-            raise ValueError(
-                "Callback must be a function that accepts only one argument"
-            )
-
-        self.stderr_callback = callback
-
-    def run_command_with_progress(
-        self, popen_kwargs=None, duration_override: Union[float, None] = None
-    ) -> Iterator[int]:
-        '''
-        Run an ffmpeg command, trying to capture the process output and calculate
-        the duration / progress.
-        Yields the progress in percent.
-
-        Args:
-            popen_kwargs (dict, optional): A dict to specify extra arguments to the popen call, e.g. { creationflags: CREATE_NO_WINDOW }
-            duration_override (float, optional): The duration in seconds. If not specified, it will be calculated from the ffmpeg output.
-
-        Raises:
-            RuntimeError: If the command fails, an exception is raised.
-
-        Yields:
-            Iterator[int]: A generator that yields the progress in percent.
-        '''
-        if self.dry_run:
-            return self.cmd
-
-        total_dur: Union[None, int] = None
-        if _uses_error_loglevel(self.cmd):
-            total_dur = _probe_duration(self.cmd)
-
-        cmd_with_progress = (
-            [self.cmd[0]] + ["-progress", "-", "-nostats"] + self.cmd[1:]
-        )
-
-        stderr = []
-        base_popen_kwargs = self.base_popen_kwargs.copy()
-        if popen_kwargs is not None:
-            base_popen_kwargs.update(popen_kwargs)
-
-        if sys.platform == "wind32":
-            self.process = subprocess.Popen(
-                cmd_with_progress,
-                **base_popen_kwargs,
-                creationflags=subprocess.CREATE_NO_WINDOW,
-            )  # type: ignore
-        else:
-            self.process = subprocess.Popen(
-                cmd_with_progress,
-                **base_popen_kwargs,
-            )  # type: ignore
-
-        yield 0
-
-        while True:
-            if self.process.stdout is None:
-                continue
-
-            stderr_line = (
-                self.process.stdout.readline().decode("utf-8", errors="replace").strip()
-            )
-
-            if self.stderr_callback:
-                self.stderr_callback(stderr_line)
-
-            if stderr_line == '' and self.process.poll() is not None:
-                break
-
-            stderr.append(stderr_line.strip())
-
-            self.stderr = "\n".join(stderr)
-
-            if total_dur is None:
-                total_dur_match = self.DUR_REGEX.search(stderr_line)
-                if total_dur_match:
-                    total_dur = to_ms(**total_dur_match.groupdict())
-                    continue
-                elif duration_override is not None:
-                    # use the override (should apply in the first loop)
-                    total_dur = int(duration_override * 1000)
-                    continue
-
-            if total_dur:
-                progress_time = FfmpegProgress.TIME_REGEX.search(stderr_line)
-                if progress_time:
-                    elapsed_time = to_ms(**progress_time.groupdict())
-                    yield int(elapsed_time * 100/ total_dur)
-
-        if self.process is None or self.process.returncode != 0:
-            #print(self.process)
-            #print(self.process.returncode)
-            _pretty_stderr = "\n".join(stderr)
-            raise RuntimeError(f"Error running command {self.cmd}: {_pretty_stderr}")
-
-        yield 100
-        self.process = None
-
-    def quit_gracefully(self) -> None:
-        '''
-        Quit the ffmpeg process by sending 'q'
-
-        Raises:
-            RuntimeError: If no process is found.
-        '''
-        if self.process is None:
-            raise RuntimeError("No process found. Did you run the command?")
-
-        self.process.communicate(input=b"q")
-        self.process.kill()
-        self.process = None
-
-    def quit(self) -> None:
-        '''
-        Quit the ffmpeg process by sending SIGKILL.
-
-        Raises:
-            RuntimeError: If no process is found.
-        '''
-        if self.process is None:
-            raise RuntimeError("No process found. Did you run the command?")
-
-        self.process.kill()
-        self.process = None
-
-
-#=======================================================================================================================================#
-
+VERSION = "1.3.7"
 
 def stop_ffmpeg_windows(error_messages_callback=None):
     try:
         tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
         ffmpeg_pid = None
         for line in tasklist_output.split('\n'):
             if "ffmpeg" in line:
@@ -1151,38 +885,67 @@
         if not self.ffmpeg_check():
             if self.error_messages_callback:
                 self.error_messages_callback("ffmpeg: Executable not found on machine.")
             else:
                 print("ffmpeg: Executable not found on machine.")
                 raise Exception("Dependency not found: ffmpeg")
 
-        command = [
-                    "ffmpeg",
-                    "-y",
-                    "-i", media_filepath,
-                    "-ac", str(self.channels),
-                    "-ar", str(self.rate),
-                    "-loglevel", "error",
-                    "-hide_banner",
-                    temp.name
-                  ]
+        ffmpeg_command = [
+                            "ffmpeg",
+                            "-y",
+                            "-i", media_filepath,
+                            "-ac", str(self.channels),
+                            "-ar", str(self.rate),
+                            "-loglevel", "error",
+                            "-hide_banner",
+                            temp.name
+                         ]
 
         try:
             # RUNNING ffmpeg WITHOUT SHOWING PROGRESSS
             #use_shell = True if os.name == "nt" else False
             #subprocess.check_output(command, stdin=open(os.devnull), shell=use_shell)
 
+            '''
             # RUNNING ffmpeg WITH PROGRESSS
             ff = FfmpegProgress(command)
             percentage = 0
             for progress in ff.run_command_with_progress():
                 percentage = progress
                 if self.progress_callback:
                     self.progress_callback(media_filepath, percentage)
             temp.close()
+            '''
+
+            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+            else:
+                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+
+            if sys.platform == "win32":
+                process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+            else:
+                process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+
+            for line in process.stdout:
+                if "time=" in line:
+                    #print(line)
+                    time_str = line.split("time=")[1].split()[0]
+                    #print("time_str = %s" %time_str)
+                    current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+                    #print("current_duration = %s" %current_duration)
+                    if current_duration>0:
+                        percentage = int(current_duration*100/total_duration)
+                        if self.progress_callback:
+                            self.progress_callback(media_filepath, percentage)
+
+            temp.close()
 
             return temp.name, self.rate
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
                 self.error_messages_callback("Cancelling all tasks")
             else:
@@ -1745,17 +1508,17 @@
                 exe_file = os.path.join(path, program)
                 if is_exe(exe_file):
                     return exe_file
         return None
 
     @staticmethod
     def ffmpeg_check():
-        if WavConverter.which("ffmpeg"):
+        if MediaSubtitleRenderer.which("ffmpeg"):
             return "ffmpeg"
-        if WavConverter.which("ffmpeg.exe"):
+        if MediaSubtitleRenderer.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
     def __init__(self, subtitle_path=None, language="eng", output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
         self.language = language
         self.output_path = output_path
@@ -1797,21 +1560,38 @@
                                 "-scodec", "mov_text",
                                 "-metadata:s:s:0",
                                 f"language={shlex.quote(self.language)}",
                                 "-f", "mp4",
                                 "-y", self.output_path
                              ]
 
+            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+            else:
+                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
-            ff = FfmpegProgress(ffmpeg_command)
-            percentage = 0
-            for progress in ff.run_command_with_progress():
-                percentage = progress
-                if self.progress_callback:
-                    self.progress_callback(media_filepath, percentage)
+            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+
+            if sys.platform == "win32":
+                process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+            else:
+                process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+
+            for line in process.stdout:
+                if "time=" in line:
+                    #print(line)
+                    time_str = line.split("time=")[1].split()[0]
+                    #print("time_str = %s" %time_str)
+                    current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+                    #print("current_duration = %s" %current_duration)
+                    if current_duration>0:
+                        percentage = int(current_duration*100/total_duration)
+                        if self.progress_callback:
+                            self.progress_callback(media_filepath, percentage)
 
             if os.path.isfile(self.output_path):
                 return self.output_path
             else:
                 return None
 
         except KeyboardInterrupt:
@@ -1844,39 +1624,46 @@
                 exe_file = os.path.join(path, program)
                 if is_exe(exe_file):
                     return exe_file
         return None
 
     @staticmethod
     def ffmpeg_check():
-        if WavConverter.which("ffmpeg"):
+        if MediaSubtitleEmbedder.which("ffmpeg"):
             return "ffmpeg"
-        if WavConverter.which("ffmpeg.exe"):
+        if MediaSubtitleEmbedder.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
     def __init__(self, subtitle_path=None, language="eng", output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
         self.language = language
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
     def get_existing_subtitle_language(self, media_filepath):
         # Run ffprobe to get stream information
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
         command = [
                     'ffprobe',
                     '-v', 'quiet',
                     '-of', 'json',
                     '-show_entries',
                     'format:stream',
                     media_filepath
                   ]
 
-        output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, universal_newlines=True)
+        if sys.platform == "win32":
+            output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, universal_newlines=True)
+        else:
+            output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
+
         metadata = json.loads(output.stdout)
         streams = metadata['streams']
 
         # Find the subtitle stream with language metadata
         subtitle_languages = []
         for stream in streams:
             if stream['codec_type'] == 'subtitle' and 'tags' in stream and 'language' in stream['tags']:
@@ -1906,21 +1693,21 @@
                 self.error_messages_callback("ffmpeg: Executable not found on machine.")
             else:
                 print("ffmpeg: Executable not found on machine.")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             existing_languages = self.get_existing_subtitle_language(media_filepath)
-            print("existing_languages = {}".format(existing_languages))
             if self.language in existing_languages:
-                msg = (f"'{self.language}' subtitle stream already existed in {media_filepath}")
-                if self.error_messages_callback:
-                    self.error_messages_callback(msg)
-                else:
-                    print(msg)
+                # THIS 'print' THINGS WILL MAKE progresbar screwed up!
+                #msg = (f"'{self.language}' subtitle stream already existed in {media_filepath}")
+                #if self.error_messages_callback:
+                #    self.error_messages_callback(msg)
+                #else:
+                #    print(msg)
                 return
 
             else:
                 # Determine the next available subtitle index
                 next_index = len(existing_languages)
 
                 ffmpeg_command = [
@@ -1934,20 +1721,55 @@
                                     '-scodec', 'mov_text',
                                     '-metadata:s:s:' + str(next_index), f'language={shlex.quote(self.language)}',
                                     '-map', '0',
                                     '-map', '1',
                                     self.output_path
                                  ]
 
+
+                '''
+                # USING ffmpeg_progress_yield MODULE
                 ff = FfmpegProgress(ffmpeg_command)
                 percentage = 0
                 for progress in ff.run_command_with_progress():
                     percentage = progress
                     if self.progress_callback:
                         self.progress_callback(media_filepath, percentage)
+                '''
+
+                # WITHOUT USING ffmpeg_progress_yield MODULE
+                ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+                if sys.platform == "win32":
+                    ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                else:
+                    ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+                total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+
+                if sys.platform == "win32":
+                    process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                else:
+                    process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+
+                for line in process.stdout:
+                    if "time=" in line:
+                        #print(line)
+                        time_str = line.split("time=")[1].split()[0]
+                        #print("time_str = %s" %time_str)
+                        current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+                        #print("current_duration = %s" %current_duration)
+                        if current_duration>0:
+                            percentage = int(current_duration*100/total_duration)
+                            if self.progress_callback:
+                                self.progress_callback(media_filepath, percentage)
+
+                if os.path.isfile(self.output_path):
+                    return self.output_path
+                else:
+                    return None
 
                 if os.path.isfile(self.output_path):
                     return self.output_path
                 else:
                     return None
 
         except KeyboardInterrupt:
@@ -2088,15 +1910,15 @@
 
         ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
         ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         total_duration = float(ffprobe_process.stdout.read().decode().strip())
 
         ffmpeg_command = f'ffmpeg -y -i "{media_filepath}" -vf "subtitles={shlex.quote(subtitle_path)}" "{output_path}"'
 
-        widgets = [f"Rendering subtitles with {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+        widgets = [f"Rendering subtitles into {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
         pbar = ProgressBar(widgets=widgets, maxval=100).start()
         percentage = 0
 
         if sys.platform == "win32":
             process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
         else:
             process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
@@ -2140,16 +1962,20 @@
             return
 
         else:
             # Determine the next available subtitle index
             next_index = len(existing_languages)
 
             ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
-            ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-            total_duration = float(ffprobe_process.stdout.read().decode().strip())
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+            else:
+                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
 
             ffmpeg_command = [
                                 'ffmpeg',
                                 '-y',
                                 '-i', media_filepath,
                                 '-sub_charenc', 'UTF-8',
                                 '-i', subtitle_path,
@@ -2200,15 +2026,15 @@
 
 
 def show_error_messages(messages):
     print(messages)
 
 
 def main():
-    global pbar
+    global pbar, pbar2
 
     if sys.platform == "win32":
         stop_ffmpeg_windows(error_messages_callback=show_error_messages)
     else:
         stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
     remove_temp_files("flac", error_messages_callback=show_error_messages)
@@ -2368,39 +2194,42 @@
     print("CHECKING EXISTING SUBTITLES STREAMS")
     print("===================================")
 
     if do_translate == False:
 
         for media_filepath in media_filepaths:
             ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
-            print("Checking existing '{}' subtites streams in {}".format(ffmpeg_src_language_code, media_filepath))
+            #print("Checking existing '{}' subtites streams in {}".format(ffmpeg_src_language_code, media_filepath))
+            print("Checking %s" %media_filepath)
 
             subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
             subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
             if subtitle_streams_data and subtitle_streams_data != []:
 
                 src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
                 if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                    print(f"'{ffmpeg_src_language_code}' subtitle stream already existed in {media_filepath}")
+                    #print(f"'{ffmpeg_src_language_code}' subtitle stream already existed in {media_filepath}")
+                    print("Is '%s' subtitle stream exist          : Yes" %(ffmpeg_src_language_code.center(3)))
                     subtitle_stream_regions = []
                     subtitle_stream_transcripts = []
                     for entry in src_subtitle_stream_timed_subtitles:
                         subtitle_stream_regions.append(entry[0])
                         subtitle_stream_transcripts.append(entry[1])
                     base, ext = os.path.splitext(media_filepath)
                     src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
                     writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                     print(f"Extracting '{ffmpeg_src_language_code}'subtitle stream as      : {src_subtitle_filepath}")
                     writer.write(src_subtitle_filepath)
                     removed_media_filepaths.append(media_filepath)
 
                 else:
-                    print(f"No '{ffmpeg_src_language_code}' subtitle stream found in {media_filepath}")
+                    #print(f"No '{ffmpeg_src_language_code}' subtitle stream found in {media_filepath}")
+                    print("Is '%s' subtitle stream exist          : No" %(ffmpeg_src_language_code.center(3)))
 
         print("")
 
         if removed_media_filepaths:
             for removed_media_filepath in removed_media_filepaths:
                 media_filepaths.remove(removed_media_filepath)
 
@@ -2409,67 +2238,73 @@
             sys.exit(0)
 
 
     elif do_translate == True:
 
         for media_filepath in media_filepaths:
             ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
-            print("Checking existing '{}' subtites streams in {}".format(ffmpeg_src_language_code, media_filepath))
+            #print("Checking existing '{}' subtites streams in {}".format(ffmpeg_src_language_code, media_filepath))
+            print("Checking %s" %media_filepath)
 
             subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
             subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
             if subtitle_streams_data and subtitle_streams_data != []:
 
                 src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
                 if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                    print(f"'{ffmpeg_src_language_code}' subtitle stream already existed in {media_filepath}")
+                    #print(f"'{ffmpeg_src_language_code}' subtitle stream already existed in {media_filepath}")
+                    print("Is '%s' subtitle stream exist          : Yes" %(ffmpeg_src_language_code.center(3)))
                     subtitle_stream_regions = []
                     subtitle_stream_transcripts = []
                     for entry in src_subtitle_stream_timed_subtitles:
                         subtitle_stream_regions.append(entry[0])
                         subtitle_stream_transcripts.append(entry[1])
                     base, ext = os.path.splitext(media_filepath)
                     src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
                     writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                     print(f"Extracting '{ffmpeg_src_language_code}'subtitle stream as      : {src_subtitle_filepath}")
                     writer.write(src_subtitle_filepath)
 
                 else:
-                    print(f"No '{ffmpeg_src_language_code}' subtitle stream found in {media_filepath}")
+                    #print(f"No '{ffmpeg_src_language_code}' subtitle stream found in {media_filepath}")
+                    print("Is '%s' subtitle stream exist          : No" %(ffmpeg_src_language_code.center(3)))
 
         for media_filepath in media_filepaths:
             ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
-            print("Checking existing '{}' subtites streams in {}".format(ffmpeg_dst_language_code, media_filepath))
+            #print("Checking existing '{}' subtites streams in {}".format(ffmpeg_dst_language_code, media_filepath))
+            print("Checking %s" %media_filepath)
 
             subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
             subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
             if subtitle_streams_data and subtitle_streams_data != []:
 
                 src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
                 dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
 
                 if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
-                    print(f"'{ffmpeg_dst_language_code}' subtitle stream already existed in {media_filepath}")
+                    #print(f"'{ffmpeg_dst_language_code}' subtitle stream already existed in {media_filepath}")
+                    print("Is '%s' subtitle stream exist          : Yes" %(ffmpeg_dst_language_code.center(3)))
                     subtitle_stream_regions = []
                     subtitle_stream_transcripts = []
                     for entry in dst_subtitle_stream_timed_subtitles:
                         subtitle_stream_regions.append(entry[0])
                         subtitle_stream_transcripts.append(entry[1])
                     base, ext = os.path.splitext(media_filepath)
                     dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
                     writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                     print(f"Extracting '{ffmpeg_dst_language_code}'subtitle stream as      : {dst_subtitle_filepath}")
                     writer.write(dst_subtitle_filepath)
                     removed_media_filepaths.append(media_filepath)
 
                 else:
-                    print(f"No '{ffmpeg_dst_language_code}' subtitle stream found in {media_filepath}")
+                    #print(f"No '{ffmpeg_dst_language_code}' subtitle stream found in {media_filepath}")
+                    print("Is '%s' subtitle stream exist          : No" %(ffmpeg_dst_language_code.center(3)))
 
                     if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                         prompt = "Translating from %s to %s   : " %(args.src_language.center(8), args.dst_language.center(8))
                         widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=len(src_subtitle_stream_timed_subtitles)).start()
 
                         transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language, error_messages_callback=show_error_messages)
@@ -2518,16 +2353,16 @@
 
         #print("Left media_filepaths = {}".format(media_filepaths))
         if not media_filepaths:
             print("Nothing else to do, exiting")
             sys.exit(0)
 
 
-    print("NO EXISTING SUBTITLES STREAMS FOUND, PERFORMING SPEECH RECOGNITION")
-    print("==================================================================")
+    print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLE STREAMS")
+    print("===========================================================================")
 
     for media_filepath in media_filepaths:
         print("Processing {}".format(media_filepath))
 
         try:
             widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
@@ -2598,38 +2433,73 @@
                 else:
                     print("Subtitles file saved as                 : {}".format(src_subtitle_filepath))
 
                 if args.embed:
                     base, ext = os.path.splitext(media_filepath)
                     tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
                     tmp_embedded_media_filepath_2 = "{base}.embedded2.{format}".format(base=base, format=ext[1:])
+                    tmp_embedded_media_filepath_3 = "{base}.embedded3.{format}".format(base=base, format=ext[1:])
                     embedded_media_filepath = "{base}.embedded.{format}".format(base=base, format=ext[1:])
 
                     if do_translate:
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
                         ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
+
+                        '''
+                        # USING FUNCTION
                         result = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, tmp_embedded_media_filepath_1)
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
+                        if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
                             result = embed_subtitle_to_media(tmp_embedded_media_filepath_1, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, tmp_embedded_media_filepath_2)
                         else:
                             result = embed_subtitle_to_media(media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, tmp_embedded_media_filepath_2)
+                        '''
+
+                        # USING CLASS
+                        widgets = [f"Embeding \'{ffmpeg_src_language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        result = subtitle_embedder(media_filepath)
+                        pbar.finish()
+
+                        if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
+                            widgets = [f"Embeding \'{ffmpeg_dst_language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                            pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            result = subtitle_embedder(tmp_embedded_media_filepath_1)
+                            pbar.finish()
+                        elif (not os.path.isfile(tmp_embedded_media_filepath_1)) and os.path.isfile(dst_subtitle_filepath):
+                            widgets = [f"Embeding \'{ffmpeg_dst_language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                            pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            result = subtitle_embedder(media_filepath)
+                            pbar.finish()
+
 
                         if os.path.isfile(tmp_embedded_media_filepath_2):
                             shutil.copy(tmp_embedded_media_filepath_2, embedded_media_filepath)
 
                         if os.path.isfile(tmp_embedded_media_filepath_1):
                             os.remove(tmp_embedded_media_filepath_1)
                         if os.path.isfile(tmp_embedded_media_filepath_2):
                             os.remove(tmp_embedded_media_filepath_2)
 
                     else:
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
-                        result = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, tmp_embedded_media_filepath_1)
-                        shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                        os.remove(tmp_embedded_media_filepath_1)
+
+                        #result = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, tmp_embedded_media_filepath_1)
+
+                        widgets = [f"Embeding \'{ffmpeg_src_language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        result = subtitle_embedder(media_filepath)
+                        pbar.finish()
+
+                        if tmp_embedded_media_filepath_1:
+                            shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
+                            os.remove(tmp_embedded_media_filepath_1)
 
                     if os.path.isfile(embedded_media_filepath):
                         print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
 
                 if not args.embed:
                     completed_tasks += 1
                 elif args.embed:
```

### Comparing `autosrt-1.3.5/autosrt.egg-info/PKG-INFO` & `autosrt-1.3.7/autosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.5
+Version: 1.3.7
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.5/setup.py` & `autosrt-1.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.5/test/test1.py` & `autosrt-1.3.7/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.5/test/test2.py` & `autosrt-1.3.7/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.5/test/test3.py` & `autosrt-1.3.7/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.5/test/test4.py` & `autosrt-1.3.7/test/test4.py`

 * *Files identical despite different names*

