# Comparing `tmp/naverplaceapi-0.1.8.tar.gz` & `tmp/naverplaceapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naverplaceapi-0.1.8.tar", max compression
+gzip compressed data, was "naverplaceapi-0.1.9.tar", max compression
```

## Comparing `naverplaceapi-0.1.8.tar` & `naverplaceapi-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      556 2023-11-04 15:54:07.783976 naverplaceapi-0.1.8/naverplaceapi/__init__.py
--rw-r--r--   0        0        0        0 2023-10-27 11:01:09.144187 naverplaceapi-0.1.8/naverplaceapi/mixin/__init__.py
--rw-r--r--   0        0        0      168 2023-11-02 10:38:09.569278 naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1052 2023-11-04 15:43:08.372057 naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/announce.cpython-38.pyc
--rw-r--r--   0        0        0     1039 2023-11-04 15:43:08.572463 naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/booking.cpython-38.pyc
--rw-r--r--   0        0        0     1631 2023-11-04 15:43:08.581224 naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/broadcast.cpython-38.pyc
--rw-r--r--   0        0        0      979 2023-11-04 15:43:08.574226 naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/menu.cpython-38.pyc
--rw-r--r--   0        0        0     3915 2023-11-04 15:43:08.576224 naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/place.cpython-38.pyc
--rw-r--r--   0        0        0      993 2023-11-04 15:43:08.577225 naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/promotions.cpython-38.pyc
--rw-r--r--   0        0        0     2531 2023-11-04 15:43:08.579224 naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/review.cpython-38.pyc
--rw-r--r--   0        0        0      787 2023-11-02 10:38:09.811859 naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-10-27 11:11:23.804287 naverplaceapi-0.1.8/naverplaceapi/mixin/_query.py
--rw-r--r--   0        0        0      815 2023-11-04 14:32:08.638094 naverplaceapi-0.1.8/naverplaceapi/mixin/announce.py
--rw-r--r--   0        0        0      823 2023-11-04 14:32:08.949874 naverplaceapi-0.1.8/naverplaceapi/mixin/booking.py
--rw-r--r--   0        0        0     1661 2023-11-04 14:33:12.440956 naverplaceapi-0.1.8/naverplaceapi/mixin/broadcast.py
--rw-r--r--   0        0        0      812 2023-11-04 14:33:12.415955 naverplaceapi-0.1.8/naverplaceapi/mixin/menu.py
--rw-r--r--   0        0        0     4573 2023-11-04 15:54:07.699690 naverplaceapi-0.1.8/naverplaceapi/mixin/place.py
--rw-r--r--   0        0        0      698 2023-11-04 14:33:12.524073 naverplaceapi-0.1.8/naverplaceapi/mixin/promotions.py
--rw-r--r--   0        0        0     1028 2023-11-02 10:25:59.035199 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__init__.py
--rw-r--r--   0        0        0      804 2023-11-02 10:38:09.698098 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1219 2023-11-02 10:38:09.712519 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_announcements.cpython-38.pyc
--rw-r--r--   0        0        0     1543 2023-11-02 10:38:09.711522 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_booking_items.cpython-38.pyc
--rw-r--r--   0        0        0     1121 2023-11-02 10:38:09.714519 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_popular_menus.cpython-38.pyc
--rw-r--r--   0        0        0     1899 2023-11-02 10:38:09.709893 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_promotions.cpython-38.pyc
--rw-r--r--   0        0        0    11668 2023-11-04 15:43:08.485586 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_restaurant.cpython-38.pyc
--rw-r--r--   0        0        0    11821 2023-11-02 10:38:09.704893 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_restaurants.cpython-38.pyc
--rw-r--r--   0        0        0     1281 2023-11-02 10:38:09.702892 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_ugc_reviews.cpython-38.pyc
--rw-r--r--   0        0        0     1814 2023-11-02 10:38:09.708892 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_visitor_review_photos_in_visitor_review_tab.cpython-38.pyc
--rw-r--r--   0        0        0     2847 2023-11-02 10:38:09.701894 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_visitor_review_stats.cpython-38.pyc
--rw-r--r--   0        0        0     1072 2023-11-02 10:38:09.706894 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_visitor_review_theme_lists.cpython-38.pyc
--rw-r--r--   0        0        0     4871 2023-11-02 10:38:09.700097 naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_visitor_reviews.cpython-38.pyc
--rw-r--r--   0        0        0     1165 2023-11-01 09:05:12.489513 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_announcements.py
--rw-r--r--   0        0        0     1483 2023-10-31 02:14:45.030466 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_booking_items.py
--rw-r--r--   0        0        0      980 2023-10-31 02:56:26.253470 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_popular_menus.py
--rw-r--r--   0        0        0     1959 2023-10-31 02:43:37.594527 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_promotions.py
--rw-r--r--   0        0        0    12153 2023-11-02 12:29:45.625388 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_restaurant.py
--rw-r--r--   0        0        0    11996 2023-10-27 11:40:43.963451 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_restaurants.py
--rw-r--r--   0        0        0     1162 2023-10-30 12:38:18.153714 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_ugc_reviews.py
--rw-r--r--   0        0        0     1654 2023-11-01 09:47:28.947929 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_visitor_review_photos_in_visitor_review_tab.py
--rw-r--r--   0        0        0     2677 2023-10-30 12:38:18.078015 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_visitor_review_stats.py
--rw-r--r--   0        0        0      922 2023-11-01 09:51:54.509688 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_visitor_review_theme_lists.py
--rw-r--r--   0        0        0     4861 2023-10-30 12:23:36.750903 naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_visitor_reviews.py
--rw-r--r--   0        0        0     3133 2023-11-04 15:43:07.410998 naverplaceapi-0.1.8/naverplaceapi/mixin/review.py
--rw-r--r--   0        0        0      754 2023-11-01 08:34:14.629967 naverplaceapi-0.1.8/naverplaceapi/mixin/utils.py
--rw-r--r--   0        0        0      286 2023-11-04 15:54:07.690664 naverplaceapi-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        5 2023-11-01 11:39:23.358093 naverplaceapi-0.1.8/README.md
--rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 naverplaceapi-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      556 2023-11-04 15:58:55.032033 naverplaceapi-0.1.9/naverplaceapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-27 11:01:09.144187 naverplaceapi-0.1.9/naverplaceapi/mixin/__init__.py
+-rw-r--r--   0        0        0      168 2023-11-02 10:38:09.569278 naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1052 2023-11-04 15:43:08.372057 naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/announce.cpython-38.pyc
+-rw-r--r--   0        0        0     1039 2023-11-04 15:43:08.572463 naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/booking.cpython-38.pyc
+-rw-r--r--   0        0        0     1631 2023-11-04 15:43:08.581224 naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/broadcast.cpython-38.pyc
+-rw-r--r--   0        0        0      979 2023-11-04 15:43:08.574226 naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/menu.cpython-38.pyc
+-rw-r--r--   0        0        0     3915 2023-11-04 15:43:08.576224 naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/place.cpython-38.pyc
+-rw-r--r--   0        0        0      993 2023-11-04 15:43:08.577225 naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/promotions.cpython-38.pyc
+-rw-r--r--   0        0        0     2531 2023-11-04 15:43:08.579224 naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/review.cpython-38.pyc
+-rw-r--r--   0        0        0      787 2023-11-02 10:38:09.811859 naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-10-27 11:11:23.804287 naverplaceapi-0.1.9/naverplaceapi/mixin/_query.py
+-rw-r--r--   0        0        0      815 2023-11-04 14:32:08.638094 naverplaceapi-0.1.9/naverplaceapi/mixin/announce.py
+-rw-r--r--   0        0        0      823 2023-11-04 14:32:08.949874 naverplaceapi-0.1.9/naverplaceapi/mixin/booking.py
+-rw-r--r--   0        0        0     1661 2023-11-04 14:33:12.440956 naverplaceapi-0.1.9/naverplaceapi/mixin/broadcast.py
+-rw-r--r--   0        0        0      812 2023-11-04 14:33:12.415955 naverplaceapi-0.1.9/naverplaceapi/mixin/menu.py
+-rw-r--r--   0        0        0     4660 2023-11-04 15:58:27.524752 naverplaceapi-0.1.9/naverplaceapi/mixin/place.py
+-rw-r--r--   0        0        0      698 2023-11-04 14:33:12.524073 naverplaceapi-0.1.9/naverplaceapi/mixin/promotions.py
+-rw-r--r--   0        0        0     1028 2023-11-02 10:25:59.035199 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__init__.py
+-rw-r--r--   0        0        0      804 2023-11-02 10:38:09.698098 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1219 2023-11-02 10:38:09.712519 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_announcements.cpython-38.pyc
+-rw-r--r--   0        0        0     1543 2023-11-02 10:38:09.711522 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_booking_items.cpython-38.pyc
+-rw-r--r--   0        0        0     1121 2023-11-02 10:38:09.714519 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_popular_menus.cpython-38.pyc
+-rw-r--r--   0        0        0     1899 2023-11-02 10:38:09.709893 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_promotions.cpython-38.pyc
+-rw-r--r--   0        0        0    11668 2023-11-04 15:43:08.485586 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_restaurant.cpython-38.pyc
+-rw-r--r--   0        0        0    11821 2023-11-02 10:38:09.704893 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_restaurants.cpython-38.pyc
+-rw-r--r--   0        0        0     1281 2023-11-02 10:38:09.702892 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_ugc_reviews.cpython-38.pyc
+-rw-r--r--   0        0        0     1814 2023-11-02 10:38:09.708892 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_visitor_review_photos_in_visitor_review_tab.cpython-38.pyc
+-rw-r--r--   0        0        0     2847 2023-11-02 10:38:09.701894 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_visitor_review_stats.cpython-38.pyc
+-rw-r--r--   0        0        0     1072 2023-11-02 10:38:09.706894 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_visitor_review_theme_lists.cpython-38.pyc
+-rw-r--r--   0        0        0     4871 2023-11-02 10:38:09.700097 naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_visitor_reviews.cpython-38.pyc
+-rw-r--r--   0        0        0     1165 2023-11-01 09:05:12.489513 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_announcements.py
+-rw-r--r--   0        0        0     1483 2023-10-31 02:14:45.030466 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_booking_items.py
+-rw-r--r--   0        0        0      980 2023-10-31 02:56:26.253470 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_popular_menus.py
+-rw-r--r--   0        0        0     1959 2023-10-31 02:43:37.594527 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_promotions.py
+-rw-r--r--   0        0        0    12153 2023-11-02 12:29:45.625388 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_restaurant.py
+-rw-r--r--   0        0        0    11996 2023-10-27 11:40:43.963451 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_restaurants.py
+-rw-r--r--   0        0        0     1162 2023-10-30 12:38:18.153714 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_ugc_reviews.py
+-rw-r--r--   0        0        0     1654 2023-11-01 09:47:28.947929 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_visitor_review_photos_in_visitor_review_tab.py
+-rw-r--r--   0        0        0     2677 2023-10-30 12:38:18.078015 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_visitor_review_stats.py
+-rw-r--r--   0        0        0      922 2023-11-01 09:51:54.509688 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_visitor_review_theme_lists.py
+-rw-r--r--   0        0        0     4861 2023-10-30 12:23:36.750903 naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_visitor_reviews.py
+-rw-r--r--   0        0        0     3133 2023-11-04 15:43:07.410998 naverplaceapi-0.1.9/naverplaceapi/mixin/review.py
+-rw-r--r--   0        0        0      754 2023-11-01 08:34:14.629967 naverplaceapi-0.1.9/naverplaceapi/mixin/utils.py
+-rw-r--r--   0        0        0      286 2023-11-04 15:58:54.950513 naverplaceapi-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-11-01 11:39:23.358093 naverplaceapi-0.1.9/README.md
+-rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 naverplaceapi-0.1.9/PKG-INFO
```

### Comparing `naverplaceapi-0.1.8/naverplaceapi/__init__.py` & `naverplaceapi-0.1.9/naverplaceapi/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .mixin.booking import BookingMixin
 from .mixin.menu import MenuMixin
 from .mixin.place import PlaceMixin
 from .mixin.promotions import PromotionsMixin
 from .mixin.review import ReviewMixin
 from .mixin.broadcast import BroadcastMixin
 
