# Comparing `tmp/arz_api-1.8.2.tar.gz` & `tmp/arz_api-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arz_api-1.8.2.tar", last modified: Thu May  2 17:21:03 2024, max compression
+gzip compressed data, was "arz_api-2.0.tar", last modified: Sat May  4 17:17:07 2024, max compression
```

## Comparing `arz_api-1.8.2.tar` & `arz_api-2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 17:21:02.996077 arz_api-1.8.2/
--rw-rw-rw-   0        0        0     1089 2023-11-08 20:12:48.000000 arz_api-1.8.2/LICENSE
--rw-rw-rw-   0        0        0     1739 2024-05-02 17:21:02.995082 arz_api-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-11-08 20:15:07.000000 arz_api-1.8.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 17:21:02.940845 arz_api-1.8.2/arz_api/
--rw-rw-rw-   0        0        0     3604 2023-08-04 21:34:31.000000 arz_api-1.8.2/arz_api/__init__.py
--rw-rw-rw-   0        0        0    30351 2024-05-02 17:11:35.000000 arz_api-1.8.2/arz_api/api.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:21:02.976694 arz_api-1.8.2/arz_api/bypass_antibot/
--rw-rw-rw-   0        0        0       21 2023-05-31 18:16:38.000000 arz_api-1.8.2/arz_api/bypass_antibot/__init__.py
--rw-rw-rw-   0        0        0    35306 2023-05-31 19:17:18.000000 arz_api-1.8.2/arz_api/bypass_antibot/script.py
--rw-rw-rw-   0        0        0      247 2023-06-03 18:57:22.000000 arz_api-1.8.2/arz_api/consts.py
--rw-rw-rw-   0        0        0      563 2023-07-08 19:21:59.000000 arz_api-1.8.2/arz_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:21:02.991091 arz_api-1.8.2/arz_api/models/
--rw-rw-rw-   0        0        0      112 2023-05-31 18:48:38.000000 arz_api-1.8.2/arz_api/models/__init__.py
--rw-rw-rw-   0        0        0     4093 2024-05-01 21:05:18.000000 arz_api-1.8.2/arz_api/models/category_object.py
--rw-rw-rw-   0        0        0     5180 2024-05-01 20:44:42.000000 arz_api-1.8.2/arz_api/models/member_object.py
--rw-rw-rw-   0        0        0      512 2023-07-08 10:56:45.000000 arz_api-1.8.2/arz_api/models/other.py
--rw-rw-rw-   0        0        0     5943 2024-05-01 21:08:21.000000 arz_api-1.8.2/arz_api/models/post_object.py
--rw-rw-rw-   0        0        0     6045 2024-05-02 17:12:07.000000 arz_api-1.8.2/arz_api/models/thread_object.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:21:02.993084 arz_api-1.8.2/arz_api.egg-info/
--rw-rw-rw-   0        0        0     1739 2024-05-02 17:21:02.000000 arz_api-1.8.2/arz_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-05-02 17:21:02.000000 arz_api-1.8.2/arz_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 17:21:02.000000 arz_api-1.8.2/arz_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-02 17:21:02.000000 arz_api-1.8.2/arz_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-02 17:21:02.000000 arz_api-1.8.2/arz_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 17:21:02.999064 arz_api-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1849 2024-05-02 17:20:09.000000 arz_api-1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.107349 arz_api-2.0/
+-rw-rw-rw-   0        0        0     1089 2023-11-08 20:12:48.000000 arz_api-2.0/LICENSE
+-rw-rw-rw-   0        0        0     1737 2024-05-04 17:17:07.106350 arz_api-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-11-08 20:15:07.000000 arz_api-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.058795 arz_api-2.0/arz_api/
+-rw-rw-rw-   0        0        0     3604 2023-08-04 21:34:31.000000 arz_api-2.0/arz_api/__init__.py
+-rw-rw-rw-   0        0        0    29414 2024-05-04 16:59:06.000000 arz_api-2.0/arz_api/api.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.090105 arz_api-2.0/arz_api/bypass_antibot/
+-rw-rw-rw-   0        0        0       21 2023-05-31 18:16:38.000000 arz_api-2.0/arz_api/bypass_antibot/__init__.py
+-rw-rw-rw-   0        0        0    35306 2023-05-31 19:17:18.000000 arz_api-2.0/arz_api/bypass_antibot/script.py
+-rw-rw-rw-   0        0        0      247 2024-05-03 19:46:30.000000 arz_api-2.0/arz_api/consts.py
+-rw-rw-rw-   0        0        0      563 2023-07-08 19:21:59.000000 arz_api-2.0/arz_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.101366 arz_api-2.0/arz_api/models/
+-rw-rw-rw-   0        0        0      112 2023-05-31 18:48:38.000000 arz_api-2.0/arz_api/models/__init__.py
+-rw-rw-rw-   0        0        0     4126 2024-05-03 20:23:22.000000 arz_api-2.0/arz_api/models/category_object.py
+-rw-rw-rw-   0        0        0     4794 2024-05-03 18:06:11.000000 arz_api-2.0/arz_api/models/member_object.py
+-rw-rw-rw-   0        0        0      512 2023-07-08 10:56:45.000000 arz_api-2.0/arz_api/models/other.py
+-rw-rw-rw-   0        0        0     5600 2024-05-03 18:16:32.000000 arz_api-2.0/arz_api/models/post_object.py
+-rw-rw-rw-   0        0        0     5513 2024-05-03 20:50:47.000000 arz_api-2.0/arz_api/models/thread_object.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.104359 arz_api-2.0/arz_api.egg-info/
+-rw-rw-rw-   0        0        0     1737 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 17:17:07.110337 arz_api-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1847 2024-05-04 17:16:40.000000 arz_api-2.0/setup.py
```

### Comparing `arz_api-1.8.2/LICENSE` & `arz_api-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arz_api-1.8.2/PKG-INFO` & `arz_api-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arz_api
-Version: 1.8.2
+Version: 2.0
 Summary: Модуль для взаимодействия с форумом без Xenforo ключей
 Home-page: https://github.com/TastyBread123/Arizona-API/
 Author: TastyBread123
 Author-email: ermakovglebyt@gmail.com
 Project-URL: Documentation, https://tastybread123.github.io/Arizona-API/arz_api.html
 Keywords: python xenforo arizona roleplay samp gta
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `arz_api-1.8.2/arz_api/__init__.py` & `arz_api-2.0/arz_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8.2/arz_api/api.py` & `arz_api-2.0/arz_api/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from bs4 import BeautifulSoup
 from re import compile, findall
 from requests import session, Response
+from html import unescape
 
 from arz_api.consts import MAIN_URL
 from arz_api.bypass_antibot import bypass
 
 from arz_api.exceptions import IncorrectLoginData, ThisIsYouError
 from arz_api.models.other import Statistic
 from arz_api.models.post_object import Post, ProfilePost
 from arz_api.models.member_object import Member, CurrentMember
 from arz_api.models.thread_object import Thread
 from arz_api.models.category_object import Category
 
 
-
 class ArizonaAPI:
     def __init__(self, user_agent: str, cookie: dict, do_bypass: bool = True) -> None:
         self.user_agent = user_agent
         self.cookie = cookie
         self.session = session()
         self.session.headers = {"user-agent": user_agent}
         self.session.cookies.update(cookie)
@@ -42,44 +42,48 @@
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/account").content, 'lxml')
         user_id = int(content.find('span', {'class': 'avatar--xxs'})['data-user-id'])
         member_info = self.get_member(user_id)
 
         return CurrentMember(self, user_id, member_info.username, member_info.user_title, member_info.avatar, member_info.roles, member_info.messages_count, member_info.reactions_count, member_info.trophies_count)
 
-    
+    @property
+    def token(self) -> str:
+        """Получить токен CSRF"""
+        return BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
+
+
     def get_category(self, category_id: int) -> Category:
         """Найти раздел по ID"""
 
-        content = BeautifulSoup(self.session.get(f"{MAIN_URL}/forums/{category_id}").content, 'lxml')
-        title = content.find('h1', {'class': 'p-title-value'}).text
-        if "Упс! Мы столкнулись с некоторыми проблемами." in title:
+        request = self.session.get(f"{MAIN_URL}/forums/{category_id}?&_xfResponseType=json&_xfToken={self.token}").json()
+        if request['status'] == 'error':
             return None
 
+        content = unescape(request['html']['content'])
+        content = BeautifulSoup(content, 'lxml')
+
+        title = request['html']['title']
         try: pages_count = int(content.find_all('li', {'class': 'pageNav-page'})[-1].text)
         except IndexError: pages_count = 1
-        try: parent_category_id = int(content.find('html')['data-container-key'].strip('node-'))
-        except: parent_category_id = None
 
-        temp_url = ''
-        if parent_category_id is not None: temp_url = f'forums/{parent_category_id}/'
-        content = BeautifulSoup(self.session.get(f"{MAIN_URL}/{temp_url}").content, 'lxml')
-        
-        return Category(self, category_id, title, pages_count, parent_category_id)
+        return Category(self, category_id, title, pages_count)
     
     
     def get_member(self, user_id: int) -> Member:
         """Найти пользователя по ID (возвращает либо Member, либо None (если профиль закрыт / не существует))"""
 
-        content = BeautifulSoup(self.session.get(f"{MAIN_URL}/members/{user_id}").content, 'lxml')
-
-        username = content.find('span', {'class': 'username'})
-        if username is None:
+        request = self.session.get(f"{MAIN_URL}/members/{user_id}?&_xfResponseType=json&_xfToken={self.token}").json()
+        if request['status'] == 'error':
             return None
-        username = username.text
+
+        content = unescape(request['html']['content'])
+        content = BeautifulSoup(content, 'lxml')
+
+        username = request['html']['title']
 
         roles = []
         for i in content.find('div', {'class': 'memberHeader-banners'}).children:
             if i.text != '\n': roles.append(i.text)
 
         try: user_title = content.find('span', {'class': 'userTitle'}).text
         except AttributeError: user_title = None
@@ -87,47 +91,50 @@
         except TypeError: avatar = None
 
         messages_count = int(content.find('a', {'href': f'/search/member?user_id={user_id}'}).text.strip().replace(',', ''))
         reactions_count = int(content.find('dl', {'class': 'pairs pairs--rows pairs--rows--centered'}).find('dd').text.strip().replace(',', ''))
         trophies_count = int(content.find('a', {'href': f'/members/{user_id}/trophies'}).text.strip().replace(',', ''))
         
         return Member(self, user_id, username, user_title, avatar, roles, messages_count, reactions_count, trophies_count)
-
     
-    def get_thread(self, thread_id: int) -> Thread:
-        """Найти тему по ID (Thread если тема существует, None если недоступна / не существует)"""
 
-        content = BeautifulSoup(self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-1").content, 'lxml')
-        
-        creator_id = content.find('a', {'class': 'username'})
-        if creator_id is None:
+    def get_thread(self, thread_id: int):
+        request = self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-1?&_xfResponseType=json&_xfToken={self.token}").json()
+        if request['status'] == 'error':
             return None
+        
+        if request.get('redirect') is not None:
+            return self.get_thread(request['redirect'].strip(MAIN_URL).split('/')[1])
+
+        content = unescape(request['html']['content'])
+        content_h1 = unescape(request['html']['h1'])
+        content = BeautifulSoup(content, 'lxml')
+        content_h1 = BeautifulSoup(content_h1, 'lxml')
 
+        creator_id = content.find('a', {'class': 'username'})
         try: creator = self.get_member(int(creator_id['data-user-id']))
         except: creator = Member(self, int(creator_id['data-user-id']), content.find('a', {'class': 'username'}).text, None, None, None, None, None, None)
         
-        category = self.get_category(int(content.find('html')['data-container-key'].strip('node-')))
         create_date = int(content.find('time')['data-time'])
         
-        try: title = [i for i in content.find('h1', {'class': 'p-title-value'}).strings][-1]
-        except: title = ""
-        try: prefix = content.find('h1', {'class': 'p-title-value'}).find('span', {'class': 'label'}).text
+        title = request['html']['title']
+        try: prefix = content_h1.find('span', {'class': 'label'}).text
         except: prefix = ""
         thread_content_html = content.find('div', {'class': 'bbWrapper'})
         thread_content = thread_content_html.text
         
         try: pages_count = int(content.find_all('li', {'class': 'pageNav-page'})[-1].text)
         except IndexError: pages_count = 1
 
         is_closed = False
         if content.find('dl', {'class': 'blockStatus'}): is_closed = True
         thread_post_id = content.find('article', {'id': compile('js-post-*')})['id'].strip('js-post-')
 
-        return Thread(self, thread_id, creator, category, create_date, title, prefix, thread_content, thread_content_html, pages_count, thread_post_id, is_closed)
-    
+        return Thread(self, thread_id, creator, create_date, title, prefix, thread_content, thread_content_html, pages_count, thread_post_id, is_closed)
+
 
     def get_post(self, post_id: int) -> Post:
         """Найти пост по ID (Post если существует, None - удален / нет доступа)"""
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/posts/{post_id}").content, 'lxml')
         post = content.find('article', {'id': f'js-post-{post_id}'})
         if post is None:
@@ -190,30 +197,28 @@
         Returns:
             Объект Response модуля requests
 
         Todo:
             Cделать возврат ID новой темы
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/forums/{category_id}/post-thread?inline-mode=1", {'_xfToken': token, 'title': title, 'message_html': message_html, 'discussion_type': discussion_type, 'watch_thread': int(watch_thread)})
+        return self.session.post(f"{MAIN_URL}/forums/{category_id}/post-thread?inline-mode=1", {'_xfToken': self.token, 'title': title, 'message_html': message_html, 'discussion_type': discussion_type, 'watch_thread': int(watch_thread)})
     
 
     def set_read_category(self, category_id: int) -> Response:
         """Отметить категорию как прочитанную
 
         Attributes:
             category_id (int): ID категории
         
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/forums/{category_id}/mark-read", {'_xfToken': token})
+        return self.session.post(f"{MAIN_URL}/forums/{category_id}/mark-read", {'_xfToken': self.token})
     
 
     def watch_category(self, category_id: int, notify: str, send_alert: bool = True, send_email: bool = False, stop: bool = False) -> Response:
         """Настроить отслеживание категории
 
         Attributes:
             category_id (int): ID категории
@@ -222,117 +227,147 @@
             send_email (bool): - Отправлять ли уведомления на почту. По умолчанию False (необяз.)
             stop (bool): - Принудительное завершение отслеживания. По умолчанию False (необяз.)
 
         Returns:
             Объект Response модуля requests    
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-
-        if stop: return self.session.post(f"{MAIN_URL}/forums/{category_id}/watch", {'_xfToken': token, 'stop': "1"})
-        else: return self.session.post(f"{MAIN_URL}/forums/{category_id}/watch", {'_xfToken': token, 'send_alert': int(send_alert), 'send_email': int(send_email), 'notify': notify})
+        if stop: return self.session.post(f"{MAIN_URL}/forums/{category_id}/watch", {'_xfToken': self.token, 'stop': "1"})
+        else: return self.session.post(f"{MAIN_URL}/forums/{category_id}/watch", {'_xfToken': self.token, 'send_alert': int(send_alert), 'send_email': int(send_email), 'notify': notify})
 
 
     def get_threads(self, category_id: int, page: int = 1) -> dict:
         """Получить темы из раздела
 
         Attributes:
             category_id (int): ID категории
             page (int): Cтраница для поиска. По умолчанию 1 (необяз.)
             
         Returns:
             Словарь (dict), состоящий из списков закрепленных ('pins') и незакрепленных ('unpins') тем
         """
 
-        soup = BeautifulSoup(self.session.get(f"{MAIN_URL}/forums/{category_id}/page-{page}").content, "lxml")
+        request = self.session.get(f"{MAIN_URL}/forums/{category_id}/page-{page}?_xfResponseType=json&_xfToken={self.token}").json()
+        if request['status'] == 'error':
+            return None
+        
+        soup = BeautifulSoup(unescape(request['html']['content']), "lxml")
         result = {'pins': [], 'unpins': []}
         for thread in soup.find_all('div', compile('structItem structItem--thread.*')):
             link = thread.find_all('div', "structItem-title")[0].find_all("a")[-1]
             if len(findall(r'\d+', link['href'])) < 1: continue
 
             if len(thread.find_all('i', {'title': 'Закреплено'})) > 0: result['pins'].append(int(findall(r'\d+', link['href'])[0]))
             else: result['unpins'].append(int(findall(r'\d+', link['href'])[0]))
         
         return result
 
+    
+    def get_parent_category_of_category(self, category_id: int) -> Category:
+        """Получить родительский раздел раздела
+
+        Attributes:
+            category_id (int): ID категории
+        
+        Returns:
+            - Если существует: Объект Catrgory, в котором создан раздел
+            - Если не существует: None
+        """
+
+        content = BeautifulSoup(self.session.get(f"{MAIN_URL}/forums/{category_id}").content, 'lxml')
+        
+        parent_category_id = str(content.find('ul', {'class': 'p-breadcrumbs'}).find_all('li')[-1].find('a')['href'].split('/')[2])
+        if not parent_category_id.isdigit():
+            return None
+        
+        return self.get_category(parent_category_id)
+
 
     def get_categories(self, category_id: int) -> list:
         """Получить дочерние категории из раздела
         
         Attributes:
             category_id (int): ID категории
         
         Returns:
             Список (list), состоящий из ID дочерних категорий раздела
         """
 
-        soup = BeautifulSoup(self.session.get(f"{MAIN_URL}/forums/{category_id}").content, "lxml")
+        request = self.session.get(f"{MAIN_URL}/forums/{category_id}/page-1?_xfResponseType=json&_xfToken={self.token}").json()
+        if request['status'] == 'error':
+            return None
+        
+        soup = BeautifulSoup(unescape(request['html']['content']), "lxml")
         return [int(findall(r'\d+', category.find("a")['href'])[0]) for category in soup.find_all('div', compile('.*node--depth2 node--forum.*'))]
     
 
     # MEMBER
     def follow_member(self, member_id: int) -> Response:
         """Изменить статус подписки на пользователя
         
         Attributes:
             member_id (int): ID пользователя
         
         Returns:
             Объект Response модуля requests
         """
 
-        if member_id == self.current_member.id: raise ThisIsYouError(member_id)
+        if member_id == self.current_member.id:
+            raise ThisIsYouError(member_id)
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/members/{member_id}/follow", {'_xfToken': token})
+        return self.session.post(f"{MAIN_URL}/members/{member_id}/follow", {'_xfToken': self.token})
     
 
     def ignore_member(self, member_id: int) -> Response:
         """Изменить статус игнорирования пользователя
 
         Attributes:
             member_id (int): ID пользователя
         
         Returns:
             Объект Response модуля requests
         """
 
-        if member_id == self.current_member.id: raise ThisIsYouError(member_id)
+        if member_id == self.current_member.id:
+            raise ThisIsYouError(member_id)
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/members/{member_id}/ignore", {'_xfToken': token})
+        return self.session.post(f"{MAIN_URL}/members/{member_id}/ignore", {'_xfToken': self.token})
     
 
     def add_profile_message(self, member_id: int, message_html: str) -> Response:
         """Отправить сообщение на стенку пользователя
 
         Attributes:
             member_id (int): ID пользователя
             message_html (str): Текст сообщения. Рекомендуется использование HTML
             
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/members/{member_id}/post", {'_xfToken': token, 'message_html': message_html})
+        return self.session.post(f"{MAIN_URL}/members/{member_id}/post", {'_xfToken': self.token, 'message_html': message_html})
     
 
-    def get_profile_messages(self, member_id: int, page: int = 1) -> list:
+    def get_profile_messages(self, member_id: int, page: int = 1) -> list | None:
         """Возвращает ID всех сообщений со стенки пользователя на странице
 
         Attributes:
             member_id (int): ID пользователя
             page (int): Страница для поиска. По умолчанию 1 (необяз.)
             
         Returns:
-            Cписок (list) с ID всех сообщений профиля
+            - Cписок (list) с ID всех сообщений профиля
+            - None, если пользователя не существует / закрыл профиль
         """
 
-        soup = BeautifulSoup(self.session.get(f"{MAIN_URL}/members/{member_id}/page-{page}").content, "lxml")
+        request = self.session.get(f"{MAIN_URL}/members/{member_id}/page-{page}?_xfResponseType=json&_xfToken={self.token}").json()
+        if request['status'] == 'error':
+            return None
+        
+        soup = BeautifulSoup(unescape(request['html']['content']), "lxml")
         return [int(post['id'].strip('js-profilePost-')) for post in soup.find_all('article', {'id': compile('js-profilePost-*')})]
 
 
     # POST
     def react_post(self, post_id: int, reaction_id: int = 1) -> Response:
         """Поставить реакцию на сообщение
 
@@ -340,216 +375,176 @@
             post_id (int): ID сообщения
             reaction_id (int): ID реакции. По умолчанию 1 (необяз.)
             
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f'{MAIN_URL}/posts/{post_id}/react?reaction_id={reaction_id}', {'_xfToken': token})
+        return self.session.post(f'{MAIN_URL}/posts/{post_id}/react?reaction_id={reaction_id}', {'_xfToken': self.token})
     
 
     def edit_post(self, post_id: int, message_html: str) -> Response:
         """Отредактировать сообщение
 
         Attributes:
             post_id (int): ID сообщения
             message_html (str): Новый текст сообщения. Рекомендуется использование HTML
             
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/posts/{post_id}/edit", {"message_html": message_html, "message": message_html, "_xfToken": token})
+        return self.session.post(f"{MAIN_URL}/posts/{post_id}/edit", {"message_html": message_html, "message": message_html, "_xfToken": self.token})
 
 
     def delete_post(self, post_id: int, reason: str, hard_delete: bool = False) -> Response:
         """Удалить сообщение
 
         Attributes:
             post_id (int): ID сообщения
             reason (str): Причина для удаления
             hard_delete (bool): Полное удаление сообщения. По умолчанию False (необяз.)
         
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/posts/{post_id}/delete", {"reason": reason, "hard_delete": int(hard_delete), "_xfToken": token})
+        return self.session.post(f"{MAIN_URL}/posts/{post_id}/delete", {"reason": reason, "hard_delete": int(hard_delete), "_xfToken": self.token})
     
 
     def bookmark_post(self, post_id: int) -> Response:
         """Добавить сообщение в закладки
 
         Attributes:
             post_id (int): ID сообщения
         
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/posts/{post_id}/bookmark", {"_xfToken": token})
+        return self.session.post(f"{MAIN_URL}/posts/{post_id}/bookmark", {"_xfToken": self.token})
 
 
     # PROFILE POST
     def react_profile_post(self, post_id: int, reaction_id: int = 1) -> Response:
         """Поставить реакцию на сообщение профиля
 
         Attributes:
             post_id (int): ID сообщения профиля
             reaction_id (int): ID реакции. По умолчанию 1 (необяз.)
             
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f'{MAIN_URL}/profile-posts/{post_id}/react?reaction_id={reaction_id}', {'_xfToken': token})
+        return self.session.post(f'{MAIN_URL}/profile-posts/{post_id}/react?reaction_id={reaction_id}', {'_xfToken': self.token})
 
 
     def comment_profile_post(self, post_id: int, message_html: str) -> Response:
         """Прокомментировать сообщение профиля
 
         Attributes:
             post_id (int): ID сообщения
             message_html (str): Текст комментария. Рекомендуется использование HTML
             
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/profile-posts/{post_id}/add-comment", {"message_html": message_html, "_xfToken": token})
+        return self.session.post(f"{MAIN_URL}/profile-posts/{post_id}/add-comment", {"message_html": message_html, "_xfToken": self.token})
 
 
     def delete_profile_post(self, post_id: int, reason: str, hard_delete: bool = False) -> Response:
         """Удалить сообщение профиля
 
         Attributes:
             post_id (int): ID сообщения профиля
             reason (str): Причина для удаления
             hard_delete (bool): Полное удаление сообщения. По умолчанию False (необяз.)
         
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/profile-posts/{post_id}/delete", {"reason": reason, "hard_delete": int(hard_delete), "_xfToken": token})
+        return self.session.post(f"{MAIN_URL}/profile-posts/{post_id}/delete", {"reason": reason, "hard_delete": int(hard_delete), "_xfToken": self.token})
     
 
     def edit_profile_post(self, post_id: int, message_html: str) -> Response:
         """Отредактировать сообщение профиля
         
         Attributes:
             post_id (int): ID сообщения
             message_html (str): Новый текст сообщения. Рекомендуется использование HTML
             
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/profile-posts/{post_id}/edit", {"message_html": message_html, "message": message_html, "_xfToken": token})
+        return self.session.post(f"{MAIN_URL}/profile-posts/{post_id}/edit", {"message_html": message_html, "message": message_html, "_xfToken": self.token})
 
 
     # THREAD
-    def close_thread(self, thread_id: int) -> Response:
-        """Закрыть/открыть тему (для модерации)
-        
-        Attributes:
-            thread_id (int): ID темы
-        
-        Returns:
-            Объект Response модуля requests
-        """
-
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/threads/{thread_id}/quick-close", {'_xfToken': token})
-
-
-    def pin_thread(self, thread_id: int) -> Response:
-        """Закрепить/открепить тему (для модерации)
-        
-        Attributes:
-            thread_id (int): ID темы
-        
-        Returns:
-            Объект Response модуля requests
-        """
-
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/threads/{thread_id}/quick-stick", {'_xfToken': token})
-    
-
     def answer_thread(self, thread_id: int, message_html: str) -> Response:
         """Оставить сообщенме в теме
 
         Attributes:
             thread_id (int): ID темы
             message_html (str): Текст сообщения. Рекомендуется использование HTML
             
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/threads/{thread_id}/add-reply", {'_xfToken': token, 'message_html': message_html})
+        return self.session.post(f"{MAIN_URL}/threads/{thread_id}/add-reply", {'_xfToken': self.token, 'message_html': message_html})
 
 
     def watch_thread(self, thread_id: int, email_subscribe: bool = False, stop: bool = False) -> Response:
         """Изменить статус отслеживания темы
 
         Attributes:
             thread_id (int): ID темы
             email_subscribe (bool): Отправлять ли уведомления на почту. По умолчанию False (необяз.)
             stop (bool): - Принудительно прекратить отслеживание. По умолчанию False (необяз.)
         
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/threads/{thread_id}/watch", {'_xfToken': token, 'stop': int(stop), 'email_subscribe': int(email_subscribe)})
+        return self.session.post(f"{MAIN_URL}/threads/{thread_id}/watch", {'_xfToken': self.token, 'stop': int(stop), 'email_subscribe': int(email_subscribe)})
     
 
     def delete_thread(self, thread_id: int, reason: str, hard_delete: bool = False) -> Response:
         """Удалить тему
 
         Attributes:
             thread_id (int): ID темы
             reason (str): Причина для удаления
             hard_delete (bool): Полное удаление сообщения. По умолчанию False (необяз.)
             
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        return self.session.post(f"{MAIN_URL}/threads/{thread_id}/delete", {"reason": reason, "hard_delete": int(hard_delete), "_xfToken": token})
+        return self.session.post(f"{MAIN_URL}/threads/{thread_id}/delete", {"reason": reason, "hard_delete": int(hard_delete), "_xfToken": self.token})
     
 
     def edit_thread(self, thread_id: int, message_html: str) -> Response:
         """Отредактировать содержимое темы
 
         Attributes:
             thread_id (int): ID темы
             message_html (str): Новое содержимое ответа. Рекомендуется использование HTML
         
         Returns:
             Объект Response модуля requests
         """
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-1").content, 'lxml')
-        token = content.find('html')['data-csrf']
         thread_post_id = content.find('article', {'id': compile('js-post-*')})['id'].strip('js-post-')
-        return self.session.post(f"{MAIN_URL}/posts/{thread_post_id}/edit", {"message_html": message_html, "message": message_html, "_xfToken": token})
+        return self.session.post(f"{MAIN_URL}/posts/{thread_post_id}/edit", {"message_html": message_html, "message": message_html, "_xfToken": self.token})
     
 
     def edit_thread_info(self, thread_id: int, title: str = None, prefix_id: int = None, sticky: bool = True, opened: bool = True) -> Response:
         """Изменить заголовок и/или префикс темы
 
         Attributes:
             thread_id (int): ID темы
@@ -558,35 +553,57 @@
             sticky (bool): Закрепить (True - закреп / False - не закреп)
             opened (bool): Открыть/закрыть тему (True - открыть / False - закрыть)
         
         Returns:
             Объект Response модуля requests
         """
         
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        data = {"_xfToken": token, "sticky": sticky, "discussion_open": opened}
+        data = {"_xfToken": self.token}
 
         if title is not None: data.update({'title': title})
-        if prefix_id is not None: data.update({'prefix_id[]': prefix_id})
+        if prefix_id is not None: data.update({'prefix_id': prefix_id})
+        if opened: data.update({"discussion_open": 1})
+        if sticky: data.update({"sticky": 1})
 
         return self.session.post(f"{MAIN_URL}/threads/{thread_id}/edit", data)
     
 
+    def get_thread_category(self, thread_id: int) -> Category:
+        """Получить объект раздела, в котором создана тема
+
+        Attributes:
+            thread_id (int): ID темы
+        
+        Returns:
+            Объект Catrgory, в котормо создана тема
+        """
+        content = BeautifulSoup(self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-1").content, 'lxml')
+        
+        creator_id = content.find('a', {'class': 'username'})
+        if creator_id is None: return None
+        
+        return self.get_category(int(content.find('html')['data-container-key'].strip('node-')))
+    
+
     def get_thread_posts(self, thread_id: int, page: int = 1) -> list:
         """Получить все сообщения из темы на странице
         
         Attributes:
             thread_id (int): ID темы
             page (int): Cтраница для поиска. По умолчанию 1 (необяз.)
         
         Returns:
             Список (list), состоящий из ID всех сообщений на странице
         """
 
-        soup = BeautifulSoup(self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-{page}").content, 'lxml')
+        request = self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-{page}?_xfResponseType=json&_xfToken={self.token}").json()
+        if request['status'] == 'error':
+            return None
+        
+        soup = BeautifulSoup(unescape(request['html']['content']), "lxml")
         return [i['id'].strip('js-post-') for i in soup.find_all('article', {'id': compile('js-post-*')})]
     
 
     def react_thread(self, thread_id: int, reaction_id: int = 1) -> Response:
         """Поставить реакцию на тему
 
         Attributes:
@@ -594,29 +611,25 @@
             reaction_id (int): ID реакции. По умолчанию 1 (необяз.)
             
         Returns:
             Объект Response модуля requests
         """
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-1").content, 'lxml')
-        token = content.find('html')['data-csrf']
         thread_post_id = content.find('article', {'id': compile('js-post-*')})['id'].strip('js-post-')
-        return self.session.post(f'{MAIN_URL}/posts/{thread_post_id}/react?reaction_id={reaction_id}', {'_xfToken': token})
+        return self.session.post(f'{MAIN_URL}/posts/{thread_post_id}/react?reaction_id={reaction_id}', {'_xfToken': self.token})
 
 
     # OTHER
     def send_form(self, form_id: int, data: dict) -> Response:
         """Заполнить форму
 
         Attributes:
             form_id (int): ID формы
             data (dict): Информация для запонения в виде словаря. Форма словаря: {'question[id вопроса]' = 'необходимая информация'} | Пример: {'question[531]' = '1'}
         
         Returns:
             Объект Response модуля requests
         """
 
-        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
-        data.update({'_xfToken': token})
-        response = self.session.post(f"{MAIN_URL}/form/{form_id}/submit", data)
-
-        return response
+        data.update({'_xfToken': self.token})
+        return self.session.post(f"{MAIN_URL}/form/{form_id}/submit", data)
```

