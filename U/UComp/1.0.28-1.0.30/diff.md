# Comparing `tmp/UComp-1.0.28.tar.gz` & `tmp/UComp-1.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.28.tar", last modified: Wed Jun  7 17:06:38 2023, max compression
+gzip compressed data, was "UComp-1.0.30.tar", last modified: Wed Jun  7 17:20:54 2023, max compression
```

## Comparing `UComp-1.0.28.tar` & `UComp-1.0.30.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 17:06:38.543738 UComp-1.0.28/
--rw-rw-rw-   0        0        0      233 2023-06-06 16:58:27.000000 UComp-1.0.28/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2023-06-07 17:06:38.543738 UComp-1.0.28/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.28/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 17:06:38.528113 UComp-1.0.28/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.28/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.28/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.28/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.28/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    18991 2023-06-06 16:33:02.000000 UComp-1.0.28/UComp/UCmodule.py
--rw-rw-rw-   0        0        0       57 2023-06-06 17:02:10.000000 UComp-1.0.28/UComp/__init__.py
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.28/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    28922 2023-06-06 14:31:28.000000 UComp-1.0.28/UComp/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:06:38.543738 UComp-1.0.28/UComp.egg-info/
--rw-rw-rw-   0        0        0      304 2023-06-07 17:06:38.000000 UComp-1.0.28/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-06-07 17:06:38.000000 UComp-1.0.28/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 17:06:38.000000 UComp-1.0.28/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-07 17:06:38.000000 UComp-1.0.28/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 17:06:38.000000 UComp-1.0.28/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 17:06:38.559361 UComp-1.0.28/setup.cfg
--rw-rw-rw-   0        0        0      590 2023-06-07 17:05:58.000000 UComp-1.0.28/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:20:54.537787 UComp-1.0.30/
+-rw-rw-rw-   0        0        0      233 2023-06-06 16:58:27.000000 UComp-1.0.30/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2023-06-07 17:20:54.553433 UComp-1.0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.30/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 17:20:54.537787 UComp-1.0.30/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.30/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.30/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.30/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.30/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    22455 2023-06-07 16:57:13.000000 UComp-1.0.30/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0       57 2023-06-07 16:15:43.000000 UComp-1.0.30/UComp/__init__.py
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.30/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    27981 2023-06-07 16:58:42.000000 UComp-1.0.30/UComp/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:20:54.537787 UComp-1.0.30/UComp.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 17:20:54.553433 UComp-1.0.30/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-07 17:20:45.000000 UComp-1.0.30/setup.py
```

### Comparing `UComp-1.0.28/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.30/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.28/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.30/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.28/UComp/libopenblas.dll` & `UComp-1.0.30/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.28/UComp/tools.py` & `UComp-1.0.30/UComp/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import multiprocessing as mp
+# from UComp.UCmodule import *
 from UComp import UCmodule as uc
-# from scipy.stats import f
-# from statsmodels.tsa.stattools import acf, pacf
-# from statsmodels.stats.diagnostic import acorr_ljungbox, het_arch
-# from statsmodels.graphics.tsaplots import plot_acf, plot_pacf
 import seaborn as sns
 import scipy.stats as stats
-# import statsmodels.api as sm
-# from sklearn.neighbors import KernelDensity
+
 
 
 def obj2array(y):
-    x = y
     if isinstance(y, uc.UCmodel):
-        x = y.v
+        x = y.v.values
     elif isinstance(y, uc.ETSmodel):
-        x = y.comp[:, 0]
+        x = y.comp[:, 0].values
     elif isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
         x = y.values
+    elif isinstance(y, np.array):
+        x = y
     return x
 
 
 def pacfFun(ACF):
     nCoef = len(ACF)
     fi = np.zeros(nCoef)
     fi[0] = ACF[0]
@@ -39,32 +36,14 @@
          fi[i + 1] = (ACF[i + 1] - (sum(fi[0 : i + 1] * iACF[::-1]))) / (1 - sum(fi * ACF))
          PACF[i + 1] = fi[i + 1]
          iACF = fi[0 : i + 1]
          fi[0 : i + 1] -= fi[i + 1] * iACF[::-1]
     return PACF
 
 
