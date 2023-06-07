# Comparing `tmp/gregory_online-0.2.6.tar.gz` & `tmp/gregory_online-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gregory_online-0.2.6.tar", last modified: Tue Jun  6 11:51:21 2023, max compression
+gzip compressed data, was "gregory_online-0.2.7.tar", last modified: Wed Jun  7 09:59:02 2023, max compression
```

## Comparing `gregory_online-0.2.6.tar` & `gregory_online-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:51:21.696676 gregory_online-0.2.6/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-06 11:51:21.696676 gregory_online-0.2.6/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-06 11:51:15.000000 gregory_online-0.2.6/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:51:21.692676 gregory_online-0.2.6/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50588 2023-06-06 11:51:18.000000 gregory_online-0.2.6/bin/gregory_online
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:51:21.692676 gregory_online-0.2.6/gregory_online/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2022-09-16 15:11:00.000000 gregory_online-0.2.6/gregory_online/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-17 17:33:40.000000 gregory_online-0.2.6/gregory_online/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12513 2023-06-05 13:30:27.000000 gregory_online-0.2.6/gregory_online/fetchnp.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 14:10:17.000000 gregory_online-0.2.6/gregory_online/histo_analyze.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3957 2023-06-02 15:39:44.000000 gregory_online-0.2.6/gregory_online/histo_displ.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-06 11:16:18.000000 gregory_online-0.2.6/gregory_online/histo_global_cont.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-05-31 13:39:18.000000 gregory_online-0.2.6/gregory_online/histo_io.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:29:49.000000 gregory_online-0.2.6/gregory_online/histo_np_ops.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-20 14:10:17.000000 gregory_online-0.2.6/gregory_online/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-20 14:10:17.000000 gregory_online-0.2.6/gregory_online/topbar.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2022-09-16 15:11:00.000000 gregory_online-0.2.6/gregory_online/utilone.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3279 2023-06-06 11:50:54.000000 gregory_online-0.2.6/gregory_online/utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-06 11:51:21.692676 gregory_online-0.2.6/gregory_online.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      589 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       65 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-06 11:51:21.000000 gregory_online-0.2.6/gregory_online.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-06 11:51:21.696676 gregory_online-0.2.6/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1200 2023-06-01 12:16:03.000000 gregory_online-0.2.6/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-07 09:59:02.364765 gregory_online-0.2.7/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-07 09:59:02.364765 gregory_online-0.2.7/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-07 09:58:51.000000 gregory_online-0.2.7/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-07 09:59:02.364765 gregory_online-0.2.7/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    52156 2023-06-07 09:58:54.000000 gregory_online-0.2.7/bin/gregory_online
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-07 09:59:02.364765 gregory_online-0.2.7/gregory_online/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2022-09-16 15:11:00.000000 gregory_online-0.2.7/gregory_online/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-17 17:33:40.000000 gregory_online-0.2.7/gregory_online/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12513 2023-06-05 13:30:27.000000 gregory_online-0.2.7/gregory_online/fetchnp.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 14:10:17.000000 gregory_online-0.2.7/gregory_online/histo_analyze.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3957 2023-06-02 15:39:44.000000 gregory_online-0.2.7/gregory_online/histo_displ.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-06 11:16:18.000000 gregory_online-0.2.7/gregory_online/histo_global_cont.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-05-31 13:39:18.000000 gregory_online-0.2.7/gregory_online/histo_io.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:29:49.000000 gregory_online-0.2.7/gregory_online/histo_np_ops.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-20 14:10:17.000000 gregory_online-0.2.7/gregory_online/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-20 14:10:17.000000 gregory_online-0.2.7/gregory_online/topbar.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2022-09-16 15:11:00.000000 gregory_online-0.2.7/gregory_online/utilone.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3279 2023-06-06 11:50:54.000000 gregory_online-0.2.7/gregory_online/utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-07 09:59:02.364765 gregory_online-0.2.7/gregory_online.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      589 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       65 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-07 09:59:02.364765 gregory_online-0.2.7/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1200 2023-06-01 12:16:03.000000 gregory_online-0.2.7/setup.py
```

### Comparing `gregory_online-0.2.6/PKG-INFO` & `gregory_online-0.2.7/gregory_online.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gregory_online
-Version: 0.2.6
+Name: gregory-online
+Version: 0.2.7
 Summary: Online watching HTTP server of ROOT on port 9009
 Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gregory_online-0.2.6/README.md` & `gregory_online-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/bin/gregory_online` & `gregory_online-0.2.7/bin/gregory_online`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,18 @@
 h1np_last_interval = 20
 h1np_substr = None # h1np - backg
 #----load separately
 h1np_backg = None
 h1np_backg_lt = 100  # background livetime
 
 
+
+deadt = 0 #  for influx
+deadtavg = [0,0] #  long term dt for histosave # NOT USED
+deadttot = 0
 # global h1np,h1np_diff,h1np_old,h1np_old_age,h1np_substr,h1np_backg,h1np_backg_lt, cala, calb, cala_bg, calb_bg
 
 
 
 # def udpsend(message):
 #     """
 #     send to local seread running instance
@@ -253,14 +257,15 @@
     print("i... ")
 
     # ---------------- container stuff
     global histograms, canvases, range_and_peaks
     global gregory_started
     global last_fit_res
     global ECALIB, ECALIBa, ECALIBb # calibrations
+    global deadtavg, deadt, deadttot # avg not used; tot from h1np
     #
     # --------------    other stuff
     #global h1np,h1np_diff,h1np_old,h1np_old_age,h1np_substr,h1np_backg,h1np_backg_lt
     global h1np,h1np_diff,h1np_old,h1np_last_interval,h1np_substr,h1np_backg,h1np_backg_lt, cala, calb, cala_bg, calb_bg
 
     cmd = "" # no key command
 
@@ -359,14 +364,17 @@
 
         if  b0c01.fetch_flag():
             # if fetched - get values ==========================
 
             h1np = b0c01.get_h1np()
             h1np_diff = b0c01.get_h1np_diff()
             deltat = b0c01.get_deltat()
+            if runtime>b0c01.get_runtime():
+                deadtavg = [0,0]
+
             runtime = b0c01.get_runtime() # total histogram time/age; NOT last_interval
             gregory_started = b0c01.get_started()
             #if runtime.total_seconds()<=0:
             #    runtime = 1#dt.datetime.now()-dt.datetime.now()
             lenhistos = b0c01.get_lenhistos()
             #print(runtime)
 
@@ -380,15 +388,15 @@
                 warn_del = f"{fg.default}{bg.default}"
             unwarn_del = f"{fg.default}{bg.blue}"
 
             limits_calib = b0c01.get_limits_calib()
 
             rate= h1np_diff.sum()/deltat # does sum contain underflow? ->Integral() doesnot
             # I like to have underflow there...
-
+            # deadtavg  is on the line 444
 
             # print(h1np_diff[0], h1np_diff[1]) # underflow and 1st bin #1
             #------------------------- ending the small calc
 
 
 
 
@@ -424,23 +432,42 @@
                 ##display_np( h1np_substr,  "substr", "c_substr", 1, errors)
 
 
             #if ROOT.gDirectory.FindObject("backg"):
             #    fill_h_with_np(histograms["backg"],"backg")  # No livetime here
 
 
+            # __________calculate deadtime  for influx________________________
+            # just_spesum = h1np_diff[1:-1].sum()
+            just_spesum = h1np_diff.sum()
+            # print("D... just_spesum==",just_spesum, h1np_diff, h1np)
+            deadt = 0
+            if  just_spesum !=0:
+                # print("D... diff[0]==", h1np_diff[0], h1np_diff[1], len(h1np_diff) )
+                deadt = h1np_diff[0]/just_spesum*100
+
+            #______________ deadtime of all spectrum________________________-
+            just_spesum = h1np.sum()
+            # print("D... just_spesum==",just_spesum, h1np_diff, h1np)
+            deadttot = 0
+            if  just_spesum !=0:
+                # print("D... diff[0]==", h1np_diff[0], h1np_diff[1], len(h1np_diff) )
+                deadttot = h1np[0]/just_spesum*100
+            #deadtavg[0]+=deadt
+            #deadtavg[1]+=1
+
             INFLUX = True
             if INFLUX and len(h1np_diff)>2:
-                # just_spesum = h1np_diff[1:-1].sum()
-                just_spesum = h1np_diff.sum()
-                # print("D... just_spesum==",just_spesum, h1np_diff, h1np)
-                deadt = 0
-                if  just_spesum !=0:
-                    # print("D... diff[0]==", h1np_diff[0], h1np_diff[1], len(h1np_diff) )
-                    deadt = h1np_diff[0]/just_spesum*100
+                # # just_spesum = h1np_diff[1:-1].sum()
+                # just_spesum = h1np_diff.sum()
+                # # print("D... just_spesum==",just_spesum, h1np_diff, h1np)
+                # deadt = 0
+                # if  just_spesum !=0:
+                #     # print("D... diff[0]==", h1np_diff[0], h1np_diff[1], len(h1np_diff) )
+                #     deadt = h1np_diff[0]/just_spesum*100
                 if is_float(rate) and is_float(deadt):
                     infvals = f"rate_{spectrumname}={rate:.1f},deadt_{spectrumname}={deadt:.1f}"
                     # print("D...",infvals)
                     influxwrite("test", f"greg",  infvals ) # hostname added automat
 
 
 
@@ -597,29 +624,29 @@
                 if thisname in histograms.keys():
                     #print("i... pksearch", thisname)
                     # i need sigma 1 here !
                     tspe = ROOT.TSpectrum()
                     res = tspe.Search( histograms[thisname], 1, "nodraw", 0.05 )
 
                     print(f"i... {res} peaks detected")
-                    print("D... 1")
+                    #print("D... 1")
                     pkfuncs = histograms[thisname].GetListOfFunctions()
-                    print("D... 2")
+                    #print("D... 2")
                     pm = pkfuncs.FindObject("TPolyMarker");
-                    print("D... 3")
+                    #print("D... 3")
                     xvec = pm.GetX()
-                    print("D... 4")
+                    #print("D... 4")
                     xvecso = np.array( [] )
-                    print("D... 5")
+                    #print("D... 5")
                     for j in range(pm.GetN()):
-                        print("D... 5 .... ",j)
+                        print(f"D... 5 .... {j:02d}  {float(xvec[j]):7.2f}" )
                         xvecso = np.append( xvecso, float(xvec[j]) )
-                    print("D... 6")
+                    #print("D... 6")
                     xvecso = np.sort( xvecso )# xvecso = sorted(xvecso)
-                    print("D... 7")
+                    #print("D... 7")
                     print("========== i  remember these peaks for the next fit ======")
                     range_and_peaks["rng"] = get_ene_range(histograms[thisname])
                     range_and_peaks["spe"] = thisname
                     range_and_peaks["pks"] = xvecso
                     #print("i... ", len(xvecso), f" {thisname}:",xvecso)
                     print( f"i... {fg.green}OK{fg.default}",range_and_peaks )
 
@@ -676,47 +703,50 @@
                             if i.find("area")>=0: print( f"          {i:10s} {res[i]:.4f} ")
 
 
         elif cmd == "c":   # ***CMD***  CALIB =======
             print(f"i... c: {arg}       datalen= {len(ECALIB)} _______________________" )
             print("i...    c Ene     channel")
             print("i...    c Isotope channel")
+            print("i...    c [Isotope|Ene]   f    ... for fit result as the bin")
             print("i...    c r  ....  reset calibration data")
             for ik in ECALIBdb.keys():
                 print(f"i...         | {ik:7s} | {ECALIBdb[ik]:8.2f} |")
             print( "             _________________________________")
+
             if len(arg)>0:
                 eline = None # energy of the line
                 bline = None # bin of the line
                 dbline = 1
                 if len(arg.split())<1:
                     print(f"X... {fg.red} give me {bg.white}'c  ene bin'{bg.default} OR 'c  reset' ==  'c r'{fg.default}")
                     # break
                 elif arg.split()[0]=="reset" or arg.split()[0]=="r" :  # ** reset **
                     ECALIB = []
                     ECALIBa = 1
                     ECALIBb = 0
                     print("i... {fg.yellow} RESET! e-calibration done{fg.default} ")
-                    # break
+                # decompose the arguments....
                 else:
                     ok = True
                     eline, bline = None,None
-                    if is_float(arg.split()[0]):   # ** energy **
+                    if is_float(arg.split()[0]):   # ** energy was given **
                         eline = float(arg.split()[0])
-                    elif arg.split()[0].upper() in ECALIBdb.keys():
+                    elif arg.split()[0].upper() in ECALIBdb.keys(): #** 40K was given **
                         eline = ECALIBdb[arg.split()[0].upper()]
-                    else:
+                    else: # ** something else happened**
                         print("X... problem if not float nor in DB",arg.split() )
                         ok = False
-                    print(f"D... ... eline {eline}")
+                    #print(f"D... ... eline {eline}")
 
                     print(arg.split(), arg.split()[1], is_float(arg.split()[1]))
+                    # BIN to be decoded
                     if len(arg.split())>1 and is_float(arg.split()[1]):   # ** bin **
                         bline = float(arg.split()[1])
-                        print(f"D... bline={bline}")
+                        #print(f"D... bline={bline}")
                     # taking from fit....
                     elif len(arg.split())>1 and arg.split()[1]=="f":      # ** f=fitted bin **
                         if "channel" in last_fit_res:
                             bline = last_fit_res["channel"]
                             dbline = last_fit_res["dchannel"]
                             print("i... GETTING LAST FITTED PEAK for calibration bin", bline)
                         else:
@@ -865,15 +895,15 @@
                     print("X... zoom's  energy is not float")
                 if middle is not None:
                     is_zoomed =[ True, middle ]
                     for i in histograms.keys():
                         histo_zoomenergy( histograms[i] ,
                                       is_zoomed[1] - config.CONFIG["window"]/2,
                                       is_zoomed[1] + config.CONFIG["window"]/2 )
-            elif "is_zoomed" in globals() and is_zoomed[0]:
+            elif "is_zoomed" in locals() and is_zoomed[0]:
                 config.CONFIG["window"] = config.CONFIG["window"]/2
                 for i in histograms.keys():
                     histo_zoomenergy( histograms[i] ,
                                       is_zoomed[1] - config.CONFIG["window"]/2,
                                       is_zoomed[1] + config.CONFIG["window"]/2 )
 
 
@@ -939,20 +969,23 @@
                 print("i... cmd t needs time from start 3600s 1h 1:00:00")
                 continue
             arg = time2seconds(arg)
             print(f"i... arg: seconds == {arg} ")
             b0c01.set_started_before( arg) # ON "T" time
 
         elif cmd == "s":   # ***CMD*** #============= s save
-            print("i... just save total")
-            save_hist_txt( "tot" , total_time = runtime.total_seconds() , started = b0c01.started, deadtime = 0 )
+            #deadt2 = 0
+            #if deadtavg[1]>0:
+            #    deadt2 = deadtavg[0]/deadtavg[1]
+            print("i... just save total, deadtime = ",deadttot)
+            save_hist_txt( "tot" , total_time = runtime.total_seconds() , started = b0c01.started, deadtime = deadttot/100 )
             if len(arg)>0:
                 thisname = arg.split()[0]
                 if thisname in histograms.keys():
-                    save_hist_txt( thisname , total_time = runtime.total_seconds() , started = b0c01.started, deadtime = 0 , errors = True)
+                    save_hist_txt( thisname , total_time = runtime.total_seconds() , started = b0c01.started, deadtime = deadttot/100 , errors = True)
 
 
         elif cmd == "a":   # ***CMD***  AGE ========== a age_of_diff histo
             if  arg=="":
                 print("i... cmd a needs time")
                 continue
             arg = time2seconds(arg)
```

