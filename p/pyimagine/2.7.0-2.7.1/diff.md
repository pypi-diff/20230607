# Comparing `tmp/pyimagine-2.7.0.tar.gz` & `tmp/pyimagine-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimagine-2.7.0.tar", last modified: Tue Jun  6 08:06:26 2023, max compression
+gzip compressed data, was "pyimagine-2.7.1.tar", last modified: Wed Jun  7 08:42:46 2023, max compression
```

## Comparing `pyimagine-2.7.0.tar` & `pyimagine-2.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 08:06:26.963749 pyimagine-2.7.0/
--rw-rw-rw-   0        0        0    35823 2023-06-06 07:13:27.000000 pyimagine-2.7.0/LICENSE
--rw-rw-rw-   0        0        0     3294 2023-06-06 08:06:26.963749 pyimagine-2.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     2378 2023-06-06 08:04:15.000000 pyimagine-2.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 08:06:26.939752 pyimagine-2.7.0/pyimagine/
--rw-rw-rw-   0        0        0       66 2023-06-06 07:29:12.000000 pyimagine-2.7.0/pyimagine/__init__.py
--rw-rw-rw-   0        0        0    40680 2023-06-05 19:16:09.000000 pyimagine-2.7.0/pyimagine/constants.py
--rw-rw-rw-   0        0        0      156 2023-06-05 19:24:08.000000 pyimagine-2.7.0/pyimagine/exceptions.py
--rw-rw-rw-   0        0        0     1290 2023-06-06 06:50:07.000000 pyimagine-2.7.0/pyimagine/utils.py
--rw-rw-rw-   0        0        0     7271 2023-06-06 07:59:42.000000 pyimagine-2.7.0/pyimagine/vyroai.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:06:26.963749 pyimagine-2.7.0/pyimagine.egg-info/
--rw-rw-rw-   0        0        0     3294 2023-06-06 08:06:26.000000 pyimagine-2.7.0/pyimagine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-06 08:06:26.000000 pyimagine-2.7.0/pyimagine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 08:06:26.000000 pyimagine-2.7.0/pyimagine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-06 08:06:26.000000 pyimagine-2.7.0/pyimagine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-06 08:06:26.000000 pyimagine-2.7.0/pyimagine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 08:06:26.963749 pyimagine-2.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1230 2023-06-06 07:36:10.000000 pyimagine-2.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:06:26.963749 pyimagine-2.7.0/test/
--rw-rw-rw-   0        0        0     1892 2023-06-06 08:00:40.000000 pyimagine-2.7.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:42:45.994888 pyimagine-2.7.1/
+-rw-rw-rw-   0        0        0    35823 2023-06-07 07:31:40.000000 pyimagine-2.7.1/LICENSE
+-rw-rw-rw-   0        0        0     3407 2023-06-07 08:42:45.994888 pyimagine-2.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2491 2023-06-07 08:27:32.000000 pyimagine-2.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 08:42:45.963576 pyimagine-2.7.1/pyimagine/
+-rw-rw-rw-   0        0        0       66 2023-06-07 08:12:04.000000 pyimagine-2.7.1/pyimagine/__init__.py
+-rw-rw-rw-   0        0        0    44546 2023-06-07 08:37:05.000000 pyimagine-2.7.1/pyimagine/constants.py
+-rw-rw-rw-   0        0        0      240 2023-06-07 08:24:35.000000 pyimagine-2.7.1/pyimagine/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2023-06-07 08:22:50.000000 pyimagine-2.7.1/pyimagine/utils.py
+-rw-rw-rw-   0        0        0     7587 2023-06-07 08:36:19.000000 pyimagine-2.7.1/pyimagine/vyroai.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:42:45.994888 pyimagine-2.7.1/pyimagine.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-06-07 08:42:45.000000 pyimagine-2.7.1/pyimagine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-07 08:42:45.000000 pyimagine-2.7.1/pyimagine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 08:42:45.000000 pyimagine-2.7.1/pyimagine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-07 08:42:45.000000 pyimagine-2.7.1/pyimagine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-07 08:42:45.000000 pyimagine-2.7.1/pyimagine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 08:42:45.994888 pyimagine-2.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2023-06-07 08:12:04.000000 pyimagine-2.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:42:45.994888 pyimagine-2.7.1/test/
+-rw-rw-rw-   0        0        0     1911 2023-06-07 08:35:57.000000 pyimagine-2.7.1/test/test.py
```

### Comparing `pyimagine-2.7.0/LICENSE` & `pyimagine-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimagine-2.7.0/PKG-INFO` & `pyimagine-2.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimagine
-Version: 2.7.0
+Version: 2.7.1
 Summary: Python library for AI-powered image manipulation.
 Home-page: https://github.com/hyugogirubato/pyimagine
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: art,image,ai,stable-diffusion
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,15 +57,15 @@
 from pyimagine import Imagine
 from pyimagine.constants import Inspiration
 
 # Initialize Imagine
 imagine = Imagine()
 
 # Generate an inspired image