### Comparing `arz_api-1.8.2/arz_api/bypass_antibot/script.py` & `arz_api-2.0/arz_api/bypass_antibot/script.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8.2/arz_api/exceptions.py` & `arz_api-2.0/arz_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8.2/arz_api/models/category_object.py` & `arz_api-2.0/arz_api/models/category_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from requests import Response
 from typing import TYPE_CHECKING
+from arz_api.consts import MAIN_URL
 
 if TYPE_CHECKING:
     from arz_api import ArizonaAPI
 
 
 class Category:
-    def __init__(self, API: 'ArizonaAPI', id: int, title: str, pages_count: int, parent_category_id: int) -> None:
+    def __init__(self, API: 'ArizonaAPI', id: int, title: str, pages_count: int) -> None:
         self.API = API
         self.id = id
         """**ID категории**"""
         self.title = title
         """**Название категории**"""
         self.pages_count = pages_count
         """**Количество страниц в категории**"""
-        self.parent_category_id = parent_category_id
-        """**ID предыдуще категории (родительская). Если нет - None**"""
+        self.url = f"{MAIN_URL}/forums/{self.id}/"
+        """Ссылка на объект"""
 
 
     def create_thread(self, title: str, message_html: str, discussion_type: str = 'discussion', watch_thread: int = 1) -> Response:
         """Создать тему в категории
 
         Attributes:
             title (str): Название темы
@@ -31,14 +32,27 @@
             Объект Response модуля requests
 
         Todo:
             Cделать возврат ID новой темы
         """
 
         return self.API.create_thread(self.id, title, message_html, discussion_type, watch_thread)
