# Comparing `tmp/email_profile-0.3.0.tar.gz` & `tmp/email_profile-0.4.0.tar.gz`

## Comparing `email_profile-0.3.0.tar` & `email_profile-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 email_profile-0.3.0/.env-example
--rw-r--r--   0        0        0    52850 2020-02-02 00:00:00.000000 email_profile-0.3.0/_poetry.lock
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 email_profile-0.3.0/_pyproject-poetry.toml
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 email_profile-0.3.0/example.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 email_profile-0.3.0/requirements-dev.txt
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 email_profile-0.3.0/setup.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 email_profile-0.3.0/tox.ini
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 email_profile-0.3.0/.github/workflows/python-app-code-quality.yml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 email_profile-0.3.0/.github/workflows/python-app-test.yml
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 email_profile-0.3.0/.github/workflows/python-publish-pypi-test.yml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 email_profile-0.3.0/.github/workflows/python-publish-pypi.yml
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/cli.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/core.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/data.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/message.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/status.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/utils.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/where.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/abstract/__init__.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/abstract/controller.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/abstract/model.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/models/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/models/attachment.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/models/email.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/models/mailbox.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/serializers/__init__.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/serializers/where.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_message.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_status.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_where_mailbox.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_where_mode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/serializers/__init__.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/serializers/test_where.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 email_profile-0.3.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 email_profile-0.3.0/LICENSE
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 email_profile-0.3.0/README.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 email_profile-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 email_profile-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 email_profile-0.4.0/.env-example
+-rw-r--r--   0        0        0    52850 2020-02-02 00:00:00.000000 email_profile-0.4.0/_poetry.lock
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 email_profile-0.4.0/_pyproject-poetry.toml
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 email_profile-0.4.0/example.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 email_profile-0.4.0/requirements-dev.txt
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 email_profile-0.4.0/setup.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 email_profile-0.4.0/tox.ini
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 email_profile-0.4.0/.github/workflows/python-app-code-quality.yml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 email_profile-0.4.0/.github/workflows/python-app-test.yml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 email_profile-0.4.0/.github/workflows/python-publish-pypi-test.yml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 email_profile-0.4.0/.github/workflows/python-publish-pypi.yml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/cli.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/core.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/data.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/message.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/status.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/utils.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/where.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/abstract/__init__.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/abstract/controller.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/abstract/model.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/models/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/models/attachment.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/models/email.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/models/mailbox.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/serializers/__init__.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 email_profile-0.4.0/email_profile/serializers/where.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/email_profile/__init__.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/email_profile/test_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/email_profile/test_message.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/email_profile/test_status.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/email_profile/test_where_mailbox.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/email_profile/test_where_mode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/email_profile/serializers/__init__.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 email_profile-0.4.0/tests/email_profile/serializers/test_where.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 email_profile-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 email_profile-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 email_profile-0.4.0/README.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 email_profile-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 email_profile-0.4.0/PKG-INFO
```

### Comparing `email_profile-0.3.0/_poetry.lock` & `email_profile-0.4.0/_poetry.lock`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/_pyproject-poetry.toml` & `email_profile-0.4.0/_pyproject-poetry.toml`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/example.py` & `email_profile-0.4.0/example.py`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/setup.py` & `email_profile-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/tox.ini` & `email_profile-0.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/.github/workflows/python-app-code-quality.yml` & `email_profile-0.4.0/.github/workflows/python-app-code-quality.yml`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/.github/workflows/python-app-test.yml` & `email_profile-0.4.0/.github/workflows/python-app-test.yml`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/.github/workflows/python-publish-pypi-test.yml` & `email_profile-0.4.0/.github/workflows/python-publish-pypi-test.yml`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/.github/workflows/python-publish-pypi.yml` & `email_profile-0.4.0/.github/workflows/python-publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/email_profile/__init__.py` & `email_profile-0.4.0/email_profile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 __author__ = 'Fernando Celmer <email@fernandocelmer.com>'
 __copyright__ = """MIT License
 
 Copyright (c) 2024 Email Profile
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `email_profile-0.3.0/email_profile/message.py` & `email_profile-0.4.0/email_profile/message.py`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/email_profile/status.py` & `email_profile-0.4.0/email_profile/status.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,19 +15,27 @@
 class Status:
 
     OK = 'OK'
     NO = 'NO'
     BAD = 'BAD'
 
     @staticmethod
-    def validate_status(status: str, raise_error: bool = True) -> StatusResponse:
+    def validate_status(
+            status: str,
+            raise_error: bool = True) -> StatusResponse:
         data = {
-            Status.OK: (True, "Login completed, now in authenticated state"),
-            Status.NO: (False, "Login failure: user name or password rejected"),
-            Status.BAD: (False, "Command unknown or arguments invalid")
+            Status.OK: (
+                True,
+                "Login completed, now in authenticated state"),
+            Status.NO: (
+                False,
+                "Login failure: user name or password rejected"),
+            Status.BAD: (
+                False,
+                "Command unknown or arguments invalid")
         }.get(status, (False, "Unknown error"))
 
         if raise_error:
             if not data[0]:
                 raise Exception(data[1])
 
         return StatusResponse(
```

### Comparing `email_profile-0.3.0/email_profile/where.py` & `email_profile-0.4.0/email_profile/where.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,16 @@
 
     _data = []
     _message = []
     _status = False
     _total = 0
 
     def __init__(self,
-                 mode: Mode = Mode.ALL,
                  mailbox: Mailbox = Mailbox.INBOX,
                  server: any = None) -> None:
-        self.mode = mode
         self.mailbox = mailbox
         self.server = server
 
     def where(self,
               since: Optional[date] = None,
               before: Optional[date] = None,
               subject: Optional[str] = None,
@@ -53,15 +51,16 @@
                 options[item] = variables[item]
 
         status, total = self.server.select(self.mailbox.capitalize())
         validate = Status.validate_status(status)
         self._status = validate.type
         self._total = int(total[0].decode())
 
-        status, data = self.server.search(None, WhereSerializer(**options).result())
+        status, data = self.server.search(
+            None, WhereSerializer(**options).result())
         validate = Status.validate_status(status)
         self._status = validate.type
         self._data = Status.validate_data(data)
 
         return self
 
     def count(self) -> int:
@@ -81,15 +80,17 @@
                 _groups += 1
 
             splited = [self._data[item::_groups] for item in range(_groups)]
 
             for group_mail in splited:
                 _sum_searching += len(group_mail)
 
-                status, messages = self.server.fetch(','.join(group_mail), '(RFC822)')
+                status, messages = self.server.fetch(
+                    ','.join(group_mail), '(RFC822)'
+                )
                 messages = [message for message in messages if message != b')']
 
                 print(f"Loading: {_sum_searching}/{len(self._data)}", end="\r")
 
                 for reference, text in messages:
                     _id = int(reference.split()[0])
                     self._message.append(Message(text, _id).result())
```

### Comparing `email_profile-0.3.0/email_profile/serializers/where.py` & `email_profile-0.4.0/email_profile/serializers/where.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 """
 Dataclass Module
 """
 
 from datetime import date
 from dataclasses import dataclass, field
 
-
-class Validations:
-
-    def __post_init__(self):
-        for name, _field in self.__dataclass_fields__.items():
-            if method := getattr(self, f"validate_{name}"):
-                setattr(self, name, method(field=_field))
+from email_profile.abstract.model import Validations
 
 
 @dataclass
 class WhereSerializer(Validations):
 
     since: date = field(default="")
     before: date = field(default="")
```

### Comparing `email_profile-0.3.0/tests/email_profile/test_data.py` & `email_profile-0.4.0/tests/email_profile/test_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,112 @@
+from json import loads
+from pathlib import Path
+
 from email_profile.data import DataClass
 from email_profile.models import AttachmentModel, EmailModel
 
+from tests.conftest import text_html   # noqa: F401
+
 
-def test_instance_data_sqlalchemy():
+def test_instance_data():
     data = DataClass()
 
     assert isinstance(data, DataClass)
     assert data.email is None
     assert data.attachments == list()
 
 
-def test_data_sqlalchemy_add_email():
+def test_data_add_email():
     email = EmailModel()
     data = DataClass()
     data.add_email(model=email)
 
     assert isinstance(data.email, EmailModel)
     assert data.email == email
 
 
-def test_data_sqlalchemy_add_attachment():
+def test_data_add_attachment():
     attachment = AttachmentModel()
     data = DataClass()
     data.add_attachment(model=attachment)
 
     assert len(data.attachments) == 1
     assert isinstance(data.attachments[0], AttachmentModel)
     assert data.attachments[0] == attachment
 
 
-def test_data_sqlalchemy_json():
+def test_data_json():
     email = EmailModel(id=1)
-    attachment = AttachmentModel(id=42)
 
     data = DataClass()
     data.add_email(model=email)
-    data.add_attachment(model=attachment)
 
-    response = data.json()
+    response = data.json(create_file=False)
 
     assert isinstance(response, dict)
-    assert response.get("email")
-    assert response.get("email")["id"] == 1
-    assert response.get("attachments")[0]["id"] == 42
+    assert response.get("id") == 1
+
+
+def test_data_json_create_file():
+    file_name = "42.json"
+    path = Path("tests", "json")
+
+    email = EmailModel(id=42)
+
+    data = DataClass()
+    data.add_email(model=email)
+
+    data.json(
+        path=path,
+        create_file=True
+    )
+
+    assert path.joinpath(file_name).exists()
+
+    with open(path.joinpath(file_name), mode="r") as file:
+        email = loads(file.read())
+        assert email.get("id") == 42
+
+    path.joinpath(file_name).unlink()
+    path.rmdir()
+
+
+def test_data_html(text_html):  # noqa: F811
+    email = EmailModel(
+        id=42,
+        body_text_html=text_html
+    )
+
+    data = DataClass()
+    data.add_email(model=email)
+
+    response = data.html(create_file=False)
+
+    assert "Email Profile" in response
+
+
+def test_data_html_create_file(text_html):  # noqa: F811
+    file_name = "index.html"
+    path = Path("tests", "html")
+
+    email = EmailModel(
+        id=42,
+        body_text_html=text_html
+    )
+
+    data = DataClass()
+    data.add_email(model=email)
+
+    data.html(
+        path=path,
+        create_file=True
+    )
+
+    assert path.joinpath("42", file_name).exists()
+
+    with open(path.joinpath("42", file_name), mode="r") as file:
+        email = file.read()
+        assert "Email Profile" in email
+
+    path.joinpath("42", file_name).unlink()
+    path.joinpath("42").rmdir()
+    path.rmdir()
```

### Comparing `email_profile-0.3.0/tests/email_profile/test_status.py` & `email_profile-0.4.0/tests/email_profile/test_status.py`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/tests/email_profile/serializers/test_where.py` & `email_profile-0.4.0/tests/email_profile/serializers/test_where.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,18 @@
     input_since = datetime(1996, 5, 31)
     input_before = date.today()
     input_subject = 'abc'
 
     output_since = input_since.strftime('%d-%b-%Y')
     output_before = input_before.strftime('%d-%b-%Y')
     output_subject = input_subject
-    output_result = f'(SINCE {output_since}) (BEFORE {output_before}) (SUBJECT "{output_subject}")'
+    output_result = f'\
+        (SINCE {output_since}) \
+            (BEFORE {output_before}) \
+                (SUBJECT "{output_subject}")'
 
     serializer = WhereSerializer(
         since=input_since,
         before=input_before,
         subject=input_subject
     )
```

### Comparing `email_profile-0.3.0/.gitignore` & `email_profile-0.4.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -141,8 +141,9 @@
 .pypirc
 
 # Database
 *.sqlite3
 *.db
 
 # Others
-html
+*/html
+*/json
```

### Comparing `email_profile-0.3.0/LICENSE` & `email_profile-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `email_profile-0.3.0/README.md` & `email_profile-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -8,19 +8,30 @@
 - **Source Code**: [Link](https://github.com/FernandoCelmer/email-profile)
 
 ---
 
 ## Check list
 
 - [x] Query API Structure
+    - [x] Mailbox
+    - [x] Since
+    - [x] Before
+    - [x] Subject
+    - [x] From Who
+    - [ ] Body
+    - [ ] Unseen
 - [x] Data table structure
+- [x] Get emails
+- [x] Download Attachments
 - [x] Response JSON
-- [ ] Dump JSON
-- [x] Dump HTML
+- [x] Dump File JSON
 - [x] Response HTML
+- [x] Dump File HTML
+- [x] Response Attachment File
+- [ ] Dump Attachment File
 - [ ] CLI Email
 - [ ] Documentation
 
 ## How to install?
 
 ```python
 pip install email-profile
```

### Comparing `email_profile-0.3.0/pyproject.toml` & `email_profile-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "email-profile"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Fernando Celmer", email="email@fernandocelmer.com" },
 ]
 license = {file = "LICENSE"}
 description = "📩 Email Profile"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `email_profile-0.3.0/PKG-INFO` & `email_profile-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: email-profile
-Version: 0.3.0
+Version: 0.4.0
 Summary: 📩 Email Profile
 Project-URL: Homepage, https://github.com/linux-profile/email-profile
 Project-URL: Issues, https://github.com/linux-profile/email-profile/issues
 Project-URL: Repository, https://github.com/linux-profile/email-profile
 Project-URL: Documentation, https://github.com/linux-profile/email-profile/blob/master/README.md
 Author-email: Fernando Celmer <email@fernandocelmer.com>
 License: MIT License
@@ -52,19 +52,30 @@
 - **Source Code**: [Link](https://github.com/FernandoCelmer/email-profile)
 
 ---
 
 ## Check list
 
 - [x] Query API Structure
+    - [x] Mailbox
+    - [x] Since
+    - [x] Before
+    - [x] Subject
+    - [x] From Who
+    - [ ] Body
+    - [ ] Unseen
 - [x] Data table structure
+- [x] Get emails
+- [x] Download Attachments
 - [x] Response JSON
-- [ ] Dump JSON
-- [x] Dump HTML
+- [x] Dump File JSON
 - [x] Response HTML
+- [x] Dump File HTML
+- [x] Response Attachment File
+- [ ] Dump Attachment File
 - [ ] CLI Email
 - [ ] Documentation
 
 ## How to install?
 
 ```python
 pip install email-profile
```

