# Comparing `tmp/wagtail_resume-2.8.0.tar.gz` & `tmp/wagtail_resume-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_resume-2.8.0.tar", max compression
+gzip compressed data, was "wagtail_resume-2.9.0.tar", max compression
```

## Comparing `wagtail_resume-2.8.0.tar` & `wagtail_resume-2.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1069 2024-04-30 11:10:18.101386 wagtail_resume-2.8.0/LICENSE
--rw-r--r--   0        0        0     3496 2024-04-30 11:10:18.101386 wagtail_resume-2.8.0/README.md
--rw-r--r--   0        0        0     3813 2024-04-30 11:10:18.101386 wagtail_resume-2.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/__init__.py
--rw-r--r--   0        0        0      138 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/apps.py
--rw-r--r--   0        0        0     7326 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/blocks.py
--rw-r--r--   0        0        0     1085 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3477 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0001_initial.py
--rw-r--r--   0        0        0     1955 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0002_auto_20191227_0916.py
--rw-r--r--   0        0        0     3655 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0003_auto_20200110_1525.py
--rw-r--r--   0        0        0      467 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0004_auto_20200110_1656.py
--rw-r--r--   0        0        0     3843 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0005_auto_20200227_1224.py
--rw-r--r--   0        0        0      694 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
--rw-r--r--   0        0        0      792 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0     4472 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0008_auto_20220211_1557.py
--rw-r--r--   0        0        0      953 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0    18241 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py
--rw-r--r--   0        0        0    17599 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py
--rw-r--r--   0        0        0    17734 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py
--rw-r--r--   0        0        0    18655 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py
--rw-r--r--   0        0        0      535 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py
--rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/__init__.py
--rw-r--r--   0        0        0     4037 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/models.py
--rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/css/.gitkeep
--rw-r--r--   0        0        0     2058 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/css/resume_page.css
--rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/images/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/js/.gitkeep
--rw-r--r--   0        0        0      401 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
--rw-r--r--   0        0        0     1516 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
--rw-r--r--   0        0        0      951 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
--rw-r--r--   0        0        0      710 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
--rw-r--r--   0        0        0      653 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
--rw-r--r--   0        0        0      107 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page.html
--rw-r--r--   0        0        0     2556 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html
--rw-r--r--   0        0        0      688 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html
--rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templatetags/__init__.py
--rw-r--r--   0        0        0      139 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templatetags/wagtail_resume_extras.py
--rw-r--r--   0        0        0      142 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/urls.py
--rw-r--r--   0        0        0     2453 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/views.py
--rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 wagtail_resume-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-04 18:40:09.051622 wagtail_resume-2.9.0/LICENSE
+-rw-r--r--   0        0        0     3496 2024-05-04 18:40:09.051622 wagtail_resume-2.9.0/README.md
+-rw-r--r--   0        0        0     3813 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/apps.py
+-rw-r--r--   0        0        0     7326 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/blocks.py
+-rw-r--r--   0        0        0     1085 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3477 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1955 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0002_auto_20191227_0916.py
+-rw-r--r--   0        0        0     3655 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0003_auto_20200110_1525.py
+-rw-r--r--   0        0        0      467 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0004_auto_20200110_1656.py
+-rw-r--r--   0        0        0     3843 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0005_auto_20200227_1224.py
+-rw-r--r--   0        0        0      694 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
+-rw-r--r--   0        0        0      792 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0     4472 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0008_auto_20220211_1557.py
+-rw-r--r--   0        0        0      953 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0    18241 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py
+-rw-r--r--   0        0        0    17599 2024-05-04 18:40:09.055621 wagtail_resume-2.9.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py
+-rw-r--r--   0        0        0    17734 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py
+-rw-r--r--   0        0        0    18655 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py
+-rw-r--r--   0        0        0      535 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py
+-rw-r--r--   0        0        0        0 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/migrations/__init__.py
+-rw-r--r--   0        0        0     4037 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/models.py
+-rw-r--r--   0        0        0        0 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/static/wagtail_resume/css/.gitkeep
+-rw-r--r--   0        0        0     2547 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/static/wagtail_resume/css/resume_page.css
+-rw-r--r--   0        0        0        0 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/static/wagtail_resume/images/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/static/wagtail_resume/js/.gitkeep
+-rw-r--r--   0        0        0      401 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
+-rw-r--r--   0        0        0     1516 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
+-rw-r--r--   0        0        0      896 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
+-rw-r--r--   0        0        0      710 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
+-rw-r--r--   0        0        0      653 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
+-rw-r--r--   0        0        0      107 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/resume_page.html
+-rw-r--r--   0        0        0     2559 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html
+-rw-r--r--   0        0        0      688 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html
+-rw-r--r--   0        0        0        0 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templatetags/__init__.py
+-rw-r--r--   0        0        0      139 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/templatetags/wagtail_resume_extras.py
+-rw-r--r--   0        0        0      142 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/urls.py
+-rw-r--r--   0        0        0     2453 2024-05-04 18:40:09.059621 wagtail_resume-2.9.0/wagtail_resume/views.py
+-rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 wagtail_resume-2.9.0/PKG-INFO
```

### Comparing `wagtail_resume-2.8.0/LICENSE` & `wagtail_resume-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/README.md` & `wagtail_resume-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/pyproject.toml` & `wagtail_resume-2.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "wagtail-resume"
 authors = ["Adin Hodovic <hodovicadin@gmail.com>"]
 license = "MIT"