-def ts(y, start='1990', freq='A'):
-    """
-    Converts a numpy vector or matrix into a pandas time series
-    """
-    if isinstance(y, list):
-        y = np.array(y)
-    elif isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
-        return y
-    if len(y.shape) > 1 and y.shape[0] < y.shape[1]:
-        y = y.T
-    time = pd.date_range(start=start, periods=y.shape[0], freq=freq)
-    y = np.array(y, dtype=float)
-    if len(y.shape) > 1:
-        return pd.DataFrame(y, time)
-    else:
-        return pd.Series(y, time)
-
-
 def removeNaNs(x):
     """
     Remove nans at beginning or end of vector
 
     x: a vector or a ts object
 
     Returns:
@@ -152,48 +131,45 @@
     xl = np.linspace(min(x), max(x), 130)
     y = np.exp(-0.5 * ((xl - np.mean(x)) ** 2) / varx) / np.sqrt(2 * np.pi * varx) * (max(x) - min(x)) * nbins
     ax1.plot(xl, y, color='black', linestyle='--')
     ax1.set_xlabel('Values')
     ax1.set_ylabel('Frequency')
     # QQ plot
     theoretical_quantiles = stats.norm.ppf(np.linspace(0.01, 0.99, num=100))
-    empirical_quantiles = np.percentile((x - np.mean(x)) / stdx, np.linspace(0, 100, num=100))
-    ax2.scatter(empirical_quantiles, theoretical_quantiles, color='blue', alpha=0.5)
-    ax2.plot([-3, 3], [-3, 3], color='red')
+    # empirical_quantiles = np.percentile((x - np.mean(x)) / stdx, np.linspace(0, 100, num=100))
+    empirical_quantiles = np.percentile(x, np.linspace(0, 100, num=100))
+    ax2.scatter(theoretical_quantiles, empirical_quantiles, color='blue', alpha=0.5)
+    x1, x2 = theoretical_quantiles[0], theoretical_quantiles[-1]
+    ax2.plot([x1, x2], [x1 * stdx + np.nanmean(x), x2 * stdx + np.nanmean(x)], color='red')
     ax2.set_ylabel('Theoretical quantiles')
     ax2.set_xlabel('Empirical quantiles')
     # Gaussianity test
     stat, pvalue = stats.shapiro(x)
     print('Shapiro Gaussianity test:')
     print('=========================')
     print(f"Stat: {stat:.4f}   P-value: {pvalue:.4f}")
 
 
-def ident(y, nCoef=None, s=12, nPar=0, axes=None):
+def ident(y, nCoef=None, nPar=0, axes=None):
+    if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
+        s = y.resample('Y').count()[1]
+    else:
+        s = 1
     x = obj2array(y)
     if nCoef is None:
         nCoef = max(min(37, int(np.floor(len(x) / 4))), s)
     x = (x - np.nanmean(x))  / np.nanstd(x)
     n = len(x[~np.isnan(x)])
     # ACF and PACF with Ljung Box tests and plots
     ACF = np.full(nCoef, 0.0)
-    PACF = np.full(nCoef, 0.0)
-    fi = np.full(nCoef, 0.0)
     BAND = 2 / np.sqrt(n)
     for i in range(nCoef):
-        prod = x[-n + i : ] * x[: n - i]
+        prod = x[-n + i + 1: ] * x[: n - i - 1]
         prod1 = prod[~np.isnan(prod)]
         ACF[i] = sum(prod1) / len(prod1)
-    # PACF[0] = fi[0] = ACF[0]
-    # for i in range(nCoef - 1):
-    #      iACF = ACF[: i + 1]
-    #      fi[i + 1] = (ACF[i + 1] - (sum(fi[0 : i + 1] * iACF[::-1]))) / (1 - sum(fi * ACF))
-    #      PACF[i + 1] = fi[i + 1]
-    #      iACF = fi[0 : i + 1]
-    #      fi[0 : i + 1] -= fi[i + 1] * iACF[::-1]
     PACF = pacfFun(ACF)
     SIGa = np.where(ACF > BAND, "+", ".")
     SIGa = np.where(ACF < -BAND, "-", SIGa)
     SIGp = np.where(PACF > BAND, "+", ".")
     SIGp = np.where(PACF < -BAND, "-", SIGp)
     BOX = n * (n + 2) * np.cumsum((ACF ** 2) / (np.array(n, dtype=float) - range(1, nCoef + 1)))
     gl = range(1 - nPar, nCoef + 1 - nPar)
@@ -201,14 +177,15 @@
     pval = 1 - stats.chi2.cdf(BOX, gl)
     out = pd.DataFrame({"SACF": np.round(ACF, 3),
                         "sa": SIGa,
                         "LB": np.round(BOX, 3),
                         "p.val": np.round(pval, 3),
                         "SPACF": np.round(PACF, 3),
                         "sp": SIGp})
+    out.index += 1
     if axes == None:
         plotAcfPacf(ACF, PACF, s, n)
     return out
 
 
 def plotBar(ACF, ax, s=1, n=None, label="ACF"):
     nCoef = len(ACF)
@@ -296,15 +273,14 @@
     pval = stats.f.cdf(varStat, n1, n1)
     out = pd.DataFrame({
         "Portion_of_data": [np.round(parts, 4)],
         "F_statistic": [np.round(varStat, 4)],
         "p.value": [np.round(pval, 4)]
     })
     out.index = [""]
-    print(out)
     return out
 
 
 def conv(*args):
     """
     1D convolution: filtering or polynomial multiplication
 
