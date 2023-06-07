# Comparing `tmp/biocartograph-0.6.1.tar.gz` & `tmp/biocartograph-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocartograph-0.6.1.tar", last modified: Fri Jun  2 09:32:44 2023, max compression
+gzip compressed data, was "biocartograph-0.6.2.tar", last modified: Wed Jun  7 09:18:17 2023, max compression
```

## Comparing `biocartograph-0.6.1.tar` & `biocartograph-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-02 09:32:44.406843 biocartograph-0.6.1/
--rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-06-01 15:35:36.000000 biocartograph-0.6.1/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-02 09:32:44.406843 biocartograph-0.6.1/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-06-01 15:35:36.000000 biocartograph-0.6.1/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-02 09:32:44.405843 biocartograph-0.6.1/biocartograph.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-02 09:32:44.000000 biocartograph-0.6.1/biocartograph.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)      334 2023-06-02 09:32:44.000000 biocartograph-0.6.1/biocartograph.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-06-02 09:32:44.000000 biocartograph-0.6.1/biocartograph.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-06-02 09:32:44.000000 biocartograph-0.6.1/biocartograph.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-06-02 09:32:44.406843 biocartograph-0.6.1/setup.cfg
--rw-r--r--   0 rictjo    (1000) users      (100)      955 2023-06-02 09:32:03.000000 biocartograph-0.6.1/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-02 09:32:44.405843 biocartograph-0.6.1/src/
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-02 09:32:44.406843 biocartograph-0.6.1/src/biocartograph/
--rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-06-01 15:35:36.000000 biocartograph-0.6.1/src/biocartograph/__init__.py
--rw-r--r--   0 rictjo    (1000) users      (100)     3334 2023-06-01 15:35:36.000000 biocartograph-0.6.1/src/biocartograph/composition.py
--rw-r--r--   0 rictjo    (1000) users      (100)    16747 2023-06-02 09:32:03.000000 biocartograph-0.6.1/src/biocartograph/enrichment.py
--rw-r--r--   0 rictjo    (1000) users      (100)    22401 2023-06-01 15:35:36.000000 biocartograph-0.6.1/src/biocartograph/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (100)    26154 2023-06-01 15:35:36.000000 biocartograph-0.6.1/src/biocartograph/special.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-07 09:18:17.767916 biocartograph-0.6.2/
+-rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-06-01 15:35:36.000000 biocartograph-0.6.2/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-07 09:18:17.767916 biocartograph-0.6.2/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-06-01 15:35:36.000000 biocartograph-0.6.2/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-07 09:18:17.766916 biocartograph-0.6.2/biocartograph.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-07 09:18:17.000000 biocartograph-0.6.2/biocartograph.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)      334 2023-06-07 09:18:17.000000 biocartograph-0.6.2/biocartograph.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-06-07 09:18:17.000000 biocartograph-0.6.2/biocartograph.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-06-07 09:18:17.000000 biocartograph-0.6.2/biocartograph.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-06-07 09:18:17.767916 biocartograph-0.6.2/setup.cfg
+-rw-r--r--   0 rictjo    (1000) users      (100)      955 2023-06-07 09:15:40.000000 biocartograph-0.6.2/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-07 09:18:17.766916 biocartograph-0.6.2/src/
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-07 09:18:17.767916 biocartograph-0.6.2/src/biocartograph/
+-rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-06-01 15:35:36.000000 biocartograph-0.6.2/src/biocartograph/__init__.py
+-rw-r--r--   0 rictjo    (1000) users      (100)     3334 2023-06-01 15:35:36.000000 biocartograph-0.6.2/src/biocartograph/composition.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    16747 2023-06-02 09:32:03.000000 biocartograph-0.6.2/src/biocartograph/enrichment.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    22401 2023-06-01 15:35:36.000000 biocartograph-0.6.2/src/biocartograph/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    26687 2023-06-07 09:15:40.000000 biocartograph-0.6.2/src/biocartograph/special.py
```

### Comparing `biocartograph-0.6.1/LICENSE` & `biocartograph-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.1/PKG-INFO` & `biocartograph-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.6.1
+Version: 0.6.2
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.6.1/README.md` & `biocartograph-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.1/biocartograph.egg-info/PKG-INFO` & `biocartograph-0.6.2/biocartograph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.6.1
+Version: 0.6.2
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.6.1/setup.py` & `biocartograph-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name         = "biocartograph",
-    version      = "0.6.1",
+    version      = "0.6.2",
     author       = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description  = "Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/rictjo/biocarta",
     packages = setuptools.find_packages('src'),
