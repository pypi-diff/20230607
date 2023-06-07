# Comparing `tmp/wikibaseintegrator-0.8.2.tar.gz` & `tmp/wikibaseintegrator-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wikibaseintegrator-0.8.2.tar", last modified: Fri Aug  7 22:07:04 2020, max compression
+gzip compressed data, was "dist/wikibaseintegrator-0.9.0.tar", last modified: Fri Oct  9 17:35:05 2020, max compression
```

## Comparing `wikibaseintegrator-0.8.2.tar` & `wikibaseintegrator-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (116)    17921 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    14737 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      277 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1315 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/
--rw-r--r--   0 runner    (1001) docker     (116)      259 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1563 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_backoff.py
--rw-r--r--   0 runner    (1001) docker     (116)     9380 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_fastrun.py
--rw-r--r--   0 runner    (1001) docker     (116)     1916 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_item_creation.py
--rw-r--r--   0 runner    (1001) docker     (116)      513 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_item_generator.py
--rw-r--r--   0 runner    (1001) docker     (116)      367 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_wd_search.py
--rw-r--r--   0 runner    (1001) docker     (116)      415 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_wdi_login.py
--rw-r--r--   0 runner    (1001) docker     (116)     7934 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (116)     1314 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_backoff.py
--rw-r--r--   0 runner    (1001) docker     (116)     1450 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_config.py
--rw-r--r--   0 runner    (1001) docker     (116)   145783 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_core.py
--rw-r--r--   0 runner    (1001) docker     (116)    25719 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_fastrun.py
--rw-r--r--   0 runner    (1001) docker     (116)     8688 2020-08-07 22:07:03.000000 wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_login.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/wikibaseintegrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    17921 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/wikibaseintegrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      766 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/wikibaseintegrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/wikibaseintegrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      120 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/wikibaseintegrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2020-08-07 22:07:04.000000 wikibaseintegrator-0.8.2/wikibaseintegrator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-09 17:35:05.000000 wikibaseintegrator-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)    17752 2020-10-09 17:35:05.000000 wikibaseintegrator-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    14588 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      277 2020-10-09 17:35:05.000000 wikibaseintegrator-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1225 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-09 17:35:05.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/
+-rw-r--r--   0 runner    (1001) docker     (116)      260 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-09 17:35:05.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7995 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1618 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9392 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_fastrun.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1945 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_item_creation.py
+-rw-r--r--   0 runner    (1001) docker     (116)      513 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_item_generator.py
+-rw-r--r--   0 runner    (1001) docker     (116)      367 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_wd_search.py
+-rw-r--r--   0 runner    (1001) docker     (116)      407 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_wdi_login.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1314 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1421 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)   135340 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_core.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28527 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_fastrun.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8741 2020-10-09 17:34:57.000000 wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_login.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-09 17:35:05.000000 wikibaseintegrator-0.9.0/wikibaseintegrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    17752 2020-10-09 17:35:04.000000 wikibaseintegrator-0.9.0/wikibaseintegrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      769 2020-10-09 17:35:05.000000 wikibaseintegrator-0.9.0/wikibaseintegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-09 17:35:04.000000 wikibaseintegrator-0.9.0/wikibaseintegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       57 2020-10-09 17:35:04.000000 wikibaseintegrator-0.9.0/wikibaseintegrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2020-10-09 17:35:04.000000 wikibaseintegrator-0.9.0/wikibaseintegrator.egg-info/top_level.txt
```

### Comparing `wikibaseintegrator-0.8.2/PKG-INFO` & `wikibaseintegrator-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: wikibaseintegrator
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python package for reading and writing to/from Wikibase
-Home-page: https://github.com/Mystou/WikibaseIntegrator
+Home-page: https://github.com/LeMyst/WikibaseIntegrator
 Author: Myst and WikidataIntegrator authors
 License: MIT
 Description: # Wikibase Integrator #