+    
+
+    def get_parent_category(self) -> 'Category':
+        """Получить родительский раздел
+
+        Attributes:
+            thread_id (int): ID темы
+        
+        Returns:
+            Объект Catrgory, в котормо создана тема
+        """
+
+        return self.API.get_parent_category_of_category(self.id)
 
 
     def set_read(self) -> Response:
         """Отметить категорию как прочитанную
         
         Returns:
             Объект Response модуля requests
@@ -80,16 +94,7 @@
         """Получить дочерние категории из раздела
         
         Returns:
             Список (list), состоящий из ID дочерних категорий раздела
         """
 
         return self.API.get_categories(self.id)
-    
-
-    def get_url(self) -> str:
-        """Получить ссылку на объект
-        
-        Returns:
-            Ссылку в формате https://forum.arizona-rp.com/forums/x/"""
-        
-        return f"https://forum.arizona-rp.com/forums/{self.id}/"
```

### Comparing `arz_api-1.8.2/arz_api/models/member_object.py` & `arz_api-2.0/arz_api/models/member_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,15 @@
 from arz_api.consts import MAIN_URL
 
 if TYPE_CHECKING:
     from arz_api.api import ArizonaAPI
 
 
 class Member:
-    API: 'ArizonaAPI'  # Объект ArizonaAPI
-
-    id: int
-    username: str
-    user_title: str
-    avatar: str
-    roles: list
-    
-    messages_count: int
-    reactions_count: int
-    trophies_count: int
-
-    def __init__(self, API, id: int, username: str, user_title: str, avatar: str, roles: list, messages_count: int, reactions_count: int, trophies_count: int) -> None:
+    def __init__(self, API : 'ArizonaAPI', id: int, username: str, user_title: str, avatar: str, roles: list, messages_count: int, reactions_count: int, trophies_count: int) -> None:
         self.API = API
         self.id = id
         """**ID пользователя**"""
         self.username = username
         """**Имя пользователя**"""
         self.user_title = user_title
         """**Звание пользователя**"""
