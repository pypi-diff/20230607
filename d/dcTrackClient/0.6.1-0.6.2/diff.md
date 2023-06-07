# Comparing `tmp/dctrackclient-0.6.1.tar.gz` & `tmp/dctrackclient-0.6.2.tar.gz`

## Comparing `dctrackclient-0.6.1.tar` & `dctrackclient-0.6.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    14469 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/.gitignore
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    17764 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/../README.md
--rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    16849 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    19970 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/../README.md
+-rw-r--r--   0        0        0    20592 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/PKG-INFO
```

### Comparing `dctrackclient-0.6.1/src/dcTrackClient/__init__.py` & `dctrackclient-0.6.2/src/dcTrackClient/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -172,7 +172,39 @@
     def searchLocations(self, pageNumber: int, pageSize: int, payload: dict):
         """Search for Locations by user supplied search criteria. Returns a list of Locations with the "selectedColumns" returned in the payload."""
         return self.__request('POST', '/api/v2/quicksearch/locations/?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize) + '&', payload)
 
     def getLocationFieldList(self):
         """Returns a list of all Location fields."""
         return self.__request('GET', '/api/v2/quicksearch/locations/locationListFields/?')
+
+    def getSublocationTree(self):
+        """Get the sublocation tree."""
+        return self.__request('GET', '/api/v2/subLocations/tree/?')
+
+    def getSublocations(self, locationId: int):
+        """Get all sub-locations for a given location in the hierarchy. The locationId is the ID of the location to get the sub-locations for."""
+        return self.__request('GET', '/api/v2/subLocations/list/' + str(locationId) + '/?')
+
+    def getSublocationsOfType(self, locationId: int, typeCode: str):
+        """Get all sub-locations of given type for a given location in the hierarchy. The locationId is the id of the location you are querying the sub-location types for. The type is one of either 5016 and 5017 for rows and aisles respectively."""
+        return self.__request('GET', '/api/v2/subLocations/' + str(locationId) + '/type/' + str(typeCode) + '/?')
+
+    def getChildSublocations(self, subLocationId: int):
+        """Get all child sub-locations for a given sub-location in the hierarchy. The locationId is the ID of the location to fetch the sub-locations for. The subLocationId is the ID of the parent sub-location that you are querying the children of."""
+        return self.__request('GET', '/api/v2/subLocations/' + str(subLocationId) + '/children/?')
+
+    def getSublocation(self, subLocationId: int):
+        """Get details for a given sub-location. The subLocationId is the id of the sub-location you are querying for."""
+        return self.__request('GET', '/api/v2/subLocations/' + str(subLocationId) + '/?')
+
+    def createSublocation(self, payload: dict):
+        """Add a new sub-location to the given location. Returns a list from the Sub-Location Hash."""
+        return self.__request('POST', '/api/v2/subLocations/?', payload)
+
+    def updateSublocation(self, subLocationId: int, payload: dict):
+        """Update a sub-location. Returns a list from the Sub-Location Hash."""
+        return self.__request('PUT', '/api/v2/subLocations/' + str(subLocationId) + '/?', payload)
+
+    def deleteSublocation(self, subLocationId: int):
+        """Deletes the given sub-location. The locationId is the ID of the location that the sub-location belongs to and the subLocationId is the ID of the location you are querying. Returns a success message upon success."""
+        return self.__request('DELETE', '/api/v2/subLocations/' + str(subLocationId) + '/?')
```

### Comparing `dctrackclient-0.6.1/pyproject.toml` & `dctrackclient-0.6.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.6.1/../README.md` & `dctrackclient-0.6.2/../README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.6.1
+pip install dcTrackClient==0.6.2
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.6.1
+npm i dctrackclient@0.6.2
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -570,7 +570,79 @@
 
 ## getLocationFieldList()
 > Returns a list of all Location fields.
 ```
 GET api/v2/quicksearch/locations/locationListFields
 ```
 *No parameters.*
+
+## getSublocationTree()
+> Get the sublocation tree.
+```
+GET api/v2/subLocations/tree
+```
+*No parameters.*
+
+## getSublocations(locationId)
+> Get all sub-locations for a given location in the hierarchy. The locationId is the ID of the location to get the sub-locations for.
+```
+GET api/v2/subLocations/list/{locationId}
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+
+## getSublocationsOfType(locationId, typeCode)
+> Get all sub-locations of given type for a given location in the hierarchy. The locationId is the id of the location you are querying the sub-location types for. The type is one of either 5016 and 5017 for rows and aisles respectively.
+```
+GET api/v2/subLocations/{locationId}/type/{typeCode}
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+|typeCode|string|
+
+## getChildSublocations(subLocationId)
+> Get all child sub-locations for a given sub-location in the hierarchy. The locationId is the ID of the location to fetch the sub-locations for. The subLocationId is the ID of the parent sub-location that you are querying the children of.
+```
+GET api/v2/subLocations/{subLocationId}/children
+```
+|Parameter|Type|
+|---|---|
+|subLocationId|number|
+
+## getSublocation(subLocationId)
+> Get details for a given sub-location. The subLocationId is the id of the sub-location you are querying for.
+```
+GET api/v2/subLocations/{subLocationId}
+```
+|Parameter|Type|
+|---|---|
+|subLocationId|number|
+
+## createSublocation(payload)
+> Add a new sub-location to the given location. Returns a list from the Sub-Location Hash.
+```
+POST api/v2/subLocations payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## updateSublocation(subLocationId, payload)
+> Update a sub-location. Returns a list from the Sub-Location Hash.
+```
+PUT api/v2/subLocations/{subLocationId} payload
+```
+|Parameter|Type|
+|---|---|
+|subLocationId|number|
+|payload|object|
+
+## deleteSublocation(subLocationId)
+> Deletes the given sub-location. The locationId is the ID of the location that the sub-location belongs to and the subLocationId is the ID of the location you are querying. Returns a success message upon success.
+```
+DELETE api/v2/subLocations/{subLocationId}
+```
+|Parameter|Type|
+|---|---|
+|subLocationId|number|
```

### Comparing `dctrackclient-0.6.1/PKG-INFO` & `dctrackclient-0.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.6.1
+Version: 0.6.2
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,20 +20,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.6.1
+pip install dcTrackClient==0.6.2
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.6.1
+npm i dctrackclient@0.6.2
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -586,7 +586,79 @@
 
 ## getLocationFieldList()
 > Returns a list of all Location fields.
 ```
 GET api/v2/quicksearch/locations/locationListFields
 ```
 *No parameters.*
+
+## getSublocationTree()
+> Get the sublocation tree.
+```
+GET api/v2/subLocations/tree
+```
+*No parameters.*
+
+## getSublocations(locationId)
+> Get all sub-locations for a given location in the hierarchy. The locationId is the ID of the location to get the sub-locations for.
+```
+GET api/v2/subLocations/list/{locationId}
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+
+## getSublocationsOfType(locationId, typeCode)
+> Get all sub-locations of given type for a given location in the hierarchy. The locationId is the id of the location you are querying the sub-location types for. The type is one of either 5016 and 5017 for rows and aisles respectively.
+```
+GET api/v2/subLocations/{locationId}/type/{typeCode}
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+|typeCode|string|
+
+## getChildSublocations(subLocationId)
+> Get all child sub-locations for a given sub-location in the hierarchy. The locationId is the ID of the location to fetch the sub-locations for. The subLocationId is the ID of the parent sub-location that you are querying the children of.
+```
+GET api/v2/subLocations/{subLocationId}/children
+```
+|Parameter|Type|
+|---|---|
+|subLocationId|number|
+
+## getSublocation(subLocationId)
+> Get details for a given sub-location. The subLocationId is the id of the sub-location you are querying for.
+```
+GET api/v2/subLocations/{subLocationId}
+```
+|Parameter|Type|
+|---|---|
+|subLocationId|number|
+
+## createSublocation(payload)
+> Add a new sub-location to the given location. Returns a list from the Sub-Location Hash.
+```
+POST api/v2/subLocations payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## updateSublocation(subLocationId, payload)
+> Update a sub-location. Returns a list from the Sub-Location Hash.
+```
+PUT api/v2/subLocations/{subLocationId} payload
+```
+|Parameter|Type|
+|---|---|
+|subLocationId|number|
+|payload|object|
+
+## deleteSublocation(subLocationId)
+> Deletes the given sub-location. The locationId is the ID of the location that the sub-location belongs to and the subLocationId is the ID of the location you are querying. Returns a success message upon success.
+```
+DELETE api/v2/subLocations/{subLocationId}
+```
+|Parameter|Type|
+|---|---|
+|subLocationId|number|
```

