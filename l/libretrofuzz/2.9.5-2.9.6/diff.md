# Comparing `tmp/libretrofuzz-2.9.5.tar.gz` & `tmp/libretrofuzz-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.9.5.tar", max compression
+gzip compressed data, was "libretrofuzz-2.9.6.tar", max compression
```

## Comparing `libretrofuzz-2.9.5.tar` & `libretrofuzz-2.9.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/LICENSE
--rw-r--r--   0        0        0     7570 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/README.rst
--rw-r--r--   0        0        0       22 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    50675 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      992 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/pyproject.toml
--rw-r--r--   0        0        0     8775 2023-06-06 12:37:29.654121 libretrofuzz-2.9.5/setup.py
--rw-r--r--   0        0        0     8799 2023-06-06 12:37:29.655128 libretrofuzz-2.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/LICENSE
+-rw-r--r--   0        0        0     7570 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/README.rst
+-rw-r--r--   0        0        0       22 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    48253 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      992 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/pyproject.toml
+-rw-r--r--   0        0        0     8775 2023-06-07 00:05:25.661933 libretrofuzz-2.9.6/setup.py
+-rw-r--r--   0        0        0     8799 2023-06-07 00:05:25.662751 libretrofuzz-2.9.6/PKG-INFO
```

### Comparing `libretrofuzz-2.9.5/LICENSE` & `libretrofuzz-2.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.5/README.rst` & `libretrofuzz-2.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.5/libretrofuzz/__main__.py` & `libretrofuzz-2.9.6/libretrofuzz/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 import unicodedata
 import asyncio
 import subprocess
 import configparser
 #external libraries
 import typer
 from PIL import Image, ImageOps
-from prompt_toolkit.input import create_input
 from rapidfuzz import process, fuzz
 from bs4 import BeautifulSoup
 from questionary import Style, select
 from httpx import RequestError, HTTPStatusError, Client, AsyncClient
 from tqdm import trange, tqdm
 
 #makes a class with these fields, which are the subdir names on the server system dir of the types of thumbnails
@@ -55,872 +54,896 @@
             r'\u0009\u000a\u000b\u000c\u000d\u000e\u000f\u0010\u0011\u0012\u0013\u0014\u0015' + \
             r'\u0016\u0017\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f\u003a\u002a\u003f\u005c\u002f\u0026]' \
             )
 #external terminal image viewer application
 viewer = None
 
 if sys.platform == 'win32': #this is for 64 bits too
-    #this order is to make 'portable' installs have priority in windows, a concept that doesn't exist in linux or macosx
-    #these are the default 32 and 64 bits installer paths, since there is no way to know what the user choses, check the defaults only.
-    CONFIG = Path(r'C:/RetroArch-Win64/retroarch.cfg')
+  #this order is to make 'portable' installs have priority in windows, a concept that doesn't exist in linux or macosx
+  #these are the default 32 and 64 bits installer paths, since there is no way to know what the user choses, check the defaults only.
+  CONFIG = Path(r'C:/RetroArch-Win64/retroarch.cfg')
+  if not CONFIG.exists():
+    CONFIG = Path(r'C:/RetroArch/retroarch.cfg')
     if not CONFIG.exists():
-        CONFIG = Path(r'C:/RetroArch/retroarch.cfg')
-        if not CONFIG.exists():
-            typer.echo('Portable install default location config not found, trying with APPDATA location')
-            var = os.getenv('APPDATA')
-            if var:
-                CONFIG = Path(var, 'RetroArch', 'retroarch.cfg')
+      typer.echo('Portable install default location config not found, trying with APPDATA location')
+      var = os.getenv('APPDATA')
+      if var:
+        CONFIG = Path(var, 'RetroArch', 'retroarch.cfg')
 elif sys.platform == 'darwin':
-    CONFIG = Path(Path.home(), 'Library', 'Application Support', 'RetroArch', 'config', 'retroarch.cfg')
+  CONFIG = Path(Path.home(), 'Library', 'Application Support', 'RetroArch', 'config', 'retroarch.cfg')
 else: #all the rest based on linux. If they arent based on linux, they'll try the else and fail harmlessly later
-    var = os.getenv('XDG_CONFIG_HOME')
-    if var:
-        CONFIG = Path(var, 'retroarch', 'retroarch.cfg')
-    else:
-        CONFIG = Path(Path.home(), '.config', 'retroarch', 'retroarch.cfg')
+  var = os.getenv('XDG_CONFIG_HOME')
+  if var:
+    CONFIG = Path(var, 'retroarch', 'retroarch.cfg')
+  else:
+    CONFIG = Path(Path.home(), '.config', 'retroarch', 'retroarch.cfg')
 
 #-----------------------------------------------------------------------------
 #keyboard listener, and exceptions to interrupt downloads or stop the program
 #-----------------------------------------------------------------------------
 
 class StopPlaylist(Exception):
-    '''this is thrown when http status 521 happens.
-    cloudflare uses when it can't find the server.
-    Note, parts of server might still be available
-    so this only stops a playlist in libretro-fuzzall'''
-    def __init__(self):
-        super().__init__()
+  '''this is thrown when http status 521 happens.
+  cloudflare uses when it can't find the server.
+  Note, parts of server might still be available
+  so this only stops a playlist in libretro-fuzzall'''
+  def __init__(self):
+    super().__init__()
 class StopDownload(Exception):
-    def __init__(self):
-        super().__init__()
+  def __init__(self):
+    super().__init__()
 class ContinueDownload(Exception):
-    def __init__(self):
-        super().__init__()
+  def __init__(self):
+    super().__init__()
 class StopProgram(Exception):
-    def __init__(self):
-        super().__init__()
+  def __init__(self):
+    super().__init__()
 
 skip = False
 escape  = False
 enter = False
 
 @contextmanager
 def handleContinueDownload():
   try:
     yield
   except ContinueDownload:
     pass
 def checkDownload():
-    '''threading.get_native_id() in this and other acesses of these variables
-       confirms all accesses are in synchronous functions on one thread so
-       there is no need to use any lock, async or not.
-    '''
-    global skip
-    global escape
-    global enter
-    if escape:
-        raise StopProgram()
-    if skip:
-        raise StopDownload()
-    if enter:
-        raise ContinueDownload()
+  '''threading.get_native_id() in this and other acesses of these variables
+     confirms all accesses are in synchronous functions on one thread so
+     there is no need to use any lock, async or not.
+  '''
+  global skip
+  global escape
+  global enter
+  if escape:
+    raise StopProgram()
+  if skip:
+    raise StopDownload()
+  if enter:
+    raise ContinueDownload()
 def checkEscape():
-    '''only called when it doesn't matter if a escape will happen, usually at the start of a iteration or the preparation phase'''
-    #so we can reset skip here, since it wont matter either way and will help remove false skip positives from the key event loop
+  '''only called when it doesn't matter if a escape will happen, usually at the start of a iteration or the preparation phase'''
+  #so we can reset skip here, since it wont matter either way and will help remove false skip positives from the key event loop
+  global skip
+  skip = False
+  global enter
+  enter = False
+  global escape
+  if escape:
+    raise StopProgram()
+
+from prompt_toolkit.input import create_input
+@asynccontextmanager
+async def lock_keys():
+  '''blocks key echoing for this console and recognizes most keys
+     including many combinations, user kill still works, alt+tab...
+     it also serves as a quit program and skip download shortcut
+     from: https://python-prompt-toolkit.readthedocs.io/en/master/pages/asking_for_input.html
+     Since this is decorated with a asynccontextmanager, it's guarded by async with
+     https://docs.python.org/3/reference/compound_stmts.html#async-with
+
+     since prompt_toolkit (3.0) input.attach attaches to a already running event asyncio event loop,
+     these key checks run essentially 'forever' in the same thread as the main one.
+
+     This is event loop is not cooperative (although it's thread safe, since it's a single thread)
+     so stale 'skip' (not ctrl-c or escape, since those exit right away) can be set to 'True' with a
+     logical check error of set while a nondownload iteration was running then check on a unrelated one.
+     So then you should reset skip on the 'checkescape' function at the start of every iteration
+  '''
+  input = create_input()
+  def keys_ready():
     global skip
-    skip = False
-    global enter
-    enter = False
     global escape
-    if escape:
-        raise StopProgram()
-@asynccontextmanager
-async def lock_keys() -> None:
-    '''blocks key echoing for this console and recognizes most keys
-       including many combinations, user kill still works, alt+tab...
-       it also serves as a quit program and skip download shortcut
-       from: https://python-prompt-toolkit.readthedocs.io/en/master/pages/asking_for_input.html
-       Since this is decorated with a asynccontextmanager, it's guarded by async with
-       https://docs.python.org/3/reference/compound_stmts.html#async-with
-       
-       since prompt_toolkit (3.0) input.attach attaches to a already running event asyncio event loop,
-       these key checks run essentially 'forever' in the same thread as the main one.
-       
-       This is event loop is not cooperative (although it's thread safe, since it's a single thread)
-       so stale 'skip' (not ctrl-c or escape, since those exit right away) can be set to 'True' with a
-       logical check error of set while a nondownload iteration was running then check on a unrelated one.
-       So then you should reset skip on the 'checkescape' function at the start of every iteration
-    '''
-    done = asyncio.Event()
-    input = create_input()
-    def keys_ready():
-        global skip
-        global escape
-        global enter
-        #ctrl-c needs flush, so this chain
-        for key_press in chain(input.read_keys(), input.flush_keys()):
-            if key_press.key == 'escape' or key_press.key == 'c-c': #esc or control-c
-                escape = True
-                done.set()
-            elif key_press.key == 'c-m': #linefeed or the final result of enter on both unix and windows
-                enter = True
-                done.set()
-            else:
-                skip = True
-
+    global enter
+    #ctrl-c needs flush, so this chain
+    for key_press in chain(input.read_keys(), input.flush_keys()):
+      if key_press.key == 'escape' or key_press.key == 'c-c': #esc or control-c
+        escape = True
+      elif key_press.key == 'c-m': #linefeed or the final result of enter on both unix and windows
+        enter = True
+      else:
+        skip = True
+  try:
     with input.raw_mode():