@@ -38,14 +26,18 @@
         self.messages_count = messages_count
         """**Количество сообщений в счетчике**"""
         self.reactions_count = reactions_count
         """**Количество реакций в счетчике**"""
         self.trophies_count = trophies_count
         """**Количество баллов в счетчике**"""
 
+        self.url = f"{MAIN_URL}/members/{self.id}/"
+        """Ссылка на объект"""
+        
+
     def follow(self) -> Response:
         """Изменить статус подписки на пользователя
         
         Returns:
             Объект Response модуля requests
         """
 
@@ -79,22 +71,14 @@
             page (int): Страница для поиска. По умолчанию 1 (необяз.)
             
         Returns:
             Cписок (list) с ID всех сообщений профиля
         """
 
         return self.API.get_profile_messages(self.id, page)
-    
-    def get_url(self) -> str:
-        """Получить ссылку на объект
-        
-        Returns:
-            Ссылку в формате https://forum.arizona-rp.com/members/x/"""
-        
-        return f"https://forum.arizona-rp.com/members/{self.id}/"
 
 
 class CurrentMember(Member):
     follow = property(doc='Forbidden method for Current Member object')
     ignore = property(doc='Forbidden method for Current Member object')
 
     def edit_avatar(self, upload_photo: str) -> Response:
```

### Comparing `arz_api-1.8.2/arz_api/models/other.py` & `arz_api-2.0/arz_api/models/other.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8.2/arz_api/models/post_object.py` & `arz_api-2.0/arz_api/models/post_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from requests import Response
 from typing import TYPE_CHECKING
+from arz_api.consts import MAIN_URL
 
 if TYPE_CHECKING:
     from arz_api import ArizonaAPI
     from arz_api.models import Member, Thread
 
 
 class Post:
@@ -17,14 +18,16 @@
         """**Объект Thread темы, в которой оставлено сообщение**"""
         self.create_date = create_date
         """**Дата отправки сообщения в UNIX**"""
         self.bb_content = bb_content
         """**Сырое содержимое сообщения**"""
         self.text_content = text_content
         """**Текст из сообщения**"""
+        self.url = f"{MAIN_URL}/posts/{self.id}/"
+        """Ссылка на объект"""
 
 
     def react(self, reaction_id: int = 1) -> Response:
         """Поставить реакцию на сообщение
 
         Attributes:
             reaction_id (int): ID реакции. По умолчанию 1 (необяз.)
@@ -65,23 +68,15 @@
     
     def bookmark(self) -> Response:
         """Добавить сообщение в закладки
         
         Returns:
             Объект Response модуля requests"""
         return self.API.bookmark_post(self.id)
-    
 
-    def get_url(self) -> str:
-        """Получить ссылку на объект
-        
-        Returns:
-            Ссылку в формате https://forum.arizona-rp.com/posts/x/"""
-        
-        return f"https://forum.arizona-rp.com/posts/{self.id}/"
 
 
 class ProfilePost:
     def __init__(self, API: 'ArizonaAPI', id: int, creator: 'Member', profile: 'Member', create_date: int, bb_content: str, text_content: str) -> None:
         self.API = API
         self.id = id
         """**ID сообщения профиля**"""
