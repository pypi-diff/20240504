# Comparing `tmp/django_dynamic_theme-0.0.6.tar.gz` & `tmp/django_dynamic_theme-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_theme-0.0.6.tar", max compression
+gzip compressed data, was "django_dynamic_theme-0.0.7.tar", max compression
```

## Comparing `django_dynamic_theme-0.0.6.tar` & `django_dynamic_theme-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     1068 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/LICENSE
--rw-r--r--   0        0        0     1738 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/README.md
--rw-r--r--   0        0        0        0 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/__init__.py
--rw-r--r--   0        0        0      713 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/admin.py
--rw-r--r--   0        0        0      498 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/apps.py
--rw-r--r--   0        0        0      475 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/context_processor.py
--rw-r--r--   0        0        0      141 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/errors.py
--rw-r--r--   0        0        0     1243 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/middleware.py
--rw-r--r--   0        0        0      516 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0001_initial.py
--rw-r--r--   0        0        0      436 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0002_background_name.py
--rw-r--r--   0        0        0      484 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0003_alter_background_primary_bg.py
--rw-r--r--   0        0        0     1241 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py
--rw-r--r--   0        0        0      733 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py
--rw-r--r--   0        0        0      526 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0006_alter_theme_background.py
--rw-r--r--   0        0        0      664 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py
--rw-r--r--   0        0        0      434 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0008_alter_theme_default.py
--rw-r--r--   0        0        0      976 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0009_navbar.py
--rw-r--r--   0        0        0      507 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0010_theme_navbar.py
--rw-r--r--   0        0        0      612 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0011_navbar_font_size.py
--rw-r--r--   0        0        0      479 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0012_navbar_text_color.py
--rw-r--r--   0        0        0      566 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0013_navbar_text_opacity.py
--rw-r--r--   0        0        0      604 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py
--rw-r--r--   0        0        0        0 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/__init__.py
--rw-r--r--   0        0        0     4942 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/models.py
--rw-r--r--   0        0        0      582 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/signals.py
--rw-r--r--   0        0        0        0 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/utill/__init__.py
--rw-r--r--   0        0        0      506 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/utill/color_converter.py
--rw-r--r--   0        0        0      740 2024-05-02 16:12:58.710385 django_dynamic_theme-0.0.6/django_dynamic_theme/utill/scss_editor.py
--rw-r--r--   0        0        0      743 2024-05-02 16:12:58.714385 django_dynamic_theme-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 django_dynamic_theme-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1738 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/admin.py
+-rw-r--r--   0        0        0      498 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/apps.py
+-rw-r--r--   0        0        0      475 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/context_processor.py
+-rw-r--r--   0        0        0      141 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/errors.py
+-rw-r--r--   0        0        0     1243 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/middleware.py
+-rw-r--r--   0        0        0      516 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0001_initial.py
+-rw-r--r--   0        0        0      436 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0002_background_name.py
+-rw-r--r--   0        0        0      484 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0003_alter_background_primary_bg.py
+-rw-r--r--   0        0        0     1241 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py
+-rw-r--r--   0        0        0      733 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py
+-rw-r--r--   0        0        0      526 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0006_alter_theme_background.py
+-rw-r--r--   0        0        0      664 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py
+-rw-r--r--   0        0        0      434 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0008_alter_theme_default.py
+-rw-r--r--   0        0        0      976 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0009_navbar.py
+-rw-r--r--   0        0        0      507 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0010_theme_navbar.py
+-rw-r--r--   0        0        0      612 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0011_navbar_font_size.py
+-rw-r--r--   0        0        0      479 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0012_navbar_text_color.py
+-rw-r--r--   0        0        0      566 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0013_navbar_text_opacity.py
+-rw-r--r--   0        0        0      604 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py
+-rw-r--r--   0        0        0      940 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0015_mediagallery.py
+-rw-r--r--   0        0        0      529 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0016_theme_media_gallery.py
+-rw-r--r--   0        0        0        0 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/__init__.py
+-rw-r--r--   0        0        0     6297 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/models.py
+-rw-r--r--   0        0        0      582 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/signals.py
+-rw-r--r--   0        0        0        0 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/utill/__init__.py
+-rw-r--r--   0        0        0      506 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/utill/color_converter.py
+-rw-r--r--   0        0        0      740 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/utill/scss_editor.py
+-rw-r--r--   0        0        0      743 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 django_dynamic_theme-0.0.7/PKG-INFO
```

### Comparing `django_dynamic_theme-0.0.6/LICENSE` & `django_dynamic_theme-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/README.md` & `django_dynamic_theme-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/admin.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/admin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Models for Themes"""
 
 from django.contrib import admin
 
-from django_dynamic_theme.models import Background, Navbar, Theme
+from django_dynamic_theme.models import Background, MediaGallery, Navbar, Theme
 
 
 @admin.register(Theme)
 class ThemeAdmin(admin.ModelAdmin):
     """
     The admin model to maange the themes."""
 
@@ -18,14 +18,29 @@
     """
     The admin model to set the backgrounds.
     """
 
     list_display = ["primary_bg"]
 
 
+@admin.register(MediaGallery)
+class MediaGalleryAdmin(admin.ModelAdmin):
+    """
+    The admin model for the media gallery.
+    """
+
+    list_display = [
+        "margin_left",
+        "margin_right",
+        "max_width",
+        "item_align",
+        "row_margin_top",
+    ]
+
+
 @admin.register(Navbar)
 class NavbarAdmin(admin.ModelAdmin):
     """
     The admin model for the navigation bar.
     """
 
     list_display = [
```

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/middleware.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/middleware.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0001_initial.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0006_alter_theme_background.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0006_alter_theme_background.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0009_navbar.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0009_navbar.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0011_navbar_font_size.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0011_navbar_font_size.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0013_navbar_text_opacity.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0013_navbar_text_opacity.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/models.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -82,14 +82,44 @@
     def export(self) -> str:
         """
         Exports it's values as string in SCSS format.
         """
         return f"background: {self.primary_bg};"
 
 
+class MediaGallery(ThemeElement):
+    """
+    A specialization of a n-dimensional list for the purpose of videos / images.
+    :param margin_left: The margin of the entire media gallery on left side.
+    :param margin_right: The margin of the entire media gallery on right side.
+    :param max_width: The maximum width of the entire media gallery.
+    :param item_align: The align of the single items within a row.
+    :param row_margin_top: The top margin between rows.
+    """
+
+    margin_left = models.CharField(max_length=50)
+    margin_right = models.CharField(max_length=50)
+    max_width = models.CharField(max_length=50)
+    item_align = models.CharField(max_length=50)
+    row_margin_top = models.CharField(max_length=50)
+
+    def export(self) -> str:
+        margin_left = f"margin-left: {self.margin_left};"
+        margin_right = f"margin-right: {self.margin_right};"
+        max_width = f"max-width: {self.max_width};"
+        text_align = f"text-align: {self.item_align};"
+        row = f".row {{margin-top: {self.row_margin_top};}}"
+        media_gallery = f""".mediagallery {{{margin_left}
+{margin_right}
+{max_width}
+{text_align}
+{row}}}"""
+        return media_gallery
+
+
 class Navbar(ThemeElement):
     """Stores the theming of bootstrap 5 nav bar"""
 
     background_color = ColorField()
     opacity = models.DecimalField(
         max_digits=3,
         decimal_places=2,
@@ -125,14 +155,17 @@
     """
     Combines all values.
     """
 
     name = models.CharField(max_length=50)
     default = models.BooleanField(default=False)
     background: Background = models.ForeignKey(Background, on_delete=models.CASCADE)
+    media_gallery: MediaGallery = models.ForeignKey(
+        MediaGallery, default=None, null=True, on_delete=models.DO_NOTHING
+    )
     navbar: Navbar = models.ForeignKey(
         Navbar, default=None, null=True, on_delete=models.CASCADE
     )
 
     # pylint: disable=too-few-public-methods
     class Meta:
         """Meta class of the Theme."""
@@ -153,15 +186,17 @@
         return f"static/{self.name}.scss"
 
     # pylint: disable=no-member
     def export(self) -> str:
         """
         Exports all listed configurations as string in SCSS format.
         """
-        return f"body {{{self.background.export()}}}\n{self.navbar.export()}"
+        return f"""body {{{self.background.export()}}}
+{self.media_gallery.export()}
+{self.navbar.export()}"""
 
     def write_export(self) -> None:
         """Writes the content of the export to the file."""
         scss_editor = ScssEditor(self.path)
         scss_editor.write(self.export())
 
     def save(self, *args, **kwargs) -> None:
```

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/signals.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/signals.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/django_dynamic_theme/utill/scss_editor.py` & `django_dynamic_theme-0.0.7/django_dynamic_theme/utill/scss_editor.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.6/pyproject.toml` & `django_dynamic_theme-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-dynamic-theme"
-version = "0.0.6"
+version = "0.0.7"
 description = "This enables the administrator of a django website to change the theme on the fly."
 authors = ["Segelzwerg <25705862+Segelzwerg@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 django = "^5.0"
```

### Comparing `django_dynamic_theme-0.0.6/PKG-INFO` & `django_dynamic_theme-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-theme
-Version: 0.0.6
+Version: 0.0.7
 Summary: This enables the administrator of a django website to change the theme on the fly.
 Author: Segelzwerg
 Author-email: 25705862+Segelzwerg@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-dynamic-theme Version: 0.0.6 Summary: This
+Metadata-Version: 2.1 Name: django-dynamic-theme Version: 0.0.7 Summary: This
 enables the administrator of a django website to change the theme on the fly.
 Author: Segelzwerg Author-email: 25705862+Segelzwerg@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=5.0,<6.0) Requires-Dist: django-colorfield
 (>=0.11.0,<0.12.0) Requires-Dist: django-compressor (>=4.4,<5.0) Requires-Dist:
```