```

### Comparing `biocartograph-0.6.1/src/biocartograph/composition.py` & `biocartograph-0.6.2/src/biocartograph/composition.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.1/src/biocartograph/enrichment.py` & `biocartograph-0.6.2/src/biocartograph/enrichment.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.1/src/biocartograph/quantification.py` & `biocartograph-0.6.2/src/biocartograph/quantification.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.1/src/biocartograph/special.py` & `biocartograph-0.6.2/src/biocartograph/special.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,25 +118,25 @@
                       use_exclusion:str = 'pruned' ) -> list :
     check_set  = {'tsv','csv','xlsx'}
     if dir_string[-1] != '/':
         dir_string += '/'
     if not ( dir_string[0] == '~' or dir_string[0] == '/' ) :
         print ( "INCLOMPLETE DIRECTORY" )
     import os
-    contents = os.listdir(dir_string)
-    what = []
+    contents	= os.listdir(dir_string)
+    what	= []
     for thing in contents :
         if 'str' in str(type(use_exclusion)):
             if 'pruned' in thing :
                 continue
         if thing.split('.')[-1] in check_set :
             what.append( [dir_string+thing ,'\t' if '.tsv' in thing else ',' if '.csv' in thing else 'X' if '.xlsx' in thing else ' ' ] )
     return ( what )
 
-def prune_dataframe( df:pd.DataFrame , indices:str , property_name:str , value_name:str ) -> pd.DataFrame :
+def prune_dataframe ( df:pd.DataFrame , indices:str , property_name:str , value_name:str ) -> pd.DataFrame :
         from biocartograph.special import pivot_data
         pdf = pivot_data( df, index = indices , column = property_name , values = value_name )
         pdf = pdf.dropna( )
         pdf = pdf.iloc[ np.inf != np.abs( 1.0/np.std(pdf.values,1) ) ,
                         np.inf != np.abs( 1.0/np.std(pdf.values,0) ) ].copy().apply(pd.to_numeric)
         pdf .loc[:,indices] = pdf.index
         mdf = pdf.melt( id_vars = [indices] )
@@ -152,15 +152,14 @@
         with open(file[0],'r') as input :
             for line in input :
                 columns = line.replace('\n','').split(file[1])
                 file_lookup[file[0]] = [ c for c in columns if len(c)>0 ]
                 break
     return ( file_lookup )
 
-
 def reformat_results_to_gmtfile_pcfile (	header_str:str          = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' ,
 						hierarchy_file:str	= 'resdf_f.tsv' ,
 						hierarchy_id:str	= 'cids.user.'  ,
 						axis:int = 0, order:str = 'descending'  , bRedundant:bool=False ,
 						hierarchy_level_label:str = 'HCLN' , bErrorCheck:bool = False ) -> tuple[list] :
     #
     df = pd.read_csv( header_str+hierarchy_file , sep='\t' , index_col=0 )
@@ -172,15 +171,15 @@
     if not bCreatePC :
         print ( 'NOT ENOUGH LABELS FOR CONSTRUCTING A HIERARCHY' )
         print ( 'SINGLE LABELING SUPPLIED : ' , hierarchy_id )
         print ( 'FLAT GMT FOR CLUSTERS WILL BE CONSTRUCTED' )
         gmtdf = df.groupby(hierarchy_id).apply(lambda x:x.index.values.tolist())
         GMTS = list()
         for name,entry in zip(gmtdf.index,gmtdf.values) :