@@ -91,14 +86,16 @@
         """**Объект Member профиля, в котором оставлено сообщение**"""
         self.create_date = create_date
         """**Дата отправки сообщения в UNIX**"""
         self.bb_content = bb_content
         """**Сырое содержимое сообщения**"""
         self.text_content = text_content
         """**Текст из сообщения**"""
+        self.url = f"{MAIN_URL}/profile-posts/{self.id}/"
+        """Ссылка на объект"""
 
 
     def react(self, reaction_id: int = 1) -> Response:
         """Поставить реакцию на сообщение профиля
 
         Attributes:
             reaction_id (int): ID реакции. По умолчанию 1 (необяз.)
@@ -144,16 +141,7 @@
             message_html (str): Новое содержание сообщения профиля. Рекомендуется использование HTML
         
         Returns:
             Объект Response модуля requests
         """
 
         return self.API.edit_profile_post(self.id, message_html)
-
-
-    def get_url(self) -> str:
-        """Получить ссылку на объект
-        
-        Returns:
-            Ссылку в формате https://forum.arizona-rp.com/profile-posts/x/"""
-        
-        return f"https://forum.arizona-rp.com/profile-posts/{self.id}/"
```

### Comparing `arz_api-1.8.2/arz_api/models/thread_object.py` & `arz_api-2.0/arz_api/models/thread_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from requests import Response
 from typing import TYPE_CHECKING