@@ -318,24 +294,14 @@
     """
     n = len(args)
     if n > 2:
         return conv(args[0], conv(*args[1:]))
     else:
         # Convolution of two vectors
        return np.convolve(args[0], args[1])
-        # x = np.asarray(args[0])
-        # y = np.asarray(args[1])
-        # lx = len(x)
-        # ly = len(y)
-        # lz = lx + ly - 1
-        # z = np.zeros(lz)
-        # for i in range(lx):
-        #     for j in range(ly):
-        #         z[i + j] += x[i] * y[j]
-        # return z
 
 
 def armaFilter(MA, AR, y):
     """
     Filter of time series
 
     MA: MA numerator polynomial
@@ -396,16 +362,14 @@
     for i in range(n):
         poli = np.concatenate(([1], np.zeros(seas[i] - 1), [-1]))
         if difs[i] > 0:
             for j in range(difs[i]):
                 pol = np.convolve(pol, poli)
     dx = armaFilter(pol, [1], y)
     dx = dx[:len(y) - len(pol) + 1]
-    if isinstance(y, pd.Series):
-        dx = pd.Series(dx, index=y.index[:len(dx)])
     return dx
 
 
 def roots(x):
     """
     Roots of polynomial
 
@@ -713,15 +677,15 @@
     plotH = pd.DataFrame(metrics, index=np.arange(1, h + 1))
     plt.plot(plotH)
     plt.ylabel("Error metric")
     plt.show(block=False)
     return outj
 
 
-def Accuracy(py, y, s=None, collectFun=np.mean):
+def Accuracy(py, y, collectFun=np.mean):
     """
     Accuracy for 1 time series y and several forecasting
     methods py and h steps ahead py is h x nMethods x nSeries
     Inputs:
         py:         matrix of forecasts (h x nMethods x nForecasts)
         y:          a matrix of actual values (n x nForecasts)
         s:          seasonal period, number of observations per year
