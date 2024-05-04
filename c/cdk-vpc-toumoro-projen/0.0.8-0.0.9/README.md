# Comparing `tmp/cdk-vpc-toumoro-projen-0.0.8.tar.gz` & `tmp/cdk-vpc-toumoro-projen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-vpc-toumoro-projen-0.0.8.tar", last modified: Thu May  2 19:03:35 2024, max compression
+gzip compressed data, was "cdk-vpc-toumoro-projen-0.0.9.tar", last modified: Thu May  2 19:20:06 2024, max compression
```

## Comparing `cdk-vpc-toumoro-projen-0.0.8.tar` & `cdk-vpc-toumoro-projen-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:03:35.678888 cdk-vpc-toumoro-projen-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-02 19:03:14.000000 cdk-vpc-toumoro-projen-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 19:03:14.000000 cdk-vpc-toumoro-projen-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 19:03:35.678888 cdk-vpc-toumoro-projen-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 19:03:14.000000 cdk-vpc-toumoro-projen-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 19:03:14.000000 cdk-vpc-toumoro-projen-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:03:35.678888 cdk-vpc-toumoro-projen-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-02 19:03:14.000000 cdk-vpc-toumoro-projen-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:03:35.674888 cdk-vpc-toumoro-projen-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:03:35.674888 cdk-vpc-toumoro-projen-0.0.8/src/cdk-vpc-toumoro-projen/
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-02 19:03:14.000000 cdk-vpc-toumoro-projen-0.0.8/src/cdk-vpc-toumoro-projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:03:35.674888 cdk-vpc-toumoro-projen-0.0.8/src/cdk-vpc-toumoro-projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-02 19:03:14.000000 cdk-vpc-toumoro-projen-0.0.8/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23289 2024-05-02 19:03:14.000000 cdk-vpc-toumoro-projen-0.0.8/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpn-toumoro-projen@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:03:14.000000 cdk-vpc-toumoro-projen-0.0.8/src/cdk-vpc-toumoro-projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:03:35.678888 cdk-vpc-toumoro-projen-0.0.8/src/cdk_vpc_toumoro_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 19:03:35.000000 cdk-vpc-toumoro-projen-0.0.8/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-02 19:03:35.000000 cdk-vpc-toumoro-projen-0.0.8/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:03:35.000000 cdk-vpc-toumoro-projen-0.0.8/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 19:03:35.000000 cdk-vpc-toumoro-projen-0.0.8/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 19:03:35.000000 cdk-vpc-toumoro-projen-0.0.8/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:06.002659 cdk-vpc-toumoro-projen-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 19:20:06.002659 cdk-vpc-toumoro-projen-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:20:06.002659 cdk-vpc-toumoro-projen-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:05.998659 cdk-vpc-toumoro-projen-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:05.998659 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:05.998659 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23273 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:06.002659 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
```

### Comparing `cdk-vpc-toumoro-projen-0.0.8/LICENSE` & `cdk-vpc-toumoro-projen-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-vpc-toumoro-projen-0.0.8/PKG-INFO` & `cdk-vpc-toumoro-projen-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-vpc-toumoro-projen-0.0.8/setup.py` & `cdk-vpc-toumoro-projen-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-vpc-toumoro-projen",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "A CDK construct library to create a VPC with public and private subnets.",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk-vpc-toumoro-projen",
         "cdk-vpc-toumoro-projen._jsii"
     ],
     "package_data": {
         "cdk-vpc-toumoro-projen._jsii": [
-            "cdk-vpn-toumoro-projen@0.0.8.jsii.tgz"
+            "cdk-vpc-toumoro-projen@0.0.9.jsii.tgz"
         ],
         "cdk-vpc-toumoro-projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-vpc-toumoro-projen-0.0.8/src/cdk-vpc-toumoro-projen/__init__.py` & `cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
 class VpcBase(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
-    jsii_type="cdk-vpn-toumoro-projen.VpcBase",
+    jsii_type="cdk-vpc-toumoro-projen.VpcBase",
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         cidr: builtins.str,
@@ -38,29 +38,29 @@
         '''
         :param scope: -
         :param id: -
         :param cidr: 
         :param max_azs: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b21636b94b5a78fd95eb046647e71c792f5451749562ba2fe296e7e8436153cc)
+            type_hints = typing.get_type_hints(_typecheckingstub__7e3010ee1a172e4b1e59ff3f52ffda9e2c13c33133ed35298483e4ecbad5cb08)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = VpcProps(cidr=cidr, max_azs=max_azs)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="vpc")
     def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.Vpc:
         return typing.cast(_aws_cdk_aws_ec2_ceddda9d.Vpc, jsii.get(self, "vpc"))
 
 
 @jsii.data_type(
-    jsii_type="cdk-vpn-toumoro-projen.VpcProps",
+    jsii_type="cdk-vpc-toumoro-projen.VpcProps",
     jsii_struct_bases=[],
     name_mapping={"cidr": "cidr", "max_azs": "maxAzs"},
 )
 class VpcProps:
     def __init__(
         self,
         *,
@@ -68,15 +68,15 @@
         max_azs: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param cidr: 
         :param max_azs: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bfadf3be538979ec46f9a852283d79e4c96be9885403c851efd8c64ee91f7578)
+            type_hints = typing.get_type_hints(_typecheckingstub__9e4ca0a64414ac01f1cb33a9c52cbdf1d6944723ded23e6fbdd5101c0defc3a7)
             check_type(argname="argument cidr", value=cidr, expected_type=type_hints["cidr"])
             check_type(argname="argument max_azs", value=max_azs, expected_type=type_hints["max_azs"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "cidr": cidr,
         }
         if max_azs is not None:
             self._values["max_azs"] = max_azs
@@ -107,24 +107,24 @@
 __all__ = [
     "VpcBase",
     "VpcProps",
 ]
 
 publication.publish()
 
-def _typecheckingstub__b21636b94b5a78fd95eb046647e71c792f5451749562ba2fe296e7e8436153cc(
+def _typecheckingstub__7e3010ee1a172e4b1e59ff3f52ffda9e2c13c33133ed35298483e4ecbad5cb08(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     cidr: builtins.str,
     max_azs: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bfadf3be538979ec46f9a852283d79e4c96be9885403c851efd8c64ee91f7578(
+def _typecheckingstub__9e4ca0a64414ac01f1cb33a9c52cbdf1d6944723ded23e6fbdd5101c0defc3a7(
     *,
     cidr: builtins.str,
     max_azs: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdk-vpc-toumoro-projen-0.0.8/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO` & `cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