-inspired_image = imagine.inspire(Inspiration.INSPIRATION_01)
+inspired_image = imagine.sdinsp(Inspiration.INSPIRATION_01)
 
 # Variate an image
 original_image = open("image.jpg", "rb").read()
 variated_image = imagine.variate(original_image, prompt="Create something amazing!")
 
 # Upscale an image
 upscaled_image = imagine.upscale(original_image)
@@ -79,11 +79,12 @@
 ### Exceptions
 
 The following exceptions can be raised by PyImagine:
 
 - `InvalidWord`: Raised when a banned word is found in the prompt. By default, if the `restricted` flag is set to `True`
   during initialization, the library will raise an `InvalidWord` exception. You can customize this behavior by setting
   `restricted` to `False` to replace banned words with alternative words instead of raising an exception.
+- `InvalidSize`: Raised when attempting to perform an operation that requires both images to have the same size.
 
 ### License
 
 This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pyimagine/blob/main/LICENSE).
```

### Comparing `pyimagine-2.7.0/README.md` & `pyimagine-2.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from pyimagine import Imagine
 from pyimagine.constants import Inspiration
 
 # Initialize Imagine
 imagine = Imagine()
 
 # Generate an inspired image
-inspired_image = imagine.inspire(Inspiration.INSPIRATION_01)
+inspired_image = imagine.sdinsp(Inspiration.INSPIRATION_01)
 
 # Variate an image
 original_image = open("image.jpg", "rb").read()
 variated_image = imagine.variate(original_image, prompt="Create something amazing!")
 
 # Upscale an image
 upscaled_image = imagine.upscale(original_image)
@@ -55,11 +55,12 @@
 ### Exceptions
 
 The following exceptions can be raised by PyImagine:
 
 - `InvalidWord`: Raised when a banned word is found in the prompt. By default, if the `restricted` flag is set to `True`
   during initialization, the library will raise an `InvalidWord` exception. You can customize this behavior by setting
   `restricted` to `False` to replace banned words with alternative words instead of raising an exception.
+- `InvalidSize`: Raised when attempting to perform an operation that requires both images to have the same size.
 
 ### License
 
 This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pyimagine/blob/main/LICENSE).
```

### Comparing `pyimagine-2.7.0/pyimagine/constants.py` & `pyimagine-2.7.1/pyimagine/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Generated by the firebase web compiler.  DO NOT EDIT!
 # source: firebase.py
 
 from enum import Enum
 
 # Banned