-        with input.attach(keys_ready):
-            #ignore keys in buffer before we are ready
-            input.read_keys()
-            input.flush_keys()
-            typer.echo(typer.style(f'Press escape to quit, enter to continue and most other non-meta keys to skip downloads', bold=True))
-            yield done
+      with input.attach(keys_ready):
+        #ignore keys in buffer before we are ready
+        input.read_keys()
+        input.flush_keys()
+        typer.echo(typer.style(f'Press escape to quit, enter to continue and most other non-meta keys to skip downloads', bold=True))
+        yield
+  finally:
+    #in windows 7 and python 3.8 for some reason prompt_toolkit
+    #tries to send a 'handle ready' not 'remove' event after detaching (the with above)
+    #not sure if it happens in python later than 3.8. This throws a 'RuntimeError: Event Loop is closed'
+    #the sleep avoids it
+    if sys.platform == "win32":
+      await asyncio.sleep(0.1)
 
 #----------------non contextual str manipulation------------------------
 def link(uri, label=None, parameters=''):
-    '''
-    Found in https://gist.github.com/egmontkob/eb114294efbcd5adb1944c9f3cb5feda
-    '''
-    if type(uri) is str: #just hover text and show same hyperlinks if possible
-        import urllib.parse
-        uri = urllib.parse.quote(uri)
-    if label is None:
-        label = uri
-    # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
-    escape_mask = '\033]8;{};{}\033\\{}\033]8;;\033\\'
-    return escape_mask.format(parameters, uri, label)
+  '''
+  Found in https://gist.github.com/egmontkob/eb114294efbcd5adb1944c9f3cb5feda
+  '''
+  if type(uri) is str: #just hover text and show same hyperlinks if possible
+    uri = quote(uri)
+  if label is None:
+    label = uri
+  # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
+  escape_mask = '\033]8;{};{}\033\\{}\033]8;;\033\\'
+  return escape_mask.format(parameters, uri, label)
 
 ppatterns = { '()': regex.compile(r'\([^)(]*\)'), '[]': regex.compile(r'\[[^][]*\]') }
 def removeparenthesis(s, open_p='(', close_p=')'):
-    nb_rep = 1
-    key = open_p+close_p
-    try:
-      pattern = ppatterns[key]
-    except:
-      pattern =  regex.compile(fr'\{open_p}[^{close_p}{open_p}]*\{close_p}')
-      ppatterns[key] = pattern
-    while (nb_rep):
-        (s, nb_rep) = regex.subn(pattern, '', s)
-    return s
+  nb_rep = 1
+  key = open_p+close_p
+  try:
+    pattern = ppatterns[key]
+  except:
+    pattern =  regex.compile(fr'\{open_p}[^{close_p}{open_p}]*\{close_p}')
+    ppatterns[key] = pattern
+  while (nb_rep):
+    (s, nb_rep) = regex.subn(pattern, '', s)
+  return s
 
 spatterns = { ' - ': regex.compile(rf'.*( - .*)'), ': ': regex.compile(rf'.*(: .*)') }
 before_metadata = regex.compile(r'(^[^[({]*)')
 def nosubtitle_aux(t,subtitle_marker=' - '):
-    #last subtitle marker and everything there until the end (last because i noticed that 'subsubtitles' exist,
-    #for instance, ultima 7 - part 1|2 - subtitle
-    try:
-      pattern = spatterns[subtitle_marker]
-    except:
-      pattern = regex.compile(rf'.*({subtitle_marker}.*)')
-      spatterns[subtitle_marker] = pattern
-    name_without_meta = regex.search(before_metadata, t)
-    subtitle = regex.search(pattern, name_without_meta.group(1) if name_without_meta else t)
-    if subtitle:
-        t = t[0:subtitle.start(1)] + ' ' + t[subtitle.end(1):]
-    return t
+  #last subtitle marker and everything there until the end (last because i noticed that 'subsubtitles' exist,
+  #for instance, ultima 7 - part 1|2 - subtitle
+  try:
+    pattern = spatterns[subtitle_marker]
+  except:
+    pattern = regex.compile(rf'.*({subtitle_marker}.*)')
+    spatterns[subtitle_marker] = pattern
+  name_without_meta = regex.search(before_metadata, t)
+  subtitle = regex.search(pattern, name_without_meta.group(1) if name_without_meta else t)
+  if subtitle:
+    t = t[0:subtitle.start(1)] + ' ' + t[subtitle.end(1):]
+  return t
 
 def replacemany(our_str, to_be_replaced, replace_with):
-    for nextchar in to_be_replaced:
-        our_str = our_str.replace(nextchar, replace_with)
-    return our_str
+  for nextchar in to_be_replaced:
+    our_str = our_str.replace(nextchar, replace_with)
+  return our_str
 
 def removefirst(name: str, suf: str):
-    return name.replace(suf, '', 1)
+  return name.replace(suf, '', 1)
 
 def removeprefix(name: str, pre: str):
-    if name.startswith(pre):
-        return name[len(pre):]
-    return name
+  if name.startswith(pre):
+    return name[len(pre):]
+  return name
 
 #----------------Used to check the existence of a sixtel compatible terminal image viewer-------------------------------
 def which(executable):
-    flips = shutil.which(executable)
-    if not flips:
-        flips = shutil.which(executable, path=os.path.dirname(__file__))
-    if not flips:
-        flips = shutil.which(executable, path=os.getcwd())
-    return flips
+  flips = shutil.which(executable)
+  if not flips:
+    flips = shutil.which(executable, path=os.path.dirname(__file__))
+  if not flips:
+    flips = shutil.which(executable, path=os.getcwd())
+  return flips
 
 #-----------------------------------------------------------------------------------------------------------------------
 #The heart of the program, what orders titles to be 'more similar' or less to the local labels (after the normalization)
 #-----------------------------------------------------------------------------------------------------------------------
 class TitleScorer(object):
-    def __init__(self):
-      #rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way)
-      #so it uses internal api to prevent a possible early exit at == 100
-      self._RF_ScorerPy = { 'get_scorer_flags': lambda **kwargs: {'optimal_score': MAX_SCORE, 'worst_score': 0, 'flags': (1 << 6)} }
-
-    def __call__(self, s1, s2, processor=None, score_cutoff=None):
-      if (min(len(s1),len(s2)) / max(len(s1),len(s2))) < 0.3:
-        #ideally this branch wouldn't exist, but since many games do not have
-        #images, they get caught up on a short title being completely contained in another
-        #token_set_ratio gives that 100. Skip if the smaller name length is less than 30%
-        return 0
-      #names are whitespace and case normalized
-      if s1 == s2:
-        return MAX_SCORE
-      prefix = len(os.path.commonprefix([s1, s2]))
-      #score_cutoff needs to be 0 from a combination of 3 factors that create a bug:
-      #1. the caller of this, extract passes the 'current best score' as score_cutoff
-      #2. the token_set_ratio function returns 0 if the calculated score < score_cutoff
-      #3. 'current best score' includes the prefix, which this call can't include in 2.
-      similarity = fuzz.token_set_ratio(s1,s2,processor=None,score_cutoff=0)
-      #Combine the scorer with a common prefix heuristic to give priority to longer similar
-      #names, this helps prevents false positives for shorter strings which token set ratio
-      #is prone because it sets score to 100 if one string words are completely on the other.
-      return min(MAX_SCORE-1,similarity + prefix)
+  def __init__(self):
+    #rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way)
+    #so it uses internal api to prevent a possible early exit at == 100
+    self._RF_ScorerPy = { 'get_scorer_flags': lambda **kwargs: {'optimal_score': MAX_SCORE, 'worst_score': 0, 'flags': (1 << 6)} }
+
+  def __call__(self, s1, s2, processor=None, score_cutoff=None):
+    if (min(len(s1),len(s2)) / max(len(s1),len(s2))) < 0.3:
+      #ideally this branch wouldn't exist, but since many games do not have
+      #images, they get caught up on a short title being completely contained in another
+      #token_set_ratio gives that 100. Skip if the smaller name length is less than 30%
+      return 0
+    #names are whitespace and case normalized
+    if s1 == s2:
+      return MAX_SCORE
+    prefix = len(os.path.commonprefix([s1, s2]))
+    #score_cutoff needs to be 0 from a combination of 3 factors that create a bug:
+    #1. the caller of this, extract passes the 'current best score' as score_cutoff
+    #2. the token_set_ratio function returns 0 if the calculated score < score_cutoff
+    #3. 'current best score' includes the prefix, which this call can't include in 2.
+    similarity = fuzz.token_set_ratio(s1,s2,processor=None,score_cutoff=0)
+    #Combine the scorer with a common prefix heuristic to give priority to longer similar
+    #names, this helps prevents false positives for shorter strings which token set ratio
+    #is prone because it sets score to 100 if one string words are completely on the other.
+    return min(MAX_SCORE-1,similarity + prefix)
 
 #-----------------------------------------------------------------------------------------------------------------------------
 # Normalization functions, part of the functions that change both local labels and remote names to be more similar to compare
 #-----------------------------------------------------------------------------------------------------------------------------
 camelcase_pattern = regex.compile(r'(\p{Lu}\p{Ll}+)')
 #number sequences in the middle (not start or end) of a string that start with 0
 zero_lead_pattern = regex.compile(r'([^\d])0+([1-9])')
 def normalizer(t, nometa, hack):