+from arz_api.consts import MAIN_URL
 
 if TYPE_CHECKING:
     from arz_api.models.member_object import Member
     from arz_api.models.category_object import Category
     from arz_api import ArizonaAPI
 
 
 class Thread:
-    def __init__(self, API: 'ArizonaAPI', id: int, creator: 'Member', category: 'Category', create_date: int, title: str, prefix: str, content: str, html_content: str, pages_content: int, thread_post_id: int, is_closed: bool) -> None:
+    def __init__(self, API: 'ArizonaAPI', id: int, creator: 'Member', create_date: int, title: str, prefix: str, content: str, html_content: str, pages_content: int, thread_post_id: int, is_closed: bool) -> None:
         self.API = API
         self.id = id
         """**ID темы**"""
         self.creator = creator
         """**Объект Member создателя темы**"""
-        self.category = category
-        """**Объект Category раздела, в котором создана тема**"""
         self.create_date = create_date
         """**Дата создания темы в UNIX**"""
         self.title = title
         """**Заголовок темы**"""
         self.prefix = prefix
         """**Префикс темы**"""
         self.content = content
@@ -28,34 +27,16 @@
         """**Сырой контент темы**"""
         self.pages_count = pages_content
         """**Количество страниц с ответами в теме**"""
         self.is_closed = is_closed
         """**Закрыта ли тема**"""
         self.thread_post_id = thread_post_id
         """**ID сообщения темы (post_id)**"""