-BANNED_WORDS = ['cock', 'dick', 'cumshot', 'fuck', 'sperm', 'naked', 'ass', 'tits', 'fingering', 'masturbate', 'bitch', 'blowjob', 'prostitute', 'dickhead', 'pussy', 'asshole', 'boobs', 'boob', 'breast', 'dildo', 'erection', 'dick', 'licking', 'nude', 'penis', 'porn', 'vagina', 'threesome', 'orgy', 'bdsm', 'condom', 'sexting', 'squirt', 'testicles', 'anal', 'bukkake', 'creampie', 'stripper', 'strap-on', 'missionary', 'clitoris', 'cock ring', 'doggy style', 'sex', 'lingerie', 'milf', 'oral', 'sucking', 'straddle', 'bondage', 'orgasm', 'slut', 'cumming', 'ode', "men's milk", 'jerk', 'cunt', 'anal', 'anus', 'adult film', 'adult movie', 'adult video', 'anal', 'ass', 'bdsm', 'bestiality', 'bisexual', 'bitch', 'boobies', 'boobys', 'bound & gagged', 'bound and gagged', 'breast', 'breasts', 'butt', 'cock', 'condom', 'cuck-old', 'cuckold', 'cum', 'cum-shot', 'cunt', 'deep throat', 'dick', 'erotic', 'escort', 'fuck', 'fucking', 'fucked', 'fucks', 'hentai', 'hustler', 'jerking off', 'kinky', 'lesbian', 'naked', 'nude', 'orgasm', 'nudity', 'penis', 'porn', 'pornagraphy', 'pussy', 'rape', 'semen', 'sex', 'sexual', 'slut', 'threesome', 'tube8', 'twink', 'upskirt', 'vagina', 'virgin', 'whore', 'xxx', 'nudity', 'milfs', 'porn']
+BANNED_WORDS = ['erotism', 'bitches', 'neonazi', 'menstral', 'felch', 'masturbating', 'cum', 'tushy', 'fucktards', 'gore', 'bukkake', 'nipples', 'deapthroating', 'gloryhole', 'quim', 'dick', 'cunt', 'nawashi', 'pussy', 'clitoris', 'squirting', 'deep-throating', 'slut', 'tube8', 'tit', 'breast', 'breasts', 'faggot', 'spunk', 'crucified', 'grope', 'bareback', 'spooge', 'booty', 'doggie style', 'doggy style', 'emetophilia', 'adult film', 'tranny', 'flesh', 'ballgag', 'licking', 'cornhole', 'threesome', 'dong', 'cialis', 'pedobear', 'voyeurweb', 'pornhab', 'pornhub', 'oppai', 'schlong', 'shrimping', 'succubus', 'scissoring', 'asshat', 'bastard', 'skimpy', 'boudoir', 'badonkers', 'asslover', 'erections', 'ponyplay', 'pornography', 'orgasm', 'dickhead', 'orgie', 'adult video', 'hardcore', 'butt', 'poontang', 'pornstar', 'sexting', 'scantily', 'pornagraphy', 'viagra', 'deep thraoting', 'semen', 'sucking', 'hentai', 'big ass', 'sexy female', 'kike', 'yaoi', 'invisible clothes', 'foreskin', 'boobies', 'no shirt', 'zero clothes', 'penis', 'sexual', 'erotica', 'nymphomania', 'beastiality', 'babeland', 'ejaculation', 'penis', 'sexuality', 'asshore', 'jizz', 'glory hole', 'nude', 'doggiestyle', 'shit', 'gay', 'fetish', 'nazi', 'genitals', 'cocks', 'pus', 'hardcore', 'shemale', 'bitch', 'zoophilia', 'nipple', 'frotting', 'poop', 'pisspig', 'torture', 'carpetmuncher', 'handjob', 'anus', 'corpse', 'shibari', 'pornhub', 'assmunch', 'circlejerk', 'penetration', 'buttcheeks', 'femdom', 'cock ring', 'sucks', 'fisting', 'nigger', 'jerk off', 'rule34', 'nympho', 'cuck-old', 'contraceptive', 'asslicker', 'cum-shot', 'hentai', 'nipple', 'fart', 'bondage', 'dendrophilia', 'fucker', 'ovaries', 'asses', 'assjockey', 'homoerotic', 'hooker', '2g1c', 'yiff', 'fingering', 'nambla', 'bdsm', 'clunge', 'barely dressed', 'pussyboy', 'nsfw', 'asswipe', 'cumming', 'pubes', 'sodomy', 'menstrual', 'butthole', 'pissing', 'fascist', 'nutten', 'sodomize', 'pthc', 'titties', 'bimbos', 'transman', 'tits', 'make out', 'vagina', 'clusterfuck', 'assfuck', 'fuckin', 'assman', 'twink', 'kinkster', 'erection', 'blumpkin', 'slaughter', 'bodily fluids', 'pegging', 'voyuer', 'orgy', 'dingleberry', 'bbw', 'jerk', 'topless', 'asskisser', 'dominatrix', 'cowgirl', 'sexually', 'booty', 'deep-throat', 'thot', 'naked', 'knobbing', 'cuck', 'hard-on', 'felching', 'deepthroat', 'poop', 'fucking', 'doggystyle', 'wank', 'bisexual', 'assmuncher', 'urophilia', 'milf', 'suck', 'undressing', 'dommes', 'gangbang', 'twerk', 'bigass', 'cleavage', 'vaginamen', 'dick', 'condom', 's&m', 'figging', 'strapon', 'punany', 'lgbt', 'cunnilingus', 'masturbate', 'hermaphrodite', 'cumshots', 'pedophile', 'deepthroating', 'daterape', 'smallpussy', 'livesex', 'barely legal', 'gay', 'nudity', 'incest', 'deep-thraoting', 'deap throating', 'busty', 'voluptuous', 'thumbzilla', 'boob', 'youporn', 'bangbus', 'moan', 'throating', 'crotch', 'erotic', 'fucked', 'coprophilia', 'missionary', 'rimming', 'deep throat', 'nymphomania', 'tribadism', 'arse', 'succubus', 'arsehole', 'deepthraoting', 'femdon', 'splooge', 'asskiss', 'poopchute', 'gokkun', 'zoophilia', 'cuckold', 'disturbing', 'transsexual', 'voluptuous', 'surgery', 'asspacker', 'asslick', 'no clothes', 'playboy', 'fag', 'dildo', 'deap-throating', 'milking', 'fudgepacker', 'oral', 'coon', 'bruises', 'playboy', 'autoerotic', 'female body parts', 'voyeur', 'footjob', 'bung', 'assmonkey', 'rapist', 'g-spot', 'menstraul', 'masturbation', 'ass', 'erotic', 'jerking off', 'jerk', 'jerking', 'panty', 'ass', 'anilingus', 'brown pudding', 'phallus', 'noclothes', 'octopussy', 'asswhore', 'badfuck', 'labia', 'anus', 'bdsm', 'hooters', 'assholes', 'porn', 'wearing nothing', 'bestiality', 'ahegao', 'bullshit', 'slavegirl', 'farts', 'fellatio', 'cannibal', 'clit', 'inappropriate', 'shitty', 'warts', 'queef', 'squirt', 'sperm', 'acrotomophilia', 'porno', 'piercing', 'hardon', 'assklown', 'massacre', 'deep-thraot', 'asshole', 'muffdiving', 'deep thraot', 'facesitting', 'kinbaku', 'strap-on', 'lesbian', 'vagina', 'queaf', 'sultry', 'raping', 'creampie', 'strappado', 'xxx', 'infant nudity', 'tryphophobia', 'brothel', 'crucifixion', 'lgbtq', 'perv', 'titty', 'anal', 'dirty', 'cleaver', 'shota', 'pervert', 'cannibalism', 'shit', 'jigaboo', 'rectum', 'lovemaking', 'towelhead', 'urethra', 'bastinado', 'camgirl', 'vulva', 'barenaked', 'omorashi', 'bollocks', 'tubgirl', 'deapthroat', 'rimjob', 'cock', 'rape', 'cucked', 'asspirate', 'blowjob', 'jiggerboo', 'bosom', 'mammaries', 'sugar daddy', 'minge', 'feltch', 'bulldyke', 'sultry', 'whore', 'testicles', 'xx', 'camwhore', 'motherfucker', 'booba', 'deap-throat', 'breasts', 'sperm', 'bondage', 'kinky', 'xxx', 'cumshot', 'boobys', 'ecchi', 'sex', 'juggs', 'asspuppies', 'boobs', 'fuck', 'upskirt', 'busty', 'horny', 'menpussy', 'transgender', 'deep throating', 'nimphomania', 'deap throat', 'bang', 'piss', 'bangbros', 'prophet', 'milfs', 'sexcam', 'butt plug', 'doggy style', 'intercourse', 'fucks', 'voyeurism', 'dolcett']
 
 
 # KEY = (parameter, images, thumbnail)
 class Mode(Enum):
 	SCRIBBLE = ('scribble', 'assets/imageRemix_modes/scribble.webp', 'assets/imageRemix_modes/thumb_scribble.webp')
 	DEPTH = ('depth', 'assets/imageRemix_modes/depth.webp', 'assets/imageRemix_modes/thumb_depth.webp')
 	SEGMENTATION = ('seg', 'assets/imageRemix_modes/seg.webp', 'assets/imageRemix_modes/thumb_seg.webp')
 	OPEN_POSE = ('openpose', 'assets/imageRemix_modes/openpose.webp', 'assets/imageRemix_modes/thumb_openpose.webp')
