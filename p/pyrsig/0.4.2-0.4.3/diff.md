# Comparing `tmp/pyrsig-0.4.2.tar.gz` & `tmp/pyrsig-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrsig-0.4.2.tar", last modified: Fri Jun  2 19:11:47 2023, max compression
+gzip compressed data, was "dist/pyrsig-0.4.3.tar", last modified: Wed Jun  7 12:44:27 2023, max compression
```

## Comparing `pyrsig-0.4.2.tar` & `pyrsig-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 19:11:47.000000 pyrsig-0.4.2/
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.2/setup.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-02 19:11:47.000000 pyrsig-0.4.2/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.2/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/requires.txt
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.2/pyrsig/tests/test_api.py
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.2/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2450 2023-06-02 19:05:44.000000 pyrsig-0.4.2/pyrsig/tests/test_ioapi.py
--rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.2/pyrsig/tests/test_misc.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.4.2/pyrsig/tests/test_dataframes.py
--rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.2/pyrsig/tests/test_coards.py
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.2/pyrsig/tests/test_gui.py
--rw-r--r--   0 bhenders (83225) romo       (131)    47853 2023-06-02 19:11:29.000000 pyrsig-0.4.2/pyrsig/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-06-02 19:11:47.000000 pyrsig-0.4.2/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.2/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-07 12:44:27.000000 pyrsig-0.4.3/
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.3/setup.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-07 12:44:27.000000 pyrsig-0.4.3/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.3/LICENSE
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/requires.txt
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig/
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.3/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.3/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3182 2023-06-07 12:10:43.000000 pyrsig-0.4.3/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.3/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2774 2023-06-07 12:09:56.000000 pyrsig-0.4.3/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.3/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.3/pyrsig/tests/test_gui.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    48873 2023-06-07 12:29:16.000000 pyrsig-0.4.3/pyrsig/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-06-07 12:44:27.000000 pyrsig-0.4.3/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.3/README.md
```

### Comparing `pyrsig-0.4.2/setup.py` & `pyrsig-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.2/PKG-INFO` & `pyrsig-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.2/LICENSE` & `pyrsig-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.2/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.4.3/pyrsig.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.2/pyrsig/tests/test_api.py` & `pyrsig-0.4.3/pyrsig/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.2/pyrsig/tests/test_ioapi.py` & `pyrsig-0.4.3/pyrsig/tests/test_ioapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,29 @@
         )
         ds = rsigapi.to_ioapi(
             'tropomi.offl.no2.nitrogendioxide_tropospheric_column'
         )
         print(ds.dims)
 
 
+def test_tropomi_merc():
+    from .. import RsigApi
+    import tempfile
+
+    with tempfile.TemporaryDirectory() as td:
+        rsigapi = RsigApi(
+            bdate='2022-03-01', workdir=td,
+            bbox=(-97, 20, -65, 50), grid_kw='NORTHSOUTHAM'
+        )
+        ds = rsigapi.to_ioapi(
+            'tropomi.offl.no2.nitrogendioxide_tropospheric_column'
+        )
+        print(ds.dims)
+
+
 def test_tropomi_cache():
     from .. import RsigApi
     import tempfile
 
     with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
             bdate='2022-03-01', workdir=td,
@@ -81,7 +96,22 @@
             bbox=(-97, 20, -65, 50), encoding={'zlib': True, 'complevel': 1}
         )
         ds = rsigapi.to_ioapi(
             'tropomi.offl.no2.nitrogendioxide_tropospheric_column',
             withmeta=True, removegz=True
         )
         print(ds.dims, len(ds.attrs['metadata']))
+
+
+def test_equates():
+    from .. import RsigApi
+    import tempfile
+
+    with tempfile.TemporaryDirectory() as td:
+        rsigapi = RsigApi(
+            bdate='2016-03-01', workdir=td,
+            bbox=(-97, 20, -65, 50)
+        )
+        ds = rsigapi.to_ioapi(
+            'cmaq.equates.conus.aconc.O3'
+        )
+        print(ds.dims)
```

### Comparing `pyrsig-0.4.2/pyrsig/tests/test_dataframes.py` & `pyrsig-0.4.3/pyrsig/tests/test_dataframes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 def test_viirsnoaa():
-    """currently not operational. I don't yet know why"""
     from .. import RsigApi
     import tempfile
 
     with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
             bdate='2022-03-01', bbox=(-85, 30, -70, 45), workdir=td
         )
@@ -80,7 +79,20 @@
         )
         print(df.shape)
         rsigapi = RsigApi(workdir=td, overwrite=True)
         df = rsigapi.to_dataframe(
             'aqs.no2', bdate='2022-03-01T00', edate='2022-03-01T01'
         )
         print(df.shape)