-version = "2.8.0"
+version = "2.9.0"
 readme = "README.md"
 homepage = "https://github.com/adinhodovic/wagtail-resume"
 repository = "https://github.com/adinhodovic/wagtail-resume"
 documentation = "https://github.com/adinhodovic/wagtail-resume"
 description = "A Wagtail project made to simplify creation of resumes for developers."
 keywords = ["Resume", "Django", "Wagtail", "CMS"]
 classifiers = [
```

### Comparing `wagtail_resume-2.8.0/wagtail_resume/blocks.py` & `wagtail_resume-2.9.0/wagtail_resume/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po` & `wagtail_resume-2.9.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0001_initial.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0002_auto_20191227_0916.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0002_auto_20191227_0916.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0003_auto_20200110_1525.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0003_auto_20200110_1525.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0005_auto_20200227_1224.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0005_auto_20200227_1224.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0008_auto_20220211_1557.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0008_auto_20220211_1557.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py` & `wagtail_resume-2.9.0/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/models.py` & `wagtail_resume-2.9.0/wagtail_resume/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/css/resume_page.css` & `wagtail_resume-2.9.0/wagtail_resume/static/wagtail_resume/css/resume_page.css`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 body {
   margin: 0;
   color: #212121;
 }
 
 p {
+  font-size: 1rem;
   line-height: 1.5;
+}
+
+li {
   font-size: 1rem;
 }
 
 h2 {
   font-weight: 600;
   font-size: 1.3rem;
 }
@@ -104,16 +108,14 @@
 a {
   color: #4652f6;
   text-decoration: none;
   background-color: transparent;
 }
 
 .photo {
-  margin-bottom: 2.5rem;
-  margin-top: 1rem;
   border-radius: 50%;
   width: 250px;
 }
 
 .social-links img {
   width: 1.5rem;
 }
@@ -122,19 +124,14 @@
   vertical-align: super;
 }
 
 .date {
   color: #5b5b55;
 }
 
-.fas,
-.fab {
-  font-size: 1.5rem;
-}
-
 .pdf {
   display: None;
 }
 
 .personal-info {
   align-items: center;
   display: flex;
@@ -177,7 +174,62 @@
     display: block;
   }
 
   .photo {
     width: 45%;
   }
 }
+
+/* Print styles */
+@media print {
+  h1 {
+    font-size: 1.3rem;
+  }
+
+  h2 {
+    font-size: 1.1rem;
+  }
+
+  p,
+  li,
+  h3,
+  a {
+    font-size: 0.8rem;
+  }
+
+  .mt-1 {
+    margin-top: 0.125rem;
+  }
+
+  .mb-1 {
+    margin-bottom: 0.125rem;
+  }
+
+  .mb-2 {
+    margin-bottom: 0.25rem;
+  }
+
+  .mt-2 {
+    margin-top: 0.25rem;
+  }
+
+  .mt-3 {
+    margin-top: 0.5rem;
+  }
+
+  .mt-4 {
+    margin-top: 1.5rem;
+  }
+
+  hr {
+    margin-top: 0.5rem;
+    margin-bottom: 0.5rem;
+  }
+
+  .social-links img {
+    width: 1rem;
+  }
+
+  .photo {
+    width: 200px;
+  }
+}
```

### Comparing `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html` & `wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html` & `wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html`

 * *Files 8% similar despite different names*

```diff
@@ -15,13 +15,13 @@
     {{ experience.from_date }} -
     {% if experience.currently_working_here %}
       <b>{% trans "Present" %}</b>
     {% else %}
       {{ experience.to_date }}
     {% endif %}
   </p>
-  <div style="margin-top: 1.5rem;">{{ experience.text | markdown }}</div>
+  <div class="mt-3">{{ experience.text | markdown }}</div>
   {% if not forloop.last %}<hr />{% endif %}
 {% endfor %}
 {% if value.maximum_experiences_displayed > 0 %}
-  <p style="margin-top:2rem; font-weight:600; font-style: italic;">{{ value.maximum_experiences_user_text }}</p>
+  <h3 class="mt-4 italic">{{ value.maximum_experiences_user_text }}</h3>
 {% endif %}
```

#### html2text {}

```diff
@@ -8,9 +8,9 @@
 {% endif %}
 {{ experience.from_date }} - {% if experience.currently_working_here %} {{%%
 ttrraannss ""PPrreesseenntt"" %%}} {% else %} {{ experience.to_date }} {% endif %}
 {{ experience.text | markdown }}
 {% if not forloop.last %}
 ===============================================================================
 {% endif %} {% endfor %} {% if value.maximum_experiences_displayed > 0 %}
-{{ value.maximum_experiences_user_text }}
+******** {{{{ vvaalluuee..mmaaxxiimmuumm__eexxppeerriieenncceess__uusseerr__tteexxtt }}}} ********
 {% endif %}
```

### Comparing `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html` & `wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html` & `wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html` & `wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   }
 </style>
 {% endwith %}
 {# djlint:on #}
 <body style="font-family:{% if page.font %} '{{ page.font|title }}',{% endif %} 'Roboto Condensed', sans-serif">
   <div class="container">
     <div class="resume">
-      <div class="personal-info mt-2 mb-1">
+      <div class="personal-info">
         <div>
           <h2 class="mt-2 mb-0">{{ page.full_name }}</h2>
           {% if page.role %}<h2 class="mt-2">{{ page.role }}</h2>{% endif %}
           <div class="social-links">
             {% for social_link in page.social_links %}
               <div class="social-links">
                 <a class="social-link" href="{{ social_link.value.url }}">
@@ -41,15 +41,15 @@
               </div>
             {% endfor %}
           </div>
           {% if page.display_last_update %}
             <p class="small italic mt-1">Last update: {{ page.latest_revision_created_at|date }}</p>
           {% endif %}
         </div>
-        <div>{% image page.photo original class="photo" %}</div>
+        <div class="mt-4">{% image page.photo original class="photo" %}</div>
       </div>
       <div>
         <h2 class="mt-4 mb-0">
           {% if page.about_icon %}<i class="{{ page.about_icon }}"></i>{% endif %}
           <span>{% trans "About" %}</span>
         </h2>
         <hr />
```

### Comparing `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html` & `wagtail_resume-2.9.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/wagtail_resume/views.py` & `wagtail_resume-2.9.0/wagtail_resume/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.8.0/PKG-INFO` & `wagtail_resume-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-resume
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Wagtail project made to simplify creation of resumes for developers.
 Home-page: https://github.com/adinhodovic/wagtail-resume
 License: MIT
 Keywords: Resume,Django,Wagtail,CMS
 Author: Adin Hodovic
 Author-email: hodovicadin@gmail.com
 Requires-Python: >=3.10,<4.0
```