+	CANNY = ('canny', 'assets/imageRemix_modes/canny.webp', 'assets/imageRemix_modes/thumb_canny.webp')
 
 
 # KEY = ratio
 class Ratio(Enum):
 	RATIO_1X1 = "1:1"
 	RATIO_4X3 = "4:3"
 	RATIO_3X2 = "3:2"
```

### Comparing `pyimagine-2.7.0/pyimagine/utils.py` & `pyimagine-2.7.1/pyimagine/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,7 +41,13 @@
 
     if vowel:
         chars.insert(2, chars[1])
     else:
         i = random.randint(0, size)
         chars.insert(i + 1, chars[i])
     return "".join(chars)
+
+
+def same_size(src1: bytes, src2: bytes) -> bool:
+    width1, height1 = Image.open(BytesIO(src1)).size
+    width2, height2 = Image.open(BytesIO(src2)).size
+    return width1 == width2 and height1 == height2
```

### Comparing `pyimagine-2.7.0/pyimagine/vyroai.py` & `pyimagine-2.7.1/pyimagine/vyroai.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import requests
 from langdetect import detect
 from requests import Response
 from requests_toolbelt import MultipartEncoder
 
 from pyimagine.constants import Style, Inspiration, Ratio, Mode, BANNED_WORDS
-from pyimagine.exceptions import InvalidWord
-from pyimagine.utils import bytes2png, clear_dict, get_cfg, get_word
+from pyimagine.exceptions import InvalidWord, InvalidSize
+from pyimagine.utils import bytes2png, clear_dict, get_cfg, get_word, same_size
 
 
 class DeviantArt(Enum):
     ID = 23185
     SECRET = "fae0145a0736611056a5196a122c0d36"
 
 