+
+
+def test_cmaqequates():
+    """currently not operational. I don't yet know why"""
+    from .. import RsigApi
+    import tempfile
+
+    with tempfile.TemporaryDirectory() as td:
+        rsigapi = RsigApi(
+            bdate='2016-03-01', bbox=(-85, 30, -70, 45), workdir=td
+        )
+        ds = rsigapi.to_dataframe('cmaq.equates.conus.aconc.O3')
+        print(ds.shape)
```

### Comparing `pyrsig-0.4.2/pyrsig/tests/test_coards.py` & `pyrsig-0.4.3/pyrsig/tests/test_coards.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.2/pyrsig/tests/test_gui.py` & `pyrsig-0.4.3/pyrsig/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.2/pyrsig/__init__.py` & `pyrsig-0.4.3/pyrsig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = ['RsigApi', 'RsigGui', 'open_ioapi']
-__version__ = '0.4.2'
+__version__ = '0.4.3'
 
 import pandas as pd
 
 
 _def_grid_kw = {
     '12US1': dict(
         GDNAM='12US1', GDTYP=2, NCOLS=459, NROWS=299,
@@ -46,14 +46,19 @@
         P_ALP=1., P_BET=45., P_GAM=-98., XCENT=-98., YCENT=90.
     ),
     '36NHEMI2': dict(
         GDNAM='36NHEMI2', GDTYP=6, NCOLS=187 * 3, NROWS=187 * 3,
         XORIG=-10098000.0, YORIG=-10098000.0, XCELL=36000., YCELL=36000.,
         P_ALP=1., P_BET=45., P_GAM=-98., XCENT=-98., YCENT=90.
     ),
+    'NORTHSOUTHAM': dict(
+        GDNAM='NORTHSOUTHAM', GDTYP=7, NCOLS=179, NROWS=154,
+        XORIG=251759.25, YORIG=-1578187., XCELL=27000., YCELL=27000.,
+        P_ALP=0., P_BET=0., P_GAM=-98., XCENT=-98., YCENT=0.
+    ),
 }
 
 _shared_grid_kw = dict(
     VGTYP=7, VGTOP=5000., NLAYS=35, earth_radius=6370000., g=9.81, R=287.04,
     A=50., T0=290, P0=1000e2, REGRID_AGGREGATE='None'
 )
 
@@ -109,15 +114,17 @@
     'tropomi.offl.hcho.formaldehyde_tropospheric_vertical_column',
     'tropomi.offl.co.carbonmonoxide_total_column',
     'tropomi.offl.ch4.methane_mixing_ratio',
     'tropomi.offl.ch4.methane_mixing_ratio_bias_corrected',
     'viirsnoaa.jrraod.AOD550', 'viirsnoaa.vaooo.AerosolOpticalDepth_at_550nm',
 )
 
-_point_prefixes = ('airnow', 'aqs', 'purpleair', 'pandora')
+_nocorner_prefixes = ('airnow', 'aqs', 'purpleair', 'pandora', 'cmaq')
+_nolonlats_prefixes = ('cmaq',)
+_noregrid_prefixes = ('cmaq',)
 
 
 def _actionf(msg, action, ErrorTyp=None):
     """
     Convenience function for warning or raising an error.
 
     Arguments
@@ -344,15 +351,15 @@
         projstr = (
             '+proj=stere +lat_0={lat_0} +lat_ts={P_BET} +lon_0={XCENT}'
             + ' +x_0={x_0} +y_0={y_0} +R={earth_radius} +to_meter={XCELL}'
             + ' +no_defs'
         ).format(lat_0=props['P_ALP'] * 90, **props)
     elif props['GDTYP'] == 7:
         projstr = (
-            '+proj=merc +R={earth_radius} +lat_ts=0 +lon_0={XORIG}'
+            '+proj=merc +R={earth_radius} +lat_ts=0 +lon_0={XCENT}'
             + ' +x_0={x_0} +y_0={y_0} +to_meter={XCELL}'
             + ' +no_defs'
         ).format(**props)
     else:
         raise ValueError('GDTYPE {GDTYP} not implemented'.format(**props))
 
     return projstr
@@ -607,14 +614,22 @@
                 'out_in_flag': 0, 'freq': 'hourly',
                 'maximum_difference': 5, 'maximum_ratio': 0.70,
                 'agg_pct': 75, 'api_key': '<your key here>'
             }
 
         self.purpleair_kw = purpleair_kw
 
+    def set_grid_kw(self, grid_kw):
+        if isinstance(grid_kw, str):
+            if grid_kw not in _def_grid_kw:
+                raise KeyError('unknown grid, you must specify properites')
+            grid_kw = _def_grid_kw[grid_kw].copy()
+
+        self.grid_kw = grid_kw
+
     def resize_grid(self, clip=True):
         """
         Update grid_kw property so that it only covers the bbox by adjusting
         the XORIG, YORIG, NCOLS and NROWS. If clip is True, this has the affect
         of reducing the number of rows and columns. This is useful when the
         area of interest is much smaller than the grid defined in grid_kw.
 