-            GMTS.append(  hierarchy_level_label + '-' + 'cluster id ' + str(name) + '\t' + str(name) + '\t' + '\t'.join(entry)  )
+            GMTS .append(  hierarchy_level_label + '-' + 'cluster id ' + str(name) + '\t' + str(name) + '\t' + '\t'.join(entry)  )
         return ( GMTS , None )
     df.loc[:,hierarchy_id+'0'] = 1 # ROOT
     #
     cvs = sorted([ v[::-1] for v in np.max( df,0 ).items() ] )
     if cvs[0][0] >= cvs[-1][0] :
         print ( 'WARNING: UNUSABLE ORDER' )
     if len(cvs) < 2 :
@@ -242,15 +241,14 @@
         if item[0] in relevant_set :
             GMTS.append( '\t'.join([ item[0],'TEXT', *list(item[1]) ]) )
     PCL = []
     for item in  PCD.items() :
         PCL.append([ -1, item[0] , item[1] ])
     return ( GMTS, PCL )
 
-
 def reformat_results_and_print_gmtfile_pcfile ( header_str:str          = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' ,
 						hierarchy_file:str      = 'resdf_f.tsv' ,
                                                 hierarchy_id:str        = 'cids.user.' ,
                                                 axis:int = 0, order:str = 'descending' ,
                                                 hierarchy_level_label:str = 'HCLN' ) -> list[str] :
     GMTS,PCL = reformat_results_to_gmtfile_pcfile (	hierarchy_file		=  hierarchy_file ,
                                                 	header_str		=  header_str ,
@@ -273,15 +271,15 @@
         print ( "parent\tchild" , file = pc_of )
         for g in PCL :
             print ( g[1]+'\t'+g[2], file = pc_of)
         pc_of.close()
     return( gmtname , pcname )
 
 def rescreen (  header_str:str          = "../results/DMHMSY_Wed_Apr__5_10_02_33_2023_" ,
-                full_solution:str       = "hierarch_f.tsv" ,
+                full_solution:str       = "hierarch_f.tsv" , bVerbose:bool=False ,
                 o_filename:str          = None ) -> pd.DataFrame :
     #
     filename            = header_str + full_solution
     #
     df = pd.read_csv( filename , sep='\t', index_col=0 )
     df.index = range(len(df))
     #
@@ -291,15 +289,16 @@
     for i in range( L ) :
         arow = df.iloc[i,:].values
         for item in Counter( list( Counter( arow ).values() ) ).items() :
             if item[0] in full_result_dict :
                 full_result_dict[ item[0] ] += item[1]
             else :
                 full_result_dict[ item[0] ]  = item[1]
-        print ( 'DONE' , i , 'OF' , L, 'OR',i/L )
+        if bVerbose:
+            print ( 'DONE' , i , 'OF' , L, 'OR',i/L )
     df_ = pd.DataFrame( full_result_dict.items() , columns=['k','v'] )
     if not o_filename is None :
         df_.to_csv( o_filename , sep='\t' )
     return ( df_ )
 
 def contraction ( value:float , q:float , d:float ) -> float :
     if value <= 0 :
@@ -321,27 +320,25 @@
         d_ = 1.0/list(set(sorted( b )))[1]
     if q is None :
         q_ = np.quantile( b , q=quantile )
     # THIS OPERATION IS SLOW
     P  = np.array(list(map( lambda x:contraction(x , q=q_ , d=d_) , b ))).reshape(nm)
     return ( P )
 
-
 def contract_df ( a:pd.DataFrame , d:float=None , q:float=None , quantile:float=0.05 ) -> pd.DataFrame :
     nm = np.shape(a.values)
     b  = a.values.reshape(-1)
     d_,q_ = d,q
     if d is None :
         d_ = 1.0/list(set(sorted( b )))[1]
     if q is None :
         q_ = np.quantile( b , q=quantile )
     # THIS OPERATION IS SLOWER
     return ( a.apply( lambda x : pd.Series([contraction(x_ , q=q_ , d=d_ ) for x_ in x],name=x.name,index=x.index) )  )
 
-
 def generate_hulls ( df:pd.DataFrame , gid:str = 'cids.max' , hid:str='UMAP.' ,
                      cid:str = None , xid:str = None ,
                      incremental:bool=False, qhull_options:str = None , bPlottered:bool=False ) -> dict :
     #
     # CONSIDERING SWTICH FROM QHULL TO FASTER AND TOPOLOGICALLY
     # BETTER ALTERNATIVE IN THE FUTURE
     #
@@ -373,15 +370,15 @@
         points		= np.array( ahull[0] )
         convex_hull	= ahull[1]
         if bPlottered :
             plt .plot ( points[:,0],points[:,1],'o' )
         hull_border  = [ [ *points[convex_hull.vertices,i], points[convex_hull.vertices[0],i] ] for i in range(len(projection_crds)) ]
         convex_hull_center  = np.mean(points,0)
         all_convex_hulls[ gid_nr ] = { 'area':convex_hull.area , 'center':convex_hull_center , 'border':hull_border,
-					'info' : 'scipy spatial ConvexHull : ' + qhull_options if not qhull_options is None else 'default settings' }
+					    'info' : 'scipy spatial ConvexHull : ' + qhull_options if not qhull_options is None else 'default settings' }
         if bPlottered :
             plt.plot ( hull_border[0] , hull_border[1] , 'r-')
             plt.plot ( convex_hull_center[0] , convex_hull_center[1] , '*k' )
     if bPlottered :
         plt .show()
     return ( all_convex_hulls )
 