### Comparing `gregory_online-0.2.6/gregory_online/config.py` & `gregory_online-0.2.7/gregory_online/config.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online/fetchnp.py` & `gregory_online-0.2.7/gregory_online/fetchnp.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online/histo_analyze.py` & `gregory_online-0.2.7/gregory_online/histo_analyze.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online/histo_displ.py` & `gregory_online-0.2.7/gregory_online/histo_displ.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online/histo_global_cont.py` & `gregory_online-0.2.7/gregory_online/histo_global_cont.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online/histo_io.py` & `gregory_online-0.2.7/gregory_online/histo_io.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online/histo_np_ops.py` & `gregory_online-0.2.7/gregory_online/histo_np_ops.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online/key_enter.py` & `gregory_online-0.2.7/gregory_online/key_enter.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online/topbar.py` & `gregory_online-0.2.7/gregory_online/topbar.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online/utils.py` & `gregory_online-0.2.7/gregory_online/utils.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/gregory_online.egg-info/PKG-INFO` & `gregory_online-0.2.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gregory-online
-Version: 0.2.6
+Name: gregory_online
+Version: 0.2.7
 Summary: Online watching HTTP server of ROOT on port 9009
 Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gregory_online-0.2.6/gregory_online.egg-info/SOURCES.txt` & `gregory_online-0.2.7/gregory_online.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.6/setup.py` & `gregory_online-0.2.7/setup.py`

 * *Files identical despite different names*