@@ -60,15 +60,15 @@
         r.raise_for_status()
         return r
 
     def thumb(self, item: Union[Style, Inspiration, Mode]) -> bytes:
         href = item.value[2 if isinstance(item, Style) else 1]
         return bytes2png(self._request(method="GET", url=f"{self.cdn}/{href}").content)
 
-    def inspire(self, inspiration: Inspiration = Inspiration.INSPIRATION_01) -> bytes:
+    def sdinsp(self, inspiration: Inspiration = Inspiration.INSPIRATION_01) -> bytes:
         """Inspiration"""
         return self.sdprem(
             prompt=inspiration.value[0],
             style=next((item for item in Style if item.value[0] == inspiration.value[2]), Style.IMAGINE_V3),
             seed=inspiration.value[3])
 
     # @package k7.a;
@@ -153,30 +153,37 @@
                 "image": ("prompt_generator_temp.jpeg", content, "image/jpg")
             }
         ).text
 
     def sdimg(
             self,
             content: bytes,
+            mask: bytes,
             prompt: str,
             negative: str = None,
             seed: int = None,
-            cfg: float = 9.5
+            cfg: float = 9.5,
+            priority: bool = True
     ) -> bytes:
         """Inpainting"""
+        if not same_size(content, mask):
+            raise InvalidSize("Mask size must be same as image size.")
+
         return bytes2png(self._request(
             method="POST",
             url=f"{self.api}/sdimg",
             data={
                 "model_version": self.version,
                 "prompt": prompt,
                 "negative_prompt": negative,
                 "seed": seed,
                 "cfg": get_cfg(cfg),
-                "image": ("bitmap_final_edit.jpg", content, "image/jpg")
+                "image": ("bitmap_final_edit.jpg", content, "image/jpg"),
+                "mask": ("bitmap_final_edit.jpg", mask, "image/jpg"),
+                "priority": int(priority)
             }
         ).content)
 
     def controlnet(
             self,
             content: bytes,
             prompt: str,
```

### Comparing `pyimagine-2.7.0/pyimagine.egg-info/PKG-INFO` & `pyimagine-2.7.1/pyimagine.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimagine
-Version: 2.7.0
+Version: 2.7.1
 Summary: Python library for AI-powered image manipulation.
 Home-page: https://github.com/hyugogirubato/pyimagine
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: art,image,ai,stable-diffusion
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,15 +57,15 @@
 from pyimagine import Imagine
 from pyimagine.constants import Inspiration
 
 # Initialize Imagine
 imagine = Imagine()
 
 # Generate an inspired image
-inspired_image = imagine.inspire(Inspiration.INSPIRATION_01)
+inspired_image = imagine.sdinsp(Inspiration.INSPIRATION_01)
 
 # Variate an image
 original_image = open("image.jpg", "rb").read()
 variated_image = imagine.variate(original_image, prompt="Create something amazing!")
 
 # Upscale an image
 upscaled_image = imagine.upscale(original_image)
@@ -79,11 +79,12 @@
 ### Exceptions
 
 The following exceptions can be raised by PyImagine:
 
 - `InvalidWord`: Raised when a banned word is found in the prompt. By default, if the `restricted` flag is set to `True`
   during initialization, the library will raise an `InvalidWord` exception. You can customize this behavior by setting
   `restricted` to `False` to replace banned words with alternative words instead of raising an exception.
+- `InvalidSize`: Raised when attempting to perform an operation that requires both images to have the same size.
 
 ### License
 
 This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pyimagine/blob/main/LICENSE).