@@ -445,15 +442,15 @@
     #
     for item in all_convex_hulls.items() :
         crds = item[1]['border']
         M    = len(crds[0])
         crds = np.array(crds).reshape(-1)
         crds = [ [ crds[k*M+i] for k in range(DIM) ] for i in range(M) ]
         for crd in crds :
-            file_info += sep.join([ str(item[0]) , '1' , '1' ,'primary' , *[str(c) for c in crd] , '1' , '1' ,   str(item[0])+'_1_1' ]) + '\n'
+            file_info += sep.join([ str(int(float(item[0]))) , '1' , '1' ,'primary' , *[str(c) for c in crd] , '1' , '1' ,   str(int(float(item[0])))+'_1_1' ]) + '\n'
     return ( file_info )
 
 
 def create_directory ( directory_path:str ) :
     import os
     drsp = directory_path.split('/')
     for i in range( len(drsp) ) :
@@ -477,37 +474,40 @@
 
 def generate_atlas_files ( header_str:str ,
                 fcfile:str = 'clustering/final_consensus.tsv' ,
 		nnfile:str = 'distance/nearest_neighbors.tsv' ,
                 umfile:str = 'UMAP/UMAP.tsv' ,
                 ccfile:str = 'UMAP/cluster_centers.tsv' ,
 		pofile:str = 'UMAP/UMAP_polygons.tsv' ,
+                anfile:str = 'enrichment/cluster_annotations.tsv',
                 pcadir:str = 'PCA/',
                 evadir:str = 'evaluation/',
                 nNN:int=20 ,
                 additional_directories:list[str] = ['data','enrichment','evaluation','graph','PCA','UMAP',
 					'svg'  , 'svg/heatmap','svg/bubble','svg/treemap','svg/fountain',
                                         'html' , 'html']) :
     #
     # START ATLAS GEN
     sep = '\t'
     #
     hdir_str = header_str
     if hdir_str[-1] == '_' :
         hdir_str =  hdir_str[:-1] + '/'
