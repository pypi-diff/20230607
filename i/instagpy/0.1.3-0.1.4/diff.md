# Comparing `tmp/instagpy-0.1.3.tar.gz` & `tmp/instagpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagpy-0.1.3.tar", last modified: Wed May 31 15:13:13 2023, max compression
+gzip compressed data, was "instagpy-0.1.4.tar", last modified: Wed Jun  7 14:04:24 2023, max compression
```

## Comparing `instagpy-0.1.3.tar` & `instagpy-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 15:13:13.146643 instagpy-0.1.3/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3318 2023-05-31 15:13:13.146643 instagpy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 15:13:13.131008 instagpy-0.1.3/instagpy/
--rw-rw-rw-   0        0        0       32 2023-05-20 05:51:40.000000 instagpy-0.1.3/instagpy/__init__.py
--rw-rw-rw-   0        0        0    20509 2023-05-31 15:01:45.000000 instagpy-0.1.3/instagpy/instagpy.py
--rw-rw-rw-   0        0        0     2019 2023-05-22 09:57:02.000000 instagpy-0.1.3/instagpy/path.py
--rw-rw-rw-   0        0        0     1092 2023-05-31 15:11:43.000000 instagpy-0.1.3/instagpy/request_util.py
--rw-rw-rw-   0        0        0     2512 2023-05-20 05:51:32.000000 instagpy-0.1.3/instagpy/session_util.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 12:34:47.000000 instagpy-0.1.3/instagpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 15:13:13.131008 instagpy-0.1.3/instagpy.egg-info/
--rw-rw-rw-   0        0        0     3318 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 15:13:13.146643 instagpy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-05-31 15:09:06.000000 instagpy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:04:24.915113 instagpy-0.1.4/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3318 2023-06-07 14:04:24.915113 instagpy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 14:04:24.899485 instagpy-0.1.4/instagpy/
+-rw-rw-rw-   0        0        0       32 2023-06-07 10:27:42.000000 instagpy-0.1.4/instagpy/__init__.py
+-rw-rw-rw-   0        0        0      685 2023-06-07 13:57:25.000000 instagpy-0.1.4/instagpy/config.py
+-rw-rw-rw-   0        0        0    21919 2023-06-07 13:08:43.000000 instagpy-0.1.4/instagpy/instagpy.py
+-rw-rw-rw-   0        0        0     2086 2023-06-07 10:41:45.000000 instagpy-0.1.4/instagpy/path.py
+-rw-rw-rw-   0        0        0     1092 2023-05-31 15:11:43.000000 instagpy-0.1.4/instagpy/request_util.py
+-rw-rw-rw-   0        0        0     2722 2023-06-07 13:56:52.000000 instagpy-0.1.4/instagpy/session_util.py
+-rw-rw-rw-   0        0        0     2513 2023-05-22 12:34:47.000000 instagpy-0.1.4/instagpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:04:24.915113 instagpy-0.1.4/instagpy.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:04:24.915113 instagpy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-06-07 14:03:30.000000 instagpy-0.1.4/setup.py
```

### Comparing `instagpy-0.1.3/LICENSE` & `instagpy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.3/PKG-INFO` & `instagpy-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.3
+Version: 0.1.4
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.3 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.4 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.3/README.md` & `instagpy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.3/instagpy/instagpy.py` & `instagpy-0.1.4/instagpy/instagpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,132 @@
 import requests
 import json
 import datetime
 import time
 import getpass
 import random
-from .path import *
-from .request_util import make_request
+# custom
+from . import config
 from . import session_util
 from . import utils
-
-user_agent = "Mozilla/5.0 (iPhone; CPU iPhone OS 10_3_3 like Mac OS X) AppleWebKit/603.3.8 (KHTML, like Gecko) Mobile/14G60 Instagram 12.0.0.16.90 (iPhone9,4; iOS 10_3_3; en_US; en-US; scale=2.61; gamut=wide; 1080x1920"
+from . import path
+from .request_util import make_request
 
 
 class InstaGPy:
 
-    def __init__(self, max_retries=None, proxies=None, use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None):
+    def __init__(self, max_retries=None, proxies=None, use_mutiple_account=False, session_ids=None, min_requests=None, max_requests=None, timeout=None):
         """
 
         Args:
             max_retries (int, optional): Number of retires for each request. Defaults to None.
             proxies (dict, optional): Proxies as a dictionary {'http': proxy_here,'https':proxy_here}. Residential Proxies are recommended. Defaults to None.
             use_mutiple_account (bool, optional): Set to True if want to scrape data with mutiple account sessions So that you don't get blocked. Defaults to False.
             session_ids (list, optional): List of Session IDs from Cookies. Applicable only if use_mutiple_accounts is True. Defaults to False.
             min_requests (int, optional): Minimum requests to make before shuffling a session ID. Defaults to None.
             max_requests (int, optional): Maximum requests to make before shuffling a session ID. Defaults to None.
+            timeout (int, optional): Request timeout. Defaults to None.
         """
         if use_mutiple_account and not session_ids:
             raise Exception(
                 'Either Pass a list of session_ids or set use_multiple_account to False.')
         if use_mutiple_account and session_ids:
-            self.session_ids = session_ids
             self.current_request_number = 1
             # shuffle session randomly after every nth request.
-            self.min_requests = min_requests or 3
-            self.max_requests = max_requests or 6
+            self.min_requests = min_requests or config.MIN_REQUESTS
+            self.max_requests = max_requests or config.MAX_REQUESTS
             self.shuffle_session_after = random.randint(
                 self.min_requests, self.max_requests)
             self.session_ids_container = None
+        self.session_ids = session_ids
         self.use_mutiple_account = use_mutiple_account
-        self.max_retries = max_retries or 3
-        self.session = requests.Session()
-        if proxies is not None:
-            self.session.proxies = proxies
-            self.session.verify = False
+        self.max_retries = max_retries or config.MAX_RETRIES
+        self.timeout = timeout or config.TIMEOUT
+        self.proxies = proxies
         self.generate_session()
 
+    @property
+    def me(self):
+        """Returns Logged in User Information.
+
+        Returns:
+            dict: Currently logged in User Data.
+        """
+        response = self._get_meta_data()
+        return response['config']['viewer']
+
+    def _get_meta_data(self):
+        """Returns Browser's and User's Meta Data.
+
+        Returns:
+            dict: Meta Data.
+        """
+        response = make_request(
+            path.META_DATA_URL, session=self.session, max_retries=self.max_retries)
+        return response
+
     def generate_session(self, session_id=None):
         """Generates Required Headers and Cookies. OR Generates Session from an existing Session ID.
 
         Args:
             session_id (str, optional): Session Id from Instagram Session Cookies. Defaults to None.
         """
+        self.session = requests.Session()
+        if self.proxies is not None:
+            self.session.proxies = self.proxies
+            self.session.verify = False
         self.session.headers.update(
-            {"User-Agent": user_agent})
-        make_request(base_url, session=self.session,
+            {"User-Agent": random.choice(config.USER_AGENTS)})
+        make_request(path.BASE_URL, session=self.session,
                      max_retries=self.max_retries)
-        response = requests.get(login_url)
+        response = requests.get(path.LOGIN_URL)
         if not response.cookies:
             for _ in range(self.max_retries):
-                response = self.session.get(login_url)
+                response = self.session.get(path.LOGIN_URL)
                 if response.cookies:
                     break
         csrf_token = dict(response.cookies)["csrftoken"]
+        self.session.headers.update(
+            {'x-csrftoken': csrf_token, 'X-Requested-With': "XMLHttpRequest", 'Referer': path.BASE_URL})
+        self.session.cookies = response.cookies
         if session_id:
-            "load an existing session with session_id"
+            # load an existing session with session_id
             self.session.cookies.update({'sessionid': session_id})
-            return
-        self.session.cookies = response.cookies
-        self.session.headers.update(
-            {'x-csrftoken': csrf_token, 'X-Requested-With': "XMLHttpRequest", 'Referer': login_page_url})
 
-    def shuffle_session(self):
+        try:
+            self.me
+        except:
+            pass
+        return self.session
+
+    def shuffle_session(self, ignore_requests_limit=False):
+        """Shuffle session/cookies. Takes a new session ID from self.session_ids if using with mutiple accounts.
+
+        Args:
+            ignore_requests_limit (bool, optional): Set to True to shuffle session manually regardless of min/max number of requests. Defaults to False.
+
+        Returns:
+            Session object: Session Object i.e. self.session
+        """
         if not self.use_mutiple_account:
             return
-        self.current_request_number += 1
-        if self.current_request_number % self.shuffle_session_after == 0:
-            self.shuffle_session_after = random.randint(
-                self.min_requests, self.max_requests)
+        change_session = False
+        if ignore_requests_limit:
+            change_session = True
+        if not ignore_requests_limit:
+            self.current_request_number += 1
+            if self.current_request_number % self.shuffle_session_after == 0:
+                self.shuffle_session_after = random.randint(
+                    self.min_requests, self.max_requests)
+                change_session = True
+        if change_session:
             if not self.session_ids_container:
                 self.session_ids_container = self.session_ids.copy()
             session_id = self.session_ids_container.pop()
