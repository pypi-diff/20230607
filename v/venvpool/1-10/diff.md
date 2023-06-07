# Comparing `tmp/venvpool-1.tar.gz` & `tmp/venvpool-10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/venvpool-1.tar", last modified: Sun Mar 12 20:06:52 2023, max compression
+gzip compressed data, was "dist/venvpool-10.tar", last modified: Wed Jun  7 21:40:56 2023, max compression
```

## Comparing `venvpool-1.tar` & `venvpool-10.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-03-12 20:06:52.000000 venvpool-1/
--rw-rw-r--   0 arc       (1000) arc       (1000)     5972 2023-03-12 20:06:50.000000 venvpool-1/setup.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       67 2023-03-12 20:06:52.000000 venvpool-1/setup.cfg
--rw-rw-r--   0 arc       (1000) arc       (1000)    35147 2019-11-03 21:14:06.000000 venvpool-1/COPYING
--rwxrwxr-x   0 arc       (1000) arc       (1000)    25534 2023-03-12 19:51:08.000000 venvpool-1/venvpool.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      901 2023-03-12 11:29:52.000000 venvpool-1/README.md
--rw-rw-r--   0 arc       (1000) arc       (1000)     1199 2023-03-12 20:06:52.000000 venvpool-1/PKG-INFO
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-03-12 20:06:52.000000 venvpool-1/venvpool.egg-info/
--rw-rw-r--   0 arc       (1000) arc       (1000)        1 2023-03-12 20:06:52.000000 venvpool-1/venvpool.egg-info/dependency_links.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       20 2023-03-12 20:06:52.000000 venvpool-1/venvpool.egg-info/entry_points.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      211 2023-03-12 20:06:52.000000 venvpool-1/venvpool.egg-info/SOURCES.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)        9 2023-03-12 20:06:52.000000 venvpool-1/venvpool.egg-info/top_level.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)     1199 2023-03-12 20:06:52.000000 venvpool-1/venvpool.egg-info/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-06-07 21:40:56.000000 venvpool-10/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     6010 2023-06-07 21:40:52.000000 venvpool-10/setup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       67 2023-06-07 21:40:56.000000 venvpool-10/setup.cfg
+-rw-rw-r--   0 arc       (1000) arc       (1000)    35147 2019-11-03 21:14:06.000000 venvpool-10/COPYING
+-rwxrwxr-x   0 arc       (1000) arc       (1000)    28996 2023-04-04 21:10:34.000000 venvpool-10/venvpool.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1659 2023-04-05 20:56:33.000000 venvpool-10/README.md
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1995 2023-06-07 21:40:56.000000 venvpool-10/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-06-07 21:40:56.000000 venvpool-10/venvpool.egg-info/
+-rw-rw-r--   0 arc       (1000) arc       (1000)        1 2023-06-07 21:40:54.000000 venvpool-10/venvpool.egg-info/dependency_links.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       20 2023-06-07 21:40:54.000000 venvpool-10/venvpool.egg-info/entry_points.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      211 2023-06-07 21:40:54.000000 venvpool-10/venvpool.egg-info/SOURCES.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)        9 2023-06-07 21:40:54.000000 venvpool-10/venvpool.egg-info/top_level.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1995 2023-06-07 21:40:54.000000 venvpool-10/venvpool.egg-info/PKG-INFO
```

### Comparing `venvpool-1/setup.py` & `venvpool-10/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,16 +132,16 @@
 def ext_modules():
     extensions = [path.make_ext() for path in sourceinfo.extpaths]
     return dict(ext_modules = cythonize(extensions)) if extensions else {}
 
 sourceinfo = SourceInfo('.')
 setuptools.setup(
         name = 'venvpool',
-        version = '1',
-        description = 'Run your scripts using an automated pool of virtual environments',
+        version = '10',
+        description = 'Run your Python scripts using an automated pool of virtual environments to satisfy their requirements',
         long_description = long_description(),
         long_description_content_type = 'text/markdown',
         url = 'https://github.com/combatopera/venvpool',
         author = 'Andrzej Cichocki',
         packages = sourceinfo.packages,
         py_modules = ['venvpool'],
         install_requires = [],
```

### Comparing `venvpool-1/COPYING` & `venvpool-10/COPYING`

 * *Files identical despite different names*

### Comparing `venvpool-1/venvpool.py` & `venvpool-10/venvpool.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,60 +13,115 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with venvpool.  If not, see <http://www.gnu.org/licenses/>.
 
+'eval' 'echo Not a shell script. >&2; return 1'
+__doc__ = None
+import os, sys
+
+if ('__main__' == __name__): # Hide from scriptregex.
+    propersubcommands = []
+    class _shortcut:
+        letter = None
+        def __init__(self):
+            args = sys.argv
+            if 1 < len(args):
+                a = args[1]
+                if 1 < len(a) and '-' == a[0]:
+                    self.letter = a[1]
+        def __call__(self, cls):
+            if self.letter == cls.letter:
+                sys.exit(cls.main())
+            propersubcommands.append(cls)
+            return cls
+    _shortcut = _shortcut()
+else:
+    propersubcommands = None
+    _shortcut = lambda cls: cls
+
+def _decompress(paths):
+    i = iter(paths)
+    prefix = next(i)
+    try:
+        while True:
+            yield prefix + next(i)
+    except StopIteration:
+        pass
+
+@_shortcut
+class Execute:
+
+    help = 'augment interpreter environment and exec module for internal use only'
+    letter = 'X'
+
+    @classmethod
+    def main(cls):
+        import runpy # A few thousandths.
+        assert '-X' == sys.argv.pop(1)
+        sys.path[0] = bindir = os.path.dirname(sys.executable)
+        try:
+            envpath = os.environ['PATH']
+        except KeyError:
+            envpath = bindir
+        else:
+            envpath = bindir + os.pathsep + envpath
+        os.environ['PATH'] = envpath
+        sys.path[slice(*[cls._insertionpoint(sys.path)] * 2)] = _decompress(sys.argv.pop(1).split(os.pathsep))
+        runpy.run_module(sys.argv.pop(1), run_name = '__main__', alter_sys = True)
+
+    @staticmethod
+    def _insertionpoint(v, suffix = os.sep + 'site-packages'):
+        i = n = len(v)
+        while not v[i - 1].endswith(suffix):
+            i -= 1
+            if not i:
+                return n
+        while i and v[i - 1].endswith(suffix):
+            i -= 1
+        return i
+
 from collections import OrderedDict
 from contextlib import contextmanager
 from random import shuffle # XXX: Expensive?
 from stat import S_IXUSR, S_IXGRP, S_IXOTH
-from tempfile import mkdtemp, mkstemp # TODO: Over a hundredth.
-import errno, logging, operator, os, re, shutil, sys # XXX: Still expensive?
+from tempfile import mkdtemp, mkstemp
+import errno, logging, operator, re, shutil # XXX: Still expensive?
 
 class subprocess:
 
     def __getattr__(self, name):
         import subprocess # Up to a hundredth.
         return getattr(subprocess, name)
 
 log = logging.getLogger(__name__)
-cachedir = os.path.join(os.path.expanduser('~'), '.cache', 'pyven') # TODO: Honour XDG_CACHE_HOME.
+chainrelpath = os.path.join('venvpool', 'chain.py')
 dotpy = '.py'
 executablebits = S_IXUSR | S_IXGRP | S_IXOTH
-initbinname = 'initbin.py'
 oserrors = {code: type(name, (OSError,), {}) for code, name in errno.errorcode.items()}
-pooldir = os.path.join(cachedir, 'pool')
+pooldir = os.path.join(os.environ.get('XDG_CACHE_HOME') or os.path.join(os.path.expanduser('~'), '.cache'), 'venvpool')
 scriptregex, = (r"^if\s+(?:__name__\s*==\s*{main}|{main}\s*==\s*__name__)\s*:\s*$".format(**locals()) for main in ['''(?:'__main__'|"__main__")'''])
 try:
     set_inheritable = os.set_inheritable
 except AttributeError:
     from fcntl import fcntl, FD_CLOEXEC, F_GETFD, F_SETFD
     def set_inheritable(h, inherit):
         assert inherit
         fcntl(h, F_SETFD, fcntl(h, F_GETFD) & ~FD_CLOEXEC)
 subprocess = subprocess()
 userbin = os.path.join(os.path.expanduser('~'), '.local', 'bin')
 
-def safe_name(name, unsafeseq = re.compile('[^A-Za-z0-9.]+')):
-    return unsafeseq.sub('-', name)
-
-def to_filename(name):
-    return name.replace('-', '_')
-
 def _osop(f, *args, **kwargs):
     try:
         return f(*args, **kwargs)
     except OSError as e:
         raise oserrors[e.errno](*e.args)
 
-def initlogging():
-    logging.basicConfig(format = "%(asctime)s %(levelname)s %(message)s", level = logging.DEBUG)
-
 @contextmanager
 def TemporaryDirectory():
     tempdir = mkdtemp()
     try:
         yield tempdir
     finally:
         shutil.rmtree(tempdir)
@@ -144,14 +199,30 @@
         for readlock in readlocks:
             try:
                 if _idempotentunlink(readlock):
                     yield readlock
             except oserrors[errno.EACCES]:
                 pass
 
+def _compress(paths, splitchar = os.sep):
+    if not paths:
+        yield '-' # Avoid empty word in command line.
+        return
+    firstdiff = -1
+    for firstdiff, chars in enumerate(zip(*paths)):
+        if 1 != len(set(chars)):
+            break
+    else:
+        firstdiff += 1
+    while firstdiff and paths[0][firstdiff - 1] != splitchar:
+        firstdiff -= 1
+    yield paths[0][:firstdiff]
+    for p in paths:
+        yield p[firstdiff:]
+
 class SharedDir(object):
 
     def __init__(self, dirpath):
         self.readlocks = os.path.join(dirpath, 'readlocks')
 
     def _sweep(self):
         paths = list(_compress(list(_swept(listorempty(self.readlocks)))))
@@ -186,151 +257,104 @@
         try:
             h = _osop(mkstemp, dir = self.readlocks, prefix = 'lock')[0]
             set_inheritable(h, True)
             return ReadLock(h)
         except oserrors[errno.ENOENT]:
             pass
 
-def _safewhich(name):
-    poolprefix = pooldir + os.sep
-    for bindir in os.environ['PATH'].split(os.pathsep):
-        if bindir.startswith(poolprefix) or not os.path.isabs(bindir):
-            log.debug("Ignore bin directory: %s", bindir)
-        else:
-            path = os.path.join(bindir, name)
-            if os.path.exists(path):
-                return path
+def safe_name(name):
+    return re.sub('[^A-Za-z0-9.]+', '-', name)
+
+def to_filename(name):
+    return name.replace('-', '_')
 
 class Venv(SharedDir):
 
+    @staticmethod
+    def _safewhich(name):
+        poolprefix = pooldir + os.sep
+        for bindir in os.environ['PATH'].split(os.pathsep):
+            if bindir.startswith(poolprefix) or not os.path.isabs(bindir): # XXX: Also exclude other venvs?
+                log.debug("Ignore bin directory: %s", bindir)
+            else:
+                path = os.path.join(bindir, name)
+                if os.path.exists(path):
+                    return path
+
     @property
     def site_packages(self):
         libpath = os.path.join(self.venvpath, 'lib')
         pyname, = (n for n in os.listdir(libpath) if n.startswith('python'))
         return os.path.join(libpath, pyname, 'site-packages')
 
     def __init__(self, venvpath):
         super(Venv, self).__init__(venvpath)
         self.venvpath = venvpath
 
     def create(self, pyversion):
         def isolated(*command):
             subprocess.check_call(command, cwd = tempdir, stdout = sys.stderr)
-        executable = _safewhich("python%s" % pyversion)
+        executable = self._safewhich("python%s" % pyversion)
         absvenvpath = os.path.abspath(self.venvpath) # XXX: Safe when venvpath has symlinks?
         with TemporaryDirectory() as tempdir:
             if pyversion < 3:
                 isolated('virtualenv', '-p', executable, absvenvpath)
             else:
                 isolated(executable, '-m', 'venv', absvenvpath)
                 isolated(os.path.join(absvenvpath, 'bin', 'pip'), 'install', '--upgrade', 'pip', 'setuptools', 'wheel')
+        chainpath = os.path.join(self.site_packages, chainrelpath)
+        os.mkdir(os.path.dirname(chainpath))
+        with open(chainpath, 'w') as f:
+            f.write('''import os, sys
+v = [os.path.join(os.path.dirname(sys.executable), sys.argv[1])] + sys.argv[2:]
+os.execv(v[0], v)
+''')
 
     def delete(self, label = 'transient'):
         log.debug("Delete %s venv: %s", label, self.venvpath)
         shutil.rmtree(self.venvpath)
 
     def programpath(self, name):
         return os.path.join(self.venvpath, 'bin', name)
 
-    def install(self, args, pip = None):
+    def install(self, args):
         log.debug("Install: %s", ' '.join(args))
         if args:
-            if pip is None:
-                Pip(self.programpath('pip')).pipinstall(args)
-            else:
-                Pip(pip).pipinstall(args + ['--prefix', self.venvpath])
+            Pip(self.programpath('pip')).pipinstall(args)
 
     def compatible(self, installdeps):
-        for i in installdeps.volatileprojects:
-            if not self._hasvolatileproject(i):
-                return
         for r in installdeps.pypireqs:
             version = self._reqversionornone(r.namepart)
-            if version is None or version not in r.parsed:
+            if version is None or not r.acceptversion(version):
                 return
         log.debug("Found compatible venv: %s", self.venvpath)
         return True
 
-    def _hasvolatileproject(self, info):
-        return os.path.exists(os.path.join(self.site_packages, "%s-%s.dist-info" % (to_filename(safe_name(info.config.name)), info.devversion())))
-
     def _reqversionornone(self, name):
         patterns = [re.compile(format % nameregex) for nameregex in [re.escape(to_filename(safe_name(name)).lower())] for format in [
             "^%s-(.+)[.]dist-info$",
             "^%s-([^-]+).*[.]egg-info$"]]
         for lowername in (n.lower() for n in os.listdir(self.site_packages)):
             for p in patterns:
                 m = p.search(lowername)
                 if m is not None:
                     return m.group(1)
 
     def run(self, mode, localreqs, module, scriptargs, **kwargs):
-        argv = [os.path.join(self.venvpath, 'bin', 'python'), __file__, '-x', os.pathsep.join(_compress(localreqs)), module] + scriptargs
+        argv = [os.path.join(self.venvpath, 'bin', 'python'), __file__, '-X', os.pathsep.join(_compress(localreqs)), module] + scriptargs
         if 'call' == mode:
             return subprocess.call(argv, **kwargs)
         if 'check_call' == mode:
             return subprocess.check_call(argv, **kwargs)
+        if 'check_output' == mode:
+            return subprocess.check_output(argv, **kwargs)
         if 'exec' == mode:
             os.execv(argv[0], argv, **kwargs)
         raise ValueError(mode)
 
-def _compress(paths, splitchar = os.sep):
-    if not paths:
-        yield '-' # Avoid empty word in command line.
-        return
-    firstdiff = -1
-    for firstdiff, chars in enumerate(zip(*paths)):
-        if 1 != len(set(chars)):
-            break
-    else:
-        firstdiff += 1
-    while firstdiff and paths[0][firstdiff - 1] != splitchar:
-        firstdiff -= 1
-    yield paths[0][:firstdiff]
-    for p in paths:
-        yield p[firstdiff:]
-
-def _decompress(paths):
-    i = iter(paths)
-    prefix = next(i)
-    try:
-        while True:
-            yield prefix + next(i)
-    except StopIteration:
-        pass
-
-class Execute:
-
-    letter = 'x'
-
-    @staticmethod
-    def main():
-        import runpy # A few thousandths.
-        assert '-x' == sys.argv.pop(1)
-        sys.path[0] = bindir = os.path.dirname(sys.executable)
-        try:
-            envpath = os.environ['PATH']
-        except KeyError:
-            envpath = bindir
-        else:
-            envpath = bindir + os.pathsep + envpath
-        os.environ['PATH'] = envpath
-        sys.path[slice(*[_insertionpoint(sys.path)] * 2)] = _decompress(sys.argv.pop(1).split(os.pathsep))
-        runpy.run_module(sys.argv.pop(1), run_name = '__main__', alter_sys = True)
-
-def _insertionpoint(v, suffix = os.sep + 'site-packages'):
-    i = n = len(v)
-    while not v[i - 1].endswith(suffix):
-        i -= 1
-        if not i:
-            return n
-    while i and v[i - 1].endswith(suffix):
-        i -= 1
-    return i
-
 class Pool:
 
     @property
     def versiondir(self):
         return os.path.join(pooldir, str(self.pyversion))
 
     def __init__(self, pyversion):
@@ -341,14 +365,15 @@
         self.readonlyorreadwrite = {
             False: self.readonly,
             True: self.readwrite,
         }
         self.pyversion = pyversion
 
     def _newvenv(self, installdeps):
+        log.info('Create new venv.')
         try:
             _osop(os.makedirs, self.versiondir)
         except oserrors[errno.EEXIST]:
             pass
         venv = Venv(mkdtemp(dir = self.versiondir, prefix = 'venv'))
         with _onerror(venv.delete):
             venv.create(self.pyversion)
@@ -417,32 +442,14 @@
                             os.remove(p) # Cross-platform.
                             os.rename(q, p)
         try:
             yield venv
         finally:
             venv.writeunlock()
 
-class BaseReq:
-
-    @classmethod
-    def parselines(cls, lines):
-        from pkg_resources import parse_requirements # Expensive module!
-        return [cls(parsed) for parsed in parse_requirements(lines)]
-
-    @property
-    def namepart(self):
-        return self.parsed.name
-
-    @property
-    def reqstr(self):
-        return str(self.parsed)
-
-    def __init__(self, parsed):
-        self.parsed = parsed
-
 class FastReq:
 
     class Version:
 
         def __init__(self, operator, splitversion):
             self.operator = operator
             self.splitversion = splitversion
@@ -450,175 +457,194 @@
         def accept(self, splitversion):
             def pad(v):
                 return v + [0] * (n - len(v))
             versions = [splitversion, self.splitversion]
             n = max(map(len, versions))
             return self.operator(*map(pad, versions))
 
-    @staticmethod
-    def _splitversion(versionstr):
-        return [int(k) for k in versionstr.split('.')]
+    class DevSegment:
+
+        def __init__(self, n):
+            self.n = n
+
+    @classmethod
+    def _splitversion(cls, versionstr, devprefix = 'dev'):
+        return [cls.DevSegment(int(k[len(devprefix):])) if k.startswith(devprefix) else int(k) for k in versionstr.split('.')]
 
     s = r'\s*'
-    name = '([A-Za-z0-9._-]+)' # Slightly more lenient than PEP 508.
-    version = "(<|<=|!=|==|>=|>){s}([0-9.]+)".format(**locals()) # Subset of features.
-    versionmatch = re.compile("^{s}{version}{s}$".format(**locals())).search
-    getmatch = re.compile("^{s}{name}{s}({version}{s}(?:,{s}{version}{s})*)?$".format(**locals())).search
-    skipmatch = re.compile("^{s}(?:#|$)".format(**locals())).search
-    del s, name, version
+    nameregex = '[A-Za-z0-9._-]+' # Slightly more lenient than PEP 508.
+    extras = r"\[{s}(?:{nameregex}{s}(?:,{s}{nameregex}{s})*)?]".format(**locals())
+    version = "(<|<=|!=|==|>=|>){s}([0-9.]+(?:[.]dev[0-9]+)?)".format(**locals()) # Subset of features.
+    versionregex = "^{s}{version}{s}$".format(**locals())
+    getregex = "^{s}({nameregex}){s}({extras}{s})?({version}{s}(?:,{s}{version}{s})*)?$".format(**locals())
+    skipregex = "^{s}(?:#|$)".format(**locals())
+    del s, extras, version
     operators = {
         '<': operator.lt,
         '<=': operator.le,
         '!=': operator.ne,
         '==': operator.eq,
         '>=': operator.ge,
         '>': operator.gt,
     }
 
     @classmethod
     def parselines(cls, lines):
         def g():
             for line in lines:
-                if cls.skipmatch(line) is not None:
+                if re.search(cls.skipregex, line) is not None:
                     continue
-                namepart, versionspec = cls.getmatch(line).groups()[:2]
+                namepart, extras, versionspec = re.search(cls.getregex, line).groups()[:3]
+                extras = () if extras is None else tuple(sorted(set(re.findall(cls.nameregex, extras)))) # TODO LATER: Normalisation.
                 versions = []
                 reqstrversions = []
                 if versionspec is not None:
                     for onestr in versionspec.split(','):
-                        operatorstr, versionstr = cls.versionmatch(onestr).groups()
+                        operatorstr, versionstr = re.search(cls.versionregex, onestr).groups()
                         versions.append(cls.Version(cls.operators[operatorstr], cls._splitversion(versionstr)))
                         reqstrversions.append(operatorstr + versionstr)
-                yield cls(namepart, versions, namepart + ','.join(sorted(reqstrversions)))
+                yield cls(namepart, extras, versions, namepart + ("[%s]" % ','.join(extras) if extras else '') + ','.join(sorted(reqstrversions)))
         return list(g())
 
-    @property
-    def parsed(self):
-        return self
-
-    def __init__(self, namepart, versions, reqstr):
+    def __init__(self, namepart, extras, versions, reqstr):
         self.namepart = namepart
+        self.extras = extras
         self.versions = versions
         self.reqstr = reqstr
 
-    def __contains__(self, versionstr):
+    def acceptversion(self, versionstr):
         splitversion = self._splitversion(versionstr)
         return all(v.accept(splitversion) for v in self.versions)
 
-class SimpleInstallDeps:
+class ParsedRequires:
 
-    volatileprojects = ()
+    parselines = staticmethod(FastReq.parselines)
 
-    def __init__(self, requires, pip = None, reqcls = BaseReq):
-        self.pypireqs = reqcls.parselines(requires)
-        self.pip = pip
-        self.reqcls = reqcls
+    def __init__(self, requires):
+        self.pypireqs = self.parselines(requires)
 
     def invoke(self, venv):
-        venv.install([r.reqstr for r in self.pypireqs], self.pip)
+        venv.install([r.reqstr for r in self.pypireqs])
 
-    def poplocalreqs(self, workspace, makerequirementslines):
+    def poplocalreqs(self, workspace):
         local = OrderedDict()
         reqs = list(self.pypireqs)
         del self.pypireqs[:]
         while reqs:
             nextreqs = []
             for req in reqs:
                 projectdir = os.path.join(workspace, req.namepart)
-                if projectdir in local:
-                    continue
-                if os.path.exists(projectdir):
-                    local[projectdir] = None
-                    nextreqs.extend(self.reqcls.parselines(makerequirementslines(projectdir))) # FIXME: Can pass None into parselines.
-                else:
-                    self.pypireqs.append(req)
+                if projectdir not in local:
+                    if os.path.exists(projectdir):
+                        requirementslines = _getrequirementslinesornone(projectdir, req.extras)
+                        if requirementslines is None:
+                            raise NoRequirementsFoundException("%s[%s]" % (projectdir, ','.join(req.extras)))
+                        nextreqs.extend(self.parselines(requirementslines))
+                        local[projectdir] = None
+                    else:
+                        self.pypireqs.append(req)
             reqs = nextreqs
         return list(local)
 
-def _getrequirementslinesornone(projectdir):
+def _getrequirementslinesornone(projectdir, extras):
     def linesornone(acceptnull, *names):
         path = os.path.join(projectdir, *names)
         if os.path.exists(path):
             log.debug("Found requirements: %s", path)
             with open(path) as f:
                 return f.read().splitlines()
         if acceptnull:
             log.debug("Null requirements: %s", path)
             return []
+    if extras:
+        log.warning("Ignore extras %s in: %s", ','.join(extras), projectdir) # TODO: Find extra requirements as well.
     v = linesornone(False, 'requirements.txt')
     if v is not None:
         return v
     names = [name for name in os.listdir(projectdir) if name.endswith('.egg-info')]
     if names:
         name, = names # XXX: Could there legitimately be multiple?
         return linesornone(True, name, 'requires.txt')
 
-class Command:
+def initlogging():
+    logging.basicConfig(format = "%(asctime)s %(levelname)s %(message)s", level = logging.DEBUG)
+
+class ParserCommand:
 
     @classmethod
     def main(cls):
         from argparse import ArgumentParser # Two or three hundredths.
         initlogging()
-        parser = cls.createparser(ArgumentParser)
+        parser = ArgumentParser(description = cls.help)
         if cls.letter is not None:
-            parser.add_argument('-' + cls.letter, action = 'store_true')
-        parser.add_argument('-v', action = 'store_true')
+            parser.add_argument('-' + cls.letter, action = 'store_true', help = 'select this subcommand')
+        cls.initparser(parser)
+        parser.add_argument('-v', action = 'store_true', help = 'show debug logging')
         args = parser.parse_args()
         if cls.letter is not None:
             assert getattr(args, cls.letter)
         if not args.v:
             logging.getLogger().setLevel(logging.INFO)
         cls.mainimpl(args)
 
-class Launch(Command):
-
-    letter = 'l'
-
-    @staticmethod
-    def createparser(parsercls):
-        parser = parsercls(add_help = False)
-        parser.add_argument('--pip')
-        parser.add_argument('scriptpath', type = os.path.abspath) # XXX: Safe when scriptpath has symlinks?
-        parser.add_argument('scriptargs', nargs = '*')
-        return parser
-
-    @classmethod
-    def mainimpl(cls, args):
-        scriptpath = args.scriptpath
-        assert scriptpath.endswith(dotpy)
-        projectdir, requirementslines = _findrequirements(os.path.dirname(scriptpath))
-        installdeps = SimpleInstallDeps(requirementslines, args.pip, FastReq)
-        localreqs = installdeps.poplocalreqs(os.path.normpath(os.path.join(projectdir, '..')), _getrequirementslinesornone)
-        localreqs.insert(0, projectdir)
-        module = os.path.relpath(scriptpath[:-len(dotpy)], projectdir).replace(os.sep, '.')
-        with Pool(sys.version_info.major).readonly(installdeps) as venv: # TODO: Likely to be major 2 when launching manually.
-            venv.run('exec', localreqs, module, args.scriptargs)
-
 class NoRequirementsFoundException(Exception): pass
 
 def _findrequirements(projectdir):
     while True:
-        requirementslines = _getrequirementslinesornone(projectdir)
+        requirementslines = _getrequirementslinesornone(projectdir, ())
         if requirementslines is not None:
             return projectdir, requirementslines
         parent = os.path.dirname(projectdir)
         if parent == projectdir:
             raise NoRequirementsFoundException
         projectdir = parent
 
-class Activate(Command):
+@_shortcut
+class Launch(ParserCommand):
 
+    help = 'launch a script with the interpreter and requirements it needs'
+    letter = 'L'
+
+    @staticmethod
+    def initparser(parser):
+        parser.add_argument('--req', help = 'use the given requirement specifier only')
+        parser.add_argument('scriptpath', help = 'should be preceded by a -- arg')
+        parser.add_argument('scriptarg', nargs = '*', help = 'arguments for scriptpath')
+
+    @classmethod
+    def mainimpl(cls, args):
+        scriptpath = args.scriptpath
+        assert scriptpath.endswith(dotpy)
+        reqstr = args.req
+        if reqstr is None:
+            scriptpath = os.path.abspath(scriptpath) # XXX: Is abspath safe when scriptpath has symlinks?
+            projectdir, requirementslines = _findrequirements(os.path.dirname(scriptpath))
+            installdeps = ParsedRequires(requirementslines)
+            localreqs = installdeps.poplocalreqs(os.path.normpath(os.path.join(projectdir, '..')))
+            localreqs.insert(0, projectdir)
+            module = os.path.relpath(scriptpath[:-len(dotpy)], projectdir).replace(os.sep, '.')
+        else:
+            installdeps = ParsedRequires([reqstr])
+            localreqs = []
+            module = scriptpath[:-len(dotpy)].replace(os.sep, '.')
+        with Pool(sys.version_info.major).readonly(installdeps) as venv: # TODO: Likely to be major 2 when launching manually.
+            venv.run('exec', localreqs, module, args.scriptarg)
+
+class Activate(ParserCommand):
+
+    help = 'create and maintain wrapper scripts'
     letter = None
 
     @staticmethod
-    def createparser(parsercls):
-        parser = parsercls()
-        parser.add_argument('-f', action = 'store_true')
-        parser.add_argument('projectdir', nargs = '*', default = ['.'])
-        return parser
+    def initparser(parser):
+        group = parser.add_mutually_exclusive_group()
+        for cls in propersubcommands:
+            group.add_argument('-' + cls.letter, action = 'store_true', help = 'subcommand to ' + cls.help)
+        parser.add_argument('-f', action = 'store_true', help = 'overwrite existing scripts')
+        parser.add_argument('projectdir', nargs = '*', default = ['.'], help = 'projects to search for runnable modules')
 
     @classmethod
     def mainimpl(cls, args):
         for projectdir in args.projectdir:
             try:
                 cls._scan(_findrequirements(os.path.realpath(projectdir))[0], 3, args.f) # XXX: Always 3?
             except NoRequirementsFoundException:
@@ -632,48 +658,62 @@
                     path = os.path.join(dirpath, name)
                     with open(path) as f:
                         if re.search(scriptregex, f.read(), re.MULTILINE) is not None:
                             yield path
 
     @classmethod
     def _scan(cls, projectdir, pyversion, force):
-        venvpoolpath = os.path.realpath(__file__)
         for srcpath in cls._srcpaths(projectdir):
             if not checkpath(projectdir, srcpath):
                 log.debug("Not a project source file: %s", srcpath)
                 continue
             command = commandornone(srcpath)
             if command is None:
                 log.debug("Bad source name: %s", srcpath)
                 continue
-            text = """#!/usr/bin/env python{pyversion}
+            cls.install(force, command, pyversion, None, srcpath)
+
+    @staticmethod
+    def install(force, command, pyversion, reqstrornone, *words):
+        def allwords():
+            if reqstrornone is not None:
+                yield '--req'
+                yield reqstrornone
+            yield '--'
+            for w in words:
+                yield w
+        def identical():
+            mode = os.stat(scriptpath).st_mode
+            if mode | executablebits == mode:
+                with open(scriptpath) as f:
+                    return f.read() == text
+        wordsrepr = ', '.join(map(repr, allwords()))
+        venvpoolpath = os.path.realpath(__file__)
+        text = """#!/usr/bin/env python{pyversion}
 import sys
-sys.argv[1:1] = '-l', '--', {srcpath!r}
+sys.argv[1:1] = '-L', {wordsrepr}
 __file__ = {venvpoolpath!r}
 with open(__file__) as f: venvpoolsrc = f.read()
 del sys, f
 exec(venvpoolsrc)
 """.format(**locals())
-            scriptpath = os.path.join(userbin, command) # TODO: Warn if shadowed.
-            if os.path.exists(scriptpath):
-                mode = os.stat(scriptpath).st_mode
-                if mode | executablebits == mode:
-                    with open(scriptpath) as f:
-                        if f.read() == text:
-                            log.debug("Identical: %s", scriptpath)
-                            continue
-                if not force:
-                    log.info("Exists: %s", scriptpath)
-                    continue
-                log.info("Overwrite: %s", scriptpath)
-            else:
-                log.info("Create: %s", scriptpath)
-            with open(scriptpath, 'w') as f:
-                f.write(text)
-            os.chmod(scriptpath, os.stat(scriptpath).st_mode | executablebits)
+        scriptpath = os.path.join(userbin, command) # TODO: Warn if shadowed.
+        if os.path.exists(scriptpath):
+            if identical():
+                log.debug("Identical: %s", scriptpath)
+                return
+            if not force:
+                log.info("Exists: %s", scriptpath)
+                return
+            log.info("Overwrite: %s", scriptpath)
+        else:
+            log.info("Create: %s", scriptpath)
+        with open(scriptpath, 'w') as f:
+            f.write(text)
+        os.chmod(scriptpath, os.stat(scriptpath).st_mode | executablebits)
 
 def checkpath(projectdir, path):
     while True:
         path = os.path.dirname(path)
         if path == projectdir:
             return True
         if not os.path.exists(os.path.join(path, '__init__.py')): # XXX: What about namespace packages?
@@ -681,33 +721,35 @@
 
 def commandornone(srcpath):
     name = os.path.basename(srcpath)
     name = os.path.basename(os.path.dirname(srcpath)) if '__init__.py' == name else name[:-len(dotpy)]
     if '-' not in name:
         return name.replace('_', '-')
 
-class Compact(Command):
+@_shortcut
+class Compact(ParserCommand):
 
-    letter = 'c'
+    help = 'compact the pool of venvs'
+    letter = 'C'
 
     @staticmethod
-    def createparser(parsercls):
-        return parsercls()
+    def initparser(parser):
+        pass
 
     @classmethod
     def mainimpl(cls, args): # XXX: Combine venvs with orthogonal dependencies?
         venvtofreeze = {}
         try:
             for versiondir in listorempty(pooldir):
                 for venv in listorempty(versiondir, Venv):
                     if venv.trywritelock():
                         venvtofreeze[venv] = set(subprocess.check_output([venv.programpath('pip'), 'freeze'], universal_newlines = True).splitlines())
                     else:
                         log.debug("Busy: %s", venv.venvpath)
-            log.info('Find redundant venvs.')
+            log.debug('Find redundant venvs.')
             while True:
                 venv = cls._redundantvenv(venvtofreeze)
                 if venv is None:
                     break
                 venv.delete('redundant')
                 venvtofreeze.pop(venv)
             cls._compactvenvs([l.venvpath for l in venvtofreeze])
@@ -725,22 +767,44 @@
     @staticmethod
     def _compactvenvs(venvpaths):
         log.info("Compact %s venvs.", len(venvpaths))
         if venvpaths:
             subprocess.check_call(['jdupes', '-Lrq'] + venvpaths)
         log.info('Compaction complete.')
 
-def main():
-    try:
-        firstarg = sys.argv[1]
-    except IndexError:
-        pass
-    else:
-        if firstarg.startswith('-'):
-            letter = firstarg[1]
-            for cls in Execute, Launch, Compact:
-                if letter == cls.letter:
-                    return cls.main()
-    Activate.main()
+@_shortcut
+class ConsoleScripts(ParserCommand):
 
-if ('__main__' == __name__): # Hide from scriptregex.
-    main()
+    help = 'activate all console scripts of the given requirement specifier'
+    letter = 'S'
+
+    @staticmethod
+    def initparser(parser):
+        parser.add_argument('-f', action = 'store_true', help = 'overwrite existing scripts')
+        parser.add_argument('spec', help = 'a requirement specifier')
+
+    @classmethod
+    def mainimpl(cls, args):
+        from inspect import getsource # About two hundredths.
+        spec, = FastReq.parselines([args.spec])
+        pyversion = 3
+        with TemporaryDirectory() as tempdir:
+            with open(os.path.join(tempdir, 'list.py'), 'w') as f:
+                f.write("class C:\n%sC.%s(%r)\n" % (getsource(cls._commands), cls._commands.__name__, spec.namepart))
+            with Pool(pyversion).readonly(ParsedRequires(['importlib-metadata', spec.reqstr])) as venv:
+                names = set(venv.run('check_output', [tempdir], 'list', [], universal_newlines = True).splitlines())
+        for name in names:
+            Activate.install(args.f, name, pyversion, spec.reqstr, chainrelpath, name)
+
+    @staticmethod
+    def _commands(distname):
+        from importlib_metadata import distribution, files
+        for ep in distribution(distname).entry_points:
+            if 'console_scripts' == ep.group:
+                print(ep.name)
+        for p in files(distname):
+            t = p.parts
+            if 5 == len(t) and ('..', '..', '..', 'bin') == t[:4]:
+                print(t[4])
+
+if propersubcommands is not None:
+    Activate.main()
```

### Comparing `venvpool-1/PKG-INFO` & `venvpool-10/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,78 @@
 Metadata-Version: 2.1
 Name: venvpool
-Version: 1
-Summary: Run your scripts using an automated pool of virtual environments
+Version: 10
+Summary: Run your Python scripts using an automated pool of virtual environments to satisfy their requirements
 Home-page: https://github.com/combatopera/venvpool
 Author: Andrzej Cichocki
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # venvpool
-Run your scripts using an automated pool of virtual environments
+Run your Python scripts using an automated pool of virtual environments to satisfy their requirements
 
 ## Install
+<!--
 These are generic installation instructions.
+-->
+The activate script is a single file with no requirements of its own other than Python 2 or 3.
 
+<!--
 ### To use, permanently
 The quickest way to get started is to install the current release from PyPI:
 ```
 pip3 install --user venvpool
 ```
 
 ### To use, temporarily
 If you prefer to keep .local clean, install to a virtualenv:
 ```
 python3 -m venv venvname
 venvname/bin/pip install venvpool
 . venvname/bin/activate
 ```
+-->
+### To use
+Download the latest activate script into your personal scripts directory:
+```
+cd ~/.local/bin
+wget https://raw.githubusercontent.com/combatopera/venvpool/trunk/activate
+chmod +x activate
+```
 
 ### To develop
 First clone the repo using HTTP or SSH:
 ```
 git clone https://github.com/combatopera/venvpool.git
 git clone git@github.com:combatopera/venvpool.git
 ```
+<!--
 Now use pyven's pipify to create a setup.py, which pip can then use to install the project editably:
 ```
 python3 -m venv pyvenvenv
 pyvenvenv/bin/pip install pyven
 pyvenvenv/bin/pipify venvpool
 
 python3 -m venv venvname
 venvname/bin/pip install -e venvpool
 . venvname/bin/activate
 ```
+-->
+Now symlink the activate script:
+```
+ln -s "$PWD/venvpool/activate" ~/.local/bin/
+```
+
+## Commands
+
+### activate
+Create and maintain wrapper scripts in ~/.local/bin for all runnable modules in the given projects, or the current project if none given.
+
+### activate -S
+Create/maintain wrappers for all console_scripts of the given requirement specifier.
+
+### activate -C
+Compact the pool of venvs.
```

### Comparing `venvpool-1/venvpool.egg-info/PKG-INFO` & `venvpool-10/venvpool.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,78 @@
 Metadata-Version: 2.1
 Name: venvpool
-Version: 1
-Summary: Run your scripts using an automated pool of virtual environments
+Version: 10
+Summary: Run your Python scripts using an automated pool of virtual environments to satisfy their requirements
 Home-page: https://github.com/combatopera/venvpool
 Author: Andrzej Cichocki
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # venvpool
-Run your scripts using an automated pool of virtual environments
+Run your Python scripts using an automated pool of virtual environments to satisfy their requirements
 
 ## Install
+<!--
 These are generic installation instructions.
+-->
+The activate script is a single file with no requirements of its own other than Python 2 or 3.
 
+<!--
 ### To use, permanently
 The quickest way to get started is to install the current release from PyPI:
 ```
 pip3 install --user venvpool
 ```
 
 ### To use, temporarily
 If you prefer to keep .local clean, install to a virtualenv:
 ```
 python3 -m venv venvname
 venvname/bin/pip install venvpool
 . venvname/bin/activate
 ```
+-->
+### To use
+Download the latest activate script into your personal scripts directory:
+```
+cd ~/.local/bin
+wget https://raw.githubusercontent.com/combatopera/venvpool/trunk/activate
+chmod +x activate
+```
 
 ### To develop
 First clone the repo using HTTP or SSH:
 ```
 git clone https://github.com/combatopera/venvpool.git
 git clone git@github.com:combatopera/venvpool.git
 ```
+<!--
 Now use pyven's pipify to create a setup.py, which pip can then use to install the project editably:
 ```
 python3 -m venv pyvenvenv
 pyvenvenv/bin/pip install pyven
 pyvenvenv/bin/pipify venvpool
 
 python3 -m venv venvname
 venvname/bin/pip install -e venvpool
 . venvname/bin/activate
 ```
+-->
+Now symlink the activate script:
+```
+ln -s "$PWD/venvpool/activate" ~/.local/bin/
+```
+
+## Commands
+
+### activate
+Create and maintain wrapper scripts in ~/.local/bin for all runnable modules in the given projects, or the current project if none given.
+
+### activate -S
+Create/maintain wrappers for all console_scripts of the given requirement specifier.
+
+### activate -C
+Compact the pool of venvs.
```