-    if nometa:
-        t = removeparenthesis(t,'(',')')
-    if not hack:
-        t = removeparenthesis(t,'[',']')
-    #change all common ascci symbol characters we aren't going to use after this (, and ')
-    t = replacemany(t, '_()[]{}-.!?#"', ' ')
-    #strips just because the user may have made a mistake naming the source
-    #(or the replacement above introduce boundary spaces)
-    t = t.strip()
-    #remove any number leading 0, except at the end or the start of the string
-    #where it is likely a important part of the name, not a file manager sort workaround
-    t = regex.sub(zero_lead_pattern, r'\1\2', t)
-    #CamelCaseNames for local labels are common when there are no spaces,
-    #do this to normalize definite articles in normalization with spaces only (minimizes changes)
-    t = ' '.join([s.strip() for s in regex.split(camelcase_pattern, t) if s])
-    #normalize case
-    t = t.lower()
-    #beginning and end definite articles in several european languages (people move them)
-    #make sure we're only removing the start and end forms with spaces
-    t = removefirst(t, ', the')
-    t = removeprefix(t, 'the ')
-    t = removefirst(t, ', los')
-    t = removeprefix(t, 'los ')
-    t = removefirst(t, ', las')
-    t = removeprefix(t, 'las ')
-    t = removefirst(t, ', les')
-    t = removeprefix(t, 'les ')
-    t = removefirst(t, ', le')
-    t = removeprefix(t, 'le ')
-    t = removefirst(t, ', la')
-    t = removeprefix(t, 'la ')
-    t = removefirst(t, ', l\'')
-    #L' sometimes ommits the space so always remove L' at the start even without space
-    t = removeprefix(t, 'l\'')  #if there is a extra space the next join will remove it
-    t = removefirst(t, ', der')
-    t = removeprefix(t, 'der ')
-    t = removefirst(t, ', die')
-    t = removeprefix(t, 'die ')
-    t = removefirst(t, ', das')
-    t = removeprefix(t, 'das ')
-    t = removefirst(t, ', el')
-    t = removeprefix(t, 'el ')
-    t = removefirst(t, ', os')
-    t = removeprefix(t, 'os ')
-    t = removefirst(t, ', as')
-    t = removeprefix(t, 'as ')
-    t = removefirst(t, ', o')
-    t = removeprefix(t, 'o ')
-    t = removefirst(t, ', a')
-    t = removeprefix(t, 'a ')
-    #remove the symbols used in the definite article normalization
-    t = replacemany(t, ',\'', '')
-    #this makes sure that if a remote name has ' and ' instead of ' _ ' to replace ' & ' it works
-    #': ' doesn't need this because ':' is a forbidden character and both '_' and '-' turn to ''
-    t = t.replace(' and ',  '')
-    #Tries to make roman numerals in the range 1-20 equivalent to normal numbers (to handle names that change it).
-    #If both sides are roman numerals there is no harm done if XXIV gets turned into 204 in both sides.
-    t = t.replace('xviii', '18')
-    t = t.replace('xvii',  '17')
-    t = t.replace('xvi' ,  '16')
-    t = t.replace('xiii',  '13')
-    t = t.replace('xii' ,  '12')
-    t = t.replace('xiv' ,  '14')
-    t = t.replace('xv'  ,  '15')
-    t = t.replace('xix',   '19')
-    t = t.replace('xx',   '20')
-    t = t.replace('xi',   '11')
-    t = t.replace('viii', '8')
-    t = t.replace('vii',  '7')
-    t = t.replace('vi' ,  '6')
-    t = t.replace('iii',  '3')
-    t = t.replace('ii' ,  '2')
-    t = t.replace('iv' ,  '4')
-    t = t.replace('v'  ,  '5')
-    t = t.replace('ix',   '9')
-    t = t.replace('x',   '10')
-    t = t.replace('i',    '1')
-    #remove diacritics (does nothing to asian languages diacritics, only for 2 to 1 character combinations)
-    t = u''.join([c for c in unicodedata.normalize('NFKD', t) if not unicodedata.combining(c)])
-    #normalize spaces (don't remove them for other later score methods to be able to reorder tokens
-    return ' '.join(t.split())
+  if nometa:
+    t = removeparenthesis(t,'(',')')
+  if not hack:
+    t = removeparenthesis(t,'[',']')
+  #change all common ascci symbol characters we aren't going to use after this (, and ')
+  t = replacemany(t, '_()[]{}-.!?#"', ' ')
+  #strips just because the user may have made a mistake naming the source
+  #(or the replacement above introduce boundary spaces)
+  t = t.strip()
+  #remove any number leading 0, except at the end or the start of the string
+  #where it is likely a important part of the name, not a file manager sort workaround
+  t = regex.sub(zero_lead_pattern, r'\1\2', t)
+  #CamelCaseNames for local labels are common when there are no spaces,
+  #do this to normalize definite articles in normalization with spaces only (minimizes changes)
+  t = ' '.join([s.strip() for s in regex.split(camelcase_pattern, t) if s])
+  #normalize case
+  t = t.lower()
+  #beginning and end definite articles in several european languages (people move them)
+  #make sure we're only removing the start and end forms with spaces
+  t = removefirst(t, ', the')
+  t = removeprefix(t, 'the ')
+  t = removefirst(t, ', los')
+  t = removeprefix(t, 'los ')
+  t = removefirst(t, ', las')
+  t = removeprefix(t, 'las ')
+  t = removefirst(t, ', les')
+  t = removeprefix(t, 'les ')
+  t = removefirst(t, ', le')
+  t = removeprefix(t, 'le ')
+  t = removefirst(t, ', la')
+  t = removeprefix(t, 'la ')
+  t = removefirst(t, ', l\'')
+  #L' sometimes ommits the space so always remove L' at the start even without space
+  t = removeprefix(t, 'l\'')  #if there is a extra space the next join will remove it
+  t = removefirst(t, ', der')
+  t = removeprefix(t, 'der ')
+  t = removefirst(t, ', die')
+  t = removeprefix(t, 'die ')
+  t = removefirst(t, ', das')
+  t = removeprefix(t, 'das ')
+  t = removefirst(t, ', el')
+  t = removeprefix(t, 'el ')
+  t = removefirst(t, ', os')
+  t = removeprefix(t, 'os ')
+  t = removefirst(t, ', as')
+  t = removeprefix(t, 'as ')
+  t = removefirst(t, ', o')
+  t = removeprefix(t, 'o ')
+  t = removefirst(t, ', a')
+  t = removeprefix(t, 'a ')
+  #remove the symbols used in the definite article normalization
+  t = replacemany(t, ',\'', '')
+  #this makes sure that if a remote name has ' and ' instead of ' _ ' to replace ' & ' it works
+  #': ' doesn't need this because ':' is a forbidden character and both '_' and '-' turn to ''
+  t = t.replace(' and ',  '')
+  #Tries to make roman numerals in the range 1-20 equivalent to normal numbers (to handle names that change it).
+  #If both sides are roman numerals there is no harm done if XXIV gets turned into 204 in both sides.
+  t = t.replace('xviii', '18')
+  t = t.replace('xvii',  '17')
+  t = t.replace('xvi' ,  '16')
+  t = t.replace('xiii',  '13')
+  t = t.replace('xii' ,  '12')
+  t = t.replace('xiv' ,  '14')
+  t = t.replace('xv'  ,  '15')
+  t = t.replace('xix',   '19')
+  t = t.replace('xx',   '20')
+  t = t.replace('xi',   '11')
+  t = t.replace('viii', '8')
+  t = t.replace('vii',  '7')
+  t = t.replace('vi' ,  '6')
+  t = t.replace('iii',  '3')
+  t = t.replace('ii' ,  '2')
+  t = t.replace('iv' ,  '4')
+  t = t.replace('v'  ,  '5')
+  t = t.replace('ix',   '9')
+  t = t.replace('x',   '10')
+  t = t.replace('i',    '1')
+  #remove diacritics (does nothing to asian languages diacritics, only for 2 to 1 character combinations)
+  t = u''.join([c for c in unicodedata.normalize('NFKD', t) if not unicodedata.combining(c)])
+  #normalize spaces (don't remove them for other later score methods to be able to reorder tokens
+  return ' '.join(t.split())
 
 def nosubtitle_normalizer(t, nometa, hack):
-    return normalizer(nosubtitle_aux(t), nometa, hack)
+  return normalizer(nosubtitle_aux(t), nometa, hack)
 
 #---------------------------------------------------------------------------------
 # Initalization functions, since there are two main programs so the code is reused
 #---------------------------------------------------------------------------------
 class RzipReader(object):
-    """used to abstract the libretro compressed playlist format"""
-    def __init__(self, file_name):
-        self.file_name = file_name
-
-    @contextmanager
-    def open(self):
-        with open(self.file_name, 'rb') as file:
-            header = file.read(6)
-        with open(self.file_name, 'rb') as file:
-            if header.decode() == '#RZIPv':
-                file.read(8) #skip all the header parts
-                chunksize = unpack('<I', file.read(4) )[0] #little endian
-                totalsize = unpack('<Q', file.read(8) )[0]
-                checksize = 0
-                #collect all the file into a 'byte file' object
-                with io.BytesIO() as f:
-                    #for each chunk of zlib compressed file parts
-                    bsize = file.read(4)
-                    while bsize != b'':
-                        size = unpack('<I', bsize)[0]
-                        dbytes = zlib.decompress(file.read(size))
-                        checksize += len(dbytes)
-                        f.write( dbytes )
-                        bsize = file.read(4)
-                    assert checksize == totalsize, f'{checksize} != {totalsize}'
-                    f.seek(0) #reset for the next reader.
-                    yield io.TextIOWrapper(f)
-            else:
-                yield io.TextIOWrapper(file)
+  """used to abstract the libretro compressed playlist format"""
+  def __init__(self, file_name):
+    self.file_name = file_name
+
+  @contextmanager
+  def open(self):
+    with open(self.file_name, 'rb') as file:
+      header = file.read(6)
+    with open(self.file_name, 'rb') as file:
+      if header.decode() == '#RZIPv':
+        file.read(8) #skip all the header parts
+        chunksize = unpack('<I', file.read(4) )[0] #little endian
+        totalsize = unpack('<Q', file.read(8) )[0]
+        checksize = 0
+        #collect all the file into a 'byte file' object
+        with io.BytesIO() as f:
+          #for each chunk of zlib compressed file parts
+          bsize = file.read(4)
+          while bsize != b'':
+            size = unpack('<I', bsize)[0]
+            dbytes = zlib.decompress(file.read(size))
+            checksize += len(dbytes)
+            f.write( dbytes )
+            bsize = file.read(4)
+          assert checksize == totalsize, f'{checksize} != {totalsize}'
+          f.seek(0) #reset for the next reader.
+          yield io.TextIOWrapper(f)
+      else:
+        yield io.TextIOWrapper(file)
 
 def readPlaylistAndPrepareDirectories(playlist: Path, temp_dir: Path, thumbnails_dir: Path):