-__VERSION__ = "0.1.8"
+__VERSION__ = "0.1.9"
 
 DEFAULT_LOGGER = logging.getLogger("naverplaceapi")
 
 class Client(
     PlaceMixin,
     ReviewMixin,
     BroadcastMixin,
```

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/announce.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/announce.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/booking.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/booking.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/broadcast.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/broadcast.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/menu.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/menu.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/place.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/place.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/promotions.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/promotions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/review.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/review.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/__pycache__/utils.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/announce.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/announce.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/booking.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/booking.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/broadcast.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/broadcast.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/menu.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/menu.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/place.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/place.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 class PlaceMixin:
 
     def search_places(self, keyword: str, page_no: int, page_size: int, proxy=None):
         data = query.get_restaurants.create(keyword, page_no, page_size)
         print("proxy: ", proxy)
+        print("keyword: ", keyword, " page_no: ", page_no, " paeg_size; ", page_size)
         response = requests.post("https://pcmap-api.place.naver.com/graphql", headers=HEADERS, data=json.dumps(data), proxies={"http":proxy})
         response.raise_for_status()
         response_data = response.json()
         graphql_data = response_data['data']['restaurants']
         return graphql_data
 
     def get_place(self, business_id, proxy=None):
```

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/promotions.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/promotions.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__init__.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__init__.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/__init__.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_announcements.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_announcements.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_booking_items.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_booking_items.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_popular_menus.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_popular_menus.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_promotions.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_promotions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_restaurant.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_restaurant.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_restaurants.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_restaurants.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_ugc_reviews.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_ugc_reviews.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_visitor_review_photos_in_visitor_review_tab.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_visitor_review_photos_in_visitor_review_tab.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_visitor_review_stats.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_visitor_review_stats.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_visitor_review_theme_lists.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_visitor_review_theme_lists.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/__pycache__/get_visitor_reviews.cpython-38.pyc` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/__pycache__/get_visitor_reviews.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_announcements.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_announcements.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_booking_items.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_booking_items.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_popular_menus.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_popular_menus.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_promotions.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_promotions.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_restaurant.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_restaurant.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_restaurants.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_restaurants.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_ugc_reviews.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_ugc_reviews.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_visitor_review_photos_in_visitor_review_tab.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_visitor_review_photos_in_visitor_review_tab.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_visitor_review_stats.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_visitor_review_stats.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_visitor_review_theme_lists.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_visitor_review_theme_lists.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/query/get_visitor_reviews.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/query/get_visitor_reviews.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/review.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/review.py`

 * *Files identical despite different names*

### Comparing `naverplaceapi-0.1.8/naverplaceapi/mixin/utils.py` & `naverplaceapi-0.1.9/naverplaceapi/mixin/utils.py`

 * *Files identical despite different names*