-
-
-    def close(self) -> Response:
-        """Закрыть/открыть тему (для модерации)
-        
-        Returns:
-            Объект Response модуля requests
-        """
-
-        return self.API.close_thread(self.id)
-
-
-    def pin(self) -> Response:
-        """Закрепить/открепить тему (для модерации)
-        
-        Returns:
-            Объект Response модуля requests
-        """
-
-        return self.API.pin_thread(self.id)
+        self.url = f"{MAIN_URL}/threads/{self.id}/"
+        """Ссылка на объект"""
     
 
     def answer(self, message_html: str) -> Response:
         """Оставить сообщение в теме
 
         Attributes:
             message_html (str): Cодержание ответа. Рекомендуется использование HTML
@@ -146,14 +127,15 @@
         Returns:
             Объект Response модуля requests
         """
 
         return self.API.react_thread(self.id, reaction_id)
     
 
-    def get_url(self) -> str:
-        """Получить ссылку на объект
+    def get_category(self) -> 'Category':
+        """Получить родительский раздел раздела
         
         Returns:
-            Ссылку в формате https://forum.arizona-rp.com/threads/x/"""
-        
-        return f"https://forum.arizona-rp.com/threads/{self.id}/"
+            Объект Catrgory, в котором создан раздел
+        """
+
+        return self.API.get_thread_category(self.id)
```

### Comparing `arz_api-1.8.2/arz_api.egg-info/PKG-INFO` & `arz_api-2.0/arz_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arz_api
-Version: 1.8.2
+Version: 2.0
 Summary: Модуль для взаимодействия с форумом без Xenforo ключей
 Home-page: https://github.com/TastyBread123/Arizona-API/
 Author: TastyBread123
 Author-email: ermakovglebyt@gmail.com
 Project-URL: Documentation, https://tastybread123.github.io/Arizona-API/arz_api.html
 Keywords: python xenforo arizona roleplay samp gta
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `arz_api-1.8.2/arz_api.egg-info/SOURCES.txt` & `arz_api-2.0/arz_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arz_api-1.8.2/setup.py` & `arz_api-2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name='arz_api',
-  version='1.8.2',
+  version='2.0',
   author='TastyBread123',
   author_email='ermakovglebyt@gmail.com',
   description='Модуль для взаимодействия с форумом без Xenforo ключей',
   long_description="""# Arizona-API
 API для взаимодействия с ресурсами Arizona без необходимости в получении API ключа xenforo у администраторов форума. Вы можете просто найти ваши куки (рекомендую для этого отдельные расширения) и начинать разработку!
 
 # Описание проекта
```