-    '''create directories that are children of temp_dir and thumbnails_dir that have the
-       subdirs needed to move files created on them from one to the other, so you don't
-       need to care to create directories for every file processed.
-       
-       return a list of game names and 'db_names' (stripped of extension): [(names: str,db_names: str)]
-       db_names without extension are the system directory names libretro searchs for the thumbnail.
-    '''
-    names = []
-    dbs   = set()
-    try:
-        with RzipReader(playlist).open() as f:
-            data = json.load(f)
-            for r in data['items']:
-                assert 'label' in r and r['label'].strip() != '', f'\n{json.dumps(r,indent=4)} of playlist {playlist} has no label'
-                assert 'db_name' in r and r['db_name'].endswith('.lpl'), f'\n{json.dumps(r,indent=4)} of playlist {playlist} has no valid db_name'
-                #add the label name and the db name (it's a playlist name, minus the extension '.lpl')
-                db = r['db_name'][:-4]
-                dbs.add(db)
-                names.append( (r['label'], db) )
-    except json.JSONDecodeError:
-        #older version of the playlist format, this has no error correction; the extra lines after the
-        #game entries can be between 0 and 5, because retroarch will ignore lines missing at the end.
-        with RzipReader(playlist).open() as f:
-            #make sure not to count empty lines, which might break the assumptions made here
-            data = [ x for x in map(str.strip, f.readlines()) if x ]
-            gamelineslen = len(data) - (len(data) % 6)
-            for i in range(0,gamelineslen, 6):
-                name = data[i+1]
-                db   = data[i+5][:-4]
-                dbs.add(db)
-                names.append( (name, db) )
-    #create the directories we will 'maybe' need. This is not so problematic
-    #as it seems since likely len(dbs) == 1, so 6 directories per playlist
-    #versus having os.makedirs called hundred of times for larger playlists
-    #this is vulnerable to ToCToU deletion but everything is with directories
-    for parent in [temp_dir, thumbnails_dir]:
-        for db in dbs:
-            for dirname in Thumbs._fields:
-                os.makedirs(Path(parent, db, dirname), exist_ok=True)
-    return names
+  '''create directories that are children of temp_dir and thumbnails_dir that have the
+     subdirs needed to move files created on them from one to the other, so you don't
+     need to care to create directories for every file processed.
+     return a list of game names and 'db_names' (stripped of extension): [(names: str,db_names: str)]
+     db_names without extension are the system directory names libretro searchs for the thumbnail.
+  '''
+  names = []
+  dbs   = set()
+  try:
+    with RzipReader(playlist).open() as f:
+      data = json.load(f)
+      for r in data['items']:
+        assert 'label' in r and r['label'].strip() != '', f'\n{json.dumps(r,indent=4)} of playlist {playlist} has no label'
+        assert 'db_name' in r and r['db_name'].endswith('.lpl'), f'\n{json.dumps(r,indent=4)} of playlist {playlist} has no valid db_name'
+        #add the label name and the db name (it's a playlist name, minus the extension '.lpl')
+        db = r['db_name'][:-4]
+        dbs.add(db)
+        names.append( (r['label'], db) )
+  except json.JSONDecodeError:
+    #older version of the playlist format, this has no error correction; the extra lines after the
+    #game entries can be between 0 and 5, because retroarch will ignore lines missing at the end.
+    with RzipReader(playlist).open() as f:
+      #make sure not to count empty lines, which might break the assumptions made here
+      data = [ x for x in map(str.strip, f.readlines()) if x ]
+      gamelineslen = len(data) - (len(data) % 6)
+      for i in range(0,gamelineslen, 6):
+        name = data[i+1]
+        db   = data[i+5][:-4]
+        dbs.add(db)
+        names.append( (name, db) )
+  #create the directories we will 'maybe' need. This is not so problematic
+  #as it seems since likely len(dbs) == 1, so 6 directories per playlist
+  #versus having os.makedirs called hundred of times for larger playlists
+  #this is vulnerable to ToCToU deletion but everything is with directories
+  for parent in [temp_dir, thumbnails_dir]:
+    for db in dbs:
+      for dirname in Thumbs._fields:
+        os.makedirs(Path(parent, db, dirname), exist_ok=True)
+  return names
 
 def getPath(cfg: Path, setting: str, default_value: str):
-    '''returns paths inside of a cfg file setting'''
-    with open(cfg) as f:
-        file_content = '[DUMMY]\n' + f.read()
-    configParser = configparser.RawConfigParser()
-    configParser.read_string(file_content)
-    try:
-        fdir = os.path.expanduser(configParser['DUMMY'][setting].strip('"'))
-    except:
-        return None
-    if fdir.startswith(':\\'):
-        fdir = fdir[2:]
-        #imagine a retroarch.cfg file created in windows is read in posix
-        if os.sep == '/':
-            fdir = fdir.replace('\\', '/')
-        return cfg.parent / fdir
-    elif fdir == 'default':
-        if default_value:
-            return cfg.parent / default_value
-        else:
-            return None
-    return Path(fdir)
+  '''returns paths inside of a cfg file setting'''
+  with open(cfg) as f:
+    file_content = '[DUMMY]\n' + f.read()
+  configParser = configparser.RawConfigParser()
+  configParser.read_string(file_content)
+  try:
+    fdir = os.path.expanduser(configParser['DUMMY'][setting].strip('"'))
+  except:
+    return None
+  if fdir.startswith(':\\'):
+    fdir = fdir[2:]
+    #imagine a retroarch.cfg file created in windows is read in posix
+    if os.sep == '/':
+        fdir = fdir.replace('\\', '/')
+    return cfg.parent / fdir
+  elif fdir == 'default':
+    if default_value:
+      return cfg.parent / default_value
+    else:
+      return None
+  return Path(fdir)
 
 def error(error: str):
-    typer.echo(typer.style(error, fg=typer.colors.RED, bold=True))
+  typer.echo(typer.style(error, fg=typer.colors.RED, bold=True))
 
 def test_common_errors(cfg: Path, playlist: str, system: str, address: str):
-    '''returns a tuple with (playlist_dir: Path, thumbnail_dir: Path, PLAYLISTS: [Path], SYSTEMS: [str]) '''
-    #stop showing the variables - a library installed this behind my back
-    try:
-      from rich.traceback import install
-      install(show_locals=False)
-    except ImportError:
-      pass
-    global ADDRESS
-    ADDRESS = address.rstrip('/')
-    global viewer
-    viewer = which('chafa')
-    if not viewer:
-        typer.echo(f'Shell image viewer chafa was not found')
-    if not cfg or not cfg.is_file():
-        error(f'Invalid Retroarch cfg file: {cfg}')
-        raise typer.Exit(code=1)
-    thumbnails_directory = getPath(cfg, 'thumbnails_directory', 'thumbnails')
-    if not thumbnails_directory or not thumbnails_directory.is_dir() or not os.access(thumbnails_directory, os.W_OK):
-        error(f'Invalid retroarch.cfg line: thumbnails_directory="{thumbnails_directory}"')
-        raise typer.Exit(code=1)
-    playlist_dir = getPath(cfg, 'playlist_directory', 'playlists')
-    if not playlist_dir or not playlist_dir.is_dir() or not os.access(playlist_dir, os.R_OK):
-        error(f'Invalid retroarch.cfg line: playlist_directory="{playlist_dir}"')
-        raise typer.Exit(code=1)
-    PLAYLISTS = [ pl for pl in playlist_dir.glob('./*.lpl') if pl.is_file() and os.access(pl, os.R_OK) ]
-    if not PLAYLISTS:
-        error(f'Invalid playlist files in playlist directory: {playlist_dir}')
-        raise typer.Exit(code=1)
-    if playlist and Path(playlist_dir, playlist) not in PLAYLISTS:
-        error(f'Invalid user provided playlist: {playlist}')
-        raise typer.Exit(code=1)
-
-    try:
-        with Client() as client:
-            page = client.get(ADDRESS, timeout=15)
-            soup = BeautifulSoup(page.text, 'html.parser')
-        SYSTEMS = [ unquote(node.get('href')[:-1]) for node in soup.find_all('a') if node.get('href').endswith('/') and not node.get('href').endswith('../') ]
-    except (RequestError,HTTPStatusError) as err:
-        error(f'Could not get the remote thumbnail system names, exiting: {err}')
-        raise typer.Exit(code=1)
-    if system and system not in SYSTEMS:
-        error(f'The user provided system name {system} does not match any remote thumbnail system names')
-        raise typer.Exit(code=1)
-    return (playlist_dir, thumbnails_directory, sorted(PLAYLISTS), sorted(SYSTEMS))
+  '''returns a tuple with (playlist_dir: Path, thumbnail_dir: Path, PLAYLISTS: [Path], SYSTEMS: [str]) '''
+  #stop showing the variables - a library installed this behind my back
+  try:
+    from rich.traceback import install
+    install(show_locals=False)
+  except ImportError:
+    pass
+  global ADDRESS
+  ADDRESS = address.rstrip('/')
+  global viewer
+  viewer = which('chafa')
+  if not viewer:
+    typer.echo(f'Shell image viewer chafa was not found')
+  if not cfg or not cfg.is_file():
+    error(f'Invalid Retroarch cfg file: {cfg}')
+    raise typer.Exit(code=1)
+  thumbnails_directory = getPath(cfg, 'thumbnails_directory', 'thumbnails')
+  if not thumbnails_directory or not thumbnails_directory.is_dir() or not os.access(thumbnails_directory, os.W_OK):
+    error(f'Invalid retroarch.cfg line: thumbnails_directory="{thumbnails_directory}"')
+    raise typer.Exit(code=1)
+  playlist_dir = getPath(cfg, 'playlist_directory', 'playlists')
+  if not playlist_dir or not playlist_dir.is_dir() or not os.access(playlist_dir, os.R_OK):
+    error(f'Invalid retroarch.cfg line: playlist_directory="{playlist_dir}"')
+    raise typer.Exit(code=1)
+  PLAYLISTS = [ pl for pl in playlist_dir.glob('./*.lpl') if pl.is_file() and os.access(pl, os.R_OK) ]
+  if not PLAYLISTS:
+    error(f'Invalid playlist files in playlist directory: {playlist_dir}')
+    raise typer.Exit(code=1)
+  if playlist and Path(playlist_dir, playlist) not in PLAYLISTS:
+    error(f'Invalid user provided playlist: {playlist}')
+    raise typer.Exit(code=1)
+  #windows can only print images and urls in windows 10 up (requires a better console)
+  #since python 3.8 is the very minimum of this application, it can only be used on windows 7 and up
+  #ie: we only have to disallow 7, 8
+  basic_verbose = False
+  import platform
+  if sys.platform == "win32" and platform.release() in ('7','8','8.1'):
+    typer.echo(f'Disabling rich verbose and image output because your windows does not support it')
+    basic_verbose = True
+  try:
+    with Client() as client:
+      page = client.get(ADDRESS, timeout=15)
+      soup = BeautifulSoup(page.text, 'html.parser')
+    SYSTEMS = [ unquote(node.get('href')[:-1]) for node in soup.find_all('a') if node.get('href').endswith('/') and not node.get('href').endswith('../') ]
+  except (RequestError,HTTPStatusError) as err:
+    error(f'Could not get the remote thumbnail system names, exiting: {err}')
+    raise typer.Exit(code=1)
+  if system and system not in SYSTEMS:
+    error(f'The user provided system name {system} does not match any remote thumbnail system names')
+    raise typer.Exit(code=1)
+  return (basic_verbose, playlist_dir, thumbnails_directory, sorted(PLAYLISTS), sorted(SYSTEMS))
 
 #####################
 # Main programs code
 #####################