+    elif  hdir_str[-1] != '/' :
+        hdir_str += '/'
     #
     df_sol_     = pd.read_csv( header_str + 'resdf_f.tsv' , sep=sep , index_col=0 ) # SHOULD BE ASSERTED
     df_pca_     = pd.read_csv( header_str + 'pcas_df.tsv' , sep=sep , index_col=0 ) # SHOULD BE ASSERTED
     df_pca_s    = pd.read_csv( header_str + 'pcaw_df.tsv' , sep=sep , index_col=0 ) # SHOULD BE ASSERTED
     if 'str' in str(type(pcadir)) :
         if pcadir[-1] != '/' :
             pcadir += '/'
         create_directory ( hdir_str + pcadir )
         df_pca_ .to_csv( hdir_str + pcadir + 'pca_analytes_df.tsv' )
-        df_pca_s.to_csv( hdir_str + pcadir +  'pca_samples_df.tsv' )
+        df_pca_s.to_csv( hdir_str + pcadir + 'pca_samples_df.tsv'  )
     #
     if 'str' in str(type(evadir)) :
         if evadir[-1] != '/' :
             evadir += '/'
         create_directory ( hdir_str + evadir )
         e1df = pd.read_csv( header_str + 'soldf_f.tsv' , sep=sep , index_col=0 )
         e1df .to_csv( hdir_str + evadir + 'solution_analytes.tsv' ,sep=sep )
@@ -536,14 +536,15 @@
     final_consensus_df = df_sol_.loc[:,['cids.max']].rename(columns={'cids.max':'cluster'}).copy()
     final_consensus_df .index.name = 'gene'
     final_consensus_df .to_csv( hdir_str + fcfile, sep=sep )
     #
     create_directory ( hdir_str + '/'.join( umfile.split('/')[:-1]) )
     udf = df.loc[:,[c for c in df.columns if 'UMAP' in c ] ]
     udf .columns = [ c.replace('.','_') for c in udf.columns ]
+    udf = udf .rename( columns={'UMAP_0_scaled':'UMAP_1_scaled','UMAP_1_scaled':'UMAP_2_scaled'} )
     udf .to_csv( hdir_str + umfile, sep=sep )
     #
     create_directory ( hdir_str + '/'.join( ccfile.split('/')[:-1]) )
     ccinfo = cluster_center_information( all_hulls )
     o_f = open( hdir_str + ccfile,'w')
     print ( ccinfo , file=o_f )
     o_f .close()
@@ -564,23 +565,26 @@
         create_directory ( hdir_str + dir )
     #
     # CHECK FOR ENRICHMENTS
     hdr_dir   = '/'.join( header_str.split('/')[:-1] )
     id_tag    = header_str.split('/')[-1]
     import os
     enr_files = [ l for l in set(os.listdir(hdr_dir)) if id_tag in l and ('treemap' in l or 'GFA' in l or 'enrichment' in l ) ]
-    if len(enr_files) > 0 :
+    if len( enr_files ) > 0 :
         for f in enr_files :
             os.system('cp ' + hdr_dir + '/' + f + ' ' +  hdir_str + 'enrichment/' + f )
+    from biocartograph.enrichment import auto_annotate_clusters
+    an_df	= auto_annotate_clusters ( header_str )
+    create_directory ( hdir_str + '/'.join( anfile.split('/')[:-1]) )
+    an_df	.to_csv( hdir_str + anfile , sep='\t' )
 
-
-if __name__ == '__main__':
+if __name__ == '__main__' :
     #
-    reformat_results_and_print_gmtfile_pcfile(header_str = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' )
-    reformat_results_and_print_gmtfile_pcfile(header_str = '../results/DMHMSY_Fri_Mar_17_16_00_47_2023_' )
+    reformat_results_and_print_gmtfile_pcfile( header_str = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' )
+    reformat_results_and_print_gmtfile_pcfile( header_str = '../results/DMHMSY_Fri_Mar_17_16_00_47_2023_' )
     #
     results_dir = '../results/'
     header_str  = results_dir + 'DMHMSY_Wed_May__3_11_48_58_2023_'
     #
     generate_atlas_files ( header_str = header_str )
     """ ,
                 nnfile = 'distance/nearest_neighbors.tsv' ,
```