@@ -735,15 +699,15 @@
     #' @rdname Accuracy
     :rtype: object
     """
     # Accuracy for 1 time series y and several forecasting methods py and h steps ahead
     # py is h x nMethods x nSeries
     # y is n x nSeries
     spy = len(py.shape)
-    if isinstance(py, pd.Series) and isinstance(y, pd.Series):
+    if (isinstance(py, pd.Series) or isinstance(py, pd.DataFrame)) and isinstance(y, pd.Series):
         tpy = py.index
         ty = y.index
         if min(tpy) - max(ty) > 1e-5:
             raise ValueError("No errors to estimate, check dates!!!")
         if max(tpy) - max(ty) > 1e-5:
             # Cut forecasts
             py = py.head(np.where(max(ty) == tpy)[0])
@@ -798,60 +762,67 @@
                                    np.nanmean(np.abs(e), axis=0) / np.nanmean(np.abs(fRW), axis=0),
                                    np.nansum(np.abs(e), axis=0) / np.nansum(np.abs(fRW), axis=0),
                                    np.sqrt(np.nansum(p * p, axis=0) / np.nansum(theil * theil, axis=0))))
         out[i, :] = collectFun(aux, axis=1)
     return pd.DataFrame(out, index=rownames, columns=colnames)
 
 
-def tsDisplay(y, nCoef=None, nPar=0, s=12):
-    x = obj2array(y)
+def tsDisplay(y, nCoef=None, nPar=0):
+    if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
+        s = y.resample('Y').count()[1]
+    else:
+        s = 1
+    # x = obj2array(y)
     # if s is None:
     #     s = frequency(x)
     fig = plt.figure(figsize=(8, 6))
     ax1 = fig.add_subplot(2, 1, 1)
-    ax1.plot(x)
+    ax1.plot(y)
     ax1.set_xlabel('Time')
     ax1.set_ylabel('Value')
     ax2 = fig.add_subplot(2, 2, 3)
     ax3 = fig.add_subplot(2, 2, 4)
-    out = ident(x, nCoef, s, nPar, True)
+    out = ident(y, nCoef, nPar, True)
     plotAcfPacf(np.array(out["SACF"]), np.array(out["SPACF"]), s, len(y), [ax2, ax3])
     plt.show(block=False)
 
 
-def tests(x, parts=1/3, nCoef=None, nPar=0, s=12, avoid=16):
+def tests(x, parts=1/3, nCoef=None, nPar=0, avoid=16):
     """
     Tests on a time series
 
     y: a vector, ts or tsibble object
     parts: proportion of sample to include in ratio of variances test
     nCoef: number of autocorrelation coefficients to estimate
     nPar: number of parameters in a model if y is a residual
     s: seasonal period, number of observations per year
     avoid: number of observations to avoid at beginning of sample to eliminate initial effects
 
     Author:
     Diego J. Pedregal
     """
-    x = obj2array(x)
+    if isinstance(x, pd.Series) or isinstance(x, pd.DataFrame):
+        s = x.resample('Y').count()[1]
+    else:
+        s = 1
     print("Summary statistics:")
     print("===================")
     print(sumStats(x))
     print("Autocorrelation tests:")
     print("=====================")
     nCoef = min(25, len(x) / 4)
     # Plot figure
     fig = plt.figure(figsize=(8, 6))
     ax1 = fig.add_subplot(4, 1, 1)
     ax1.plot(x)
     ax1.set_xlabel('Time')
     ax1.set_ylabel('Value')
     ax2 = fig.add_subplot(4, 2, 3)
     ax3 = fig.add_subplot(4, 2, 4)
-    out = ident(x, nCoef, s, nPar, [ax2, ax3])
+    out = ident(x, nCoef, nPar, [ax2, ax3])
     plotAcfPacf(np.array(out["SACF"]), np.array(out["SPACF"]), s, len(x), [ax2, ax3])
     print(out)
     ax4 = fig.add_subplot(4, 2, 5)
     ax5 = fig.add_subplot(4, 2, 6)
     pGAUSS = gaussTest(x, [ax4, ax5])
     print("Ratio of variance tests:")
     print("=======================")
```

### Comparing `UComp-1.0.28/setup.py` & `UComp-1.0.30/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.28',
+    version='1.0.30',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
     package_data={'UComp': ['*.pyd', 'libopenblas.dll']},
     keywords='paquete ejemplo',
     install_requires=[
         'numpy>=1.18.0',
         'requests>=2.25.0',
+        'seaborn',
+        'pandas',
+        'matplotlib',
+        'scipy',
     ],
-)
+)
```