+
 def mainfuzzsingle(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
-        playlist: str = typer.Option(None, metavar='NAME', help='Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.'),
-        system: str = typer.Option(None, metavar='NAME', help='Directory name in the server to download thumbnails. If not provided, asked from the user.'),
-        wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
-        wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
-        filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
-        score: int = typer.Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
-        nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
-        noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
-        nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
-        nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
-        nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
-        hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
-        before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
-        address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
-        verbose: Optional[int] = typer.Option(None, '--verbose', min=1, metavar='N', help=f'Show mininame, len N list (maxscore, server mininame).')
-    ):
-    if playlist and not playlist.lower().endswith('.lpl'):
-        playlist = playlist + '.lpl'
-    
-    playlist_dir, thumbnails_dir, PLAYLISTS, SYSTEMS = test_common_errors(cfg, playlist, system, address)
-    
-    custom_style = Style([
-        ('answer', 'fg:green bold'),
-    ])
-    
-    #ask user for these 2 arguments if they're still not set
+  playlist: str = typer.Option(None, metavar='NAME', help='Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.'),
+  system: str = typer.Option(None, metavar='NAME', help='Directory name in the server to download thumbnails. If not provided, asked from the user.'),
+  wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
+  wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
+  filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
+  score: int = typer.Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
+  nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
+  noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
+  nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
+  nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
+  nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
+  hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
+  before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
+  address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
+  verbose: Optional[int] = typer.Option(None, '--verbose', min=1, metavar='N', help=f'Show mininame, len N list (maxscore, server mininame).')
+  ):
+  if playlist and not playlist.lower().endswith('.lpl'):
+    playlist = playlist + '.lpl'
+
+  basic_verbose,playlist_dir,thumbnails_dir,PLAYLISTS,SYSTEMS = test_common_errors(cfg,playlist,system,address)
+  if basic_verbose : noimage = True
+
+  custom_style = Style([
+    ('answer', 'fg:green bold'),
+  ])
+
+  #ask user for these 2 arguments if they're still not set
+  if not playlist:
+    display_playlists = list(map(os.path.basename, PLAYLISTS))
+    playlist = select('Which playlist do you want to download thumbnails for?', display_playlists, style=custom_style, qmark='').ask()
     if not playlist:
-        display_playlists = list(map(os.path.basename, PLAYLISTS))
-        playlist = select('Which playlist do you want to download thumbnails for?', display_playlists, style=custom_style, qmark='').ask()
-        if not playlist:
-            raise typer.Exit()
-    
+      raise typer.Exit()
+
+  if not system:
+    #start with the playlist system selected, if any
+    playlist_sys = playlist[:-4]
+    question = 'Which directory should be used to download thumbnails?'
+    system = select(question, SYSTEMS, style=custom_style, qmark='', default=playlist_sys if playlist_sys in SYSTEMS else None).ask()
     if not system:
-        #start with the playlist system selected, if any
-        playlist_sys = playlist[:-4]
-        question = 'Which directory should be used to download thumbnails?'
-        system = select(question, SYSTEMS, style=custom_style, qmark='', default=playlist_sys if playlist_sys in SYSTEMS else None).ask()
-        if not system:
-            raise typer.Exit()
-    
-    async def runit():
-        try:
-            async with lock_keys(), AsyncClient() as client:
-                #temporary dir for downloads (required to prevent clobbering of files in case of no internet and filters being used)
-                #parent directory of this temp dir is the same as the retroarch thumbnail dir to make moving the file just renaming it, not copy it
-                with TemporaryDirectory(prefix='libretrofuzz', dir=thumbnails_dir) as tmpdir:
-                    typer.echo(typer.style(f'{playlist} -> {system}', bold=True))
-                    names = readPlaylistAndPrepareDirectories(Path(playlist_dir, playlist), tmpdir, thumbnails_dir)
-                    await downloader(names,system,wait_before,wait_after,filters,score,noimage,nomerge,nofail,nometa,hack,nosubtitle,verbose,before,tmpdir,thumbnails_dir,client)
-        except StopPlaylist as e:
-            error(f'Cloudflare is down for {system}')
-            raise typer.Exit(code=1)
-        except StopProgram as e:
-            error(f'Cancelled by user, exiting')
-            raise typer.Exit()
-    asyncio.run(runit(), debug=False)
+      raise typer.Exit()
+
+  async def runit():
+    try:
+      async with lock_keys(), AsyncClient() as client:
+        #temporary dir for downloads (required to prevent clobbering of files in case of no internet and filters being used)
+        #parent directory of this temp dir is the same as the RA thumbnail dir to make mv the file just renaming it, not cp it
+        with TemporaryDirectory(prefix='libretrofuzz', dir=thumbnails_dir) as tmpdir:
+          typer.echo(typer.style(f'{playlist} -> {system}', bold=True))
+          names = readPlaylistAndPrepareDirectories(Path(playlist_dir, playlist), tmpdir, thumbnails_dir)
+          await downloader(names,system,wait_before,wait_after,filters,score,noimage,nomerge,nofail,nometa, \
+                           hack,nosubtitle,verbose,basic_verbose,before,tmpdir,thumbnails_dir,client)
+    except StopPlaylist as e:
+      error(f'Cloudflare is down for {system}')
+      raise typer.Exit(code=1)
+    except StopProgram as e:
+      error(f'Cancelled by user, exiting')
+      raise typer.Exit()
+  asyncio.run(runit(), debug=False)
 
 def mainfuzzall(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
-        wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
-        wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
-        filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
-        score: int = typer.Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
-        nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
-        noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
-        nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
-        nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
-        nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
-        hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
-        before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
-        address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
-        verbose: Optional[int] = typer.Option(None, '--verbose', min=1, metavar='N', help=f'Show mininame, len N list (maxscore, server mininame).')
-    ):
-    playlist_dir, thumbnails_dir, PLAYLISTS, SYSTEMS = test_common_errors(cfg, None, None, address)
-    
-    notInSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS if os.path.basename(playlist)[:-4] not in SYSTEMS]
-    for playlist, system in notInSystems:
-        PLAYLISTS.remove(playlist)
-    inSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS ]
-    
-    async def runit():
-        try:
-            async with lock_keys(), AsyncClient() as client:
-                with TemporaryDirectory(prefix='libretrofuzz', dir=thumbnails_dir) as tmpdir:
-                    for playlist, system in notInSystems:
-                        typer.echo(typer.style(f'Custom playlist skipped: ', fg=typer.colors.RED, bold=True)+typer.style(f'{system}.lpl', bold=True))
-                    for playlist, system in inSystems:
-                        typer.echo(typer.style(f'{system}.lpl -> {system}', bold=True))
-                        names = readPlaylistAndPrepareDirectories(playlist, tmpdir, thumbnails_dir)
-                        try:
-                            await downloader(names,system,wait_before,wait_after,filters,score,noimage,nomerge,nofail,nometa,hack,nosubtitle,verbose,before,tmpdir,thumbnails_dir,client)
-                        except StopPlaylist as e:
-                            error(f'Cloudflare is down for {system}')
-        except StopProgram as e:
-            error(f'Cancelled by user, exiting')
-            raise typer.Exit()
-    asyncio.run(runit(), debug=False)
+  wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
+  wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
+  filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
+  score: int = typer.Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
+  nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
+  noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
+  nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
+  nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
+  nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
+  hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
+  before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
+  address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
+  verbose: Optional[int] = typer.Option(None, '--verbose', min=1, metavar='N', help=f'Show mininame, len N list (maxscore, server mininame).')
+  ):
+  basic_verbose,playlist_dir,thumbnails_dir,PLAYLISTS,SYSTEMS = test_common_errors(cfg,None,None,address)
+  if basic_verbose : noimage = True
+
+  notInSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS if os.path.basename(playlist)[:-4] not in SYSTEMS]
+  for playlist, system in notInSystems:
+    PLAYLISTS.remove(playlist)
+  inSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS ]
 
-async def downloadgamenames(client, system):
-    """returns [ dict(Game_Name, Game_Url), dict(Game_Name, Game_Url), dict(Game_Name, Game_Url) ]
-        for each of the server directories '/Named_Boxarts/', '/Named_Titles/', '/Named_Snaps/'
-        (potentially some of these dicts may be empty if the server doesn't have the directory)
-    """
-    lr_thumbs = ADDRESS+'/'+quote(system) #then get the thumbnails from the system name
-    args = []
+  async def runit():
     try:
-        for tdir in ['/Named_Boxarts/', '/Named_Titles/', '/Named_Snaps/']:
-            lr_thumb = lr_thumbs+tdir
-            response = ''
-            async with client.stream('GET', lr_thumb, timeout=15) as r:
-                async for chunk in r.aiter_text(4096):
-                    checkEscape()
-                    response += chunk
-            #not found is ok, since some server system directories do not have all the subdirectories
-            if r.status_code == 404:
-                l1 = {}
-            elif r.status_code == 521:
-                raise StopPlaylist()
-            else:
-                #will go to except if there is a another error
-                r.raise_for_status()
-                soup = BeautifulSoup(response, 'html.parser')
-                l1 = { unquote(Path(node.get('href')).name[:-4]) : lr_thumb+node.get('href') for node in soup.find_all('a') if node.get('href').endswith('.png')}
-            args.append(l1)
-    except (RequestError,HTTPStatusError) as err:
-        error(f'Could not get the remote thumbnail game names, exiting: {err}')
-        raise typer.Exit(code=1)
-    return args
+      async with lock_keys(), AsyncClient() as client:
+        with TemporaryDirectory(prefix='libretrofuzz', dir=thumbnails_dir) as tmpdir:
+          for playlist, system in notInSystems:
+            typer.echo(typer.style(f'Custom playlist skipped: ', fg=typer.colors.RED, bold=True) + \
+                       typer.style(f'{system}.lpl', bold=True))
+          for playlist, system in inSystems:
+            typer.echo(typer.style(f'{system}.lpl -> {system}', bold=True))
+            names = readPlaylistAndPrepareDirectories(playlist, tmpdir, thumbnails_dir)
+            try:
+              await downloader(names,system,wait_before,wait_after,filters,score,noimage,nomerge,nofail,nometa, \
+                               hack,nosubtitle,verbose,basic_verbose,before,tmpdir,thumbnails_dir,client)
+            except StopPlaylist as e:
+              error(f'Cloudflare is down for {system}')
+    except StopProgram as e:
+      error(f'Cancelled by user, exiting')
+      raise typer.Exit()
+  asyncio.run(runit(), debug=False)
+
+async def downloadgamenames(client, system):
+  """returns [ dict(Game_Name, Game_Url), dict(Game_Name, Game_Url), dict(Game_Name, Game_Url) ]
+      for each of the server directories '/Named_Boxarts/', '/Named_Titles/', '/Named_Snaps/'
+      (potentially some of these dicts may be empty if the server doesn't have the directory)
+  """
+  lr_thumbs = ADDRESS+'/'+quote(system) #then get the thumbnails from the system name
+  args = []
+  try:
+    for tdir in ['/Named_Boxarts/', '/Named_Titles/', '/Named_Snaps/']:
+      lr_thumb = lr_thumbs+tdir
+      response = ''
+      async with client.stream('GET', lr_thumb, timeout=15) as r:
+        async for chunk in r.aiter_text(4096):
+          checkEscape()
+          response += chunk
+      #not found is ok, since some server system directories do not have all the subdirectories
+      if r.status_code == 404:
+        l1 = {}
+      elif r.status_code == 521:
+        raise StopPlaylist()
+      else:
+        #will go to except if there is a another error
+        r.raise_for_status()
+        soup = BeautifulSoup(response, 'html.parser')
+        l1 = { unquote(Path(node.get('href')).name[:-4]) : lr_thumb+node.get('href') for node in soup.find_all('a') if node.get('href').endswith('.png')}
+      args.append(l1)
+  except (RequestError,HTTPStatusError) as err:
+    error(f'Could not get the remote thumbnail game names, exiting: {err}')
+    raise typer.Exit(code=1)
+  return args
 
 async def downloader(names: [(str,str)],
                system: str,
                wait_before: Optional[float],
                wait_after: Optional[float],
                filters: Optional[List[str]],
                score: int,
                noimage : bool, nomerge: bool, nofail: bool, nometa: bool, hack: bool, nosubtitle: bool, verbose: Optional[int],
+               basic_verbose : bool,
                before: Optional[str],
                tmpdir: Path,
                thumbnails_dir: Path,
                client: AsyncClient
                ):
-    #not a error to pass a empty playlist
-    if len(names) == 0:
-        return
-    thumbs = Thumbs._make( await downloadgamenames(client, system) )
-    #before implies that the names of the playlists may be cut, so the hack and meta matching must be disabled
+  #not a error to pass a empty playlist
+  if len(names) == 0:
+    return
+  thumbs = Thumbs._make( await downloadgamenames(client, system) )
+  #before implies that the names of the playlists may be cut, so the hack and meta matching must be disabled
+  if before:
+    hack = False
+    nometa = True
+  #no-fail is equivalent to max fuzz
+  if nofail:
+    score = 0
+
+  #preprocess data so it's not redone every loop iteration.
+  title_scorer = TitleScorer()
+  #normalize with or without subtitles, besides the remote_names this is used on the iterated local names later
+  norm = nosubtitle_normalizer if nosubtitle else normalizer
+  #we choose the highest similarity of all 3 directories, since no mixed matches are allowed
+  remote_names = set()
+  remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
+  #turn into a set, original key and normalized value.
+  remote_names = { x : norm(x, nometa, hack) for x in remote_names }
+  for (name,destination) in names:
+    await asyncio.sleep(0) #update key status
+    checkEscape()          #check key status
+    #if the user used filters, filter everything that doesn't match any of the globs
+    if filters and not any(map(lambda x : fnmatch.fnmatch(name, x), filters)):
+      continue
+    #to simplify this code, the forbidden characters are replaced twice,
+    #on the string that is going to be the filename and the modified string copy of that that is going to be matched.
+    #it could be done only once, but that would require separating the colon character for subtitle matching,
+    #and the 'before' operation would have to find the index before the match to apply it after. A mess.
+
+    nameaux = name
+
+    #'before' has priority over subtitle removal
     if before:
-        hack = False
-        nometa = True
-    #no-fail is equivalent to max fuzz
-    if nofail:
-        score = 0
-    
-    #preprocess data so it's not redone every loop iteration.
-    title_scorer = TitleScorer()
-    #normalize with or without subtitles, besides the remote_names this is used on the iterated local names later
-    norm = nosubtitle_normalizer if nosubtitle else normalizer
-    #we choose the highest similarity of all 3 directories, since no mixed matches are allowed
-    remote_names = set()
-    remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
-    #turn into a set, original key and normalized value.
-    remote_names = { x : norm(x, nometa, hack) for x in remote_names }
-    for (name,destination) in names:
-        #allow a slighty async pause to be able to update the key status if never won a single score
-        await asyncio.sleep(0)
-        #if called escape without being in a download zone, exit right away without a cancel print
-        checkEscape()
-        #if the user used filters, filter everything that doesn't match any of the globs
-        if filters and not any(map(lambda x : fnmatch.fnmatch(name, x), filters)):
-            continue
-        #to simplify this code, the forbidden characters are replaced twice,
-        #on the string that is going to be the filename and the modified string copy of that that is going to be matched.
-        #it could be done only once, but that would require separating the colon character for subtitle matching,
-        #and the 'before' operation would have to find the index before the match to apply it after. A mess.
-        
-        nameaux = name
-        
-        #'before' has priority over subtitle removal
-        if before:
-            #Ignore metadata and get the string before it
-            name_without_meta = regex.search(before_metadata, nameaux)
-            if name_without_meta:
-                before_index = name_without_meta.group(1).find(before)
-                if before_index != -1:
-                    nameaux = nameaux[0:before_index]
-        
-        #there is a second form of subtitles, which doesn't appear in the thumbnail server directly but can appear in linux game names
-        #that can be more faithful to the real name. It uses the colon character, which is forbidden in windows and only applies to filenames.
-        #Note that this does mean that if the servername has 'Name_ subtitle.png' and not 'Name - subtitle.png' there is less chance of a match,
-        #but that is rarer on the server than the opposite.
-        #not to mention that this only applies if the user signals 'no-subtitle', which presumably means they tried without it - which does match.
-        if nosubtitle:
-            nameaux = nosubtitle_aux(nameaux, ': ')
-        
-        #only the local names should have forbidden characters
-        name = regex.sub(forbidden, '_', name )
-        nameaux = regex.sub(forbidden, '_', nameaux )
-
-        #unlike the server thumbnails, normalization wasn't done yet
-        nameaux = norm(nameaux, nometa, hack)
-        
-        #operate on cache (to speed up by not applying normalization every iteration)
-        #the normalization can make it so that the winner has the same score as the runner up(s) so to make sure we catch at least
-        #two thumbnails for cases where that happens, we check both best scores if we can't find a thumb in a server directory
-        result = process.extract(nameaux, remote_names, scorer=title_scorer,processor=None,limit=verbose or 1,score_cutoff=None)
-        #build the verbose format and decompose the first result, with a optimization if verbose is not on
-        thumb_normal, thumb_score, thumb_name = (None, 0, None)
-        verbose_format = []
-        if verbose:
-          for r in reversed(result):
-            thumb_normal, thumb_score, thumb_name = r
-            color = typer.colors.RED if thumb_score < score else typer.colors.GREEN
-            linke = link(thumb_name, thumb_normal)
-            verbose_format.insert(0, f"{typer.style(f'{int(thumb_score)}', fg=f'{color}', bold=True)} {linke}")
-          verbose_format = ', '.join(verbose_format)
-        elif len(result) > 0:
-          thumb_normal, thumb_score, thumb_name = result[0]
-        #hack, if result 1 and 2 have equal scores use the second thumbnail as a alternative if missing a thumb type
-        #this is done because it's relatively common for the server to have a case mistake on thumb types
-        thumb_name2 = None
-        if len(result) >= 2:
-          if result[0][1] == result[1][1]:
-            thumb_name2 = result[1][2]
-        #formating legos
-        name_format    = link(name,nameaux) + ' -> ' + verbose_format if verbose else f'{name} -> {thumb_name}'
-        success_format = f'{typer.style("Success",   fg=typer.colors.GREEN, bold=True)}: {name_format}'
-        failure_format = f'{typer.style("Failure",     fg=typer.colors.RED, bold=True)}: {name_format}'
-        missing_format = f'{typer.style("Missing",     fg=typer.colors.RED, bold=True)}: {name_format}'
-        cancel_format  = f'{typer.style("Skipped",        fg=(135,135,135), bold=True)}: {name_format}'
-        nomerge_format = f'{typer.style("Nomerge",        fg=(128,128,128), bold=True)}: {name_format}'
-        getting_format = f'{typer.style("Getting",    fg=typer.colors.BLUE, bold=True)}: {name_format}'
-        waiting_format = f'{typer.style("Waiting",  fg=typer.colors.YELLOW, bold=True)}: {name_format}' \
-                         + typer.style(' {remaining_s:2.1f}s', fg=typer.colors.RED, bold=True)
-        if thumb_name and thumb_score >= score:
-            allow = True
-            #these parent directories were created when reading the playlist, more efficient than doing it a playlist game loop
-            real_thumb_dir = Path(thumbnails_dir,destination)
-            down_thumb_dir = Path(tmpdir,destination)
-            if not filters and nomerge:
-                #to implement no-merge you have to disable downloads on 'at least one' thumbnail (including user added ones)
-                missing_thumbs = 0
-                missing_server_thumbs = 0
-                for dirname in Thumbs._fields:
-                    real = Path(real_thumb_dir, dirname, name + '.png')
-                    if not real.exists():
-                        missing_thumbs += 1
-                        if thumb_name in getattr(thumbs, dirname) or thumb_name2 in getattr(thumbs, dirname):
-                            missing_server_thumbs += 1
-                allow = missing_thumbs == 3
-                #despite the above, print only for when it would download if it was allowed, otherwise it is confusing
-                if not allow and missing_server_thumbs > 0:
-                    typer.echo(nomerge_format)
-            if allow:
-                first_wait      = wait_before is not None
-                downloaded_once = False
-                downloaded_dict = dict() #dictionary of thumbnailtype -> (old Path, new Path), paths may not exist
-                try:
-                    for dirname in Thumbs._fields:
-                        real = Path(real_thumb_dir, dirname, name + '.png')
-                        temp = Path(down_thumb_dir, dirname, name + '.png')
-                        downloaded_dict[dirname] = (real, temp)
-                        #something to download
-                        thumbmap = getattr(thumbs, dirname)
-                        url = thumbmap[thumb_name] if thumb_name in thumbmap else thumbmap.get(thumb_name2, None)
-                        #with filters/reset you always download, and without only if it doesn't exist already.
-                        if url and (filters or not real.exists()):
-                            download_format = f'{getting_format}' '{bar:-9b}' f'{dirname[6:-1]}' ' {percentage:3.0f}%: {bar:10u}'
-                            if await download(client,url,temp,download_format,missing_format,waiting_format,first_wait,wait_before,MAX_RETRIES):
-                                first_wait = False
-                                downloaded_once = True
-                        elif filters:
-                            #nothing to download but we want to remove images that may be there in the case of --filter.
-                            real.unlink(missing_ok=True)
-                    if not noimage and viewer and downloaded_once:
-                        displayImages(downloaded_dict)
-                        if wait_after is not None:
-                            await printwait(wait_after, waiting_format)
-                except StopProgram as e:
-                    typer.echo(cancel_format)
-                    raise e
-                except StopDownload as e:
-                    downloaded_once = False
-                    typer.echo(cancel_format)
-                if downloaded_once:
-                    for (old, new) in downloaded_dict.values():
-                        if new.exists():
-                            shutil.move(new, old)
-                    typer.echo(success_format)
-        else:
-            if verbose:
-              typer.echo(failure_format)
-            if filters:
+      #Ignore metadata and get the string before it
+      name_without_meta = regex.search(before_metadata, nameaux)
+      if name_without_meta:
+        before_index = name_without_meta.group(1).find(before)
+        if before_index != -1:
+          nameaux = nameaux[0:before_index]
+
+    #there is a second form of subtitles, which doesn't appear in the thumbnail server
+    #but can appear in linux game names. It uses the colon character, which is forbidden
+    #in windows. Note that this does mean that if the servername has 'Name_ subtitle.png'
+    #and not 'Name - subtitle.png' there is less chance of a match, but that is rarer than opposite.
+    #not to mention that this only applies if the user signals 'no-subtitle',
+    #which presumably means they tried without it - which does match.
+    if nosubtitle:
+      nameaux = nosubtitle_aux(nameaux, ': ')
+
+    #only the local names should have forbidden characters
+    name = regex.sub(forbidden, '_', name )
+    nameaux = regex.sub(forbidden, '_', nameaux )
+
+    #unlike the server thumbnails, normalization wasn't done yet
+    nameaux = norm(nameaux, nometa, hack)
+
+    #operate on cache (to speed up by not applying normalization every iteration)
+    #the normalization can make it so that the winner has the same score as the runner up(s) so to make sure we catch at least
+    #two thumbnails for cases where that happens, we check both best scores if we can't find a thumb in a server directory
+    result = process.extract(nameaux, remote_names, scorer=title_scorer,processor=None,limit=verbose or 1,score_cutoff=None)
+    #build the verbose format and decompose the first result, with a optimization if verbose is not on
+    thumb_normal, thumb_score, thumb_name = (None, 0, None)
+    verbose_format = []
+    if verbose:
+      for r in reversed(result):
+        thumb_normal, thumb_score, thumb_name = r
+        color = typer.colors.RED if thumb_score < score else typer.colors.GREEN
+        verbose_score = typer.style(f'{int(thumb_score)}', fg=f'{color}', bold=True)
+        verbose_name  = thumb_normal if basic_verbose else link(thumb_name, thumb_normal)
+        verbose_format.insert(0, f"{verbose_score} {verbose_name}")
+      verbose_format = ', '.join(verbose_format)
+    elif len(result) > 0:
+      thumb_normal, thumb_score, thumb_name = result[0]
+    #hack, if result 1 and 2 have equal scores use the second thumbnail as a alternative if missing a thumb type
+    #this is done because it's relatively common for the server to have a case mistake on thumb types
+    thumb_name2 = None
+    if len(result) >= 2:
+      if result[0][1] == result[1][1]:
+        thumb_name2 = result[1][2]
+    #formating legos
+    name_format    = nameaux if basic_verbose else link(name,nameaux)
+    dull_format    = f'{name} -> {thumb_name}'
+    line_format    = name_format + ' -> ' + verbose_format if verbose else dull_format
+    success_format = f'{typer.style("Success",   fg=typer.colors.GREEN, bold=True)}: {line_format}'
+    failure_format = f'{typer.style("Failure",     fg=typer.colors.RED, bold=True)}: {line_format}'
+    missing_format = f'{typer.style("Missing",     fg=typer.colors.RED, bold=True)}: {line_format}'
+    skipped_format = f'{typer.style("Skipped",        fg=(135,135,135), bold=True)}: {line_format}'
+    nomerge_format = f'{typer.style("Nomerge",        fg=(128,128,128), bold=True)}: {line_format}'
+    getting_format = f'{typer.style("Getting",    fg=typer.colors.BLUE, bold=True)}: {dull_format}' \
+                     + typer.style(' {percentage:3.0f}%', fg=typer.colors.BLUE, bold=True)
+    waiting_format = f'{typer.style("Waiting",  fg=typer.colors.YELLOW, bold=True)}: {dull_format}' \
+                     + typer.style(' {remaining_s:2.1f}s', fg=typer.colors.RED, bold=True)                         
+    if thumb_name and thumb_score >= score:
+      allow = True
+      #these parent directories were created when reading the playlist, more efficient than doing it a playlist game loop
+      real_thumb_dir = Path(thumbnails_dir,destination)
+      down_thumb_dir = Path(tmpdir,destination)
+      if not filters and nomerge:
+        #to implement no-merge you have to disable downloads on 'at least one' thumbnail (including user added ones)
+        missing_thumbs = 0
+        missing_server_thumbs = 0
+        for dirname in Thumbs._fields:
+          real = Path(real_thumb_dir, dirname, name + '.png')
+          if not real.exists():
+            missing_thumbs += 1
+            if thumb_name in getattr(thumbs, dirname) or thumb_name2 in getattr(thumbs, dirname):
+              missing_server_thumbs += 1
+        allow = missing_thumbs == 3
+        #despite the above, print only for when it would download if it was allowed, otherwise it is confusing
+        if not allow and missing_server_thumbs > 0:
+          typer.echo(nomerge_format)
+      if allow:
+        first_wait      = wait_before is not None
+        downloaded_once = False
+        downloaded_dict = dict() #dictionary of thumbnailtype -> (old Path, new Path), paths may not exist
+        try:
+          for dirname in Thumbs._fields:
+            real = Path(real_thumb_dir, dirname, name + '.png')
+            temp = Path(down_thumb_dir, dirname, name + '.png')
+            downloaded_dict[dirname] = (real, temp)
+            #something to download
+            thumbmap = getattr(thumbs, dirname)
+            url = thumbmap[thumb_name] if thumb_name in thumbmap else thumbmap.get(thumb_name2, None)
+            #with filters/reset you always download, and without only if it doesn't exist already.
+            if url and (filters or not real.exists()):
+              if await download(client,url,temp,getting_format,missing_format,waiting_format,first_wait,wait_before,MAX_RETRIES):
+                first_wait = False
+                downloaded_once = True
+            elif filters:
               #nothing to download but we want to remove images that may be there in the case of --filter.
-              for dirname in Thumbs._fields:
-                Path(thumbnails_dir,destination, dirname, name + '.png').unlink(missing_ok=True)
+              real.unlink(missing_ok=True)
+          if not noimage and viewer and downloaded_once:
+            displayImages(downloaded_dict)
+            if wait_after is not None:
+              await printwait(wait_after, waiting_format)
+        except StopProgram as e:
+          typer.echo(skipped_format)
+          raise e
+        except StopDownload as e:
+          downloaded_once = False
+          typer.echo(skipped_format)
+        if downloaded_once:
+          for (old, new) in downloaded_dict.values():
+            if new.exists():
+              shutil.move(new, old)
+          typer.echo(success_format)
+    else:
+      if verbose:
+        typer.echo(failure_format)
+      if filters:
+        #nothing to download but we want to remove images that may be there in the case of --filter.
+        for dirname in Thumbs._fields:
+          Path(thumbnails_dir,destination, dirname, name + '.png').unlink(missing_ok=True)
 
 async def printwait(wait : Optional[float], waiting_format: str):