-        [![Build Status](https://travis-ci.org/Mystou/WikibaseIntegrator.svg?branch=master)](https://travis-ci.org/Mystou/WikibaseIntegrator)
+        [![Build Status](https://travis-ci.org/LeMyst/WikibaseIntegrator.svg?branch=master)](https://travis-ci.org/LeMyst/WikibaseIntegrator)
         [![Pyversions](https://img.shields.io/pypi/pyversions/wikibaseintegrator.svg)](https://pypi.python.org/pypi/wikibaseintegrator)
         [![PyPi](https://img.shields.io/pypi/v/wikibaseintegrator.svg)](https://pypi.python.org/pypi/wikibaseintegrator)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Mystou/WikibaseIntegrator/master)
         
         # WikibaseIntegrator / WikidataIntegrator #
-        WikibaseIntegrator (wbi) is a fork from [WikidataIntegrator](https://github.com/SuLab/WikidataIntegrator) (wdi) whose purpose is to be focused on Wikibase only.
+        WikibaseIntegrator (wbi) is a fork from [WikidataIntegrator](https://github.com/SuLab/WikidataIntegrator) (wdi) whose purpose is to be focused on Wikibase compatibility.
         The main changes are :
         * Rename the files from wdi_ to wbi_ to avoid confusion
         * Removal of wdi_helpers from the repository
         * Removal of references handlers from the repository, but they can still be used with the ItemEngine
         
         Wikidata is always the default endpoint for all functions.
         
@@ -48,27 +47,31 @@
           * WDTabularData -> TabularData
           * WDTime -> Time
           * WDUrl -> Url
         * ItemEngine parameter changes:
           * wd_item_id -> item_id
         * ItemEngine attribute changes:
           * wd_item_id -> item_id
+        * Change wbi_core.set_aliases parameter named 'append' to 'if_exists' with a value of APPEND (default) or REPLACE
+        * Remove CONCEPT_BASE_URI wbi_config option and classes' parameter. It's now derived from WIKIBASE_URL.
+        * wbi_core.log() has been removed. Please use your own logging implementation.
         
         # Installation #
-        The easiest way to install WikibaseIntegrator is using `pip` or `pip3`. WikibaseIntegrator supports python 3.6 and higher, hence the suggestion for pip3. If python2 is installed pip will lead to an error indicating missing dependencies. 
+        The easiest way to install WikibaseIntegrator is using `pip` or `pip3`.
+        WikibaseIntegrator supports python 3.6 and higher, hence the suggestion for pip3.
+        If python2 is installed pip will lead to an error indicating missing dependencies. 
         
-        ```
+        ```bash
         pip3 install wikibaseintegrator
         ```
         
         You can also clone the repo and execute with administrator rights or install into a virtualenv.
         
         ```bash
-        
-        git clone https://github.com/Mystou/WikibaseIntegrator.git
+        git clone https://github.com/LeMyst/WikibaseIntegrator.git
         
         cd WikibaseIntegrator
         
         python3 setup.py install
         ```
         
         To test for correct installation, start a python console and execute the following (Will retrieve the Wikidata item for ['Human'](https://www.wikidata.org/entity/Q5)):
@@ -80,69 +83,68 @@
         
         # to check successful installation and retrieval of the data, you can print the json representation of the item
         print(my_first_wikidata_item.get_json_representation())
         ```
         
         # The Core Parts #
         
-        wbi_core supports two modes it can be operated in, a normal mode, updating each item at a time and a 'fastrun' mode, which is pre-loading data locally and then just updating items if the new data provided is differing from what is in Wikidata. The latter mode allows for great speedups (measured up to 9x) when tens of thousand of Wikidata 
-        items need to be checked if they require updates but only a small number will finally be updated, a situation usually encountered when keeping Wikidata in sync with an external resource. 
+        wbi_core supports two modes it can be operated in, a normal mode, updating each item at a time and a 'fastrun' mode, which is pre-loading data locally and then just updating items if the new data provided is differing from what is in Wikidata.
+        The latter mode allows for great speedups (measured up to 9x) when tens of thousand of Wikidata items need to be checked if they require updates but only a small number will finally be updated, a situation usually encountered when keeping Wikidata in sync with an external resource. 
         
         wbi_core consists of a central class called ItemEngine and Login for authenticating with Wikidata/Wikipedia.
         
         ## wbi_core.ItemEngine ##
         This is the central class which does all the heavy lifting.
         
         Features:
-        
-         * Load a Wikibase item based on data to be written (e.g. a unique central identifier)
-         * Load a Wikibase item based on its Wikibase item id (aka QID)
-         * Checks for conflicts automatically (e.g. multiple items carrying a unique central identifier will trigger an exception)
-         * Checks automatically if the correct item has been loaded by comparing it to the data provided
-         * All Wikibase data types implemented
-         * A dedicated ItemEngine.write() method allows loading and consistency checks of data before any write to Wikibase is performed
-         * Full access to the whole Wikibase item as a JSON document
-         * Minimize the number of HTTP requests for reads and writes to improve performance
-         * Method to easily execute [SPARQL](https://query.wikidata.org) queries on the Wikibase SPARQL endpoint. 
+        * Load a Wikibase item based on data to be written (e.g. a unique central identifier)
+        * Load a Wikibase item based on its Wikibase item id (aka QID)
+        * Checks for conflicts automatically (e.g. multiple items carrying a unique central identifier will trigger an exception)
+        * Checks automatically if the correct item has been loaded by comparing it to the data provided
+        * All Wikibase data types implemented
+        * A dedicated ItemEngine.write() method allows loading and consistency checks of data before any write to Wikibase is performed
+        * Full access to the whole Wikibase item as a JSON document
+        * Minimize the number of HTTP requests for reads and writes to improve performance
+        * Method to easily execute [SPARQL](https://query.wikidata.org) queries on the Wikibase SPARQL endpoint. 
          
         There are two ways of working with Wikibase items: 
-        
         * A user can provide data, and ItemEngine will search for and load/modify an existing item or create a new one, solely based on the data provided (preferred). This also performs consistency checks based on a set of SPARQL queries. 
         * A user can work with a selected QID to specifically modify the data on the item. This requires that the user knows what he/she is doing and should only be used with great care, as this does not perform consistency checks. 
         
         Examples below illustrate the usage of ItemEngine.
         
         ## wbi_login.Login ##
         
         ### Login with username and password ###
         wbi_login.Login provides the login functionality and also stores the cookies and edit tokens required (For security reasons, every Mediawiki edit requires an edit token).
         The constructor takes two essential parameters, username and password. Additionally, the server (default wikidata.org) and the the token renewal periods can be specified. 
         
-        ```Python     
+        ```python
+        from wikibaseintegrator import wbi_login
+        
         login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')     
         ```
         
         ### Login using OAuth1 ###
-        The Wikimedia universe currently only support authentication via OAuth1. If WBI should be used as a backend for a webapp or the bot should use OAuth for authentication, WBI supports this
-        You just need to specify consumer token and consumer secret when instantiating wbi_login.Login. In contrast to username and password login, OAuth is a 2 step process as manual user confirmation
-        for OAuth login is required. This means that the method continue_oath() needs to be called after creating the wbi_login.Login instance.
+        The Wikimedia universe currently only support authentication via OAuth1. If WBI should be used as a backend for a webapp or the bot should use OAuth for authentication, WBI supports this, you just need to specify consumer key and consumer secret when instantiating wbi_login.Login.
+        In contrast to username and password login, OAuth is a 2 step process as manual user confirmation for OAuth login is required. This means that the method continue_oauth() needs to be called after creating the wbi_login.Login instance.
         
         Example:
-        ```Python     
-        login_instance = wbi_login.Login(consumer_token='<your_consumer_token>', pwd='<your_consumer_secret>')
+        ```python
+        from wikibaseintegrator import wbi_login
+        
+        login_instance = wbi_login.Login(consumer_key='<your_consumer_key>', consumer_secret='<your_consumer_secret>')
         login_instance.continue_oauth()
         ```
         
-        The method continue_oauth() will either promt the user for a callback URL (normal bot runs) or it will take a parameter so in the case of WBI being
-        used as a backend for e.g. a web app, where the callback will provide the authentication information directly to the backend and so
-         no copy and paste of the callback URL is required.
+        The method continue_oauth() will either prompt the user for a callback URL (normal bot runs) or it will take a parameter so in the case of WBI being used as a backend for e.g. a web app, where the callback will provide the authentication information directly to the backend and so no copy and paste of the callback URL is required.
         
         ## Wikibase Data Types ##
-        Currently, Wikibase supports 17 different data types. The data types are represented as their own classes in wbi_core. Each data type has its specialties, which means that some of them
-        require special parameters (e.g. Globe Coordinates).
+        Currently, Wikibase supports 17 different data types. The data types are represented as their own classes in wbi_core.
+        Each data type has its specialties, which means that some of them require special parameters (e.g. Globe Coordinates).
         
         The data types currently implemented:
         * wbi_core.CommonsMedia
         * wbi_core.ExternalID
         * wbi_core.Form
         * wbi_core.GeoShape
         * wbi_core.GlobeCoordinate
@@ -155,57 +157,49 @@
         * wbi_core.Quantity
         * wbi_core.Sense
         * wbi_core.String
         * wbi_core.TabularData
         * wbi_core.Time
         * wbi_core.Url
         
-        For details of how to create values (=instances) with these data types, please (for now) consult the docstrings in the source code. Of note, these data type instances hold the values and, if specified,
-        data type instances for references and qualifiers. Furthermore, calling the get_value() method of an instance returns either an integer, a string or a tuple, depending on the complexity of the data type.
+        For details of how to create values (=instances) with these data types, please (for now) consult the docstrings in the source code.
+        Of note, these data type instances hold the values and, if specified, data type instances for references and qualifiers.
+        Furthermore, calling the get_value() method of an instance returns either an integer, a string or a tuple, depending on the complexity of the data type.
         
         # Helper Methods #
         
         ## Execute SPARQL queries ##
-        The method wbi_core.ItemEngine.execute_sparql_query() allows you to execute SPARQL queries without a hassle. It takes the actual
-        query string (query), optional prefixes (prefix) if you do not want to use the standard prefixes of Wikidata, the actual entpoint URL (endpoint),
-        and you can also specify a user agent for the http header sent to the SPARQL server (user_agent). The latter is very useful to let
-        the operators of the endpoint know who you are, especially if you execute many queries on the endpoint. This allows the operators of
-        the endpoint to contact you (e.g. specify a email address or the URL to your bot code repository.)
-        
-        ## Logging ##
-        The method wbi_core.ItemEngine.log() allows for using the Python built in logging functionality to collect errors and other logs.
-        It takes two parameters, the log level (level) and the log message (message). It is advisable to separate log file columns by colons
-        and always use the same number of fields, as this allows you to load the log file into databases or dataframes of R or Python.
+        The method wbi_core.ItemEngine.execute_sparql_query() allows you to execute SPARQL queries without a hassle.
+        It takes the actual query string (query), optional prefixes (prefix) if you do not want to use the standard prefixes of Wikidata, the actual entpoint URL (endpoint), and you can also specify a user agent for the http header sent to the SPARQL server (user_agent).
+        The latter is very useful to let the operators of the endpoint know who you are, especially if you execute many queries on the endpoint.
+        This allows the operators of the endpoint to contact you (e.g. specify a email address or the URL to your bot code repository.)
         
         ## Wikidata Search ##
-        The method wbi_core.ItemEngine.get_search_results() allows for string search in a Wikibase instance. This means that
-        labels, descriptions and aliases can be searched for a string of interest. The method takes five arguments:
-        The actual search string (search_string), an optional server (mediawiki_api_url, in case the Wikibase instance used is not Wikidata),
-        an optional user_agent, an optional max_results (default 500), an optional language (default 'en') and an option dict_id_label to return a dict of
-        item id and label as a result.
+        The method wbi_core.ItemEngine.get_search_results() allows for string search in a Wikibase instance.
+        This means that labels, descriptions and aliases can be searched for a string of interest.
+        The method takes five arguments: The actual search string (search_string), an optional server (mediawiki_api_url, in case the Wikibase instance used is not Wikidata), an optional user_agent, an optional max_results (default 500), an optional language (default 'en') and an option dict_id_label to return a dict of item id and label as a result.
          
         ## Merge Wikibase items ##
-        Sometimes, Wikibase items need to be merged. An API call exists for that, and wbi_core implements a method accordingly.
-        `wbi_core.ItemEngine.merge_items(from_id, to_id, login_obj)` takes five arguments: the QID of the item which should be
-        merged into another item (from_id), the QID of the item the first item should be
-        merged into (to_id), a login object of type wbi_login.Login() (login_obj) to provide the API call with the required authentication
-        information, a server (mediawiki_api_url) if the Wikibase instance is not Wikidata and a flag for ignoring merge conflicts (ignore_conflicts).
-        The last parameter will do a partial merge for all statements which do not conflict. This should generally be avoided because it 
-        leaves a crippled item in Wikibase. Before a merge, any potential conflicts should be resolved first.
+        Sometimes, Wikibase items need to be merged.
+        An API call exists for that, and wbi_core implements a method accordingly.
+        `wbi_core.ItemEngine.merge_items(from_id, to_id, login_obj)` takes five arguments:
+        the QID of the item which should be merged into another item (from_id), the QID of the item the first item should be merged into (to_id), a login object of type wbi_login.Login() to provide the API call with the required authentication information, a server (mediawiki_api_url) if the Wikibase instance is not Wikidata and a flag for ignoring merge conflicts (ignore_conflicts).
+        The last parameter will do a partial merge for all statements which do not conflict.
+        This should generally be avoided because it leaves a crippled item in Wikibase. Before a merge, any potential conflicts should be resolved first.
         
         # Examples (in normal mode) #
         
         ## A Minimal Bot ##
         In order to create a minimal bot based on wbi_core, three things are required:
         
         * A login object, as described above.
         * A data type object containing a value.
         * A ItemEngine object which takes the data, does the checks and performs the write.
         
-        ```Python
+        ```python
         from wikibaseintegrator import wbi_core, wbi_login
             
         # login object
         login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')
              
         # data type object, e.g. for a NCBI gene entrez ID
         entrez_gene_id = wbi_core.String(value='<some_entrez_id>', prop_nr='P351')
@@ -217,15 +211,15 @@
         wd_item = wbi_core.ItemEngine(data=data)
         wd_item.write(login_instance)
         ```
         
         ## A Minimal Bot for Mass Import ##
         An enhanced example of the previous bot just puts two of the three things into a for loop and so allows mass creation, or modification of items.
         
-        ```Python
+        ```python
         from wikibaseintegrator import wbi_core, wbi_login
             
         # login object
         login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')
         
         # We have raw data, which should be written to Wikidata, namely two human NCBI entrez gene IDs mapped to two Ensembl Gene IDs
         raw_data = {
@@ -253,20 +247,20 @@
         
         IMPORTANT: In order for the fast run mode to work, the data you provide in the constructor must contain at least one unique value/id only present on one Wikidata item, e.g. an NCBI entrez gene ID, Uniprot ID, etc.
         Usually, these would be the same unique core properties used for defining domains in wbi_core, e.g. for genes, proteins, drugs or your custom domains.
         
         Below, the normal mode run example from above, slightly modified, to meet the requirements for the fastrun mode. To enable it, ItemEngine requires two parameters, fast_run=True/False and fast_run_base_filter which 
          is a dictionary holding the properties to filter for as keys and the item QIDs as dict values. If the value is not a QID but a literal, just provide an empty string. For the above example, the dictionary looks like this:
          
-        ```Python
+        ```python
         fast_run_base_filter = {'P351': '', 'P703': 'Q15978631'}
         ```
          
         The full example:
-        ```Python
+        ```python
         from wikibaseintegrator import wbi_core, wbi_login
             
         # login object
         login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')
         
         fast_run_base_filter = {'P351': '', 'P703': 'Q15978631'}
         fast_run = True
@@ -287,15 +281,16 @@
             data = [entrez_gene_id, ensembl_transcript_id]
             
             # Search for and then edit/create new item
             wd_item = wbi_core.ItemEngine(data=data, fast_run=fast_run, fast_run_base_filter=fast_run_base_filter)
             wd_item.write(login_instance)
         ```
         
-        Note: Fastrun mode checks for equality of property/value pairs, qualifers (not including qualifier attributes), labels, aliases and description, but it ignores references by default! References can be checked in fastrun mode by setting `fast_run_use_refs` to `True`.
+        Note: Fastrun mode checks for equality of property/value pairs, qualifers (not including qualifier attributes), labels, aliases and description, but it ignores references by default!
+        References can be checked in fastrun mode by setting `fast_run_use_refs` to `True`.
         
 Keywords: Wikibase
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -304,7 +299,8 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `wikibaseintegrator-0.8.2/README.md` & `wikibaseintegrator-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Wikibase Integrator #
-[![Build Status](https://travis-ci.org/Mystou/WikibaseIntegrator.svg?branch=master)](https://travis-ci.org/Mystou/WikibaseIntegrator)
+[![Build Status](https://travis-ci.org/LeMyst/WikibaseIntegrator.svg?branch=master)](https://travis-ci.org/LeMyst/WikibaseIntegrator)
 [![Pyversions](https://img.shields.io/pypi/pyversions/wikibaseintegrator.svg)](https://pypi.python.org/pypi/wikibaseintegrator)
 [![PyPi](https://img.shields.io/pypi/v/wikibaseintegrator.svg)](https://pypi.python.org/pypi/wikibaseintegrator)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Mystou/WikibaseIntegrator/master)
 
 # WikibaseIntegrator / WikidataIntegrator #
-WikibaseIntegrator (wbi) is a fork from [WikidataIntegrator](https://github.com/SuLab/WikidataIntegrator) (wdi) whose purpose is to be focused on Wikibase only.
+WikibaseIntegrator (wbi) is a fork from [WikidataIntegrator](https://github.com/SuLab/WikidataIntegrator) (wdi) whose purpose is to be focused on Wikibase compatibility.
 The main changes are :
 * Rename the files from wdi_ to wbi_ to avoid confusion
 * Removal of wdi_helpers from the repository
 * Removal of references handlers from the repository, but they can still be used with the ItemEngine
 
 Wikidata is always the default endpoint for all functions.
 
@@ -41,27 +40,31 @@
   * WDTabularData -> TabularData
   * WDTime -> Time
   * WDUrl -> Url
 * ItemEngine parameter changes:
   * wd_item_id -> item_id
 * ItemEngine attribute changes:
   * wd_item_id -> item_id
+* Change wbi_core.set_aliases parameter named 'append' to 'if_exists' with a value of APPEND (default) or REPLACE
+* Remove CONCEPT_BASE_URI wbi_config option and classes' parameter. It's now derived from WIKIBASE_URL.
+* wbi_core.log() has been removed. Please use your own logging implementation.
 
 # Installation #
-The easiest way to install WikibaseIntegrator is using `pip` or `pip3`. WikibaseIntegrator supports python 3.6 and higher, hence the suggestion for pip3. If python2 is installed pip will lead to an error indicating missing dependencies. 
+The easiest way to install WikibaseIntegrator is using `pip` or `pip3`.
+WikibaseIntegrator supports python 3.6 and higher, hence the suggestion for pip3.
+If python2 is installed pip will lead to an error indicating missing dependencies. 
 
-```
+```bash
 pip3 install wikibaseintegrator
 ```
 
 You can also clone the repo and execute with administrator rights or install into a virtualenv.
 
 ```bash
-
-git clone https://github.com/Mystou/WikibaseIntegrator.git
+git clone https://github.com/LeMyst/WikibaseIntegrator.git
 
 cd WikibaseIntegrator
 
 python3 setup.py install
 ```
 
 To test for correct installation, start a python console and execute the following (Will retrieve the Wikidata item for ['Human'](https://www.wikidata.org/entity/Q5)):
@@ -73,69 +76,68 @@
 
 # to check successful installation and retrieval of the data, you can print the json representation of the item
 print(my_first_wikidata_item.get_json_representation())
 ```
 
 # The Core Parts #
 
-wbi_core supports two modes it can be operated in, a normal mode, updating each item at a time and a 'fastrun' mode, which is pre-loading data locally and then just updating items if the new data provided is differing from what is in Wikidata. The latter mode allows for great speedups (measured up to 9x) when tens of thousand of Wikidata 
-items need to be checked if they require updates but only a small number will finally be updated, a situation usually encountered when keeping Wikidata in sync with an external resource. 
+wbi_core supports two modes it can be operated in, a normal mode, updating each item at a time and a 'fastrun' mode, which is pre-loading data locally and then just updating items if the new data provided is differing from what is in Wikidata.
+The latter mode allows for great speedups (measured up to 9x) when tens of thousand of Wikidata items need to be checked if they require updates but only a small number will finally be updated, a situation usually encountered when keeping Wikidata in sync with an external resource. 
 
 wbi_core consists of a central class called ItemEngine and Login for authenticating with Wikidata/Wikipedia.
 
 ## wbi_core.ItemEngine ##
 This is the central class which does all the heavy lifting.
 
 Features:
-
- * Load a Wikibase item based on data to be written (e.g. a unique central identifier)
- * Load a Wikibase item based on its Wikibase item id (aka QID)
- * Checks for conflicts automatically (e.g. multiple items carrying a unique central identifier will trigger an exception)
- * Checks automatically if the correct item has been loaded by comparing it to the data provided
- * All Wikibase data types implemented
- * A dedicated ItemEngine.write() method allows loading and consistency checks of data before any write to Wikibase is performed
- * Full access to the whole Wikibase item as a JSON document
- * Minimize the number of HTTP requests for reads and writes to improve performance
- * Method to easily execute [SPARQL](https://query.wikidata.org) queries on the Wikibase SPARQL endpoint. 
+* Load a Wikibase item based on data to be written (e.g. a unique central identifier)
+* Load a Wikibase item based on its Wikibase item id (aka QID)
+* Checks for conflicts automatically (e.g. multiple items carrying a unique central identifier will trigger an exception)
+* Checks automatically if the correct item has been loaded by comparing it to the data provided
+* All Wikibase data types implemented
+* A dedicated ItemEngine.write() method allows loading and consistency checks of data before any write to Wikibase is performed
+* Full access to the whole Wikibase item as a JSON document
+* Minimize the number of HTTP requests for reads and writes to improve performance
+* Method to easily execute [SPARQL](https://query.wikidata.org) queries on the Wikibase SPARQL endpoint. 
  
 There are two ways of working with Wikibase items: 
-
 * A user can provide data, and ItemEngine will search for and load/modify an existing item or create a new one, solely based on the data provided (preferred). This also performs consistency checks based on a set of SPARQL queries. 
 * A user can work with a selected QID to specifically modify the data on the item. This requires that the user knows what he/she is doing and should only be used with great care, as this does not perform consistency checks. 
 
 Examples below illustrate the usage of ItemEngine.
 
 ## wbi_login.Login ##
 
 ### Login with username and password ###
 wbi_login.Login provides the login functionality and also stores the cookies and edit tokens required (For security reasons, every Mediawiki edit requires an edit token).
 The constructor takes two essential parameters, username and password. Additionally, the server (default wikidata.org) and the the token renewal periods can be specified. 
 
-```Python     
+```python
+from wikibaseintegrator import wbi_login
+
 login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')     
 ```
 
 ### Login using OAuth1 ###
-The Wikimedia universe currently only support authentication via OAuth1. If WBI should be used as a backend for a webapp or the bot should use OAuth for authentication, WBI supports this
-You just need to specify consumer token and consumer secret when instantiating wbi_login.Login. In contrast to username and password login, OAuth is a 2 step process as manual user confirmation
-for OAuth login is required. This means that the method continue_oath() needs to be called after creating the wbi_login.Login instance.
+The Wikimedia universe currently only support authentication via OAuth1. If WBI should be used as a backend for a webapp or the bot should use OAuth for authentication, WBI supports this, you just need to specify consumer key and consumer secret when instantiating wbi_login.Login.
+In contrast to username and password login, OAuth is a 2 step process as manual user confirmation for OAuth login is required. This means that the method continue_oauth() needs to be called after creating the wbi_login.Login instance.
 
 Example:
-```Python     
-login_instance = wbi_login.Login(consumer_token='<your_consumer_token>', pwd='<your_consumer_secret>')
+```python
+from wikibaseintegrator import wbi_login
+
+login_instance = wbi_login.Login(consumer_key='<your_consumer_key>', consumer_secret='<your_consumer_secret>')
 login_instance.continue_oauth()
 ```
 
-The method continue_oauth() will either promt the user for a callback URL (normal bot runs) or it will take a parameter so in the case of WBI being
-used as a backend for e.g. a web app, where the callback will provide the authentication information directly to the backend and so
- no copy and paste of the callback URL is required.
+The method continue_oauth() will either prompt the user for a callback URL (normal bot runs) or it will take a parameter so in the case of WBI being used as a backend for e.g. a web app, where the callback will provide the authentication information directly to the backend and so no copy and paste of the callback URL is required.
 
 ## Wikibase Data Types ##
-Currently, Wikibase supports 17 different data types. The data types are represented as their own classes in wbi_core. Each data type has its specialties, which means that some of them
-require special parameters (e.g. Globe Coordinates).
+Currently, Wikibase supports 17 different data types. The data types are represented as their own classes in wbi_core.
+Each data type has its specialties, which means that some of them require special parameters (e.g. Globe Coordinates).
 
 The data types currently implemented:
 * wbi_core.CommonsMedia
 * wbi_core.ExternalID
 * wbi_core.Form
 * wbi_core.GeoShape
 * wbi_core.GlobeCoordinate
@@ -148,57 +150,49 @@
 * wbi_core.Quantity
 * wbi_core.Sense
 * wbi_core.String
 * wbi_core.TabularData
 * wbi_core.Time
 * wbi_core.Url
 
-For details of how to create values (=instances) with these data types, please (for now) consult the docstrings in the source code. Of note, these data type instances hold the values and, if specified,
-data type instances for references and qualifiers. Furthermore, calling the get_value() method of an instance returns either an integer, a string or a tuple, depending on the complexity of the data type.
+For details of how to create values (=instances) with these data types, please (for now) consult the docstrings in the source code.
+Of note, these data type instances hold the values and, if specified, data type instances for references and qualifiers.
+Furthermore, calling the get_value() method of an instance returns either an integer, a string or a tuple, depending on the complexity of the data type.
 
 # Helper Methods #
 
 ## Execute SPARQL queries ##
-The method wbi_core.ItemEngine.execute_sparql_query() allows you to execute SPARQL queries without a hassle. It takes the actual
-query string (query), optional prefixes (prefix) if you do not want to use the standard prefixes of Wikidata, the actual entpoint URL (endpoint),
-and you can also specify a user agent for the http header sent to the SPARQL server (user_agent). The latter is very useful to let
-the operators of the endpoint know who you are, especially if you execute many queries on the endpoint. This allows the operators of
-the endpoint to contact you (e.g. specify a email address or the URL to your bot code repository.)
-
-## Logging ##
-The method wbi_core.ItemEngine.log() allows for using the Python built in logging functionality to collect errors and other logs.
-It takes two parameters, the log level (level) and the log message (message). It is advisable to separate log file columns by colons
-and always use the same number of fields, as this allows you to load the log file into databases or dataframes of R or Python.
+The method wbi_core.ItemEngine.execute_sparql_query() allows you to execute SPARQL queries without a hassle.
+It takes the actual query string (query), optional prefixes (prefix) if you do not want to use the standard prefixes of Wikidata, the actual entpoint URL (endpoint), and you can also specify a user agent for the http header sent to the SPARQL server (user_agent).
+The latter is very useful to let the operators of the endpoint know who you are, especially if you execute many queries on the endpoint.
+This allows the operators of the endpoint to contact you (e.g. specify a email address or the URL to your bot code repository.)
 
 ## Wikidata Search ##
-The method wbi_core.ItemEngine.get_search_results() allows for string search in a Wikibase instance. This means that
-labels, descriptions and aliases can be searched for a string of interest. The method takes five arguments:
-The actual search string (search_string), an optional server (mediawiki_api_url, in case the Wikibase instance used is not Wikidata),
-an optional user_agent, an optional max_results (default 500), an optional language (default 'en') and an option dict_id_label to return a dict of
-item id and label as a result.
+The method wbi_core.ItemEngine.get_search_results() allows for string search in a Wikibase instance.
+This means that labels, descriptions and aliases can be searched for a string of interest.
+The method takes five arguments: The actual search string (search_string), an optional server (mediawiki_api_url, in case the Wikibase instance used is not Wikidata), an optional user_agent, an optional max_results (default 500), an optional language (default 'en') and an option dict_id_label to return a dict of item id and label as a result.
  
 ## Merge Wikibase items ##
-Sometimes, Wikibase items need to be merged. An API call exists for that, and wbi_core implements a method accordingly.
-`wbi_core.ItemEngine.merge_items(from_id, to_id, login_obj)` takes five arguments: the QID of the item which should be
-merged into another item (from_id), the QID of the item the first item should be
-merged into (to_id), a login object of type wbi_login.Login() (login_obj) to provide the API call with the required authentication
-information, a server (mediawiki_api_url) if the Wikibase instance is not Wikidata and a flag for ignoring merge conflicts (ignore_conflicts).
-The last parameter will do a partial merge for all statements which do not conflict. This should generally be avoided because it 
-leaves a crippled item in Wikibase. Before a merge, any potential conflicts should be resolved first.
+Sometimes, Wikibase items need to be merged.
+An API call exists for that, and wbi_core implements a method accordingly.
+`wbi_core.ItemEngine.merge_items(from_id, to_id, login_obj)` takes five arguments:
+the QID of the item which should be merged into another item (from_id), the QID of the item the first item should be merged into (to_id), a login object of type wbi_login.Login() to provide the API call with the required authentication information, a server (mediawiki_api_url) if the Wikibase instance is not Wikidata and a flag for ignoring merge conflicts (ignore_conflicts).
+The last parameter will do a partial merge for all statements which do not conflict.
+This should generally be avoided because it leaves a crippled item in Wikibase. Before a merge, any potential conflicts should be resolved first.
 
 # Examples (in normal mode) #
 
 ## A Minimal Bot ##
 In order to create a minimal bot based on wbi_core, three things are required:
 
 * A login object, as described above.
 * A data type object containing a value.
 * A ItemEngine object which takes the data, does the checks and performs the write.
 
-```Python
+```python
 from wikibaseintegrator import wbi_core, wbi_login
     
 # login object
 login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')
      
 # data type object, e.g. for a NCBI gene entrez ID
 entrez_gene_id = wbi_core.String(value='<some_entrez_id>', prop_nr='P351')
@@ -210,15 +204,15 @@
 wd_item = wbi_core.ItemEngine(data=data)
 wd_item.write(login_instance)
 ```
 
 ## A Minimal Bot for Mass Import ##
 An enhanced example of the previous bot just puts two of the three things into a for loop and so allows mass creation, or modification of items.
 
-```Python
+```python
 from wikibaseintegrator import wbi_core, wbi_login
     
 # login object
 login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')
 
 # We have raw data, which should be written to Wikidata, namely two human NCBI entrez gene IDs mapped to two Ensembl Gene IDs
 raw_data = {
@@ -246,20 +240,20 @@
 
 IMPORTANT: In order for the fast run mode to work, the data you provide in the constructor must contain at least one unique value/id only present on one Wikidata item, e.g. an NCBI entrez gene ID, Uniprot ID, etc.
 Usually, these would be the same unique core properties used for defining domains in wbi_core, e.g. for genes, proteins, drugs or your custom domains.
 
 Below, the normal mode run example from above, slightly modified, to meet the requirements for the fastrun mode. To enable it, ItemEngine requires two parameters, fast_run=True/False and fast_run_base_filter which 
  is a dictionary holding the properties to filter for as keys and the item QIDs as dict values. If the value is not a QID but a literal, just provide an empty string. For the above example, the dictionary looks like this:
  
-```Python
+```python
 fast_run_base_filter = {'P351': '', 'P703': 'Q15978631'}
 ```
  
 The full example:
-```Python
+```python
 from wikibaseintegrator import wbi_core, wbi_login
     
 # login object
 login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')
 
 fast_run_base_filter = {'P351': '', 'P703': 'Q15978631'}
 fast_run = True
@@ -280,8 +274,9 @@
     data = [entrez_gene_id, ensembl_transcript_id]
     
     # Search for and then edit/create new item
     wd_item = wbi_core.ItemEngine(data=data, fast_run=fast_run, fast_run_base_filter=fast_run_base_filter)
     wd_item.write(login_instance)
 ```
 
-Note: Fastrun mode checks for equality of property/value pairs, qualifers (not including qualifier attributes), labels, aliases and description, but it ignores references by default! References can be checked in fastrun mode by setting `fast_run_use_refs` to `True`.
+Note: Fastrun mode checks for equality of property/value pairs, qualifers (not including qualifier attributes), labels, aliases and description, but it ignores references by default!
+References can be checked in fastrun mode by setting `fast_run_use_refs` to `True`.
```

### Comparing `wikibaseintegrator-0.8.2/setup.py` & `wikibaseintegrator-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.8.2"
+VERSION = "0.9.0"
 
 setup(
     name='wikibaseintegrator',
     version=VERSION,
     author='Myst and WikidataIntegrator authors',
     description='Python package for reading and writing to/from Wikibase',
     license='MIT',
     keywords='Wikibase',
-    url='https://github.com/Mystou/WikibaseIntegrator',
+    url='https://github.com/LeMyst/WikibaseIntegrator',
     packages=find_packages(),
     include_package_data=True,
     # long_description=read('README.md'),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
@@ -24,22 +24,19 @@
         "Operating System :: Microsoft :: Windows",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Developers",
         "Topic :: Utilities",
     ],
     install_requires=[
-        'requests',
-        'python-dateutil',
         'simplejson',
+        'requests',
         'pandas',
-        'tqdm',
         'mwoauth',
-        'oauthlib',
-        'sparql_slurper',
-        'ShExJSG',
-        'jsonasobj',
-        'pyshex',
-        'backoff',
-        'shexer'
+        'backoff'
     ],
+    extras_require={
+        'dev': [
+            'pytest'
+        ]
+    }
 )
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_backoff.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_backoff.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,33 +19,34 @@
         config['BACKOFF_MAX_TRIES'] = 2
         config['BACKOFF_MAX_VALUE'] = 2
         with self.assertRaises(requests.RequestException):
             bad_http_code()
         with self.assertRaises(requests.RequestException):
             bad_login()
 
-        assert good_http_code() == "200 OK"
+        assert good_http_code() == 200
 
         with self.assertRaises(json.JSONDecodeError):
             bad_json()
 
 
 @wbi_backoff()
 def bad_http_code():
-    r = requests.get("http://httpstat.us/400")
+    r = requests.get("http://httpbin.org/status/400")
     r.raise_for_status()
-    print(r.text)
+    print(r.status_code)
+    return r.status_code
 
 
 @wbi_backoff()
 def good_http_code():
-    r = requests.get("http://httpstat.us/200")
+    r = requests.get("http://httpbin.org/status/200")
     r.raise_for_status()
-    print(r.text)
-    return r.text
+    print(r.status_code)
+    return r.status_code
 
 
 @wbi_backoff()
 def bad_json():
     json.loads("<xml>I failed :(</xml>")
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_fastrun.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_fastrun.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     test_fastrun.test_query_data
     This hits live wikidata and may change !!
 
     This tests that the fast run container correctly queries data from wikidata and stores it in the appropriate format
     without getting references
     """
     frc = wbi_fastrun.FastRunContainer(base_filter={'P699': ''},
-                                       base_data_type=wbi_core.BaseDataType, engine=wbi_core.ItemEngine)
+                                       base_data_type=wbi_core.BaseDataType, engine=wbi_core.ItemEngine, debug=True)
     # get a string value
     frc._query_data('P699')
     # wikidata-item value
     frc._query_data('P31')
     # uri value
     frc._query_data('P1709')
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_item_creation.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_item_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
             wbi_core.String(value='test1', prop_nr='P2'),
             wbi_core.Math("xxx", prop_nr="P3"),
             wbi_core.ExternalID("xxx", prop_nr="P4"),
             wbi_core.ItemID("Q123", prop_nr="P5"),
             wbi_core.Time('+%Y-%m-%dT%H:%M:%SZ', "P6"),
             wbi_core.Url("http://www.google.com", "P7"),
             wbi_core.MonolingualText("xxx", prop_nr="P8"),
-            wbi_core.Quantity(5, prop_nr="P9"),
-            wbi_core.Quantity(5, upper_bound=9, lower_bound=2, prop_nr="P10"),
+            wbi_core.Quantity(-5.04, prop_nr="P9"),
+            wbi_core.Quantity(5.06, upper_bound=9.99, lower_bound=-2.22, unit="Q11573", prop_nr="P10"),
             wbi_core.CommonsMedia("xxx", prop_nr="P11"),
             wbi_core.GlobeCoordinate(1.2345, 1.2345, 12, prop_nr="P12"),
             wbi_core.GeoShape("Data:xxx.map", prop_nr="P13"),
             wbi_core.Property("P123", "P14"),
             wbi_core.TabularData("Data:xxx.tab", prop_nr="P15"),
             wbi_core.MusicalNotation("\relative c' { c d e f | g2 g | a4 a a a | g1 |}", prop_nr="P16"),
             wbi_core.Lexeme("L123", prop_nr="P17"),
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/tests/test_item_generator.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_item_generator.py`

 * *Files identical despite different names*

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/tests/tests.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/tests/test_all.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,51 +14,51 @@
 class TestMediawikiApiCall(unittest.TestCase):
     def test_all(self):
         with self.assertRaises(MWApiError):
             wbi_core.ItemEngine.mediawiki_api_call("GET", "http://www.wikidataaaaaaaaa.org",
                                                    max_retries=3, retry_after=1,
                                                    params={'format': 'json', 'action': 'wbgetentities', 'ids': 'Q42'})
         with self.assertRaises(requests.HTTPError):
-            wbi_core.ItemEngine.mediawiki_api_call("GET", "http://httpstat.us/400", max_retries=3, retry_after=1)
+            wbi_core.ItemEngine.mediawiki_api_call("GET", "http://httpbin.org/status/400", max_retries=3, retry_after=1)
 
         wbi_core.ItemEngine.mediawiki_api_call("GET", max_retries=3, retry_after=1,
                                                params={'format': 'json', 'action': 'wbgetentities', 'ids': 'Q42'})
 
 
 class TestDataType(unittest.TestCase):
     def test_wd_quantity(self):
-        dt = wbi_core.Quantity(value='34', prop_nr='P43')
+        dt = wbi_core.Quantity(value='34.5', prop_nr='P43')
 
         dt_json = dt.get_json_representation()
 
         if not dt_json['mainsnak']['datatype'] == 'quantity':
             raise
 
         value = dt_json['mainsnak']['datavalue']
 
-        if not value['value']['amount'] == '+34':
+        if not value['value']['amount'] == '+34.5':
             raise
 
         if not value['value']['unit'] == '1':
             raise
 
-        dt2 = wbi_core.Quantity(value='34', prop_nr='P43', upper_bound='35', lower_bound='33')
+        dt2 = wbi_core.Quantity(value='34.5', prop_nr='P43', upper_bound='35.3', lower_bound='33.7', unit="Q11573")
 
         value = dt2.get_json_representation()['mainsnak']['datavalue']
 
-        if not value['value']['amount'] == '+34':
+        if not value['value']['amount'] == '+34.5':
             raise
 
-        if not value['value']['unit'] == '1':
+        if not value['value']['unit'] == 'http://www.wikidata.org/entity/Q11573':
             raise
 
-        if not value['value']['upperBound'] == '+35':
+        if not value['value']['upperBound'] == '+35.3':
             raise
 
-        if not value['value']['lowerBound'] == '+33':
+        if not value['value']['lowerBound'] == '+33.7':
             raise
 
     def test_wd_geoshape(self):
         dt = wbi_core.GeoShape(value='Data:Inner_West_Light_Rail_stops.map', prop_nr='P43')
 
         dt_json = dt.get_json_representation()
 
@@ -91,16 +91,14 @@
 class TestFastRun(unittest.TestCase):
     """
     some basic tests for fastrun mode
     
     """
 
     def test_fast_run(self):
-        qid = 'Q27552312'
-
         statements = [
             wbi_core.ExternalID(value='P40095', prop_nr='P352'),
             wbi_core.ExternalID(value='YER158C', prop_nr='P705')
         ]
 
         frc = wbi_fastrun.FastRunContainer(base_filter={'P352': '', 'P703': 'Q27510868'},
                                            base_data_type=wbi_core.BaseDataType, engine=wbi_core.ItemEngine)
@@ -142,30 +140,30 @@
 
         item.set_description(descr)
         item.set_description("fghjkl")
         assert item.json_representation['descriptions']['en'] == {'language': 'en', 'value': 'fghjkl'}
         item.set_label("Earth")
         item.set_label("xfgfdsg")
         assert item.json_representation['labels']['en'] == {'language': 'en', 'value': 'xfgfdsg'}
-        item.set_aliases(["fake alias"], append=True)
+        item.set_aliases(["fake alias"], if_exists='APPEND')
         assert {'language': 'en', 'value': 'fake alias'} in item.json_representation['aliases']['en']
 
         # something thats empty (for now.., can change, so this just makes sure no exception is thrown)
         frc.check_language_data("Q2", ['Ewiase'], 'ak', 'label')
         frc.check_language_data("Q2", ['not Ewiase'], 'ak', 'label')
         frc.check_language_data("Q2", [''], 'ak', 'description')
         frc.check_language_data("Q2", [], 'ak', 'aliases')
         frc.check_language_data("Q2", ['sdf', 'sdd'], 'ak', 'aliases')
 
         item.get_label("ak")
         item.get_description("ak")
         item.get_aliases("ak")
         item.set_label("label", lang="ak")
         item.set_description("d", lang="ak")
-        item.set_aliases(["a"], lang="ak", append=True)
+        item.set_aliases(["a"], lang="ak", if_exists='APPEND')
 
 
 def test_sitelinks():
     data = [wbi_core.ItemID(value='Q12136', prop_nr='P31')]
     item = wbi_core.ItemEngine(item_id='Q622901', data=data)
     item.get_sitelink("enwiki")
     assert "enwiki" not in item.json_representation['sitelinks']
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_backoff.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_backoff.py`

 * *Files identical despite different names*

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_config.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,9 +27,9 @@
     'DISTINCT_VALUES_CONSTRAINT_QID': 'Q21502410',
     'COORDINATE_GLOBE_QID': 'http://www.wikidata.org/entity/Q2',
     'CALENDAR_MODEL_QID': 'http://www.wikidata.org/entity/Q1985727',
     'MEDIAWIKI_API_URL': 'https://www.wikidata.org/w/api.php',
     'MEDIAWIKI_INDEX_URL': 'https://www.wikidata.org/w/index.php',
     'SPARQL_ENDPOINT_URL': 'https://query.wikidata.org/sparql',
     'WIKIBASE_URL': 'http://www.wikidata.org',
-    'CONCEPT_BASE_URI': 'http://www.wikidata.org/entity/'
+    'DEFAULT_LANGUAGE': 'en'
 }
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_core.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 import copy
 import datetime
 import json
-import logging
-import os
 import re
 import time
-import warnings
 from collections import defaultdict
-from typing import List
+from warnings import warn
 
-import pandas as pd
+import pandas
 import requests
-from pyshex import ShExEvaluator
-from rdflib import Graph
-from shexer.shaper import Shaper
 
 from wikibaseintegrator.wbi_backoff import wbi_backoff
 from wikibaseintegrator.wbi_config import config
 from wikibaseintegrator.wbi_fastrun import FastRunContainer
 
 """
 Authors:
   Andra Waagmeester (andra' at ' micelio.be)
   Gregory Stupp (stuppie' at 'gmail.com)
   Sebastian Burgstaller (sebastian.burgstaller' at 'gmail.com)
   Myst
-
 """
 
 __author__ = 'Andra Waagmeester, Gregory Stupp, Sebastian Burgstaller, Myst'
 __license__ = 'MIT'
 
 
 class ItemEngine(object):
-    databases = {}
     pmids = []
 
     log_file_name = ''
     fast_run_store = []
 
     DISTINCT_VALUE_PROPS = dict()
 
     logger = None
 
     def __init__(self, item_id='', new_item=False, data=None, mediawiki_api_url=None, sparql_endpoint_url=None,
-                 wikibase_url=None, concept_base_uri=None, append_value=None, fast_run=False, fast_run_base_filter=None,
+                 wikibase_url=None, append_value=None, fast_run=False, fast_run_base_filter=None,
                  fast_run_use_refs=False, ref_handler=None, global_ref_mode='KEEP_GOOD', good_refs=None,
                  keep_good_ref_statements=False, search_only=False, item_data=None, user_agent=None, core_props=None,
                  core_prop_match_thresh=0.66, property_constraint_pid=None, distinct_values_constraint_qid=None,
                  fast_run_case_insensitive=False, debug=False):
         """
         constructor
         :param item_id: Wikibase item id
@@ -120,15 +112,14 @@
         """
         self.core_prop_match_thresh = core_prop_match_thresh
         self.item_id = item_id
         self.new_item = new_item
         self.mediawiki_api_url = config['MEDIAWIKI_API_URL'] if mediawiki_api_url is None else mediawiki_api_url
         self.sparql_endpoint_url = config['SPARQL_ENDPOINT_URL'] if sparql_endpoint_url is None else sparql_endpoint_url
         self.wikibase_url = config['WIKIBASE_URL'] if wikibase_url is None else wikibase_url
-        self.concept_base_uri = config['CONCEPT_BASE_URI'] if concept_base_uri is None else concept_base_uri
         self.property_constraint_pid = config[
             'PROPERTY_CONSTRAINT_PID'] if property_constraint_pid is None else property_constraint_pid
         self.distinct_values_constraint_qid = config[
             'DISTINCT_VALUES_CONSTRAINT_QID'] if distinct_values_constraint_qid is None else distinct_values_constraint_qid
         self.data = [] if data is None else data
         self.append_value = [] if append_value is None else append_value
         self.fast_run = fast_run
@@ -145,15 +136,18 @@
 
         self.create_new_item = False
         self.json_representation = {}
         self.statements = []
         self.original_statements = []
         self.entity_metadata = {}
         self.fast_run_container = None
-        self.require_write = True
+        if self.search_only:
+            self.require_write = False
+        else:
+            self.require_write = True
         self.sitelinks = dict()
         self.lastrevid = None  # stores last revisionid after a write occurs
 
         self.debug = debug
 
         if fast_run_case_insensitive and not search_only:
             raise ValueError("If using fast run case insensitive, search_only must be set")
@@ -204,78 +198,80 @@
         distinct_values_constraint_qid = config[
             'DISTINCT_VALUES_CONSTRAINT_QID'] if distinct_values_constraint_qid is None else distinct_values_constraint_qid
 
         pcpid = property_constraint_pid
         dvcqid = distinct_values_constraint_qid
 
         query = '''
-        PREFIX wd: <{0}/entity/>
-        PREFIX wdt: <{0}/prop/direct/>
-
         SELECT ?p WHERE {{
-            ?p wdt:{1} wd:{2}
+            ?p <{wb_url}/prop/direct/{prop_nr}> <{wb_url}/entity/{entity}>
         }}
-        '''.format(wikibase_url, pcpid, dvcqid)
+        '''.format(wb_url=wikibase_url, prop_nr=pcpid, entity=dvcqid)
         df = cls.execute_sparql_query(query, endpoint=sparql_endpoint_url, as_dataframe=True)
         if df.empty:
-            warnings.warn("Warning: No distinct value properties found\n" +
-                          "Please set P2302 and Q21502410 in your wikibase or set `core_props` manually.\n" +
-                          "Continuing with no core_props")
+            warn("Warning: No distinct value properties found\n" +
+                 "Please set P2302 and Q21502410 in your wikibase or set `core_props` manually.\n" +
+                 "Continuing with no core_props")
             cls.DISTINCT_VALUE_PROPS[sparql_endpoint_url] = set()
             return None
         df.p = df.p.str.rsplit("/", 1).str[-1]
         cls.DISTINCT_VALUE_PROPS[sparql_endpoint_url] = set(df.p)
 
     def init_data_load(self):
         if self.item_id and self.item_data:
+            if self.debug:
+                print('Load item from item_data')
             self.json_representation = self.parse_json(self.item_data)
         elif self.item_id:
+            if self.debug:
+                print('Load item from MW API from item_id')
             self.json_representation = self.get_entity()
         else:
+            if self.debug:
+                print('Try to guess item QID from props')
             qids_by_props = ''
             try:
                 qids_by_props = self.__select_item()
             except SearchError as e:
-                self.log('ERROR', str(e))
+                print('ERROR init_data_load: ', str(e))
 
             if qids_by_props:
                 self.item_id = qids_by_props
                 self.json_representation = self.get_entity()
                 self.__check_integrity()
 
         if not self.search_only:
             self.__construct_claim_json()
         else:
             self.data = []
 
     def init_fastrun(self):
         # We search if we already have a FastRunContainer with the same parameters to re-use it
         for c in ItemEngine.fast_run_store:
-            if (c.base_filter == self.fast_run_base_filter) and (c.use_refs == self.fast_run_use_refs) and \
-                    (c.sparql_endpoint_url == self.sparql_endpoint_url):
+            if (c.base_filter == self.fast_run_base_filter) \
+                    and (c.use_refs == self.fast_run_use_refs) \
+                    and (c.sparql_endpoint_url == self.sparql_endpoint_url):
                 self.fast_run_container = c
                 self.fast_run_container.ref_handler = self.ref_handler
                 self.fast_run_container.current_qid = ''
                 self.fast_run_container.base_data_type = BaseDataType
                 self.fast_run_container.engine = self.__class__
                 self.fast_run_container.mediawiki_api_url = self.mediawiki_api_url
                 self.fast_run_container.wikibase_url = self.wikibase_url
-                self.fast_run_container.concept_base_uri = self.concept_base_uri
                 self.fast_run_container.debug = self.debug
                 if self.debug:
                     print('Found an already existing FastRunContainer')
 
         if not self.fast_run_container:
             self.fast_run_container = FastRunContainer(base_filter=self.fast_run_base_filter,
                                                        base_data_type=BaseDataType,
                                                        engine=self.__class__,
                                                        sparql_endpoint_url=self.sparql_endpoint_url,
                                                        mediawiki_api_url=self.mediawiki_api_url,
                                                        wikibase_url=self.wikibase_url,
-                                                       concept_base_uri=self.concept_base_uri,
                                                        use_refs=self.fast_run_use_refs,
                                                        ref_handler=self.ref_handler,
                                                        case_insensitive=self.fast_run_case_insensitive,
                                                        debug=self.debug)
             ItemEngine.fast_run_store.append(self.fast_run_container)
 
         if not self.search_only:
@@ -332,34 +328,35 @@
         self.original_statements = copy.deepcopy(self.statements)
 
         return data
 
     @staticmethod
     def get_search_results(search_string='', mediawiki_api_url=None,
                            user_agent=None, max_results=500,
-                           language='en', dict_id_label=False):
+                           language=None, dict_id_label=False):
         """
         Performs a search in the Wikibase instance for a certain search string
         :param search_string: a string which should be searched for in the Wikibase instance
         :type search_string: str
         :param mediawiki_api_url: Specify the mediawiki_api_url.
         :type mediawiki_api_url: str
         :param user_agent: The user agent string transmitted in the http header
         :type user_agent: str
         :param max_results: The maximum number of search results returned. Default 500
         :type max_results: int
-        :param language: The language in which to perform the search. Default 'en'
+        :param language: The language in which to perform the search.
         :type language: str
         :return: returns a list of QIDs found in the search and a list of labels complementary to the QIDs
         :type dict_id_label: boolean
         :return: function return a list with a dict of id and label
         """
 
         mediawiki_api_url = config['MEDIAWIKI_API_URL'] if mediawiki_api_url is None else mediawiki_api_url
         user_agent = config['USER_AGENT_DEFAULT'] if user_agent is None else user_agent
+        language = config['DEFAULT_LANGUAGE'] if language is None else language
 
         params = {
             'action': 'wbsearchentities',
             'language': language,
             'search': search_string,
             'format': 'json',
             'limit': 50
@@ -407,15 +404,16 @@
         for x in self.statements:
             property_list.add(x.get_prop_nr())
 
         return list(property_list)
 
     def __select_item(self):
         """
-        The most likely item QID should be returned, after querying the Wikibase instance for all values in core_id properties
+        The most likely item QID should be returned, after querying the Wikibase instance for all values in core_id
+        properties
         :return: Either a single QID is returned, or an empty string if no suitable item in the Wikibase instance
         """
         qid_list = set()
         conflict_source = {}
         # This is a `hack` for if initializing the mapping relation helper fails. We can't determine the
         # mapping relation type PID or the exact match QID. If we set mrt_pid to "Pxxx", then no qualifier will
         # ever match it (and exact_qid will never get checked), and so what happens is exactly what would
@@ -438,15 +436,16 @@
 
             core_props = self.core_props
             if property_nr in core_props:
                 tmp_qids = set()
                 # if mrt_pid is "PXXX", this is fine, because the part of the SPARQL query using it is optional
                 query = statement.sparql_query.format(wb_url=self.wikibase_url, mrt_pid=mrt_pid, pid=property_nr,
                                                       value=data_point.replace("'", r"\'"))
-                results = ItemEngine.execute_sparql_query(query=query, endpoint=self.sparql_endpoint_url)
+                results = ItemEngine.execute_sparql_query(query=query, endpoint=self.sparql_endpoint_url,
+                                                          debug=self.debug)
 
                 for i in results['results']['bindings']:
                     qid = i['item_id']['value'].split('/')[-1]
                     if ('mrt' not in i) or ('mrt' in i and i['mrt']['value'].split('/')[-1] == exact_qid):
                         tmp_qids.add(qid)
 
                 qid_list.update(tmp_qids)
@@ -483,17 +482,14 @@
 
         def handle_qualifiers(old_item, new_item):
             if not new_item.check_qualifier_equality:
                 old_item.set_qualifiers(new_item.get_qualifiers())
 
         def is_good_ref(ref_block):
 
-            if len(ItemEngine.databases) == 0:
-                ItemEngine._init_ref_system()
-
             prop_nrs = [x.get_prop_nr() for x in ref_block]
             values = [x.get_value() for x in ref_block]
             good_ref = True
             prop_value_map = dict(zip(prop_nrs, values))
 
             # if self.good_refs has content, use these to determine good references
             if self.good_refs and len(self.good_refs) > 0:
@@ -507,14 +503,15 @@
                         found_good = False
 
                     if found_good:
                         return True
 
                 return False
 
+            # TODO: Rework this part for Wikibase
             # stated in, title, retrieved
             ref_properties = ['P248', 'P1476', 'P813']
 
             for v in values:
                 if prop_nrs[values.index(v)] == 'P248':
                     return True
                 elif v == 'P698':
@@ -524,39 +521,31 @@
                 if p not in prop_nrs:
                     return False
 
             for ref in ref_block:
                 pn = ref.get_prop_nr()
                 value = ref.get_value()
 
-                if pn == 'P248' and value not in ItemEngine.databases and 'P854' not in prop_nrs:
+                if pn == 'P248' and 'P854' not in prop_nrs:
                     return False
-                elif pn == 'P248' and value in ItemEngine.databases:
-                    db_props = ItemEngine.databases[value]
-                    if not any([False if x not in prop_nrs else True for x in db_props]) and 'P854' not in prop_nrs:
-                        return False
 
             return good_ref
 
         def handle_references(old_item, new_item):
             """
             Local function to handle references
             :param old_item: An item containing the data as currently in the Wikibase instance
             :type old_item: A child of BaseDataType
             :param new_item: An item containing the new data which should be written to the Wikibase instance
             :type new_item: A child of BaseDataType
             """
-            # stated in, title, language of work, retrieved, imported from
-            ref_properties = ['P248', 'P1476', 'P407', 'P813', 'P143']
             new_references = new_item.get_references()
             old_references = old_item.get_references()
 
-            if any([z.overwrite_references for y in new_references for z in y]) \
-                    or sum(map(lambda z: len(z), old_references)) == 0 \
-                    or self.global_ref_mode == 'STRICT_OVERWRITE':
+            if sum(map(lambda z: len(z), old_references)) == 0 or self.global_ref_mode == 'STRICT_OVERWRITE':
                 old_item.set_references(new_references)
 
             elif self.global_ref_mode == 'STRICT_KEEP' or new_item.statement_ref_mode == 'STRICT_KEEP':
                 pass
 
             elif self.global_ref_mode == 'STRICT_KEEP_APPEND' or new_item.statement_ref_mode == 'STRICT_KEEP_APPEND':
                 old_references.extend(new_references)
@@ -751,145 +740,198 @@
                                              .format(self.item_id, core_prop_match_count,
                                                      count_existing_ids - core_prop_match_count) +
                                              'existing unmatched core props: {}. '.format(nomatch_existing) +
                                              'statement unmatched core props: {}.'.format(nomatch_new))
         else:
             return True
 
-    def get_label(self, lang='en'):
+    def get_label(self, lang=None):
         """
         Returns the label for a certain language
         :param lang:
         :type lang: str
         :return: returns the label in the specified language, an empty string if the label does not exist
         """
+        lang = config['DEFAULT_LANGUAGE'] if lang is None else lang
+
         if self.fast_run:
             return list(self.fast_run_container.get_language_data(self.item_id, lang, 'label'))[0]
         try:
             return self.json_representation['labels'][lang]['value']
         except KeyError:
             return ''
 
-    def set_label(self, label, lang='en'):
+    def set_label(self, label, lang=None, if_exists='REPLACE'):
         """
         Set the label for an item in a certain language
         :param label: The description of the item in a certain language
         :type label: str
         :param lang: The language a label should be set for.
         :type lang: str
+        :param if_exists: If a label already exist, REPLACE it or KEEP it.
         :return: None
         """
+        lang = config['DEFAULT_LANGUAGE'] if lang is None else lang
+
+        if if_exists != 'KEEP' and if_exists != 'REPLACE':
+            raise ValueError('{} is not a valid value for if_exists (REPLACE or KEEP)'.format(if_exists))
+
+        # Skip set_label if the item already have one and if_exists is at 'KEEP'
+        if self.fast_run_container.get_language_data(self.item_id, lang, 'label') != [''] and if_exists == 'KEEP':
+            return
+
         if self.fast_run and not self.require_write:
             self.require_write = self.fast_run_container.check_language_data(qid=self.item_id,
                                                                              lang_data=[label], lang=lang,
                                                                              lang_data_type='label')
             if self.require_write:
                 self.init_data_load()
             else:
                 return
 
-        if 'labels' not in self.json_representation:
+        if 'labels' not in self.json_representation or not self.json_representation['labels'] or if_exists == 'REPLACE':
             self.json_representation['labels'] = {}
+
         self.json_representation['labels'][lang] = {
             'language': lang,
             'value': label
         }
 
-    def get_aliases(self, lang='en'):
+    def get_aliases(self, lang=None):
         """
         Retrieve the aliases in a certain language
         :param lang: The language the description should be retrieved for
         :return: Returns a list of aliases, an empty list if none exist for the specified language
         """
+        lang = config['DEFAULT_LANGUAGE'] if lang is None else lang
+
         if self.fast_run:
             return list(self.fast_run_container.get_language_data(self.item_id, lang, 'aliases'))
 
         alias_list = []
         if 'aliases' in self.json_representation and lang in self.json_representation['aliases']:
             for alias in self.json_representation['aliases'][lang]:
                 alias_list.append(alias['value'])
 
         return alias_list
 
-    def set_aliases(self, aliases, lang='en', append=True):
+    def set_aliases(self, aliases, lang=None, if_exists='APPEND'):
         """
         set the aliases for an item
         :param aliases: a list of strings representing the aliases of an item
         :param lang: The language a description should be set for
-        :param append: If true, append a new alias to the list of existing aliases, else, overwrite. Default: True
+        :param if_exists: If aliases already exist, APPEND or REPLACE
         :return: None
         """
+        lang = config['DEFAULT_LANGUAGE'] if lang is None else lang
+
+        if not isinstance(aliases, list):
+            raise ValueError('aliases must be a list')
+
+        if if_exists != 'APPEND' and if_exists != 'REPLACE':
+            raise ValueError('{} is not a valid value for if_exists (REPLACE or APPEND)'.format(if_exists))
+
         if self.fast_run and not self.require_write:
             self.require_write = self.fast_run_container.check_language_data(qid=self.item_id,
                                                                              lang_data=aliases, lang=lang,
-                                                                             lang_data_type='aliases')
+                                                                             lang_data_type='aliases',
+                                                                             if_exists=if_exists)
             if self.require_write:
                 self.init_data_load()
             else:
                 return
 
         if 'aliases' not in self.json_representation:
             self.json_representation['aliases'] = {}
 
-        if not append or lang not in self.json_representation['aliases']:
+        if if_exists == 'REPLACE' or lang not in self.json_representation['aliases']:
             self.json_representation['aliases'][lang] = []
-
-        for alias in aliases:
-            found = False
-            for current_aliases in self.json_representation['aliases'][lang]:
-                if alias.strip().lower() != current_aliases['value'].strip().lower():
-                    continue
-                else:
-                    found = True
-                    break
-
-            if not found:
+            for alias in aliases:
                 self.json_representation['aliases'][lang].append({
                     'language': lang,
                     'value': alias
                 })
+        else:
+            for alias in aliases:
+                found = False
+                for current_aliases in self.json_representation['aliases'][lang]:
+                    if alias.strip().casefold() != current_aliases['value'].strip().casefold():
+                        continue
+                    else:
+                        found = True
+                        break
 
-    def get_description(self, lang='en'):
+                if not found:
+                    self.json_representation['aliases'][lang].append({
+                        'language': lang,
+                        'value': alias
+                    })
+
+    def get_description(self, lang=None):
         """
         Retrieve the description in a certain language
         :param lang: The language the description should be retrieved for
         :return: Returns the description string
         """
+        lang = config['DEFAULT_LANGUAGE'] if lang is None else lang
+
         if self.fast_run:
             return list(self.fast_run_container.get_language_data(self.item_id, lang, 'description'))[0]
         if 'descriptions' not in self.json_representation or lang not in self.json_representation['descriptions']:
             return ''
         else:
             return self.json_representation['descriptions'][lang]['value']
 
-    def set_description(self, description, lang='en'):
+    def set_description(self, description, lang=None, if_exists='REPLACE'):
         """
         Set the description for an item in a certain language
         :param description: The description of the item in a certain language
         :type description: str
         :param lang: The language a description should be set for.
         :type lang: str
+        :param if_exists: If a description already exist, REPLACE it or KEEP it.
         :return: None
         """
+        lang = config['DEFAULT_LANGUAGE'] if lang is None else lang
+
+        if if_exists != 'KEEP' and if_exists != 'REPLACE':
+            raise ValueError('{} is not a valid value for if_exists (REPLACE or KEEP)'.format(if_exists))
+
+        # Skip set_description if the item already have one and if_exists is at 'KEEP'
+        if self.fast_run_container.get_language_data(self.item_id, lang, 'description') != [''] and if_exists == 'KEEP':
+            return
+
         if self.fast_run and not self.require_write:
-            self.require_write = self.fast_run_container.check_language_data(qid=self.item_id,
-                                                                             lang_data=[description], lang=lang,
-                                                                             lang_data_type='description')
+            self.require_write = self.fast_run_container.check_language_data(qid=self.item_id, lang_data=[description],
+                                                                             lang=lang, lang_data_type='description')
             if self.require_write:
                 self.init_data_load()
             else:
                 return
 
-        if 'descriptions' not in self.json_representation:
+        if 'descriptions' not in self.json_representation or not self.json_representation['descriptions'] \
+                or if_exists == 'REPLACE':
             self.json_representation['descriptions'] = {}
+
         self.json_representation['descriptions'][lang] = {
             'language': lang,
             'value': description
         }
 
+    def get_sitelink(self, site):
+        """
+        A method to access the interwiki links in the json.model
+        :param site: The Wikipedia site the interwiki/sitelink should be returned for
+        :return: The interwiki/sitelink string for the specified Wikipedia will be returned.
+        """
+        if site in self.sitelinks:
+            return self.sitelinks[site]
+        else:
+            return None
+
     def set_sitelink(self, site, title, badges=()):
         """
         Set sitelinks to corresponding Wikipedia pages
         :param site: The Wikipedia page a sitelink is directed to (e.g. 'enwiki')
         :param title: The title of the Wikipedia page the sitelink is directed to
         :param badges: An iterable containing Wikipedia badge strings.
         :return:
@@ -898,25 +940,14 @@
             'site': site,
             'title': title,
             'badges': badges
         }
         self.json_representation['sitelinks'][site] = sitelink
         self.sitelinks[site] = sitelink
 
-    def get_sitelink(self, site):
-        """
-        A method to access the interwiki links in the json.model
-        :param site: The Wikipedia site the interwiki/sitelink should be returned for
-        :return: The interwiki/sitelink string for the specified Wikipedia will be returned.
-        """
-        if site in self.sitelinks:
-            return self.sitelinks[site]
-        else:
-            return None
-
     def write(self, login, bot_account=True, edit_summary='', entity_type='item', property_datatype='string',
               max_retries=1000, retry_after=60):
         """
         Writes the item Json to the Wikibase instance and after successful write, updates the object with new ids and
         hashes generated by the Wikibase instance. For new items, also returns the new QIDs.
         :param login: a instance of the class PBB_login which provides edit-cookies and edit-tokens
         :param bot_account: Tell the Wikidata API whether the script should be run as part of a bot account or not.
@@ -1046,101 +1077,30 @@
                     sleep_sec = json_data['error'].get('lag', retry_after)
                     print("{}: maxlag. sleeping for {} seconds".format(datetime.datetime.utcnow(), sleep_sec))
                     time.sleep(sleep_sec)
                     continue
 
                 # readonly
                 if 'code' in json_data['error'] and json_data['error']['code'] == 'readonly':
-                    print('The wikibase instance is currently in readonly mode, waiting for {} seconds'.format(retry_after))
+                    print('The wikibase instance is currently in readonly mode, waiting for {} seconds'.format(
+                        retry_after))
                     time.sleep(retry_after)
                     continue
 
             # there is no error or waiting. break out of this loop and parse response
             break
         else:
             # the first time I've ever used for - else!!
             # else executes if the for loop completes normally. i.e. does not encouter a `break`
             # in this case, that means it tried this api call 10 times
             raise MWApiError(response.json() if response else dict())
 
         return json_data
 
     @classmethod
-    def setup_logging(cls, log_dir="./logs", log_name=None, header=None, names=None,
-                      delimiter=";", logger_name='logger'):
-        """
-        A static method which initiates log files compatible to .csv format, allowing for easy further analysis.
-        :param log_dir: allows for setting relative or absolute path for logging, default is ./logs.
-        :type log_dir: str
-        :param log_name: File name of log file to be written. e.g. "bot_run-20160204.log". Default is "bot_run"
-        and a timestamp of the current time
-        :type log_name: str
-        :param header: Log file will be prepended with header if given
-        :type header: str
-        :param names: Column names for the log file
-        :type names: list
-        :param delimiter: Log file will be delimited with `delimiter`
-        :type delimiter: str
-        """
-        names = ["level", "timestamp", "external_id", "external_id_prop", "wdid", "msg", "msg_type",
-                 "revid"] if names is None else names
-
-        if not os.path.exists(log_dir):
-            os.makedirs(log_dir)
-
-        if not log_name:
-            run_id = time.strftime('%Y%m%d_%H:%M', time.localtime())
-            log_name = "bot_run-{}.log".format(run_id)
-
-        logger = logging.getLogger(logger_name)
-        logger.setLevel(logging.DEBUG)
-
-        log_file_name = os.path.join(log_dir, log_name)
-
-        file_handler = logging.FileHandler(log_file_name, mode='a')
-        file_handler.setLevel(logging.DEBUG)
-
-        fmt = '%(levelname)s{delimiter}%(asctime)s{delimiter}%(message)s'.format(delimiter=delimiter)
-        if header:
-            header = header if header.startswith("#") else "#" + header
-            header += "\n" + delimiter.join(names)
-            formatter = FormatterWithHeader(header, fmt=fmt, datefmt='%m/%d/%Y %H:%M:%S')
-        else:
-            formatter = FormatterWithHeader(delimiter.join(names), fmt=fmt, datefmt='%m/%d/%Y %H:%M:%S')
-        file_handler.setFormatter(formatter)
-        logger.addHandler(file_handler)
-
-        cls.logger = logger
-
-    @classmethod
-    def log(cls, level, message):
-        """
-        :param level: The log level as in the Python logging documentation, 5 different possible values with increasing
-         severity
-        :type level: String of value 'DEBUG', 'INFO', 'WARNING', 'ERROR' or 'CRITICAL'.
-        :param message: The logging data which should be written to the log file. In order to achieve a csv-file
-         compatible format, all fields must be separated by a colon. Furthermore, all strings which could contain
-         colons, spaces or other special characters must be enclosed in double-quotes.
-         e.g. '{main_data_id}, "{exception_type}", "{message}", {item_id}, {duration}'.format(
-                        main_data_id=<main_id>,
-                        exception_type=<excpetion type>,
-                        message=<exception message>,
-                        item_id=<wikibase id>,
-                        duration=<duration of action>
-        :type message: str
-        """
-        if cls.logger is None:
-            cls.setup_logging()
-
-        log_levels = {'DEBUG': logging.DEBUG, 'ERROR': logging.ERROR, 'INFO': logging.INFO, 'WARNING': logging.WARNING,
-                      'CRITICAL': logging.CRITICAL}
-
-        cls.logger.log(level=log_levels[level], msg=message)
-
-    @classmethod
     def generate_item_instances(cls, items, mediawiki_api_url=None, login=None, user_agent=None):
         """
         A method which allows for retrieval of a list of Wikidata items or properties. The method generates a list of
         tuples where the first value in the tuple is the QID or property ID, whereas the second is the new instance of
         ItemEngine containing all the data of the item. This is most useful for mass retrieval of items.
         :param user_agent: A custom user agent
         :param items: A list of QIDs or property IDs
@@ -1181,45 +1141,49 @@
             item_instances.append((qid, ii))
 
         return item_instances
 
     @staticmethod
     @wbi_backoff()
     def execute_sparql_query(query, prefix=None, endpoint=None, user_agent=None, as_dataframe=False, max_retries=1000,
-                             retry_after=60):
+                             retry_after=60, debug=False):
         """
         Static method which can be used to execute any SPARQL query
         :param prefix: The URI prefixes required for an endpoint, default is the Wikidata specific prefixes
         :param query: The actual SPARQL query string
         :param endpoint: The URL string for the SPARQL endpoint. Default is the URL for the Wikidata SPARQL endpoint
         :param user_agent: Set a user agent string for the HTTP header to let the Query Service know who you are.
-        :param as_dataframe: Return result as pandas dataframe
         :type user_agent: str
+        :param as_dataframe: Return result as pandas dataframe
         :param max_retries: The number time this function should retry in case of header reports.
         :param retry_after: the number of seconds should wait upon receiving either an error code or the Query Service
          is not reachable.
+        :param debug: Enable debug output.
+        :type debug: boolean
         :return: The results of the query are returned in JSON format
         """
 
         sparql_endpoint_url = config['SPARQL_ENDPOINT_URL'] if endpoint is None else endpoint
         user_agent = config['USER_AGENT_DEFAULT'] if user_agent is None else user_agent
 
         if prefix:
             query = prefix + '\n' + query
 
         params = {
-            'query': '#Tool: wbi_core fastrun\n' + query,
+            'query': '#Tool: wbi_core execute_sparql_query\n' + query,
             'format': 'json'
         }
 
         headers = {
             'Accept': 'application/sparql-results+json',
             'User-Agent': user_agent
         }
-        response = None
+
+        if debug:
+            print(params['query'])
 
         for n in range(max_retries):
             try:
                 response = requests.post(sparql_endpoint_url, params=params, headers=headers)
             except requests.exceptions.ConnectionError as e:
                 print("Connection error: {}. Sleeping for {} seconds.".format(e, retry_after))
                 time.sleep(retry_after)
@@ -1252,146 +1216,17 @@
                 return int(item['value'])
             if item.get("datatype") == "http://www.w3.org/2001/XMLSchema#dateTime":
                 return datetime.datetime.strptime(item['value'], '%Y-%m-%dT%H:%M:%SZ')
             return item['value']
 
         results = results['results']['bindings']
         results = [{k: parse_value(v) for k, v in item.items()} for item in results]
-        df = pd.DataFrame(results)
+        df = pandas.DataFrame(results)
         return df
 
-    ## SHEX related functions
-    @staticmethod
-    def check_shex_conformance(qid, eid, sparql_endpoint_url=None, output='confirm'):
-        """
-                Static method which can be used to check for conformance of a Wikidata item to an EntitySchema any SPARQL query
-                :param qid: The URI prefixes required for an endpoint, default is the Wikidata specific prefixes
-                :param eid: The EntitySchema identifier from Wikidata
-                :param sparql_endpoint_url: The URL string for the SPARQL endpoint. Default is the URL for the Wikidata SPARQL endpoint
-                :param output: results of a test of conformance on a given shape expression
-                :return: The results of the query are returned in string format
-        """
-
-        sparql_endpoint_url = config['SPARQL_ENDPOINT_URL'] if sparql_endpoint_url is None else sparql_endpoint_url
-
-        schema = requests.get("https://www.wikidata.org/wiki/Special:EntitySchemaText/" + eid).text
-        rdfdata = Graph()
-        rdfdata.parse(config["CONCEPT_BASE_URI"] + qid + ".ttl")
-        shex_result = dict()
-
-        for result in ShExEvaluator(rdf=rdfdata, schema=schema, focus=config["CONCEPT_BASE_URI"] + qid).evaluate():
-            shex_result = dict()
-            if result.result:
-                shex_result["result"] = True
-            else:
-                shex_result["result"] = False
-            shex_result["reason"] = result.reason
-            shex_result["focus"] = result.focus
-
-        if output == "confirm":
-            return shex_result["result"]
-        elif output == "reason":
-            return shex_result["reason"]
-        else:
-            return shex_result
-
-    @staticmethod
-    def extract_shex(qid, extract_shape_of_qualifiers=False, just_direct_properties=True,
-                     comments=False, endpoint="https://query.wikidata.org/sparql"):
-        """
-        It extracts a shape tor the entity specified in qid. The shape is built w.r.t the outgoing
-        properties of the selected Wikidata entity.
-
-        Optionally, it generates as well a shape for each qualifier.
-
-        :param qid: Wikidata identifier to which other wikidata items link
-        :param extract_shape_of_qualifiers: It it is set to True, the result will contain the shape of the qid
-                selected but also the shapes of its qualifiers.
-        :param just_direct_properties: If it set to True, the shape obtained will just contain direct properties to other
-                Wikidata items. It will ignore qualifiers. Do not set to True if extract_shape_of_qualifiers is True
-        :param comments: If it is set to True, each triple constraint will have an associated comment that indicates
-               the trustworthiness of each triple constraint. This is usefull for shapes that have been extracted
-               w.r.t to the properties of more than one entity.
-        :param endpoint: The URL string for the SPARQL endpoint. Default is the URL for the Wikidata SPARQL endpoint
-
-        :return: shex content in String format
-        """
-        namespaces_dict = {
-            "http://www.w3.org/2000/01/rdf-schema#": "rdfs",
-            "http://www.wikidata.org/prop/": "p",
-            "http://www.wikidata.org/prop/direct/": "wdt",
-            "http://www.wikidata.org/entity/": "wd",
-            "http://www.w3.org/2001/XMLSchema#": "xsd",
-            "http://www.w3.org/1999/02/22-rdf-syntax-ns#": "rdf",
-            "http://www.w3.org/XML/1998/namespace": "xml",
-            "http://wikiba.se/ontology#": "wikibase",
-            "http://schema.org/": "schema",
-            "http://www.w3.org/2004/02/skos/core#": "skos"
-        }
-        namespaces_to_ignore = [  # Ignoring these namespaces, mainly just direct properties are considered.
-            "http://www.wikidata.org/prop/",
-            "http://www.wikidata.org/prop/direct-normalized/",
-            "http://schema.org/",
-            "http://www.w3.org/2004/02/skos/core#",
-            "http://wikiba.se/ontology#",
-            "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
-            "http://www.w3.org/2000/01/rdf-schema#"
-        ]
-
-        shape_map = "<http://www.wikidata.org/entity/{qid}>@<{qid}>".format(qid=qid)
-        shaper = Shaper(shape_map_raw=shape_map,
-                        url_endpoint=endpoint,
-                        disable_comments=not comments,
-                        shape_qualifiers_mode=extract_shape_of_qualifiers,
-                        namespaces_dict=namespaces_dict,
-                        namespaces_to_ignore=namespaces_to_ignore if just_direct_properties else None,
-                        namespaces_for_qualifier_props=["http://www.wikidata.org/prop/"],
-                        depth_for_building_subgraph=2 if extract_shape_of_qualifiers else 1)
-        return shaper.shex_graph(string_output=True, acceptance_threshold=0)
-
-    @staticmethod
-    def get_linked_by(qid, mediawiki_api_url=None):
-        """
-            :param qid: Wikidata identifier to which other wikidata items link
-            :param mediawiki_api_url: default to wikidata's api, but can be changed to any wikibase
-            :return:
-        """
-
-        mediawiki_api_url = config['MEDIAWIKI_API_URL'] if mediawiki_api_url is None else mediawiki_api_url
-
-        linkedby = []
-        whatlinkshere = json.loads(requests.get(
-            mediawiki_api_url + "?action=query&list=backlinks&format=json&bllimit=500&bltitle=" + qid).text)
-        for link in whatlinkshere["query"]["backlinks"]:
-            if link["title"].startswith("Q"):
-                linkedby.append(link["title"])
-        while 'continue' in whatlinkshere.keys():
-            whatlinkshere = json.loads(requests.get(
-                mediawiki_api_url + "?action=query&list=backlinks&blcontinue=" +
-                whatlinkshere['continue']['blcontinue'] + "&format=json&bllimit=50&bltitle=" + "Q42").text)
-            for link in whatlinkshere["query"]["backlinks"]:
-                if link["title"].startswith("Q"):
-                    linkedby.append(link["title"])
-        return (linkedby)
-
-    @staticmethod
-    def get_rdf(qid, format="turtle", mediawiki_api_url=None):
-        """
-            :param qid: Wikibase identifier to extract the RDF of
-            :format RDF from to return takes (turtle, ntriples, rdfxml, see https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.html)
-            :param mediawiki_api_url: default to wikidata's api, but can be changed to any wikibase
-            :return:
-        """
-
-        mediawiki_api_url = config['MEDIAWIKI_API_URL'] if mediawiki_api_url is None else mediawiki_api_url
-
-        localcopy = Graph()
-        localcopy.parse(config["CONCEPT_BASE_URI"] + qid + ".ttl")
-        return (localcopy.serialize(format=format))
-
     @staticmethod
     def merge_items(from_id, to_id, login_obj, mediawiki_api_url=None,
                     ignore_conflicts='', user_agent=None):
         """
         A static method to merge two items
         :param from_id: The QID which should be merged into another item
         :type from_id: string with 'Q' prefix
@@ -1400,14 +1235,16 @@
         :param login_obj: The object containing the login credentials and cookies
         :type login_obj: instance of wbi_login.Login
         :param mediawiki_api_url: The MediaWiki url which should be used
         :type mediawiki_api_url: str
         :param ignore_conflicts: A string with the values 'description', 'statement' or 'sitelink', separated
                 by a pipe ('|') if using more than one of those.
         :type ignore_conflicts: str
+        :param user_agent: Set a user agent string for the HTTP header to let the Query Service know who you are.
+        :type user_agent: str
         """
 
         url = config['MEDIAWIKI_API_URL'] if mediawiki_api_url is None else mediawiki_api_url
         user_agent = config['USER_AGENT_DEFAULT'] if user_agent is None else user_agent
 
         headers = {
             'content-type': 'application/x-www-form-urlencoded',
@@ -1436,48 +1273,28 @@
         except requests.HTTPError as e:
             print(e)
             # TODO: should we return this?
             return {'error': 'HTTPError'}
 
         return merge_reply.json()
 
-    # TODO: adapt this function for wikibase (if possible)
-    @classmethod
-    def _init_ref_system(cls, sparql_endpoint_url=None):
-        db_query = '''
-        SELECT DISTINCT ?db ?prop WHERE {
-            {?db wdt:P31 wd:Q2881060 . } UNION
-            {?db wdt:P31 wd:Q4117139 . } UNION
-            {?db wdt:P31 wd:Q8513 . } UNION
-            {?db wdt:P31 wd:Q324254 .}
-
-            OPTIONAL {
-              ?db wdt:P1687 ?prop .
-            }
-        }
-        '''
-
-        for x in cls.execute_sparql_query(db_query, endpoint=sparql_endpoint_url)['results']['bindings']:
-            db_qid = x['db']['value'].split('/')[-1]
-            if db_qid not in cls.databases:
-                cls.databases.update({db_qid: []})
-
-            if 'prop' in x:
-                cls.databases[db_qid].append(x['prop']['value'].split('/')[-1])
-
     @staticmethod
     def delete_item(item, reason, login, mediawiki_api_url=None, user_agent=None):
         """
         Delete an item
         :param item: a QID which should be deleted
         :type item: string
         :param reason: short text about the reason for the deletion request
         :type reason: str
         :param login: A wbi_login.Login object which contains username and password the edit should be performed with.
         :type login: wbi_login.Login
+        :param mediawiki_api_url: The MediaWiki url which should be used
+        :type mediawiki_api_url: str
+        :param user_agent: Set a user agent string for the HTTP header to let the Query Service know who you are.
+        :type user_agent: str
         """
 
         mediawiki_api_url = config['MEDIAWIKI_API_URL'] if mediawiki_api_url is None else mediawiki_api_url
         user_agent = config['USER_AGENT_DEFAULT'] if user_agent is None else user_agent
 
         params = {
             'action': 'delete',
@@ -1490,15 +1307,29 @@
             'User-Agent': user_agent
         }
         r = requests.post(url=mediawiki_api_url, data=params, cookies=login.get_edit_cookie(), headers=headers)
         print(r.json())
 
     @staticmethod
     def delete_statement(statement_id, revision, login, mediawiki_api_url=None, user_agent=None):
-
+        """
+        Delete an item
+        :param statement_id: One GUID or several (pipe-separated) GUIDs identifying the claims to be removed.
+            All claims must belong to the same entity.
+        :type statement_id: string
+        :param revision: The numeric identifier for the revision to base the modification on. This is used for detecting
+            conflicts during save.
+        :type revision: str
+        :param login: A wbi_login.Login object which contains username and password the edit should be performed with.
+        :type login: wbi_login.Login
+        :param mediawiki_api_url: The MediaWiki url which should be used
+        :type mediawiki_api_url: str
+        :param user_agent: Set a user agent string for the HTTP header to let the Query Service know who you are.
+        :type user_agent: str
+        """
         mediawiki_api_url = config['MEDIAWIKI_API_URL'] if mediawiki_api_url is None else mediawiki_api_url
         user_agent = config['USER_AGENT_DEFAULT'] if user_agent is None else user_agent
 
         params = {
             'action': 'wbremoveclaims',
             'claim': statement_id,
             'token': login.get_edit_token(),
@@ -1509,33 +1340,30 @@
         headers = {
             'User-Agent': user_agent
         }
         r = requests.post(url=mediawiki_api_url, data=params, cookies=login.get_edit_cookie(), headers=headers)
         print(r.json())
 
     # References
-    @classmethod
-    def count_references(cls, prop_id):
+    def count_references(self, prop_id):
         counts = dict()
-        for claim in cls.get_json_representation()['claims'][prop_id]:
+        for claim in self.get_json_representation()['claims'][prop_id]:
             counts[claim['id']] = len(claim['references'])
         return counts
 
-    @classmethod
-    def get_reference_properties(cls, prop_id):
+    def get_reference_properties(self, prop_id):
         references = []
-        for statements in cls.get_json_representation()['claims'][prop_id]:
+        for statements in self.get_json_representation()['claims'][prop_id]:
             for reference in statements['references']:
                 references.append(reference['snaks'].keys())
         return references
 
-    @classmethod
-    def get_qualifier_properties(cls, prop_id):
+    def get_qualifier_properties(self, prop_id):
         qualifiers = []
-        for statements in cls.get_json_representation()['claims'][prop_id]:
+        for statements in self.get_json_representation()['claims'][prop_id]:
             for reference in statements['qualifiers']:
                 qualifiers.append(reference['snaks'].keys())
         return qualifiers
 
     @classmethod
     def wikibase_item_engine_factory(cls, mediawiki_api_url=None, sparql_endpoint_url=None, name='LocalItemEngine'):
         """
@@ -1555,17 +1383,16 @@
                 kwargs['mediawiki_api_url'] = mediawiki_api_url
                 kwargs['sparql_endpoint_url'] = sparql_endpoint_url
                 super(SubCls, self).__init__(*args, **kwargs)
 
         SubCls.__name__ = name
         return SubCls
 
-    """A mixin implementing a simple __repr__."""
-
     def __repr__(self):
+        """A mixin implementing a simple __repr__."""
         return "<{klass} @{id:x} {attrs}>".format(
             klass=self.__class__.__name__,
             id=id(self) & 0xFFFFFF,
             attrs="\r\n\t ".join("{}={!r}".format(k, v) for k, v in self.__dict__.items()),
         )
 
 
@@ -1646,33 +1473,19 @@
 
 class BaseDataType(object):
     """
     The base class for all Wikibase data types, they inherit from it
     """
     DTYPE = 'base-data-type'
 
-    # example sparql query
-    """
-    SELECT * WHERE {
-      ?item_id p:P492 ?s .
-      ?s ps:P492 '614212' .
-      OPTIONAL {?s pq:P4390 ?mrt}
-    }
-    """
-
     sparql_query = '''
-        PREFIX wd: <{wb_url}/entity/>
-        PREFIX wdt: <{wb_url}/prop/direct/>
-        PREFIX p: <{wb_url}/prop/>
-        PREFIX ps: <{wb_url}/prop/statement/>
-        PREFIX pq: <{wb_url}/prop/qualifier/>
         SELECT * WHERE {{
-          ?item_id p:{pid} ?s .
-          ?s ps:{pid} '{value}' .
-          OPTIONAL {{?s pq:{mrt_pid} ?mrt}}
+          ?item_id <{wb_url}/prop/{pid}> ?s .
+          ?s <{wb_url}/prop/statement/{pid}> '{value}' .
+          OPTIONAL {{?s <{wb_url}/prop/qualifier/{mrt_pid}> ?mrt}}
         }}
     '''
 
     def __init__(self, value, snak_type, data_type, is_reference, is_qualifier, references, qualifiers, rank, prop_nr,
                  check_qualifier_equality):
         """
         Constructor, will be called by all data types.
@@ -1722,30 +1535,26 @@
         if type(prop_nr) is int:
             self.prop_nr = 'P' + str(prop_nr)
         elif prop_nr.startswith('P'):
             self.prop_nr = prop_nr
         else:
             self.prop_nr = 'P' + prop_nr
 
-        # Flag to allow complete overwrite of existing references for a value
-        self._overwrite_references = False
-
         # Internal ID and hash are issued by the Wikibase instance
         self.id = ''
         self.hash = ''
 
         self.json_representation = {
             "snaktype": self.snak_type,
             "property": self.prop_nr,
             "datavalue": {},
             "datatype": self.data_type
         }
 
-        self.snak_types = ['value', 'novalue', 'somevalue']
-        if snak_type not in self.snak_types:
+        if snak_type not in ['value', 'novalue', 'somevalue']:
             raise ValueError('{} is not a valid snak type'.format(snak_type))
 
         if self.is_qualifier and self.is_reference:
             raise ValueError('A claim cannot be a reference and a qualifer at the same time')
         if (len(self.references) > 0 or len(self.qualifiers) > 0) and (self.is_qualifier or self.is_reference):
             raise ValueError('Qualifiers or references cannot have references')
 
@@ -1786,25 +1595,14 @@
         if not (self.check_qualifier_equality and other.check_qualifier_equality) and nonequal_values:
             return True
         if nonequal_values or not equal_qualifiers:
             return True
         else:
             return False
 
-    # DEPRECATED: the property overwrite_references will be deprecated ASAP and should not be used
-    @property
-    def overwrite_references(self):
-        return self._overwrite_references
-
-    @overwrite_references.setter
-    def overwrite_references(self, value):
-        assert (value is True or value is False)
-        print('DEPRECATED!!! Calls to overwrite_references should not be used')
-        self._overwrite_references = value
-
     @property
     def statement_ref_mode(self):
         return self._statement_ref_mode
 
     @statement_ref_mode.setter
     def statement_ref_mode(self, value):
         """Set the reference mode for a statement, always overrides the global reference state."""
@@ -1863,16 +1661,16 @@
 
     def get_id(self):
         return self.id
 
     def set_id(self, claim_id):
         self.id = claim_id
 
-    def set_hash(self, hash):
-        self.hash = hash
+    def set_hash(self, claim_hash):
+        self.hash = claim_hash
 
     def get_hash(self):
         return self.hash
 
     def get_prop_nr(self):
         return self.prop_nr
 
@@ -1947,26 +1745,14 @@
             return statement
 
     @classmethod
     @JsonParser
     def from_json(cls, json_representation):
         pass
 
-    @classmethod
-    def delete_statement(cls, prop_nr):
-        """
-        This serves as an alternative constructor for BaseDataType with the only purpose of holding a WB property
-        number and an empty string value in order to indicate that the whole statement with this property number of a
-        WB item should be deleted.
-        :param prop_nr: A WB property number as string
-        :return: An instance of BaseDataType
-        """
-        return cls(value='', snak_type='value', data_type='', is_reference=False, is_qualifier=False, references=[],
-                   qualifiers=[], rank='', prop_nr=prop_nr, check_qualifier_equality=True)
-
     def equals(self, that, include_ref=False, fref=None):
         """
         Tests for equality of two statements.
         If comparing references, the order of the arguments matters!!!
         self is the current statement, the next argument is the new statement.
         Allows passing in a function to use to compare the references 'fref'. Default is equality.
         fref accepts two arguments 'oldrefs' and 'newrefs', each of which are a list of references,
@@ -1985,25 +1771,25 @@
     def refs_equal(olditem, newitem):
         """
         tests for exactly identical references
         """
         oldrefs = olditem.references
         newrefs = newitem.references
 
-        ref_equal = lambda oldref, newref: True if (len(oldref) == len(newref)) and all(
-            x in oldref for x in newref) else False
-        if len(oldrefs) == len(newrefs) and all(
-                any(ref_equal(oldref, newref) for oldref in oldrefs) for newref in newrefs):
+        def ref_equal(oldref, newref):
+            return True if (len(oldref) == len(newref)) and all(x in oldref for x in newref) else False
+
+        if len(oldrefs) == len(newrefs) and \
+                all(any(ref_equal(oldref, newref) for oldref in oldrefs) for newref in newrefs):
             return True
         else:
             return False
 
-    """A mixin implementing a simple __repr__."""
-
     def __repr__(self):
+        """A mixin implementing a simple __repr__."""
         return "<{klass} @{id:x} {attrs}>".format(
             klass=self.__class__.__name__,
             id=id(self) & 0xFFFFFF,
             attrs=" ".join("{}={!r}".format(k, v) for k, v in self.__dict__.items()),
         )
 
 
@@ -2170,23 +1956,18 @@
 
 class ItemID(BaseDataType):
     """
     Implements the Wikibase data type with a value being another item ID
     """
     DTYPE = 'wikibase-item'
     sparql_query = '''
-        PREFIX wd: <{wb_url}/entity/>
-        PREFIX wdt: <{wb_url}/prop/direct/>
-        PREFIX p: <{wb_url}/prop/>
-        PREFIX ps: <{wb_url}/prop/statement/>
-        PREFIX pq: <{wb_url}/prop/qualifier/>
         SELECT * WHERE {{
-          ?item_id p:{pid} ?s .
-          ?s ps:{pid} wd:Q{value} .
-          OPTIONAL {{?s pq:{mrt_pid} ?mrt}}
+          ?item_id <{wb_url}/prop/{pid}> ?s .
+          ?s <{wb_url}/prop/statement/{pid}> <{wb_url}/entity/Q{value}> .
+          OPTIONAL {{?s <{wb_url}/prop/qualifier/{mrt_pid}> ?mrt}}
         }}
     '''
 
     def __init__(self, value, prop_nr, is_reference=False, is_qualifier=False, snak_type='value', references=None,
                  qualifiers=None, rank='normal', check_qualifier_equality=True):
         """
         Constructor, calls the superclass BaseDataType
@@ -2254,23 +2035,18 @@
 
 class Property(BaseDataType):
     """
     Implements the Wikibase data type with value 'property'
     """
     DTYPE = 'wikibase-property'
     sparql_query = '''
-        PREFIX wd: <{wb_url}/entity/>
-        PREFIX wdt: <{wb_url}/prop/direct/>
-        PREFIX p: <{wb_url}/prop/>
-        PREFIX ps: <{wb_url}/prop/statement/>
-        PREFIX pq: <{wb_url}/prop/qualifier/>
         SELECT * WHERE {{
-          ?item_id p:{pid} ?s .
-          ?s ps:{pid} wd:P{value} .
-          OPTIONAL {{?s pq:{mrt_pid} ?mrt}}
+          ?item_id <{wb_url}/prop/{pid}> ?s .
+          ?s <{wb_url}/prop/statement/{pid}> <{wb_url}/entity/P{value}> .
+          OPTIONAL {{?s <{wb_url}/prop/qualifier/{mrt_pid}> ?mrt}}
         }}
     '''
 
     def __init__(self, value, prop_nr, is_reference=False, is_qualifier=False, snak_type='value', references=None,
                  qualifiers=None, rank='normal', check_qualifier_equality=True):
         """
         Constructor, calls the superclass BaseDataType
@@ -2339,15 +2115,15 @@
 class Time(BaseDataType):
     """
     Implements the Wikibase data type with date and time values
     """
     DTYPE = 'time'
 
     def __init__(self, time, prop_nr, precision=11, timezone=0, calendarmodel=None,
-                 concept_base_uri=None, is_reference=False, is_qualifier=False, snak_type='value',
+                 wikibase_url=None, is_reference=False, is_qualifier=False, snak_type='value',
                  references=None, qualifiers=None, rank='normal', check_qualifier_equality=True):
         """
         Constructor, calls the superclass BaseDataType
         :param time: A time representation string in the following format: '+%Y-%m-%dT%H:%M:%SZ'
         :type time: str in the format '+%Y-%m-%dT%H:%M:%SZ', e.g. '+2001-12-31T12:01:13Z'
         :param prop_nr: The property number for this claim
         :type prop_nr: str with a 'P' prefix followed by digits
@@ -2369,20 +2145,25 @@
         :param qualifiers: List with qualifier objects
         :type qualifiers: A data type with subclass of BaseDataType
         :param rank: rank of a snak with value 'preferred', 'normal' or 'deprecated'
         :type rank: str
         """
 
         calendarmodel = config['CALENDAR_MODEL_QID'] if calendarmodel is None else calendarmodel
-        concept_base_uri = config['CONCEPT_BASE_URI'] if concept_base_uri is None else concept_base_uri
+        wikibase_url = config['WIKIBASE_URL'] if wikibase_url is None else wikibase_url
+
+        self.time = None
+        self.timezone = None
+        self.precision = None
+        self.calendarmodel = None
 
         if calendarmodel.startswith('Q'):
-            calendarmodel = concept_base_uri + calendarmodel
+            calendarmodel = wikibase_url + '/entity/' + calendarmodel
 
-        # the value is composed of what is requried to define the time object
+        # the value is composed of what is required to define the Time object
         value = (time, timezone, precision, calendarmodel)
 
         super(Time, self).__init__(value=value, snak_type=snak_type, data_type=self.DTYPE, is_reference=is_reference,
                                    is_qualifier=is_qualifier, references=references, qualifiers=qualifiers, rank=rank,
                                    prop_nr=prop_nr, check_qualifier_equality=check_qualifier_equality)
 
         self.set_value(value=value)
@@ -2485,15 +2266,15 @@
 
 class MonolingualText(BaseDataType):
     """
     Implements the Wikibase data type for Monolingual Text strings
     """
     DTYPE = 'monolingualtext'
 
-    def __init__(self, value, prop_nr, language='en', is_reference=False, is_qualifier=False, snak_type='value',
+    def __init__(self, value, prop_nr, language=None, is_reference=False, is_qualifier=False, snak_type='value',
                  references=None, qualifiers=None, rank='normal', check_qualifier_equality=True):
         """
         Constructor, calls the superclass BaseDataType
         :param value: The language specific string to be used as the value
         :type value: str
         :param prop_nr: The item ID for this claim
         :type prop_nr: str with a 'P' prefix followed by digits
@@ -2509,16 +2290,17 @@
         :type references: A data type with subclass of BaseDataType
         :param qualifiers: List with qualifier objects
         :type qualifiers: A data type with subclass of BaseDataType
         :param rank: rank of a snak with value 'preferred', 'normal' or 'deprecated'
         :type rank: str
         """
 
-        self.language = language
-        value = (value, language)
+        self.language = config['DEFAULT_LANGUAGE'] if language is None else language
+
+        value = (value, self.language)
 
         super(MonolingualText, self) \
             .__init__(value=value, snak_type=snak_type, data_type=self.DTYPE, is_reference=is_reference,
                       is_qualifier=is_qualifier, references=references, qualifiers=qualifiers, rank=rank,
                       prop_nr=prop_nr, check_qualifier_equality=check_qualifier_equality)
 
         self.set_value(value)
@@ -2550,15 +2332,15 @@
     """
     Implements the Wikibase data type for quantities
     """
     DTYPE = 'quantity'
 
     def __init__(self, value, prop_nr, upper_bound=None, lower_bound=None, unit='1', is_reference=False,
                  is_qualifier=False, snak_type='value', references=None, qualifiers=None, rank='normal',
-                 check_qualifier_equality=True, concept_base_uri=None):
+                 check_qualifier_equality=True, wikibase_url=None):
         """
         Constructor, calls the superclass BaseDataType
         :param value: The quantity value
         :type value: float, str
         :param prop_nr: The item ID for this claim
         :type prop_nr: str with a 'P' prefix followed by digits
         :param upper_bound: Upper bound of the value if it exists, e.g. for standard deviations
@@ -2577,18 +2359,18 @@
         :type references: A data type with subclass of BaseDataType
         :param qualifiers: List with qualifier objects
         :type qualifiers: A data type with subclass of BaseDataType
         :param rank: rank of a snak with value 'preferred', 'normal' or 'deprecated'
         :type rank: str
         """
 
-        concept_base_uri = config['CONCEPT_BASE_URI'] if concept_base_uri is None else concept_base_uri
+        wikibase_url = config['WIKIBASE_URL'] if wikibase_url is None else wikibase_url
 
         if unit.startswith('Q'):
-            unit = concept_base_uri + unit
+            unit = wikibase_url + '/entity/' + unit
 
         v = (value, unit, upper_bound, lower_bound)
 
         super(Quantity, self).__init__(value=v, snak_type=snak_type, data_type=self.DTYPE,
                                        is_reference=is_reference, is_qualifier=is_qualifier, references=references,
                                        qualifiers=qualifiers, rank=rank, prop_nr=prop_nr,
                                        check_qualifier_equality=check_qualifier_equality)
@@ -2607,15 +2389,15 @@
                 lower_bound = self.format_amount(lower_bound)
 
             # Integrity checks for value and bounds
             try:
                 for i in [value, upper_bound, lower_bound]:
                     if i:
                         float(i)
-            except ValueError as e:
+            except ValueError:
                 raise ValueError('Value, bounds and units must parse as integers or float')
 
             if (lower_bound and upper_bound) and (float(lower_bound) > float(upper_bound)
                                                   or float(lower_bound) > float(value)):
                 raise ValueError('Lower bound too large')
 
             if upper_bound and float(upper_bound) < float(value):
@@ -2650,15 +2432,16 @@
 
         value = jsn['datavalue']['value']
         upper_bound = value['upperBound'] if 'upperBound' in value else None
         lower_bound = value['lowerBound'] if 'lowerBound' in value else None
         return cls(value=value['amount'], prop_nr=jsn['property'], upper_bound=upper_bound,
                    lower_bound=lower_bound, unit=value['unit'])
 
-    def format_amount(self, amount):
+    @staticmethod
+    def format_amount(amount):
         # Remove .0 by casting to int
         if float(amount) % 1 == 0:
             amount = int(float(amount))
 
         # Adding prefix + for positive number and 0
         if not str(amount).startswith('+') and float(amount) >= 0:
             amount = str('+{}'.format(amount))
@@ -2722,15 +2505,15 @@
 class GlobeCoordinate(BaseDataType):
     """
     Implements the Wikibase data type for globe coordinates
     """
     DTYPE = 'globe-coordinate'
 
     def __init__(self, latitude, longitude, precision, prop_nr, globe=None,
-                 concept_base_uri=None, is_reference=False, is_qualifier=False,
+                 wikibase_url=None, is_reference=False, is_qualifier=False,
                  snak_type='value', references=None, qualifiers=None, rank='normal', check_qualifier_equality=True):
         """
         Constructor, calls the superclass BaseDataType
         :param latitude: Latitute in decimal format
         :type latitude: float
         :param longitude: Longitude in decimal format
         :type longitude: float
@@ -2749,18 +2532,23 @@
         :param qualifiers: List with qualifier objects
         :type qualifiers: A data type with subclass of BaseDataType
         :param rank: rank of a snak with value 'preferred', 'normal' or 'deprecated'
         :type rank: str
         """
 
         globe = config['COORDINATE_GLOBE_QID'] if globe is None else globe
-        concept_base_uri = config['CONCEPT_BASE_URI'] if concept_base_uri is None else concept_base_uri
+        wikibase_url = config['WIKIBASE_URL'] if wikibase_url is None else wikibase_url
+
+        self.latitude = None
+        self.longitude = None
+        self.precision = None
+        self.globe = None
 
         if globe.startswith('Q'):
-            globe = concept_base_uri + globe
+            globe = wikibase_url + '/entity/' + globe
 
         value = (latitude, longitude, precision, globe)
 
         super(GlobeCoordinate, self) \
             .__init__(value=value, snak_type=snak_type, data_type=self.DTYPE, is_reference=is_reference,
                       is_qualifier=is_qualifier, references=references, qualifiers=qualifiers, rank=rank,
                       prop_nr=prop_nr, check_qualifier_equality=check_qualifier_equality)
@@ -2835,16 +2623,16 @@
 
     def set_value(self, value):
         assert isinstance(value, str) or value is None, "Expected str, found {} ({})".format(type(value), value)
         pattern = re.compile(r'Data:((?![:|#]).)+\.map')
         matches = pattern.match(value)
 
         if not matches:
-            raise ValueError(
-                'Value must start with Data: and end with .map. In addition title should not contain characters like colon, hash or pipe.')
+            raise ValueError('Value must start with Data: and end with .map. In addition title should not contain '
+                             'characters like colon, hash or pipe.')
 
         self.value = value
 
         self.json_representation['datavalue'] = {
             'value': self.value,
             'type': 'string'
         }
@@ -2951,16 +2739,16 @@
 
     def set_value(self, value):
         assert isinstance(value, str) or value is None, "Expected str, found {} ({})".format(type(value), value)
         pattern = re.compile(r'Data:((?![:|#]).)+\.tab')
         matches = pattern.match(value)
 
         if not matches:
-            raise ValueError(
-                'Value must start with Data: and end with .tab. In addition title should not contain characters like colon, hash or pipe.')
+            raise ValueError('Value must start with Data: and end with .tab. In addition title should not contain '
+                             'characters like colon, hash or pipe.')
 
         self.value = value
 
         self.json_representation['datavalue'] = {
             'value': self.value,
             'type': 'string'
         }
@@ -2977,23 +2765,18 @@
 
 class Lexeme(BaseDataType):
     """
     Implements the Wikibase data type with value 'wikibase-lexeme'
     """
     DTYPE = 'wikibase-lexeme'
     sparql_query = '''
-        PREFIX wd: <{wb_url}/entity/>
-        PREFIX wdt: <{wb_url}/prop/direct/>
-        PREFIX p: <{wb_url}/prop/>
-        PREFIX ps: <{wb_url}/prop/statement/>
-        PREFIX pq: <{wb_url}/prop/qualifier/>
         SELECT * WHERE {{
-          ?item_id p:{pid} ?s .
-          ?s ps:{pid} wd:L{value} .
-          OPTIONAL {{?s pq:{mrt_pid} ?mrt}}
+          ?item_id <{wb_url}/prop/{pid}> ?s .
+          ?s <{wb_url}/prop/statement/{pid}> <{wb_url}/entity/L{value}> .
+          OPTIONAL {{?s <{wb_url}/prop/qualifier/{mrt_pid}> ?mrt}}
         }}
     '''
 
     def __init__(self, value, prop_nr, is_reference=False, is_qualifier=False, snak_type='value', references=None,
                  qualifiers=None, rank='normal', check_qualifier_equality=True):
         """
         Constructor, calls the superclass BaseDataType
@@ -3270,21 +3053,7 @@
 
 class MergeError(Exception):
     def __init__(self, value):
         self.value = value
 
     def __str__(self):
         return repr(self.value)
-
-
-class FormatterWithHeader(logging.Formatter):
-    # http://stackoverflow.com/questions/33468174/write-header-to-a-python-log-file-but-only-if-a-record-gets-written
-    def __init__(self, header, **kwargs):
-        super(FormatterWithHeader, self).__init__(**kwargs)
-        self.header = header
-        # Override the normal format method
-        self.format = self.first_line_format
-
-    def first_line_format(self, record):
-        # First time in, switch back to the normal format function
-        self.format = super(FormatterWithHeader, self).format
-        return self.header + "\n" + self.format(record)
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_fastrun.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_fastrun.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,97 @@
+import collections
 import copy
 from collections import defaultdict
 from functools import lru_cache
 from itertools import chain
 
 from wikibaseintegrator.wbi_config import config
 
-example_Q14911732 = {'P1057':
-                         {'Q14911732-23F268EB-2848-4A82-A248-CF4DF6B256BC':
-                              {'v': 'Q847102',
-                               'ref': {'9d96507726508344ef1b8f59092fb350171b3d99':
-                                           {('P248', 'Q29458763'), ('P594', 'ENSG00000123374')}},
-                               'qual': {('P659', 'Q21067546'), ('P659', 'Q20966585')},
-                               }
-                          }
-                     }
-
 
 class FastRunContainer(object):
     def __init__(self, base_data_type, engine, mediawiki_api_url=None, sparql_endpoint_url=None, wikibase_url=None,
-                 concept_base_uri=None, base_filter=None, use_refs=False, ref_handler=None, case_insensitive=False,
-                 debug=False):
+                 base_filter=None, use_refs=False, ref_handler=None, case_insensitive=False, debug=False):
         self.prop_data = {}
         self.loaded_langs = {}
         self.statements = []
         self.base_filter = {}
         self.base_filter_string = ''
         self.prop_dt_map = {}
         self.current_qid = ''
         self.rev_lookup = defaultdict(set)
         self.rev_lookup_ci = defaultdict(set)
         self.base_data_type = base_data_type
         self.engine = engine
         self.mediawiki_api_url = config['MEDIAWIKI_API_URL'] if mediawiki_api_url is None else mediawiki_api_url
         self.sparql_endpoint_url = config['SPARQL_ENDPOINT_URL'] if sparql_endpoint_url is None else sparql_endpoint_url
         self.wikibase_url = config['WIKIBASE_URL'] if wikibase_url is None else wikibase_url
-        self.concept_base_uri = config['CONCEPT_BASE_URI'] if concept_base_uri is None else concept_base_uri
         self.case_insensitive = case_insensitive
         self.debug = debug
         self.reconstructed_statements = []
         self.use_refs = use_refs
         self.ref_handler = ref_handler
 
         if base_filter and any(base_filter):
             self.base_filter = base_filter
-
             for k, v in self.base_filter.items():
+                ks = []
+                if k.count('/') == 1:
+                    ks = k.split('/')
                 if v:
-                    self.base_filter_string += '?item wdt:{0} wd:{1} . \n'.format(k, v)
+                    if ks:
+                        self.base_filter_string += '?item <{wb_url}/prop/direct/{prop_nr1}>/<{wb_url}/prop/direct/{prop_nr2}>* <{wb_url}/entity/{entity}> .\n'.format(wb_url=self.wikibase_url, prop_nr1=ks[0], prop_nr2=ks[1], entity=v)
+                    else:
+                        self.base_filter_string += '?item <{wb_url}/prop/direct/{prop_nr}> <{wb_url}/entity/{entity}> .\n'.format(wb_url=self.wikibase_url, prop_nr=k, entity=v)
+
                 else:
-                    self.base_filter_string += '?item wdt:{0} ?zz . \n'.format(k)
+                    if ks:
+                        self.base_filter_string += '?item <{wb_url}/prop/direct/{prop_nr1}>/<{wb_url}/prop/direct/{prop_nr2}>* ?zz{prop_nr1}{prop_nr2} .\n'.format(wb_url=self.wikibase_url, prop_nr1=ks[0], prop_nr2=ks[1], entity=v)
+                    else:
+                        self.base_filter_string += '?item <{wb_url}/prop/direct/{prop_nr}> ?zz{prop_nr} .\n'.format(wb_url=self.wikibase_url, prop_nr=k, entity=v)
 
     def reconstruct_statements(self, qid):
         reconstructed_statements = []
+
         if qid not in self.prop_data:
             self.reconstructed_statements = reconstructed_statements
             return reconstructed_statements
+
         for prop_nr, dt in self.prop_data[qid].items():
             # get datatypes for qualifier props
             q_props = set(chain(*[[x[0] for x in d['qual']] for d in dt.values()]))
             r_props = set(chain(*[set(chain(*[[y[0] for y in x] for x in d['ref'].values()])) for d in dt.values()]))
             props = q_props | r_props
             for prop in props:
                 if prop not in self.prop_dt_map:
                     self.prop_dt_map.update({prop: self.get_prop_datatype(prop)})
             # reconstruct statements from frc (including qualifiers, and refs)
             for uid, d in dt.items():
                 qualifiers = []
                 for q in d['qual']:
                     f = [x for x in self.base_data_type.__subclasses__() if x.DTYPE ==
                          self.prop_dt_map[q[0]]][0]
-                    qualifiers.append(f(q[1], prop_nr=q[0], is_qualifier=True))
+                    if self.prop_dt_map[q[0]] == 'quantity' and q[2] != '1':
+                        qualifiers.append(f(q[1], prop_nr=q[0], is_qualifier=True, unit=q[2]))
+                    else:
+                        qualifiers.append(f(q[1], prop_nr=q[0], is_qualifier=True))
 
                 references = []
                 for ref_id, refs in d['ref'].items():
                     this_ref = []
                     for ref in refs:
                         f = [x for x in self.base_data_type.__subclasses__() if x.DTYPE ==
                              self.prop_dt_map[ref[0]]][0]
                         this_ref.append(f(ref[1], prop_nr=ref[0], is_reference=True))
                     references.append(this_ref)
 
                 f = [x for x in self.base_data_type.__subclasses__() if x.DTYPE ==
                      self.prop_dt_map[prop_nr]][0]
                 if self.prop_dt_map[prop_nr] == 'quantity' and d['unit'] != '1':
                     reconstructed_statements.append(
-                        f(d['v'], prop_nr=prop_nr, qualifiers=qualifiers, references=references, unit=d['unit'],
-                          concept_base_uri=self.concept_base_uri))
+                        f(d['v'], prop_nr=prop_nr, qualifiers=qualifiers, references=references, unit=d['unit']))
                 else:
                     reconstructed_statements.append(
                         f(d['v'], prop_nr=prop_nr, qualifiers=qualifiers, references=references))
 
         # this isn't used. done for debugging purposes
         self.reconstructed_statements = reconstructed_statements
         return reconstructed_statements
@@ -143,15 +145,15 @@
         else:
             matching_qids = match_sets[0].intersection(*match_sets[1:])
 
         # check if there are any items that have all of these values
         # if not, a write is required no matter what
         if not len(matching_qids) == 1:
             if self.debug:
-                print('no matches')
+                print('no matches ({})'.format(len(matching_qids)))
             return True
 
         qid = matching_qids.pop()
         self.current_qid = qid
 
     def write_required(self, data, append_props=None, cqid=None):
         del_props = set()
@@ -211,15 +213,16 @@
 
             # this is where the magic happens
             # date is a new statement, proposed to be written
             # tmp_rs are the reconstructed statements == current state of the item
             bool_vec = []
             for x in tmp_rs:
                 if (x.get_value() == date.get_value() or (
-                        self.case_insensitive and x.get_value().casefold() == date.get_value().casefold())) and x.get_prop_nr() not in del_props:
+                        self.case_insensitive and x.get_value().casefold() == date.get_value().casefold())) and \
+                        x.get_prop_nr() not in del_props:
                     if self.use_refs and self.ref_handler:
                         to_be = copy.deepcopy(x)
                         self.ref_handler(to_be, date)
                     else:
                         to_be = date
                     if x.equals(to_be, include_ref=self.use_refs):
                         bool_vec.append(True)
@@ -235,25 +238,26 @@
             if self.debug:
                 print("bool_vec: {}".format(bool_vec))
                 print('-----------------------------------')
                 for x in tmp_rs:
                     if date == x and x.get_prop_nr() not in del_props:
                         print(x.get_prop_nr(), x.get_value(), [z.get_value() for z in x.get_qualifiers()])
                         print(date.get_prop_nr(), date.get_value(), [z.get_value() for z in date.get_qualifiers()])
-                    else:
-                        if x.get_prop_nr() == date.get_prop_nr():
-                            print(x.get_prop_nr(), x.get_value(), [z.get_value() for z in x.get_qualifiers()])
-                            print(date.get_prop_nr(), date.get_value(), [z.get_value() for z in date.get_qualifiers()])
+                    elif x.get_prop_nr() == date.get_prop_nr():
+                        print(x.get_prop_nr(), x.get_value(), [z.get_value() for z in x.get_qualifiers()])
+                        print(date.get_prop_nr(), date.get_value(), [z.get_value() for z in date.get_qualifiers()])
 
             if not any(bool_vec):
                 if self.debug:
                     print(len(bool_vec))
                     print('fast run failed at', date.get_prop_nr())
                 write_required = True
             else:
+                if self.debug:
+                    print('fast run success')
                 tmp_rs.pop(bool_vec.index(True))
 
         if len(tmp_rs) > 0:
             if self.debug:
                 print('failed because not zero')
                 for x in tmp_rs:
                     print('xxx', x.get_prop_nr(), x.get_value(), [z.get_value() for z in x.get_qualifiers()])
@@ -275,15 +279,15 @@
             result = self._query_lang(lang=lang, lang_data_type=lang_data_type)
             data = self._process_lang(result)
             self.loaded_langs[lang].update({lang_data_type: data})
 
     def get_language_data(self, qid, lang, lang_data_type):
         """
         get language data for specified qid
-        :param qid:
+        :param qid:  Wikibase item id
         :param lang: language code
         :param lang_data_type: 'label', 'description' or 'aliases'
         :return: list of strings
         If nothing is found:
             If lang_data_type == label: returns ['']
             If lang_data_type == description: returns ['']
             If lang_data_type == aliases: returns []
@@ -292,55 +296,63 @@
 
         current_lang_data = self.loaded_langs[lang][lang_data_type]
         all_lang_strings = current_lang_data.get(qid, [])
         if not all_lang_strings and lang_data_type in {'label', 'description'}:
             all_lang_strings = ['']
         return all_lang_strings
 
-    def check_language_data(self, qid, lang_data, lang, lang_data_type):
+    def check_language_data(self, qid, lang_data, lang, lang_data_type, if_exists='APPEND'):
         """
         Method to check if certain language data exists as a label, description or aliases
+        :param qid: Wikibase item id
         :param lang_data: list of string values to check
         :type lang_data: list
         :param lang: language code
         :type lang: str
         :param lang_data_type: What kind of data is it? 'label', 'description' or 'aliases'?
-        :return:
+        :param if_exists: If aliases already exist, APPEND or REPLACE
+        :return: boolean
         """
-        all_lang_strings = set(x.strip().lower() for x in self.get_language_data(qid, lang, lang_data_type))
+        all_lang_strings = set(x.strip().casefold() for x in self.get_language_data(qid, lang, lang_data_type))
 
-        for s in lang_data:
-            if s.strip().lower() not in all_lang_strings:
-                print('fastrun failed at label: {}, string: {}'.format(lang_data_type, s))
-                return True
+        if if_exists == 'REPLACE':
+            return not collections.Counter(all_lang_strings) == collections.Counter(map(lambda x: x.casefold(),
+                                                                                        lang_data))
+        else:
+            for s in lang_data:
+                if s.strip().casefold() not in all_lang_strings:
+                    if self.debug:
+                        print('fastrun failed at: {}, string: {}'.format(lang_data_type, s))
+                    return True
 
         return False
 
     def get_all_data(self):
         return self.prop_data
 
     def format_query_results(self, r, prop_nr):
         """
         `r` is the results of the sparql query in _query_data and is modified in place
         `prop_nr` is needed to get the property datatype to determine how to format the value
 
         `r` is a list of dicts. The keys are:
+            sid: statement ID
             item: the subject. the item this statement is on
             v: the object. The value for this statement
-            sid: statement ID
+            unit: property unit
             pq: qualifier property
             qval: qualifier value
+            qunit: qualifier unit
             ref: reference ID
             pr: reference property
             rval: reference value
-            unit: property unit
         """
         prop_dt = self.get_prop_datatype(prop_nr)
         for i in r:
-            for value in {'item', 'sid', 'pq', 'pr', 'ref', 'unit'}:
+            for value in {'item', 'sid', 'pq', 'pr', 'ref', 'unit', 'qunit'}:
                 if value in i:
                     # these are always URIs for the local wikibase
                     i[value] = i[value]['value'].split('/')[-1]
 
             # make sure datetimes are formatted correctly.
             # the correct format is '+%Y-%m-%dT%H:%M:%SZ', but is sometimes missing the plus??
             # some difference between RDF and xsd:dateTime that I don't understand
@@ -369,26 +381,29 @@
                         self.rev_lookup_ci[i['v'].casefold()].add(i['item'])
 
             # handle qualifier value
             if 'qval' in i:
                 qual_prop_dt = self.get_prop_datatype(prop_nr=i['pq'])
                 if i['qval']['type'] == 'uri' and qual_prop_dt == 'wikibase-item':
                     i['qval'] = i['qval']['value'].split('/')[-1]
+                elif i['qval']['type'] == 'literal' and qual_prop_dt == 'quantity':
+                    i['qval'] = self.format_amount(i['qval']['value'])
                 else:
                     i['qval'] = i['qval']['value']
 
             # handle reference value
             if 'rval' in i:
                 ref_prop_dt = self.get_prop_datatype(prop_nr=i['pr'])
                 if i['rval']['type'] == 'uri' and ref_prop_dt == 'wikibase-item':
                     i['rval'] = i['rval']['value'].split('/')[-1]
                 else:
                     i['rval'] = i['rval']['value']
 
-    def format_amount(self, amount):
+    @staticmethod
+    def format_amount(amount):
         # Remove .0 by casting to int
         if float(amount) % 1 == 0:
             amount = int(float(amount))
 
         # Adding prefix + for positive number and 0
         if not str(amount).startswith('+') and float(amount) >= 0:
             amount = str('+{}'.format(amount))
@@ -410,130 +425,151 @@
             # update values for this statement (not including ref)
             d = {'v': i['v']}
             self.prop_data[qid][prop_nr][i['sid']].update(d)
 
             if 'qual' not in self.prop_data[qid][prop_nr][i['sid']]:
                 self.prop_data[qid][prop_nr][i['sid']]['qual'] = set()
             if 'pq' in i and 'qval' in i:
-                self.prop_data[qid][prop_nr][i['sid']]['qual'].add((i['pq'], i['qval']))
+                if 'qunit' in i:
+                    self.prop_data[qid][prop_nr][i['sid']]['qual'].add((i['pq'], i['qval'], i['qunit']))
+                else:
+                    self.prop_data[qid][prop_nr][i['sid']]['qual'].add((i['pq'], i['qval'], '1'))
 
             if 'ref' not in self.prop_data[qid][prop_nr][i['sid']]:
                 self.prop_data[qid][prop_nr][i['sid']]['ref'] = dict()
             if 'ref' in i:
                 if i['ref'] not in self.prop_data[qid][prop_nr][i['sid']]['ref']:
                     self.prop_data[qid][prop_nr][i['sid']]['ref'][i['ref']] = set()
                 self.prop_data[qid][prop_nr][i['sid']]['ref'][i['ref']].add((i['pr'], i['rval']))
 
             if 'unit' not in self.prop_data[qid][prop_nr][i['sid']]:
                 self.prop_data[qid][prop_nr][i['sid']]['unit'] = '1'
             if 'unit' in i:
                 self.prop_data[qid][prop_nr][i['sid']]['unit'] = i['unit']
 
-    def _query_data_refs(self, prop_nr):
+    def _query_data(self, prop_nr):
         page_size = 10000
         page_count = 0
         num_pages = None
         if self.debug:
             # get the number of pages/queries so we can show a progress bar
-            query = """PREFIX wd: <{0}/entity/>
-            PREFIX wdt: <{0}/prop/direct/>
-            PREFIX p: <{0}/prop/>
-            PREFIX ps: <{0}/prop/statement/>
-
+            query = """
             SELECT (COUNT(?item) as ?c) where {{
-                  {1}
-                  ?item p:{2} ?sid .
-            }}""".format(self.wikibase_url, self.base_filter_string, prop_nr)
+                  {base_filter}
+                  ?item <{wb_url}/prop/{prop_nr}> ?sid .
+            }}""".format(wb_url=self.wikibase_url, base_filter=self.base_filter_string, prop_nr=prop_nr)
 
             if self.debug:
                 print(query)
 
             r = self.engine.execute_sparql_query(query, endpoint=self.sparql_endpoint_url)['results']['bindings']
             count = int(r[0]['c']['value'])
             num_pages = (int(count) // page_size) + 1
             print("Query {}: {}/{}".format(prop_nr, page_count, num_pages))
         while True:
-            query = """
-                PREFIX wd: <**wikibase_url**/entity/>
-                PREFIX wdt: <**wikibase_url**/prop/direct/>
-                PREFIX p: <**wikibase_url**/prop/>
-                PREFIX ps: <**wikibase_url**/prop/statement/>
-                #Tool: wbi_core fastrun
-                SELECT ?item ?qval ?pq ?sid ?v ?ref ?pr ?rval WHERE {
-                  {
-                    SELECT ?item ?v ?sid where {
-                      **base_filter_string**
-                      ?item p:**prop_nr** ?sid .
-                      ?sid ps:**prop_nr** ?v .
-                    } GROUP BY ?item ?v ?sid
-                    ORDER BY ?sid
-                    OFFSET **offset**
-                    LIMIT **page_size**
-                  }
-                  OPTIONAL {
-                    ?sid ?pq ?qval .
-                    [] wikibase:qualifier ?pq
-                  }
-                  OPTIONAL {
-                    ?sid prov:wasDerivedFrom ?ref .
-                    ?ref ?pr ?rval .
-                    [] wikibase:reference ?pr
-                  }
-                }""".replace("**offset**", str(page_count * page_size)). \
-                replace("**base_filter_string**", self.base_filter_string). \
-                replace("**prop_nr**", prop_nr).replace("**page_size**", str(page_size)). \
-                replace("**wikibase_url**", self.wikibase_url)
+            if self.use_refs:
+                query = '''
+                    #Tool: wbi_fastrun _query_data_refs
+                    SELECT ?sid ?item ?v ?unit ?pq ?qval ?qunit ?ref ?pr ?rval
+                    WHERE
+                    {{
+                      {base_filter}
+
+                      # Get amount and unit for the statement
+                      ?item <{wb_url}/prop/{prop_nr}> ?sid .
+                      {{
+                        <{wb_url}/entity/{prop_nr}> wikibase:propertyType ?property_type .
+                        FILTER (?property_type != wikibase:Quantity)
+                        ?sid <{wb_url}/prop/statement/{prop_nr}> ?v .
+                      }}
+                      UNION
+                      {{
+                        ?sid <{wb_url}/prop/statement/value/{prop_nr}> [wikibase:quantityAmount ?v; wikibase:quantityUnit ?unit] .
+                      }}
+
+                      # Get qualifiers
+                      OPTIONAL
+                      {{
+                        {{
+                          # Get simple values for qualifiers which are not of type quantity
+                          ?sid ?propQualifier ?qval .
+                          ?pq wikibase:qualifier ?propQualifier .
+                          ?pq wikibase:propertyType ?qualifer_property_type .
+                          FILTER (?qualifer_property_type != wikibase:Quantity)
+                        }}
+                        UNION
+                        {{
+                          # Get amount and unit for qualifiers of type quantity
+                          ?sid ?pqv [wikibase:quantityAmount ?qval; wikibase:quantityUnit ?qunit] .
+                          ?pq wikibase:qualifierValue ?pqv .
+                        }}
+                      }}
+
+                      # get references
+                      OPTIONAL {{
+                        ?sid prov:wasDerivedFrom ?ref .
+                        ?ref ?pr ?rval .
+                        [] wikibase:reference ?pr
+                      }}
+                    }} ORDER BY ?sid OFFSET {offset} LIMIT {page_size}
+                    '''.format(wb_url=self.wikibase_url, base_filter=self.base_filter_string, prop_nr=prop_nr,
+                               offset=str(page_count * page_size), page_size=str(page_size))
+            else:
+                query = '''
+                    #Tool: wbi_fastrun _query_data
+                    SELECT ?sid ?item ?v ?unit ?pq ?qval ?qunit
+                    WHERE
+                    {{
+                      {base_filter}
+
+                      # Get amount and unit for the statement
+                      ?item <{wb_url}/prop/{prop_nr}> ?sid .
+                      {{
+                        <{wb_url}/entity/{prop_nr}> wikibase:propertyType ?property_type .
+                        FILTER (?property_type != wikibase:Quantity)
+                        ?sid <{wb_url}/prop/statement/{prop_nr}> ?v .
+                      }}
+                      UNION
+                      {{
+                        ?sid <{wb_url}/prop/statement/value/{prop_nr}> [wikibase:quantityAmount ?v; wikibase:quantityUnit ?unit] .
+                      }}
+
+                      # Get qualifiers
+                      OPTIONAL
+                      {{
+                        {{
+                          # Get simple values for qualifiers which are not of type quantity
+                          ?sid ?propQualifier ?qval .
+                          ?pq wikibase:qualifier ?propQualifier .
+                          ?pq wikibase:propertyType ?qualifer_property_type .
+                          FILTER (?qualifer_property_type != wikibase:Quantity)
+                        }}
+                        UNION
+                        {{
+                          # Get amount and unit for qualifiers of type quantity
+                          ?sid ?pqv [wikibase:quantityAmount ?qval; wikibase:quantityUnit ?qunit] .
+                          ?pq wikibase:qualifierValue ?pqv .
+                        }}
+                      }}
+                    }} ORDER BY ?sid OFFSET {offset} LIMIT {page_size}
+                    '''.format(wb_url=self.wikibase_url, base_filter=self.base_filter_string, prop_nr=prop_nr,
+                               offset=str(page_count * page_size), page_size=str(page_size))
 
             if self.debug:
                 print(query)
 
-            results = self.engine.execute_sparql_query(query, endpoint=self.sparql_endpoint_url)['results']['bindings']
+            results = self.engine.execute_sparql_query(query=query, endpoint=self.sparql_endpoint_url)['results']['bindings']
             self.format_query_results(results, prop_nr)
             self.update_frc_from_query(results, prop_nr)
             page_count += 1
             if num_pages:
                 print("Query {}: {}/{}".format(prop_nr, page_count, num_pages))
-            if len(results) == 0:
+            if len(results) == 0 or len(results) < page_size:
                 break
 
-    def _query_data(self, prop_nr):
-        if self.use_refs:
-            self._query_data_refs(prop_nr)
-        else:
-            query = '''
-                PREFIX wd: <{0}/entity/>
-                PREFIX wdt: <{0}/prop/direct/>
-                PREFIX p: <{0}/prop/>
-                PREFIX ps: <{0}/prop/statement/>
-                PREFIX psv: <{0}/prop/statement/value/>
-                #Tool: wbi_core fastrun
-                select ?item ?qval ?pq ?sid ?v ?unit where {{
-                  {1}
-
-                  ?item p:{2} ?sid .
-
-                  ?sid ps:{2} ?v .
-                  OPTIONAL {{
-                    ?sid ?pq ?qval .
-                    [] wikibase:qualifier ?pq
-                  }}
-                  OPTIONAL {{
-                    ?sid psv:{2} ?valuenode .
-                    ?valuenode wikibase:quantityUnit ?unit
-                  }}
-                }}
-                '''.format(self.wikibase_url, self.base_filter_string, prop_nr)
-
-            if self.debug:
-                print(query)
-
-            r = self.engine.execute_sparql_query(query=query, endpoint=self.sparql_endpoint_url)['results']['bindings']
-            self.format_query_results(r, prop_nr)
-            self.update_frc_from_query(r, prop_nr)
-
     def _query_lang(self, lang, lang_data_type):
         """
 
         :param lang:
         :param lang_data_type:
         :return:
         """
@@ -541,27 +577,23 @@
         lang_data_type_dict = {
             'label': 'rdfs:label',
             'description': 'schema:description',
             'aliases': 'skos:altLabel'
         }
 
         query = '''
-        PREFIX wd: <{0}/entity/>
-        PREFIX wdt: <{0}/prop/direct/>
-        PREFIX p: <{0}/prop/>
-        PREFIX ps: <{0}/prop/statement/>
-        #Tool: wbi_core fastrun
+        #Tool: wbi_fastrun _query_lang
         SELECT ?item ?label WHERE {{
-            {1}
+            {base_filter}
 
             OPTIONAL {{
-                ?item {2} ?label FILTER (lang(?label) = "{3}") .
+                ?item {lang_data_type} ?label FILTER (lang(?label) = "{lang}") .
             }}
         }}
-        '''.format(self.wikibase_url, self.base_filter_string, lang_data_type_dict[lang_data_type], lang)
+        '''.format(base_filter=self.base_filter_string, lang_data_type=lang_data_type_dict[lang_data_type], lang=lang)
 
         if self.debug:
             print(query)
 
         return self.engine.execute_sparql_query(query=query, endpoint=self.sparql_endpoint_url)['results']['bindings']
 
     @staticmethod
@@ -585,15 +617,14 @@
         convinience function to empty this fastrun container
         """
         self.prop_dt_map = dict()
         self.prop_data = dict()
         self.rev_lookup = defaultdict(set)
         self.rev_lookup_ci = defaultdict(set)
 
-    """A mixin implementing a simple __repr__."""
-
     def __repr__(self):
+        """A mixin implementing a simple __repr__."""
         return "<{klass} @{id:x} {attrs}>".format(
             klass=self.__class__.__name__,
             id=id(self) & 0xFFFFFF,
             attrs="\r\n\t ".join("{}={!r}".format(k, v) for k, v in self.__dict__.items()),
         )
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator/wbi_login.py` & `wikibaseintegrator-0.9.0/wikibaseintegrator/wbi_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     def __init__(self, user=None, pwd=None, mediawiki_api_url=None, mediawiki_index_url=None, token_renew_period=1800,
                  use_clientlogin=False, consumer_key=None, consumer_secret=None, callback_url='oob', user_agent=None,
                  debug=False):
         """
         This class handles several types of login procedures. Either use user and pwd authentication or OAuth.
         Wikidata clientlogin can also be used. If using one method, do NOT pass parameters for another method.
         :param user: the username which should be used for the login
+        :type user: str
         :param pwd: the password which should be used for the login
+        :type pwd: str
         :param token_renew_period: Seconds after which a new token should be requested from the Wikidata server
         :type token_renew_period: int
         :param use_clientlogin: use authmanager based login method instead of standard login.
             For 3rd party data consumer, e.g. web clients
         :type use_clientlogin: bool
         :param consumer_key: The consumer key for OAuth
         :type consumer_key: str
@@ -62,15 +64,15 @@
         self.response_qs = None
         self.callback_url = callback_url
 
         if user_agent:
             self.user_agent = user_agent
         else:
             # if a user is given append " (User:USER)" to the UA string and update that value in CONFIG
-            if user and user.lower() not in config['USER_AGENT_DEFAULT'].lower():
+            if user and user.casefold() not in config['USER_AGENT_DEFAULT'].casefold():
                 config['USER_AGENT_DEFAULT'] += " (User:{})".format(user)
             self.user_agent = config['USER_AGENT_DEFAULT']
         self.s.headers.update({
             'User-Agent': self.user_agent
         })
 
         if self.consumer_key and self.consumer_secret:
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator.egg-info/PKG-INFO` & `wikibaseintegrator-0.9.0/wikibaseintegrator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: wikibaseintegrator
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python package for reading and writing to/from Wikibase
-Home-page: https://github.com/Mystou/WikibaseIntegrator
+Home-page: https://github.com/LeMyst/WikibaseIntegrator
 Author: Myst and WikidataIntegrator authors
 License: MIT
 Description: # Wikibase Integrator #
-        [![Build Status](https://travis-ci.org/Mystou/WikibaseIntegrator.svg?branch=master)](https://travis-ci.org/Mystou/WikibaseIntegrator)
+        [![Build Status](https://travis-ci.org/LeMyst/WikibaseIntegrator.svg?branch=master)](https://travis-ci.org/LeMyst/WikibaseIntegrator)
         [![Pyversions](https://img.shields.io/pypi/pyversions/wikibaseintegrator.svg)](https://pypi.python.org/pypi/wikibaseintegrator)
         [![PyPi](https://img.shields.io/pypi/v/wikibaseintegrator.svg)](https://pypi.python.org/pypi/wikibaseintegrator)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Mystou/WikibaseIntegrator/master)
         
         # WikibaseIntegrator / WikidataIntegrator #
-        WikibaseIntegrator (wbi) is a fork from [WikidataIntegrator](https://github.com/SuLab/WikidataIntegrator) (wdi) whose purpose is to be focused on Wikibase only.
+        WikibaseIntegrator (wbi) is a fork from [WikidataIntegrator](https://github.com/SuLab/WikidataIntegrator) (wdi) whose purpose is to be focused on Wikibase compatibility.
         The main changes are :
         * Rename the files from wdi_ to wbi_ to avoid confusion
         * Removal of wdi_helpers from the repository
         * Removal of references handlers from the repository, but they can still be used with the ItemEngine
         
         Wikidata is always the default endpoint for all functions.
         
@@ -48,27 +47,31 @@
           * WDTabularData -> TabularData
           * WDTime -> Time
           * WDUrl -> Url
         * ItemEngine parameter changes:
           * wd_item_id -> item_id
         * ItemEngine attribute changes:
           * wd_item_id -> item_id
+        * Change wbi_core.set_aliases parameter named 'append' to 'if_exists' with a value of APPEND (default) or REPLACE
+        * Remove CONCEPT_BASE_URI wbi_config option and classes' parameter. It's now derived from WIKIBASE_URL.
+        * wbi_core.log() has been removed. Please use your own logging implementation.
         
         # Installation #
-        The easiest way to install WikibaseIntegrator is using `pip` or `pip3`. WikibaseIntegrator supports python 3.6 and higher, hence the suggestion for pip3. If python2 is installed pip will lead to an error indicating missing dependencies. 
+        The easiest way to install WikibaseIntegrator is using `pip` or `pip3`.
+        WikibaseIntegrator supports python 3.6 and higher, hence the suggestion for pip3.
+        If python2 is installed pip will lead to an error indicating missing dependencies. 
         
-        ```
+        ```bash
         pip3 install wikibaseintegrator
         ```
         
         You can also clone the repo and execute with administrator rights or install into a virtualenv.
         
         ```bash
-        
-        git clone https://github.com/Mystou/WikibaseIntegrator.git
+        git clone https://github.com/LeMyst/WikibaseIntegrator.git
         
         cd WikibaseIntegrator
         
         python3 setup.py install
         ```
         
         To test for correct installation, start a python console and execute the following (Will retrieve the Wikidata item for ['Human'](https://www.wikidata.org/entity/Q5)):
@@ -80,69 +83,68 @@
         
         # to check successful installation and retrieval of the data, you can print the json representation of the item
         print(my_first_wikidata_item.get_json_representation())
         ```
         
         # The Core Parts #
         
-        wbi_core supports two modes it can be operated in, a normal mode, updating each item at a time and a 'fastrun' mode, which is pre-loading data locally and then just updating items if the new data provided is differing from what is in Wikidata. The latter mode allows for great speedups (measured up to 9x) when tens of thousand of Wikidata 
-        items need to be checked if they require updates but only a small number will finally be updated, a situation usually encountered when keeping Wikidata in sync with an external resource. 
+        wbi_core supports two modes it can be operated in, a normal mode, updating each item at a time and a 'fastrun' mode, which is pre-loading data locally and then just updating items if the new data provided is differing from what is in Wikidata.
+        The latter mode allows for great speedups (measured up to 9x) when tens of thousand of Wikidata items need to be checked if they require updates but only a small number will finally be updated, a situation usually encountered when keeping Wikidata in sync with an external resource. 
         
         wbi_core consists of a central class called ItemEngine and Login for authenticating with Wikidata/Wikipedia.
         
         ## wbi_core.ItemEngine ##
         This is the central class which does all the heavy lifting.
         
         Features:
-        
-         * Load a Wikibase item based on data to be written (e.g. a unique central identifier)
-         * Load a Wikibase item based on its Wikibase item id (aka QID)
-         * Checks for conflicts automatically (e.g. multiple items carrying a unique central identifier will trigger an exception)
-         * Checks automatically if the correct item has been loaded by comparing it to the data provided
-         * All Wikibase data types implemented
-         * A dedicated ItemEngine.write() method allows loading and consistency checks of data before any write to Wikibase is performed
-         * Full access to the whole Wikibase item as a JSON document
-         * Minimize the number of HTTP requests for reads and writes to improve performance
-         * Method to easily execute [SPARQL](https://query.wikidata.org) queries on the Wikibase SPARQL endpoint. 
+        * Load a Wikibase item based on data to be written (e.g. a unique central identifier)
+        * Load a Wikibase item based on its Wikibase item id (aka QID)
+        * Checks for conflicts automatically (e.g. multiple items carrying a unique central identifier will trigger an exception)
+        * Checks automatically if the correct item has been loaded by comparing it to the data provided
+        * All Wikibase data types implemented
+        * A dedicated ItemEngine.write() method allows loading and consistency checks of data before any write to Wikibase is performed
+        * Full access to the whole Wikibase item as a JSON document
+        * Minimize the number of HTTP requests for reads and writes to improve performance
+        * Method to easily execute [SPARQL](https://query.wikidata.org) queries on the Wikibase SPARQL endpoint. 
          
         There are two ways of working with Wikibase items: 
-        
         * A user can provide data, and ItemEngine will search for and load/modify an existing item or create a new one, solely based on the data provided (preferred). This also performs consistency checks based on a set of SPARQL queries. 
         * A user can work with a selected QID to specifically modify the data on the item. This requires that the user knows what he/she is doing and should only be used with great care, as this does not perform consistency checks. 
         
         Examples below illustrate the usage of ItemEngine.
         
         ## wbi_login.Login ##
         
         ### Login with username and password ###
         wbi_login.Login provides the login functionality and also stores the cookies and edit tokens required (For security reasons, every Mediawiki edit requires an edit token).
         The constructor takes two essential parameters, username and password. Additionally, the server (default wikidata.org) and the the token renewal periods can be specified. 
         
-        ```Python     
+        ```python
+        from wikibaseintegrator import wbi_login
+        
         login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')     
         ```
         
         ### Login using OAuth1 ###
-        The Wikimedia universe currently only support authentication via OAuth1. If WBI should be used as a backend for a webapp or the bot should use OAuth for authentication, WBI supports this
-        You just need to specify consumer token and consumer secret when instantiating wbi_login.Login. In contrast to username and password login, OAuth is a 2 step process as manual user confirmation
-        for OAuth login is required. This means that the method continue_oath() needs to be called after creating the wbi_login.Login instance.
+        The Wikimedia universe currently only support authentication via OAuth1. If WBI should be used as a backend for a webapp or the bot should use OAuth for authentication, WBI supports this, you just need to specify consumer key and consumer secret when instantiating wbi_login.Login.
+        In contrast to username and password login, OAuth is a 2 step process as manual user confirmation for OAuth login is required. This means that the method continue_oauth() needs to be called after creating the wbi_login.Login instance.
         
         Example:
-        ```Python     
-        login_instance = wbi_login.Login(consumer_token='<your_consumer_token>', pwd='<your_consumer_secret>')
+        ```python
+        from wikibaseintegrator import wbi_login
+        
+        login_instance = wbi_login.Login(consumer_key='<your_consumer_key>', consumer_secret='<your_consumer_secret>')
         login_instance.continue_oauth()
         ```
         
-        The method continue_oauth() will either promt the user for a callback URL (normal bot runs) or it will take a parameter so in the case of WBI being
-        used as a backend for e.g. a web app, where the callback will provide the authentication information directly to the backend and so
-         no copy and paste of the callback URL is required.
+        The method continue_oauth() will either prompt the user for a callback URL (normal bot runs) or it will take a parameter so in the case of WBI being used as a backend for e.g. a web app, where the callback will provide the authentication information directly to the backend and so no copy and paste of the callback URL is required.
         
         ## Wikibase Data Types ##
-        Currently, Wikibase supports 17 different data types. The data types are represented as their own classes in wbi_core. Each data type has its specialties, which means that some of them
-        require special parameters (e.g. Globe Coordinates).
+        Currently, Wikibase supports 17 different data types. The data types are represented as their own classes in wbi_core.
+        Each data type has its specialties, which means that some of them require special parameters (e.g. Globe Coordinates).
         
         The data types currently implemented:
         * wbi_core.CommonsMedia
         * wbi_core.ExternalID
         * wbi_core.Form
         * wbi_core.GeoShape
         * wbi_core.GlobeCoordinate
@@ -155,57 +157,49 @@
         * wbi_core.Quantity
         * wbi_core.Sense
         * wbi_core.String
         * wbi_core.TabularData
         * wbi_core.Time
         * wbi_core.Url
         
-        For details of how to create values (=instances) with these data types, please (for now) consult the docstrings in the source code. Of note, these data type instances hold the values and, if specified,
-        data type instances for references and qualifiers. Furthermore, calling the get_value() method of an instance returns either an integer, a string or a tuple, depending on the complexity of the data type.
+        For details of how to create values (=instances) with these data types, please (for now) consult the docstrings in the source code.
+        Of note, these data type instances hold the values and, if specified, data type instances for references and qualifiers.
+        Furthermore, calling the get_value() method of an instance returns either an integer, a string or a tuple, depending on the complexity of the data type.
         
         # Helper Methods #
         
         ## Execute SPARQL queries ##
-        The method wbi_core.ItemEngine.execute_sparql_query() allows you to execute SPARQL queries without a hassle. It takes the actual
-        query string (query), optional prefixes (prefix) if you do not want to use the standard prefixes of Wikidata, the actual entpoint URL (endpoint),
-        and you can also specify a user agent for the http header sent to the SPARQL server (user_agent). The latter is very useful to let
-        the operators of the endpoint know who you are, especially if you execute many queries on the endpoint. This allows the operators of
-        the endpoint to contact you (e.g. specify a email address or the URL to your bot code repository.)
-        
-        ## Logging ##
-        The method wbi_core.ItemEngine.log() allows for using the Python built in logging functionality to collect errors and other logs.
-        It takes two parameters, the log level (level) and the log message (message). It is advisable to separate log file columns by colons
-        and always use the same number of fields, as this allows you to load the log file into databases or dataframes of R or Python.
+        The method wbi_core.ItemEngine.execute_sparql_query() allows you to execute SPARQL queries without a hassle.
+        It takes the actual query string (query), optional prefixes (prefix) if you do not want to use the standard prefixes of Wikidata, the actual entpoint URL (endpoint), and you can also specify a user agent for the http header sent to the SPARQL server (user_agent).
+        The latter is very useful to let the operators of the endpoint know who you are, especially if you execute many queries on the endpoint.
+        This allows the operators of the endpoint to contact you (e.g. specify a email address or the URL to your bot code repository.)
         
         ## Wikidata Search ##
-        The method wbi_core.ItemEngine.get_search_results() allows for string search in a Wikibase instance. This means that
-        labels, descriptions and aliases can be searched for a string of interest. The method takes five arguments:
-        The actual search string (search_string), an optional server (mediawiki_api_url, in case the Wikibase instance used is not Wikidata),
-        an optional user_agent, an optional max_results (default 500), an optional language (default 'en') and an option dict_id_label to return a dict of
-        item id and label as a result.
+        The method wbi_core.ItemEngine.get_search_results() allows for string search in a Wikibase instance.
+        This means that labels, descriptions and aliases can be searched for a string of interest.
+        The method takes five arguments: The actual search string (search_string), an optional server (mediawiki_api_url, in case the Wikibase instance used is not Wikidata), an optional user_agent, an optional max_results (default 500), an optional language (default 'en') and an option dict_id_label to return a dict of item id and label as a result.
          
         ## Merge Wikibase items ##
-        Sometimes, Wikibase items need to be merged. An API call exists for that, and wbi_core implements a method accordingly.
-        `wbi_core.ItemEngine.merge_items(from_id, to_id, login_obj)` takes five arguments: the QID of the item which should be
-        merged into another item (from_id), the QID of the item the first item should be
-        merged into (to_id), a login object of type wbi_login.Login() (login_obj) to provide the API call with the required authentication
-        information, a server (mediawiki_api_url) if the Wikibase instance is not Wikidata and a flag for ignoring merge conflicts (ignore_conflicts).
-        The last parameter will do a partial merge for all statements which do not conflict. This should generally be avoided because it 
-        leaves a crippled item in Wikibase. Before a merge, any potential conflicts should be resolved first.
+        Sometimes, Wikibase items need to be merged.
+        An API call exists for that, and wbi_core implements a method accordingly.
+        `wbi_core.ItemEngine.merge_items(from_id, to_id, login_obj)` takes five arguments:
+        the QID of the item which should be merged into another item (from_id), the QID of the item the first item should be merged into (to_id), a login object of type wbi_login.Login() to provide the API call with the required authentication information, a server (mediawiki_api_url) if the Wikibase instance is not Wikidata and a flag for ignoring merge conflicts (ignore_conflicts).
+        The last parameter will do a partial merge for all statements which do not conflict.
+        This should generally be avoided because it leaves a crippled item in Wikibase. Before a merge, any potential conflicts should be resolved first.
         
         # Examples (in normal mode) #
         
         ## A Minimal Bot ##
         In order to create a minimal bot based on wbi_core, three things are required:
         
         * A login object, as described above.
         * A data type object containing a value.
         * A ItemEngine object which takes the data, does the checks and performs the write.
         
-        ```Python
+        ```python
         from wikibaseintegrator import wbi_core, wbi_login
             
         # login object
         login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')
              
         # data type object, e.g. for a NCBI gene entrez ID
         entrez_gene_id = wbi_core.String(value='<some_entrez_id>', prop_nr='P351')
@@ -217,15 +211,15 @@
         wd_item = wbi_core.ItemEngine(data=data)
         wd_item.write(login_instance)
         ```
         
         ## A Minimal Bot for Mass Import ##
         An enhanced example of the previous bot just puts two of the three things into a for loop and so allows mass creation, or modification of items.
         
-        ```Python
+        ```python
         from wikibaseintegrator import wbi_core, wbi_login
             
         # login object
         login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')
         
         # We have raw data, which should be written to Wikidata, namely two human NCBI entrez gene IDs mapped to two Ensembl Gene IDs
         raw_data = {
@@ -253,20 +247,20 @@
         
         IMPORTANT: In order for the fast run mode to work, the data you provide in the constructor must contain at least one unique value/id only present on one Wikidata item, e.g. an NCBI entrez gene ID, Uniprot ID, etc.
         Usually, these would be the same unique core properties used for defining domains in wbi_core, e.g. for genes, proteins, drugs or your custom domains.
         
         Below, the normal mode run example from above, slightly modified, to meet the requirements for the fastrun mode. To enable it, ItemEngine requires two parameters, fast_run=True/False and fast_run_base_filter which 
          is a dictionary holding the properties to filter for as keys and the item QIDs as dict values. If the value is not a QID but a literal, just provide an empty string. For the above example, the dictionary looks like this:
          
-        ```Python
+        ```python
         fast_run_base_filter = {'P351': '', 'P703': 'Q15978631'}
         ```
          
         The full example:
-        ```Python
+        ```python
         from wikibaseintegrator import wbi_core, wbi_login
             
         # login object
         login_instance = wbi_login.Login(user='<bot user name>', pwd='<bot password>')
         
         fast_run_base_filter = {'P351': '', 'P703': 'Q15978631'}
         fast_run = True
@@ -287,15 +281,16 @@
             data = [entrez_gene_id, ensembl_transcript_id]
             
             # Search for and then edit/create new item
             wd_item = wbi_core.ItemEngine(data=data, fast_run=fast_run, fast_run_base_filter=fast_run_base_filter)
             wd_item.write(login_instance)
         ```
         
-        Note: Fastrun mode checks for equality of property/value pairs, qualifers (not including qualifier attributes), labels, aliases and description, but it ignores references by default! References can be checked in fastrun mode by setting `fast_run_use_refs` to `True`.
+        Note: Fastrun mode checks for equality of property/value pairs, qualifers (not including qualifier attributes), labels, aliases and description, but it ignores references by default!
+        References can be checked in fastrun mode by setting `fast_run_use_refs` to `True`.
         
 Keywords: Wikibase
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -304,7 +299,8 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `wikibaseintegrator-0.8.2/wikibaseintegrator.egg-info/SOURCES.txt` & `wikibaseintegrator-0.9.0/wikibaseintegrator.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 wikibaseintegrator/wbi_login.py
 wikibaseintegrator.egg-info/PKG-INFO
 wikibaseintegrator.egg-info/SOURCES.txt
 wikibaseintegrator.egg-info/dependency_links.txt
 wikibaseintegrator.egg-info/requires.txt
 wikibaseintegrator.egg-info/top_level.txt
 wikibaseintegrator/tests/__init__.py
+wikibaseintegrator/tests/test_all.py
 wikibaseintegrator/tests/test_backoff.py
 wikibaseintegrator/tests/test_fastrun.py
 wikibaseintegrator/tests/test_item_creation.py
 wikibaseintegrator/tests/test_item_generator.py
 wikibaseintegrator/tests/test_wd_search.py
-wikibaseintegrator/tests/test_wdi_login.py
-wikibaseintegrator/tests/tests.py
+wikibaseintegrator/tests/test_wdi_login.py
```