```

### Comparing `pyimagine-2.7.0/setup.py` & `pyimagine-2.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyimagine",
-    version="2.7.0",
+    version="2.7.1",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python library for AI-powered image manipulation.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pyimagine",
     packages=find_packages(),
```

### Comparing `pyimagine-2.7.0/test/test.py` & `pyimagine-2.7.1/test/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,32 +31,33 @@
         path_image = Path(input("Image: "))
         if not path_image.exists() and not path_image.is_file():
             raise Exception(f"Error: File path is invalid, {path_image}")
         usr_prompt = imagine.interrogator(content=open(path_image, mode="rb").read())
 
     usr_negative = input("Negative: ")
 
-    option, index = pick([style.name for style in list(Style)], "Style:")
+    option, _ = pick([style.name for style in list(Style)], "Style:")
     usr_style = Style[option]
 
-    option, index = pick([ratio.name for ratio in list(Ratio)], "Ratio:")
+    option, _ = pick([ratio.name for ratio in list(Ratio)], "Ratio:")
     usr_ratio = Ratio[option]
 
     os.system('cls' if os.name == 'nt' else 'clear')
     print(f"I: PyImagine version {pyimagine.__version__}")
     print(f"I: Prompt: {usr_prompt}")
     print(f"I: Negative: {usr_negative}")
     print(f"I: Style: {usr_style.name}")
     print(f"I: Ratio: {usr_ratio.name}")
 
     img_data = imagine.sdprem(
         prompt=usr_prompt,
         negative=usr_negative,
         style=usr_style,
-        ratio=usr_ratio
+        ratio=usr_ratio,
+        high_result=True
     )
 
     FILE.write_bytes(img_data)
     option, index = pick([upscale.name for upscale in list(Upscale)], "Upscale:")
     usr_upscale = Upscale[option]
 
     print(f"I: Upscale: {usr_upscale.name}")
```