-    count = int(wait/0.1)
-    with handleContinueDownload():
-      for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, colour='YELLOW', leave=False):
-        checkDownload()
-        await asyncio.sleep(0.1)
-
-async def download(client, url, destination, download_format, missing_format, waiting_format, first_wait, wait_before, max_retries):
-    '''returns True if downloaded. To download, it must have waited, if first_wait is True. Exceptions may happen instead of returning False, but they
-    are all caught outside the caller loop of thumbnail types that downloads, so the first_wait guard gets reset again and only waits once per game'''
-    while True:
-        try:
-            async with client.stream('GET', url, timeout=15) as r:
-                if r.status_code == 521: #cloudflare exploded, skip the whole playlist
-                    raise StopPlaylist()
-                if r.status_code == 404: #broken image or symlink link, skip just this thumb
-                    typer.echo(missing_format + ' ' + url)
-                    return False
-                r.raise_for_status()     #error before reading the header goes into retrying
-                length = int(r.headers['Content-Length'])
-                if length < 100:         #obviously corrupt 'thumbnail', skip this thumb
-                    typer.echo(missing_format + ' ' + url)
-                    return False
-                with open(destination, 'w+b') as f:
-                    if first_wait:
-                        await printwait(wait_before, waiting_format)
-                    with tqdm.wrapattr(f, 'write', total=length, dynamic_ncols=True, bar_format=download_format, colour='BLUE', leave=False) as w:
-                        async for chunk in r.aiter_raw(4096):
-                          with handleContinueDownload():
-                            checkDownload()
-                          w.write(chunk)
-            return True
-        except (RequestError,HTTPStatusError) as e:
-            if max_retries <= 0:
-                error(f'Download max retries exceeded, exiting')
-                raise typer.Exit(code=1)
-            max_retries -= 1
+  count = int(wait/0.1)
+  with handleContinueDownload():
+    for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, leave=False):
+      checkDownload()
+      await asyncio.sleep(0.1)
+
+async def download(client, url, destination, getting_format, missing_format, waiting_format, first_wait, wait_before, max_retries):
+  '''returns True if downloaded. To download, it must have waited, if first_wait is True. Exceptions may happen instead of returning False, but they
+  are all caught outside the caller loop of thumbnail types that downloads, so the first_wait guard gets reset again and only waits once per game
+  '''
+  while True:
+    try:
+      async with client.stream('GET', url, timeout=15) as r:
+        if r.status_code == 521: #cloudflare exploded, skip the whole playlist
+          raise StopPlaylist()
+        if r.status_code == 404: #broken image or symlink link, skip just this thumb
+          typer.echo(missing_format + ' ' + url)
+          return False
+        r.raise_for_status()     #error before reading the header goes into retrying
+        length = int(r.headers['Content-Length'])
+        if length < 100:         #obviously corrupt 'thumbnail', skip this thumb
+          typer.echo(missing_format + ' ' + url)
+          return False
+        with open(destination, 'w+b') as f:
+          if first_wait:
+            await printwait(wait_before, waiting_format)
+          with tqdm.wrapattr(f, 'write', total=length, dynamic_ncols=True, bar_format=getting_format, leave=False) as w:
+            async for chunk in r.aiter_raw(4096):
+              with handleContinueDownload():
+                checkDownload()
+              w.write(chunk)
+      return True
+    except (RequestError,HTTPStatusError) as e:
+      if max_retries <= 0:
+        error(f'Download max retries exceeded, exiting')
+        raise typer.Exit(code=1)
+      max_retries -= 1
 
 def displayImages(downloaded: dict):
-    '''dict has all the tuple (old, new) with the key of the thumbnail type str (the files may not exist)
-       this method will display the new images with a green border and the old with a gray border and missing as... missing
-    '''
-    imgs = dict()
-    colors = dict()
-    BORDER_SIZE = 4
-    #first create images for the thumbnails
-    #single frame pillow images automatically close when
-    #their image data (not header) is accessed, so you
-    #don't have to worry about closing 'the original'
-    for k,i in downloaded.items():
-        old, new = i
-        #do not create the border yet, wait for the end of the method
-        if new.exists():
-            imgs[k] = Image.open(new).convert('RGBA')
-            colors[k] = (135,255,0)
-        elif old.exists():
-            imgs[k] = Image.open(old).convert('RGBA')
-            colors[k] = (128,128,128)
-        else:
-            #default transparent images, small enough to give primacy
-            #to the others while still showing 'something missing'
-            #size taken from the SNES snapshot default resolution
-            imgs[k] = Image.new('RGBA', (256,224), (255, 0, 0, 0))
-            colors[k] = (0,0,0,0) #transparent 'border'
-    box   = imgs.get('Named_Boxarts', None)
-    title = imgs.get('Named_Titles', None)
-    snap  = imgs.get('Named_Snaps', None)
-    #we are trying to make a rectangle, where the left side has the boxart, and the right side has the snap and title, stacked vertically.
-    #the height of left and right will be the largest height on the available thumbnails, except for the borders (added after the resizes, so they look the same)
-    wanted_box_y = max([ i.size[1] for i in imgs.values() ])
-    x,y = box.size
-    if y != wanted_box_y:
-        x = max(round(x * wanted_box_y / y), 1)
-        y = wanted_box_y
-    box = box.resize((x,y))
-    #the right side will adjust the width until title and snap are the same width and the desired height is reached (minus inner borders).
-    wanted_y = wanted_box_y - BORDER_SIZE*2
-    x1, y1 = title.size
-    x2, y2 = snap.size
-    #Formulas to derive the value of samex (same width they need to reach wanted_y):
-    #wanted_y = yx1 + yx2 and yx1 = y1 * samex / x1 and yx2 = y2 * samex / x2
-    #then:
-    #wanted_y = y1/x1 * samex + y2/x2 * samex <=>
-    #wanted_y/samex = y1/x1 + y2/x2           <=>
-    #samex = wanted_y / (y1/x1 + y2/x2)
-    x1,y1 = title.size
-    x2,y2 = snap.size
-    samex = wanted_y / (y1/x1 + y2/x2)
-    new_y1 = max(1, round(y1 * samex / x1))
-    new_y2 = max(1, round(y2 * samex / x2))
-    samex  = max(1, round(samex))
-    title = title.resize((samex, new_y1))
-    snap  = snap.resize((samex, new_y2))
-    #add borders
-    box   = ImageOps.expand(box,   border=(BORDER_SIZE,)*4, fill=colors['Named_Boxarts'])
-    title = ImageOps.expand(title, border=(BORDER_SIZE,)*4, fill=colors['Named_Titles'])
-    snap  = ImageOps.expand(snap,  border=(BORDER_SIZE,)*4, fill=colors['Named_Snaps'])
-    #create a 'paste' image
-    combined = Image.new('RGBA', (box.size[0] + title.size[0], box.size[1]) )
-    combined.paste(box, box=(0,0))
-    combined.paste(title, box=(box.size[0],0))
-    combined.paste(snap, box=(box.size[0], title.size[1]))
-    #save it, print TODO if a _good_ python sixtel library happens, replace this
-    with io.BytesIO() as f:
-        combined.save(f, format='png')
-        subprocess.run([viewer, '-'], input=f.getbuffer())
+  '''dict has all the tuple (old, new) with the key of the thumbnail type str (the files may not exist)
+     this method will display the new images with a green border and the old with a gray border and missing as... missing
+  '''
+  imgs = dict()
+  colors = dict()
+  BORDER_SIZE = 4
+  #first create images for the thumbnails
+  #single frame pillow images automatically close when
+  #their image data (not header) is accessed, so you
+  #don't have to worry about closing 'the original'
+  for k,i in downloaded.items():
+    old, new = i
+    #do not create the border yet, wait for the end of the method
+    if new.exists():
+      imgs[k] = Image.open(new).convert('RGBA')
+      colors[k] = (135,255,0)
+    elif old.exists():
+      imgs[k] = Image.open(old).convert('RGBA')
+      colors[k] = (128,128,128)
+    else:
+      #default transparent images, small enough to give primacy
+      #to the others while still showing 'something missing'
+      #size taken from the SNES snapshot default resolution
+      imgs[k] = Image.new('RGBA', (256,224), (255, 0, 0, 0))
+      colors[k] = (0,0,0,0) #transparent 'border'
+  box   = imgs.get('Named_Boxarts', None)
+  title = imgs.get('Named_Titles', None)
+  snap  = imgs.get('Named_Snaps', None)
+  #we are trying to make a rectangle, where the left side has the boxart,
+  #and the right side has the snap and title, stacked vertically.
+  #the height of left and right will be the largest height on the
+  #available thumbnails, except for the borders
+  #(added after the resizes, so they look the same)
+  wanted_box_y = max([ i.size[1] for i in imgs.values() ])
+  x,y = box.size
+  if y != wanted_box_y:
+    x = max(round(x * wanted_box_y / y), 1)
+    y = wanted_box_y
+  box = box.resize((x,y))
+  #the right side will adjust the width until title and snap are the same width and the desired height is reached (minus inner borders).
+  wanted_y = wanted_box_y - BORDER_SIZE*2
+  x1, y1 = title.size
+  x2, y2 = snap.size
+  #Formulas to derive the value of samex (same width they need to reach wanted_y):
+  #wanted_y = yx1 + yx2 and yx1 = y1 * samex / x1 and yx2 = y2 * samex / x2
+  #then:
+  #wanted_y = y1/x1 * samex + y2/x2 * samex <=>
+  #wanted_y/samex = y1/x1 + y2/x2           <=>
+  #samex = wanted_y / (y1/x1 + y2/x2)
+  x1,y1 = title.size
+  x2,y2 = snap.size
+  samex = wanted_y / (y1/x1 + y2/x2)
+  new_y1 = max(1, round(y1 * samex / x1))
+  new_y2 = max(1, round(y2 * samex / x2))
+  samex  = max(1, round(samex))
+  title = title.resize((samex, new_y1))
+  snap  = snap.resize((samex, new_y2))
+  #add borders
+  box   = ImageOps.expand(box,   border=(BORDER_SIZE,)*4, fill=colors['Named_Boxarts'])
+  title = ImageOps.expand(title, border=(BORDER_SIZE,)*4, fill=colors['Named_Titles'])
+  snap  = ImageOps.expand(snap,  border=(BORDER_SIZE,)*4, fill=colors['Named_Snaps'])
+  #create a 'paste' image
+  combined = Image.new('RGBA', (box.size[0] + title.size[0], box.size[1]) )
+  combined.paste(box, box=(0,0))
+  combined.paste(title, box=(box.size[0],0))
+  combined.paste(snap, box=(box.size[0], title.size[1]))
+  #save it, print TODO if a _good_ python sixtel library happens, replace this
+  with io.BytesIO() as f:
+    combined.save(f, format='png')
+    subprocess.run([viewer, '-'], input=f.getbuffer())
 
 def fuzzsingle():
-    typer.run(mainfuzzsingle)
+  typer.run(mainfuzzsingle)
 
 def fuzzall():
-    typer.run(mainfuzzall)
+  typer.run(mainfuzzall)
 
 if __name__ == "__main__":
-    error('Please run libretro-fuzz or libretro-fuzzall instead of running the script directly')
-    raise typer.Exit(code=1)
+  error('Please run libretro-fuzz or libretro-fuzzall instead of running the script directly')
+  raise typer.Exit(code=1)
```

### Comparing `libretrofuzz-2.9.5/pyproject.toml` & `libretrofuzz-2.9.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.9.5"
+version = "2.9.6"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.9.5/setup.py` & `libretrofuzz-2.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.9.5',
+    'version': '2.9.6',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show mininame, len N list (maxscore, server mininame).\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-2.9.5/PKG-INFO` & `libretrofuzz-2.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.9.5
+Version: 2.9.6
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