-            self.generate_session(session_id=session_id)
+            return self.generate_session(session_id=session_id)
 
     def generate_query(self, query=None, count=None, user_id=None, end_cursor=None, search_surface=None, shortcode=None, is_graphql=False):
         """Generates query paramters for instagram api requests.
 
         Args:
             query (str, optional): Query endpoint. Defaults to None.
             count (int, optional): Number of results per request to extract from Instagram Database. Defaults to None.
@@ -146,15 +188,15 @@
         payload = {
             'username': username,
             'enc_password': f'#PWD_INSTAGRAM_BROWSER:0:{timestamp}:{password}',
             'queryParams': {},
             'optIntoOneTap': 'false',
             'trustedDeviceRecords': {}
         }
-        response = self.session.post(login_url, data=payload).json()
+        response = self.session.post(path.LOGIN_URL, data=payload).json()
         try:
             if response["authenticated"]:
                 print("\nSuccessfully Logged In....")
                 if save_session:
                     session_util.save_session(
                         session=self.session, filename=username)
                 return
@@ -183,15 +225,15 @@
 
         Args:
             username (str): Instagram username.
 
         Returns:
             dict: user info like username,id,bio,follower/following count etc.
         """
-        response = make_request(user_profile_endpoint.format(
+        response = make_request(path.USER_PROFILE_ENDPOINT.format(
             username), session=self.session, max_retries=self.max_retries)
         self.shuffle_session()
         return response
 
     def get_user_data(self, user_id):
         """Extracts user details. With Contact Info Like email, phone and address.
 
@@ -201,15 +243,15 @@
         Returns:
             dict: user info along with contact info.
         """
         # returns almost as same data as get_user_info method Except this one returns contact info (email/phone) as well. |LOGIN REQUIRED|
         if not self.logged_in():
             self.login()
         user_id = self.get_user_id(user_id)
-        response = make_request(user_data_endpoint.format(
+        response = make_request(path.USER_DATA_ENDPOINT.format(
             user_id), session=self.session, max_retries=self.max_retries)
         self.shuffle_session()
         return response
 
     def get_user_basic_details(self, username=None, print_formatted=False):
         """Get a brief overview of an Instagram Profile.
 
@@ -263,24 +305,24 @@
         if user['is_private']:
             raise Exception("Account is Private.")
 
         user_friends = []
         print(f'Started at : {utils.format_datetime(time.time())}\n')
         while True:
             if followers_list and user['is_verified']:
-                url = graphql_url
+                url = path.GRAPHQL_URL
                 max_data = 50
-                query_params = self.generate_query(query=followers_list_query, count=max_data, user_id=user['id'],
+                query_params = self.generate_query(query=path.FOLLOWERS_LIST_QUERY, count=max_data, user_id=user['id'],
                                                    end_cursor=end_cursor, search_surface="follow_list_page", is_graphql=True)
             else:
                 if followers_list:
-                    url = user_followers_endpoint.format(user['id'])
+                    url = path.USER_FOLLOWERS_ENDPOINT.format(user['id'])
                     max_data = 100
                 elif followings_list:
-                    url = user_followings_endpoint.format(user['id'])
+                    url = path.USER_FOLLOWINGS_ENDPOINT.format(user['id'])
                     max_data = 200
                 query_params = self.generate_query(
                     count=max_data, end_cursor=end_cursor)
 
             try:
                 response = make_request(
                     url, params=query_params, session=self.session, max_retries=self.max_retries)
@@ -349,18 +391,18 @@
         if to_date is not None:
             to_date = utils.parse_datetime(to_date)
             to_date = to_date + datetime.timedelta(days=1)
         print(f'Started at : {utils.format_datetime(time.time())}\n')
         try:
             while True:
                 query_params = self.generate_query(
-                    query=user_feed_query, user_id=user_id, count=50, end_cursor=end_cursor, is_graphql=True)
+                    query=path.USER_FEED_QUERY, user_id=user_id, count=50, end_cursor=end_cursor, is_graphql=True)
                 try:
                     response = make_request(
-                        graphql_url, params=query_params, session=self.session, max_retries=self.max_retries)
+                        path.GRAPHQL_URL, params=query_params, session=self.session, max_retries=self.max_retries)
                     data = response['data']['user']['edge_owner_to_timeline_media']
                     posts_count = data['count']
                     has_next_page = data['page_info']['has_next_page']
                     cursor = data['page_info']['end_cursor']
                     if cursor:
                         end_cursor = cursor
                     user_posts_data.extend(filter_by_date(data['edges']))
@@ -393,17 +435,17 @@
         Args:
             post_url (str): Instagram Post/Picture/Reel URL.
 
         Returns:
             dict: All the details like post_id,datetime,caption,url,location etc.
         """
         post_id = utils.get_post_id(post_url)
-        url = graphql_url
+        url = path.GRAPHQL_URL
         query_params = self.generate_query(
-            query=post_details_query, shortcode=post_id, is_graphql=True)
+            query=path.POST_DETAILS_QUERY, shortcode=post_id, is_graphql=True)
         response = make_request(
             url, params=query_params, session=self.session, max_retries=self.max_retries)
         self.shuffle_session()
         return response
 
     def get_media_url(self, response):
         """Extracts High Resolution/Quality Media URL from post details response returned from get_post_details method.
@@ -434,16 +476,16 @@
         Returns:
             dict: User About Dataset.
         """
         if not self.logged_in():
             self.login()
         user_id = self.get_user_id(username)
         data = {'referer_type': 'ProfileUsername', 'target_user_id': user_id, 'bk_client_context': {
-            'bloks_version': about_user_query, 'style_id': 'instagram'}, 'bloks_versioning_id': about_user_query}
-        response = make_request(about_user_url, method='POST', data=data,
+            'bloks_version': path.ABOUT_USER_QUERY, 'style_id': 'instagram'}, 'bloks_versioning_id': path.ABOUT_USER_QUERY}
+        response = make_request(path.ABOUT_USER_URL, method='POST', data=data,
                                 session=self.session, max_retries=self.max_retries)
         if print_formatted:
             return utils.format_about_data(response)
         self.shuffle_session()
         return response
```

### Comparing `instagpy-0.1.3/instagpy/path.py` & `instagpy-0.1.4/instagpy/path.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 from urllib.parse import urljoin
 
 # URL Path & Endpoints
-base_url = "https://www.instagram.com/"
-login_url = "https://www.instagram.com/accounts/login/ajax/"
-login_page_url = "https://www.instagram.com/accounts/login/"
-location_url = "https://www.instagram.com/explore/locations/{}"
-location_endpoint = "https://www.instagram.com/api/v1/locations/web_info/"
-# user_data_endpoint = "https://i.instagram.com/api/v1/users/{}/full_detail_info/"
-# user_data_endpoint = "https://i.instagram.com/api/v1/users/web_profile_info/?username={}"
-user_data_endpoint = "https://i.instagram.com/api/v1/users/{}/info"
-user_profile_endpoint = "https://i.instagram.com/api/v1/users/web_profile_info/?username={}"
-
+BASE_URL = "https://www.instagram.com/"
+LOGIN_URL = "https://www.instagram.com/accounts/login/ajax/"
+LOGIN_PAGE_URL = "https://www.instagram.com/accounts/login/"
+LOCATION_URL = "https://www.instagram.com/explore/locations/{}"
+LOCATION_ENDPOINT = "https://www.instagram.com/api/v1/locations/web_info/"
+# USER_DATA_ENDPOINT = "https://i.instagram.com/api/v1/users/{}/full_detail_info/"
+# USER_DATA_ENDPOINT = "https://i.instagram.com/api/v1/users/web_profile_info/?username={}"
+USER_DATA_ENDPOINT = "https://i.instagram.com/api/v1/users/{}/info"
+USER_PROFILE_ENDPOINT = "https://www.instagram.com/api/v1/users/web_profile_info/?username={}"
+META_DATA_URL = "https://www.instagram.com/data/shared_data/?__a=1"
 
 # user_followers_endpoint returns max 100 results in a single request
 # Doesnt work with verified accounts
-user_followers_endpoint = "https://i.instagram.com/api/v1/friendships/{}/followers/"
-# user_followings_endpoint returns max 200 results in a single request
-user_followings_endpoint = "https://i.instagram.com/api/v1/friendships/{}/following/"
-
-story_endpoint = "https://i.instagram.com/api/v1/feed/reels_media/?reel_ids={}"
-# story_endpoint = "https://i.instagram.com/api/v1/feed/reels_media/?media_id={}"
-location_endpoint = "https://www.instagram.com/api/v1/locations/web_info/"
+USER_FOLLOWERS_ENDPOINT = "https://i.instagram.com/api/v1/friendships/{}/followers/"
+# USER_FOLLOWINGS_ENDPOINT returns max 200 results in a single request
+USER_FOLLOWINGS_ENDPOINT = "https://i.instagram.com/api/v1/friendships/{}/following/"
+
+STORY_ENDPOINT = "https://i.instagram.com/api/v1/feed/reels_media/?reel_ids={}"
+# STORY_ENDPOINT = "https://i.instagram.com/api/v1/feed/reels_media/?media_id={}"
+LOCATION_ENDPOINT = "https://www.instagram.com/api/v1/locations/web_info/"
 
 
 # graphql query and path
-graphql_url = urljoin(base_url, "/graphql/query/")
+GRAPHQL_URL = urljoin(BASE_URL, "/graphql/query/")
 # return 50 at a time
-post_details_query = "9f8827793ef34641b2fb195d4d41151c"
-user_feed_query = "69cba40317214236af40e7efa697781d"
+POST_DETAILS_QUERY = "9f8827793ef34641b2fb195d4d41151c"
+USER_FEED_QUERY = "69cba40317214236af40e7efa697781d"
 # followers_list_query & following_list_query - both return max 50 results in a single request but work with blue tick verified accounts.
-followers_list_query = "7dd9a7e2160524fd85f50317462cff9f"
-following_list_query = "c56ee0ae1f89cdbd1c89e2bc6b8f3d18"
-
-about_user_url = "https://i.instagram.com/api/v1/bloks/apps/com.instagram.interactions.about_this_account/"
-about_user_query = "8ca96ca267e30c02cf90888d91eeff09627f0e3fd2bd9df472278c9a6c022cbb"
+FOLLOWERS_LIST_QUERY = "7dd9a7e2160524fd85f50317462cff9f"
+FOLLOWING_LIST_QUERY = "c56ee0ae1f89cdbd1c89e2bc6b8f3d18"
 
+ABOUT_USER_URL = "https://i.instagram.com/api/v1/bloks/apps/com.instagram.interactions.about_this_account/"
+ABOUT_USER_QUERY = "8ca96ca267e30c02cf90888d91eeff09627f0e3fd2bd9df472278c9a6c022cbb"
 
 if __name__ == '__main__':
     pass
```

### Comparing `instagpy-0.1.3/instagpy/request_util.py` & `instagpy-0.1.4/instagpy/request_util.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.3/instagpy/session_util.py` & `instagpy-0.1.4/instagpy/session_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import pickle
 import requests
 import os
 import instagpy as instagram
+from . import config
 
 
 def generate_new_session(path=None):
     insta = instagram.InstaGPy()
     insta.login(show_saved_sessions=False, save_session=False)
-    return save_session(session=insta.session, path=path)
+    if insta.logged_in():
+        try:
+            filename = insta.me['username']
+        except:
+            filename = None
+        return save_session(session=insta.session, filename=filename, path=path)
+    raise Exception("Couldn't LogIn, Try again...")
 
 
 def create_session_directory(path=None, directory_name=None):
     if path is None:
         path = os.getcwd()
     if directory_name is None:
-        directory_name = "Insta Saved Sessions"
+        directory_name = config.SESSION_DIRECTORY
     directory = os.path.join(path, directory_name)
     if not os.path.exists(directory):
         os.mkdir(directory)
     return directory
 
 
 def show_saved_sessions(path=None):
     if path is None:
         path = create_session_directory()
     all_files = [f"{count}. {file}" for count, file in enumerate(
         os.listdir(path), start=1) if file.endswith(".pkl")]
     all_files.append(
         f"{len(os.listdir(path))+1}. Login with a New Account.")
     for file in all_files:
-        print(file.replace("_session.pkl", ""))
+        os.path.splitext(file)[0]
     file_number = int(
         input("\nChoose a Number to Load an Exising Session : ").strip())
     if file_number != len(os.listdir(path))+1:
         filename = os.listdir(path)[file_number-1]
     else:
         path, filename = generate_new_session(path)
     return path, filename
@@ -46,15 +53,15 @@
         try:
             filename = session.cookies['ds_user_id']
         except:
             filename = str(
                 input("Enter Username/Account Name to Save the Session : ")).strip()
     if path is None:
         path = create_session_directory()
-    filename = f"{filename}_session.pkl"
+    filename = f"{filename}.pkl"
     session_id = session.cookies['sessionid']
     file_path = os.path.join(path, filename)
     with open(file_path, "wb") as file:
         pickle.dump(session_id, file)
     return path, filename
```

### Comparing `instagpy-0.1.3/instagpy/utils.py` & `instagpy-0.1.4/instagpy/utils.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.3/instagpy.egg-info/PKG-INFO` & `instagpy-0.1.4/instagpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.3
+Version: 0.1.4
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.3 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.4 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.3/setup.py` & `instagpy-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 SHORT_DESCRIPTION = "InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