@@ -953,14 +968,15 @@
         purpleair_kw = self.purpleair_kw
         tropomi_kw = self.tropomi_kw
         viirsnoaa_kw = self.viirsnoaa_kw
         if compress is None:
             compress = self.compress
 
         wlon, slat, elon, nlat = bbox
+
         if grid and request == 'GetCoverage':
             gridstr = self._build_grid(grid_kw)
         else:
             gridstr = ''
 
         if key.startswith('viirsnoaa'):
             viirsnoaastr = '&MINIMUM_QUALITY={minimum_quality}'.format(
@@ -983,27 +999,35 @@
                 '{maximum_difference}&MAXIMUM_RATIO={maximum_ratio}'
                 '&AGGREGATE={freq}&MINIMUM_AGGREGATION_COUNT_PERCENTAGE='
                 '{agg_pct}&KEY={api_key}'
             ).format(**purpleair_kw)
         else:
             purpleairstr = ''
 
-        if any([key.startswith(pre) for pre in _point_prefixes]):
+        if any([key.startswith(pre) for pre in _nocorner_prefixes]):
             cornerstr = ''
         else:
             cornerstr = f'&CORNERS={corners}'
 
+        if any([key.startswith(pre) for pre in _nolonlats_prefixes]):
+            nolonlatsstr = '&NOLONLATS=1'
+        else:
+            nolonlatsstr = ''
+
         url = (
             f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION=1.0.0'
             f'&REQUEST={request}&FORMAT={formatstr}'
             f'&TIME={bdate:%Y-%m-%dT%H:%M:%SZ}/{edate:%Y-%m-%dT%H:%M:%SZ}'
             f'&BBOX={wlon},{slat},{elon},{nlat}'
             f'&COVERAGE={key}'
             f'&COMPRESS={compress}'
-        ) + purpleairstr + viirsnoaastr + tropomistr + gridstr + cornerstr
+        ) + (
+            purpleairstr + viirsnoaastr + tropomistr + gridstr + cornerstr
+            + nolonlatsstr
+        )
 
         outpath = (
             f'{self.workdir}/{key}_{bdate:%Y-%m-%dT%H%M%SZ}'
             f'_{edate:%Y-%m-%dT%H%M%SZ}'
         )
 
         if formatstr.lower() == 'ascii':
@@ -1028,14 +1052,16 @@
         """
         grid_kw.setdefault('earth_radius', 6370000)
         GDTYP = grid_kw.get('GDTYP', 2)
         if GDTYP == 2:
             projstr = '&LAMBERT={P_ALP},{P_BET},{XCENT},{YCENT}'
         elif GDTYP == 6:
             projstr = '&STEREOGRAPHIC={XCENT},{YCENT},{P_BET}'
+        elif GDTYP == 7:
+            projstr = '&MERCATOR={P_GAM}'
         else:
             raise KeyError('GDTYP only implemented for ')
 
         gridstr = (
             '&REGRID=weighted'
             + projstr
             + '&ELLIPSOID={earth_radius},{earth_radius}'
@@ -1155,18 +1181,22 @@
             Results from download
 
         """
         import gzip
         import shutil
         import os
 
+        # If already gridded, do not use grid keywords
+        nogridkw = any([key.startswith(pre) for pre in _noregrid_prefixes])
+        grid = nogridkw is False
+
         # always use compression for network speed.
         outpath = self.get_file(
             'netcdf-ioapi', key=key, bdate=bdate, edate=edate, bbox=bbox,
-            grid=True, compress=1, verbose=verbose
+            grid=grid, compress=1, verbose=verbose
         )
         # Uncompress the netcdf file. If encoding is available, apply it
         if not self.overwrite and os.path.exists(outpath[:-3]):
             print('Using cached:', outpath[:-3])
         else:
             with gzip.open(outpath, 'rb') as f_in:
                 with open(outpath[:-3], 'wb') as f_out:
@@ -1184,15 +1214,15 @@
                         tvar.encoding.pop('_FillValue', '')
 
                 tmpf.to_netcdf(outpath[:-3], format='NETCDF4_CLASSIC')
 
         if withmeta:
             metapath = self.get_file(
                 'netcdf-ioapi', key=key, bdate=bdate, edate=edate, bbox=bbox,
-                grid=True, compress=1, request='GetMetadata', verbose=verbose
+                grid=grid, compress=1, request='GetMetadata', verbose=verbose
             )
         else:
             metapath = None
 
         f = open_ioapi(outpath[:-3], metapath=metapath)
         if removegz:
             os.remove(outpath)
```

### Comparing `pyrsig-0.4.2/README.md` & `pyrsig-0.4.3/README.md`

 * *Files identical despite different names*

