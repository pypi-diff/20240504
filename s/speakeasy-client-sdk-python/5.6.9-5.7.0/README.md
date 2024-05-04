# Comparing `tmp/speakeasy-client-sdk-python-5.6.9.tar.gz` & `tmp/speakeasy-client-sdk-python-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-5.6.9.tar", last modified: Fri Apr 19 00:12:10 2024, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-5.7.0.tar", last modified: Fri May  3 00:13:03 2024, max compression
```

## Comparing `speakeasy-client-sdk-python-5.6.9.tar` & `speakeasy-client-sdk-python-5.7.0.tar`

### file list

```diff
@@ -1,134 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.217817 speakeasy-client-sdk-python-5.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)    22454 2024-04-19 00:12:10.217817 speakeasy-client-sdk-python-5.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14621 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 00:12:10.217817 speakeasy-client-sdk-python-5.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.197817 speakeasy-client-sdk-python-5.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.201817 speakeasy-client-sdk-python-5.6.9/src/speakeasy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.201817 speakeasy-client-sdk-python-5.6.9/src/speakeasy/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/apiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    21141 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.201817 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.201817 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.201817 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.209817 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/deleteapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/deleteapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/deleteschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/deleteversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/downloadschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/downloadschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/findapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generateopenapispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generatepostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getallapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getallapiversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getchangesreportsignedurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getlintingreportsignedurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getrequestfromeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getrevisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getschemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/gettags.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getworkspaceaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getworkspacetargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/insertversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/postworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/queryeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/registerschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/uploadreport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/upsertapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/upsertapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.213817 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/accessdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/api_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/apiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/apiendpoint_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/boundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/clievent.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/embedtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/filter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/generateopenapispecdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/getnamespacesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/getrevisionsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/gettagsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/interactiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/preflightrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/preflighttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/requestmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/schemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/targetsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/unboundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/v2descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/versionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/versionmetadata_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28253 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.217817 speakeasy-client-sdk-python-5.6.9/src/speakeasy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-19 00:12:01.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:12:10.217817 speakeasy-client-sdk-python-5.6.9/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22454 2024-04-19 00:12:09.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-19 00:12:10.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:12:09.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 00:12:09.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 00:12:09.000000 speakeasy-client-sdk-python-5.6.9/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.523321 speakeasy-client-sdk-python-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-05-03 00:13:03.523321 speakeasy-client-sdk-python-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 00:13:03.523321 speakeasy-client-sdk-python-5.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.503321 speakeasy-client-sdk-python-5.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.503321 speakeasy-client-sdk-python-5.7.0/src/speakeasy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.507321 speakeasy-client-sdk-python-5.7.0/src/speakeasy/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/apiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24256 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13901 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16531 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.507321 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.507321 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.507321 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.515321 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/deleteapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/deleteapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/deleteschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/deleteversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/downloadschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/downloadschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/findapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generateopenapispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generatepostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getallapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getallapiversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getchangesreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getlintingreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getrevisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getschemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/gettags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getworkspaceaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getworkspaceeventsbytarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getworkspacetargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/insertversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/posttags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/postworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/queryeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/registerschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/searchworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/uploadreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/upsertapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/upsertapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.519321 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/accessdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/addtags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/api_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/apiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/apiendpoint_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/boundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/clievent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/embedtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/getnamespacesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/getrevisionsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/gettagsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/interactiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/preflightrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/preflighttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/requestmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/schemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/targetsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/unboundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/v2descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/versionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/versionmetadata_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28253 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.519321 speakeasy-client-sdk-python-5.7.0/src/speakeasy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-05-03 00:12:54.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:03.523321 speakeasy-client-sdk-python-5.7.0/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-05-03 00:13:03.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-03 00:13:03.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 00:13:03.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-03 00:13:03.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 00:13:03.000000 speakeasy-client-sdk-python-5.7.0/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-5.6.9/PKG-INFO` & `speakeasy-client-sdk-python-5.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.9
+Version: 5.7.0
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -85,14 +85,15 @@
         ### [artifacts](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md)
         
         * [get_blob](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_blob) - Get blob for a particular digest
         * [get_manifest](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_manifest) - Get manifest for a particular reference
         * [get_namespaces](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_namespaces) - Each namespace contains many revisions.
         * [get_revisions](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_revisions)
         * [get_tags](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_tags)
+        * [post_tags](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#post_tags) - Add tags to an existing revision
         * [preflight](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#preflight) - Get access token for communicating with OCI distribution endpoints
         
         ### [auth](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md)
         
         * [get_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
         * [get_user](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_user) - Get information about the current user.
         * [get_workspace_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
@@ -118,17 +119,18 @@
         
         * [get_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
         * [get_valid_embed_access_tokens](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
         * [revoke_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#revoke_embed_access_token) - Revoke an embed access EmbedToken.
         
         ### [events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md)
         
-        * [get_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_events) - Load recent events for a particular workspace
+        * [get_workspace_events_by_target](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_events_by_target) - Load recent events for a particular workspace
         * [get_workspace_targets](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_targets) - Load targets for a particular workspace
         * [post_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#post_workspace_events) - Post events for a specific workspace
+        * [search_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#search_workspace_events) - Search events for a particular workspace by any field
         <!-- End Available Resources and Operations [operations] -->
         
         
         
         
         
         
@@ -152,19 +154,21 @@
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
             workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceEventsRequest()
+        req = operations.GetWorkspaceEventsByTargetRequest(
+            target_id='<value>',
+        )
         
         res = None
         try:
-            res = s.events.get_workspace_events(req)
+            res = s.events.get_workspace_events_by_target(req)
         except errors.Error as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -304,15 +308,15 @@
         <!-- End Authentication [security] -->
         
         <!-- Start Global Parameters [global-parameters] -->
         ## Global Parameters
         
         A parameter is configured globally. This parameter may be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
         
-        For example, you can set `workspaceID` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_workspace_events`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+        For example, you can set `workspaceID` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_workspace_events_by_target`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
         
         
         ### Available Globals
         
         The following global parameter is available.
         
         | Name | Type | Required | Description |
@@ -329,17 +333,19 @@
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
             workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceEventsRequest()
+        req = operations.GetWorkspaceEventsByTargetRequest(
+            target_id='<value>',
+        )
         
-        res = s.events.get_workspace_events(req)
+        res = s.events.get_workspace_events_by_target(req)
         
         if res.cli_event_batch is not None:
             # handle response
             pass
         
         ```
         <!-- End Global Parameters [global-parameters] -->
```

### Comparing `speakeasy-client-sdk-python-5.6.9/README.md` & `speakeasy-client-sdk-python-5.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 ### [artifacts](docs/sdks/artifacts/README.md)
 
 * [get_blob](docs/sdks/artifacts/README.md#get_blob) - Get blob for a particular digest
 * [get_manifest](docs/sdks/artifacts/README.md#get_manifest) - Get manifest for a particular reference
 * [get_namespaces](docs/sdks/artifacts/README.md#get_namespaces) - Each namespace contains many revisions.
 * [get_revisions](docs/sdks/artifacts/README.md#get_revisions)
 * [get_tags](docs/sdks/artifacts/README.md#get_tags)
+* [post_tags](docs/sdks/artifacts/README.md#post_tags) - Add tags to an existing revision
 * [preflight](docs/sdks/artifacts/README.md#preflight) - Get access token for communicating with OCI distribution endpoints
 
 ### [auth](docs/sdks/auth/README.md)
 
 * [get_access_token](docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
 * [get_user](docs/sdks/auth/README.md#get_user) - Get information about the current user.
 * [get_workspace_access](docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
@@ -111,17 +112,18 @@
 
 * [get_embed_access_token](docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
 * [get_valid_embed_access_tokens](docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
 * [revoke_embed_access_token](docs/sdks/embeds/README.md#revoke_embed_access_token) - Revoke an embed access EmbedToken.
 
 ### [events](docs/sdks/events/README.md)
 
-* [get_workspace_events](docs/sdks/events/README.md#get_workspace_events) - Load recent events for a particular workspace
+* [get_workspace_events_by_target](docs/sdks/events/README.md#get_workspace_events_by_target) - Load recent events for a particular workspace
 * [get_workspace_targets](docs/sdks/events/README.md#get_workspace_targets) - Load targets for a particular workspace
 * [post_workspace_events](docs/sdks/events/README.md#post_workspace_events) - Post events for a specific workspace
+* [search_workspace_events](docs/sdks/events/README.md#search_workspace_events) - Search events for a particular workspace by any field
 <!-- End Available Resources and Operations [operations] -->
 
 
 
 
 
 
@@ -145,19 +147,21 @@
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
     workspace_id='<value>',
 )
 
-req = operations.GetWorkspaceEventsRequest()
+req = operations.GetWorkspaceEventsByTargetRequest(
+    target_id='<value>',
+)
 
 res = None
 try:
-    res = s.events.get_workspace_events(req)
+    res = s.events.get_workspace_events_by_target(req)
 except errors.Error as e:
     # handle exception
     raise(e)
 except errors.SDKError as e:
     # handle exception
     raise(e)
 
@@ -297,15 +301,15 @@
 <!-- End Authentication [security] -->
 
 <!-- Start Global Parameters [global-parameters] -->
 ## Global Parameters
 
 A parameter is configured globally. This parameter may be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
 
-For example, you can set `workspaceID` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_workspace_events`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+For example, you can set `workspaceID` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_workspace_events_by_target`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
 
 
 ### Available Globals
 
 The following global parameter is available.
 
 | Name | Type | Required | Description |
@@ -322,17 +326,19 @@
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
     workspace_id='<value>',
 )
 
-req = operations.GetWorkspaceEventsRequest()
+req = operations.GetWorkspaceEventsByTargetRequest(
+    target_id='<value>',
+)
 
-res = s.events.get_workspace_events(req)
+res = s.events.get_workspace_events_by_target(req)
 
 if res.cli_event_batch is not None:
     # handle response
     pass
 
 ```
 <!-- End Global Parameters [global-parameters] -->
```

### Comparing `speakeasy-client-sdk-python-5.6.9/setup.py` & `speakeasy-client-sdk-python-5.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='speakeasy-client-sdk-python',
-    version='5.6.9',
+    version='5.7.0',
     author='Speakeasy',
     description='Speakeasy API Client SDK for Python',
     url='https://github.com/speakeasy-api/speakeasy-client-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/_hooks/registration.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/_hooks/sdkhooks.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/_hooks/types.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/apiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/apis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/artifacts.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/artifacts.py`

 * *Files 7% similar despite different names*

```diff
@@ -319,14 +319,71 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
+    def post_tags(self, request: operations.PostTagsRequest) -> operations.PostTagsResponse:
+        r"""Add tags to an existing revision"""
+        hook_ctx = HookContext(operation_id='postTags', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(base_url, '/v1/artifacts/namespaces/{namespace_name}/tags', request)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        req_content_type, data, form = utils.serialize_request_body(request, operations.PostTagsRequest, "add_tags", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        res = operations.PostTagsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            pass
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
+                res.error = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+
+        return res
+
+    
+    
     def preflight(self, request: Optional[shared.PreflightRequest]) -> operations.PreflightResponse:
         r"""Get access token for communicating with OCI distribution endpoints"""
         hook_ctx = HookContext(operation_id='preflight', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/v1/artifacts/preflight'
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/auth.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,24 +164,27 @@
         def do_request():
             nonlocal req
             try:
                 req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
                 req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-                if e is not None:
-                    raise e
+                _, err = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if err is not None:
+                    raise err from e
+                raise e
 
             if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
                 result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
                 if e is not None:
                     raise e
                 if result is not None:
                     http_res = result
+                else:
+                    raise errors.SDKError('Unexpected error occurred', -1, '', None)
             else:
                 http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/embeds.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/events.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def get_workspace_events(self, request: operations.GetWorkspaceEventsRequest) -> operations.GetWorkspaceEventsResponse:
+    def get_workspace_events_by_target(self, request: operations.GetWorkspaceEventsByTargetRequest) -> operations.GetWorkspaceEventsByTargetResponse:
         r"""Load recent events for a particular workspace"""
-        hook_ctx = HookContext(operation_id='getWorkspaceEvents', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetWorkspaceEventsGlobals(
+        hook_ctx = HookContext(operation_id='getWorkspaceEventsByTarget', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetWorkspaceEventsByTargetGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/workspace/{workspaceID}/events', request, _globals)
+        url = utils.generate_url(base_url, '/v1/workspace/{workspaceID}/events/targets/{targetID}/events', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -54,15 +54,15 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetWorkspaceEventsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetWorkspaceEventsByTargetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CliEvent]])
                 res.cli_event_batch = out
             else:
                 content_type = http_res.headers.get('Content-Type')
@@ -191,24 +191,27 @@
         def do_request():
             nonlocal req
             try:
                 req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
                 req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-                if e is not None:
-                    raise e
+                _, err = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if err is not None:
+                    raise err from e
+                raise e
 
             if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
                 result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
                 if e is not None:
                     raise e
                 if result is not None:
                     http_res = result
+                else:
+                    raise errors.SDKError('Unexpected error occurred', -1, '', None)
             else:
                 http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
@@ -225,14 +228,81 @@
         elif http_res.status_code >= 400 and http_res.status_code < 500:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 500 and http_res.status_code < 600:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+        return res
+
+    
+    
+    def search_workspace_events(self, request: operations.SearchWorkspaceEventsRequest) -> operations.SearchWorkspaceEventsResponse:
+        r"""Search events for a particular workspace by any field"""
+        hook_ctx = HookContext(operation_id='searchWorkspaceEvents', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.SearchWorkspaceEventsGlobals(
+            workspace_id=self.sdk_configuration.globals.workspace_id,
+        )
+        
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(base_url, '/v1/workspace/{workspaceID}/events', request, _globals)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        res = operations.SearchWorkspaceEventsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[List[shared.CliEvent]])
+                res.cli_event_batch = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 400 and http_res.status_code < 500:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 500 and http_res.status_code < 600:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.Error)
+                raise out
+            else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/metadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/errors/error.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/errors/sdkerror.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,21 +32,23 @@
 from .getschemarevision import *
 from .getschemas import *
 from .gettags import *
 from .getuser import *
 from .getvalidembedaccesstokens import *
 from .getversionmetadata import *
 from .getworkspaceaccess import *
-from .getworkspaceevents import *
+from .getworkspaceeventsbytarget import *
 from .getworkspacetargets import *
 from .insertversionmetadata import *
+from .posttags import *
 from .postworkspaceevents import *
 from .preflight import *
 from .queryeventlog import *
 from .registerschema import *
 from .revokeembedaccesstoken import *
+from .searchworkspaceevents import *
 from .uploadreport import *
 from .upsertapi import *
 from .upsertapiendpoint import *
 from .validateapikey import *
 
-__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetBlobRequest","GetBlobResponse","GetChangesReportSignedURLRequest","GetChangesReportSignedURLResponse","GetChangesReportSignedURLSignedAccess","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetLintingReportSignedURLRequest","GetLintingReportSignedURLResponse","GetLintingReportSignedURLSignedAccess","GetManifestRequest","GetManifestResponse","GetNamespacesResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetRevisionsRequest","GetRevisionsResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetTagsRequest","GetTagsResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsGlobals","GetWorkspaceEventsRequest","GetWorkspaceEventsResponse","GetWorkspaceTargetsGlobals","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostWorkspaceEventsGlobals","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","PreflightResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaFile","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","UploadReportRequestBody","UploadReportResponse","UploadReportUploadedReport","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
+__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetBlobRequest","GetBlobResponse","GetChangesReportSignedURLRequest","GetChangesReportSignedURLResponse","GetChangesReportSignedURLSignedAccess","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetLintingReportSignedURLRequest","GetLintingReportSignedURLResponse","GetLintingReportSignedURLSignedAccess","GetManifestRequest","GetManifestResponse","GetNamespacesResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetRevisionsRequest","GetRevisionsResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetTagsRequest","GetTagsResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsByTargetGlobals","GetWorkspaceEventsByTargetRequest","GetWorkspaceEventsByTargetResponse","GetWorkspaceTargetsGlobals","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostTagsRequest","PostTagsResponse","PostWorkspaceEventsGlobals","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","PreflightResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaFile","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","SearchWorkspaceEventsGlobals","SearchWorkspaceEventsRequest","SearchWorkspaceEventsResponse","UploadReportRequestBody","UploadReportResponse","UploadReportUploadedReport","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getaccesstoken.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getblob.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getblob.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getchangesreportsignedurl.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getchangesreportsignedurl.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getlintingreportsignedurl.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getlintingreportsignedurl.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getmanifest.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getnamespaces.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getnamespaces.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getorganizations.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getorganizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getrevisions.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getrevisions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/gettags.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/gettags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getuser.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getuser.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getworkspaceaccess.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getworkspaceaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getworkspaceevents.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getworkspaceeventsbytarget.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 import requests as requests_http
 from ...models.shared import clievent as shared_clievent
 from datetime import datetime
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetWorkspaceEventsGlobals:
+class GetWorkspaceEventsByTargetGlobals:
     workspace_id: Optional[str] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'workspaceID', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class GetWorkspaceEventsRequest:
+class GetWorkspaceEventsByTargetRequest:
+    target_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'targetID', 'style': 'simple', 'explode': False }})
+    r"""Filter to only return events corresponding to a particular gen_lock_id (gen_lock_id uniquely identifies a target)"""
     after_created_at: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'after_created_at', 'style': 'form', 'explode': True }})
     r"""Filter to only return events created after this timestamp"""
-    generate_gen_lock_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'generate_gen_lock_id', 'style': 'form', 'explode': True }})
-    r"""Filter to only return events corresponding to a particular gen_lock_id (gen_lock_id uniquely identifies a target)"""
     workspace_id: Optional[str] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'workspaceID', 'style': 'simple', 'explode': False }})
     r"""Unique identifier of the workspace."""
     
 
 
 
 @dataclasses.dataclass
-class GetWorkspaceEventsResponse:
+class GetWorkspaceEventsByTargetResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
     cli_event_batch: Optional[List[shared_clievent.CliEvent]] = dataclasses.field(default=None)
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/getworkspacetargets.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/getworkspacetargets.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/postworkspaceevents.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/postworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/preflight.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/preflight.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/uploadreport.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/uploadreport.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/upsertapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/operations/validateapikey.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/operations/validateapikey.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .accessdetails import *
 from .accesstoken import *
+from .addtags import *
 from .annotations import *
 from .api import *
 from .api_input import *
 from .apiendpoint import *
 from .apiendpoint_input import *
 from .apikeydetails import *
 from .boundedrequest import *
@@ -34,8 +35,8 @@
 from .targetsdk import *
 from .unboundedrequest import *
 from .user import *
 from .v2descriptor import *
 from .versionmetadata import *
 from .versionmetadata_input import *
 
-__all__ = ["API","APIEndpoint","APIEndpointInput","APIInput","APIKeyDetails","AccessDetails","AccessToken","AccessTokenAccountType","AccessTokenUser","AccountType","Annotations","BoundedRequest","Claims","CliEvent","EmbedAccessTokenResponse","EmbedToken","FeatureFlags","Filter","Filters","GenerateBumpType","GenerateOpenAPISpecDiff","GetNamespacesResponse","GetRevisionsResponse","GetTagsResponse","InteractionType","Level","Manifest","Namespace","OpenapiDiffBumpType","Organization","OrganizationAccountType","PreflightRequest","PreflightToken","Report","RequestMetadata","Revision","Schema","SchemaDiff","Security","Tag","TargetSDK","Type","UnboundedRequest","User","V2Descriptor","ValueChange","VersionMetadata","VersionMetadataInput","Workspaces"]
+__all__ = ["API","APIEndpoint","APIEndpointInput","APIInput","APIKeyDetails","AccessDetails","AccessToken","AccessTokenAccountType","AccessTokenUser","AccountType","AddTags","Annotations","BoundedRequest","Claims","CliEvent","EmbedAccessTokenResponse","EmbedToken","FeatureFlags","Filter","Filters","GenerateBumpType","GenerateOpenAPISpecDiff","GetNamespacesResponse","GetRevisionsResponse","GetTagsResponse","InteractionType","Level","Manifest","Namespace","OpenapiDiffBumpType","Organization","OrganizationAccountType","PreflightRequest","PreflightToken","Report","RequestMetadata","Revision","Schema","SchemaDiff","Security","Tag","TargetSDK","Type","UnboundedRequest","User","V2Descriptor","ValueChange","VersionMetadata","VersionMetadataInput","Workspaces"]
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/accessdetails.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/accessdetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/accesstoken.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/accesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/annotations.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/annotations.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,31 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Annotations:
     r"""Annotations"""
     org_opencontainers_image_authors: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.authors'), 'exclude': lambda f: f is None }})
-    org_opencontainers_image_base_digest: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.base.digest'), 'exclude': lambda f: f is None }})
-    org_opencontainers_image_base_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.base.name'), 'exclude': lambda f: f is None }})
+    r"""The authors of the image"""
     org_opencontainers_image_created: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.created'), 'exclude': lambda f: f is None }})
+    r"""The time the image was created"""
     org_opencontainers_image_description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.description'), 'exclude': lambda f: f is None }})
+    r"""Human-readable description of the software packaged in the image"""
     org_opencontainers_image_documentation: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.documentation'), 'exclude': lambda f: f is None }})
+    r"""The documentation URL of the image"""
     org_opencontainers_image_licenses: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.licenses'), 'exclude': lambda f: f is None }})
     org_opencontainers_image_ref_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.ref.name'), 'exclude': lambda f: f is None }})
+    r"""Name of the reference for a target"""
     org_opencontainers_image_revision: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.revision'), 'exclude': lambda f: f is None }})
+    r"""Source control revision identifier"""
     org_opencontainers_image_source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.source'), 'exclude': lambda f: f is None }})
+    r"""The URL to get source code for building the image"""
     org_opencontainers_image_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.title'), 'exclude': lambda f: f is None }})
+    r"""Human-readable title of the image"""
     org_opencontainers_image_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.url'), 'exclude': lambda f: f is None }})
+    r"""The URL of the image"""
     org_opencontainers_image_vendor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.vendor'), 'exclude': lambda f: f is None }})
+    r"""Name of the distributing entity, organization or individual."""
     org_opencontainers_image_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org.opencontainers.image.version'), 'exclude': lambda f: f is None }})
+    r"""The version of the packaged software"""
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/api_input.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/api_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/apiendpoint_input.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/apiendpoint_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/apikeydetails.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
 from speakeasy import utils
-from typing import List, Optional
+from typing import Optional
 
-class AccountType(str, Enum):
+class OrganizationAccountType(str, Enum):
     FREE = 'free'
     SCALE_UP = 'scale-up'
     ENTERPRISE = 'enterprise'
 
-class FeatureFlags(str, Enum):
-    SCHEMA_REGISTRY = 'schema_registry'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class APIKeyDetails:
-    account_type: AccountType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_type') }})
-    feature_flags: List[FeatureFlags] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feature_flags') }})
-    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspace_id') }})
-    generation_access_unlimited: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generation_access_unlimited'), 'exclude': lambda f: f is None }})
+class Organization:
+    r"""A speakeasy organization"""
+    account_type: OrganizationAccountType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_type') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    created_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created)at'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+    slug: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('slug'), 'exclude': lambda f: f is None }})
+    updated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updated_at'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/clievent.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/clievent.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/filter_.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/filter_.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/generateopenapispecdiff.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/generateopenapispecdiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/getrevisionsresponse.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/getrevisionsresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/manifest.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/manifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/namespace.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/namespace.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/organization.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/apikeydetails.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
 from enum import Enum
 from speakeasy import utils
-from typing import Optional
+from typing import List, Optional
 
-class OrganizationAccountType(str, Enum):
+class AccountType(str, Enum):
     FREE = 'free'
     SCALE_UP = 'scale-up'
     ENTERPRISE = 'enterprise'
 
+class FeatureFlags(str, Enum):
+    SCHEMA_REGISTRY = 'schema_registry'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Organization:
-    r"""A speakeasy organization"""
-    account_type: OrganizationAccountType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_type') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    created_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created)at'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
-    slug: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('slug'), 'exclude': lambda f: f is None }})
-    updated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updated_at'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+class APIKeyDetails:
+    account_type: AccountType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_type') }})
+    feature_flags: List[FeatureFlags] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feature_flags') }})
+    org_slug: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org_slug') }})
+    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspace_id') }})
+    workspace_slug: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspace_slug') }})
+    generation_access_unlimited: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generation_access_unlimited'), 'exclude': lambda f: f is None }})
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/preflighttoken.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/preflighttoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/report.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/report.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/revision.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/revision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/security.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/tag.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/tag.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/targetsdk.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/targetsdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,11 +59,17 @@
     r"""User email from git configuration."""
     git_user_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('git_user_name'), 'exclude': lambda f: f is None }})
     r"""User's name from git configuration. (not GitHub username)"""
     hostname: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hostname'), 'exclude': lambda f: f is None }})
     r"""Remote hostname."""
     repo_label: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('repo_label'), 'exclude': lambda f: f is None }})
     r"""Label of the git repository."""
+    source_blob_digest: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source_blob_digest'), 'exclude': lambda f: f is None }})
+    r"""The blob digest of the source."""
+    source_namespace_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source_namespace_name'), 'exclude': lambda f: f is None }})
+    r"""The namespace name of the source."""
+    source_revision_digest: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source_revision_digest'), 'exclude': lambda f: f is None }})
+    r"""The revision digest of the source."""
     success: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('success'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the event was successful."""
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/user.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/v2descriptor.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/v2descriptor.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/versionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/models/shared/versionmetadata_input.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/models/shared/versionmetadata_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/organizations.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/organizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/reports.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/reports.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/requests.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/schemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/sdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/sdkconfiguration.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/sdkconfiguration.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 class SDKConfiguration:
     client: requests_http.Session
     globals: internal.Globals
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server: Optional[str] = ''
     language: str = 'python'
-    openapi_doc_version: str = '0.4.0'
-    sdk_version: str = '5.6.9'
-    gen_version: str = '2.311.1'
-    user_agent: str = 'speakeasy-sdk/python 5.6.9 2.311.1 0.4.0 speakeasy-client-sdk-python'
+    openapi_doc_version: str = '0.4.0 .'
+    sdk_version: str = '5.7.0'
+    gen_version: str = '2.319.10'
+    user_agent: str = 'speakeasy-sdk/python 5.7.0 2.319.10 0.4.0 . speakeasy-client-sdk-python'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.9
+Version: 5.7.0
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -85,14 +85,15 @@
         ### [artifacts](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md)
         
         * [get_blob](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_blob) - Get blob for a particular digest
         * [get_manifest](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_manifest) - Get manifest for a particular reference
         * [get_namespaces](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_namespaces) - Each namespace contains many revisions.
         * [get_revisions](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_revisions)
         * [get_tags](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_tags)
+        * [post_tags](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#post_tags) - Add tags to an existing revision
         * [preflight](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#preflight) - Get access token for communicating with OCI distribution endpoints
         
         ### [auth](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md)
         
         * [get_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
         * [get_user](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_user) - Get information about the current user.
         * [get_workspace_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
@@ -118,17 +119,18 @@
         
         * [get_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
         * [get_valid_embed_access_tokens](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
         * [revoke_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#revoke_embed_access_token) - Revoke an embed access EmbedToken.
         
         ### [events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md)
         
-        * [get_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_events) - Load recent events for a particular workspace
+        * [get_workspace_events_by_target](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_events_by_target) - Load recent events for a particular workspace
         * [get_workspace_targets](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_targets) - Load targets for a particular workspace
         * [post_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#post_workspace_events) - Post events for a specific workspace
+        * [search_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#search_workspace_events) - Search events for a particular workspace by any field
         <!-- End Available Resources and Operations [operations] -->
         
         
         
         
         
         
@@ -152,19 +154,21 @@
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
             workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceEventsRequest()
+        req = operations.GetWorkspaceEventsByTargetRequest(
+            target_id='<value>',
+        )
         
         res = None
         try:
-            res = s.events.get_workspace_events(req)
+            res = s.events.get_workspace_events_by_target(req)
         except errors.Error as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -304,15 +308,15 @@
         <!-- End Authentication [security] -->
         
         <!-- Start Global Parameters [global-parameters] -->
         ## Global Parameters
         
         A parameter is configured globally. This parameter may be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
         
-        For example, you can set `workspaceID` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_workspace_events`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+        For example, you can set `workspaceID` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_workspace_events_by_target`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
         
         
         ### Available Globals
         
         The following global parameter is available.
         
         | Name | Type | Required | Description |
@@ -329,17 +333,19 @@
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
             workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceEventsRequest()
+        req = operations.GetWorkspaceEventsByTargetRequest(
+            target_id='<value>',
+        )
         
-        res = s.events.get_workspace_events(req)
+        res = s.events.get_workspace_events_by_target(req)
         
         if res.cli_event_batch is not None:
             # handle response
             pass
         
         ```
         <!-- End Global Parameters [global-parameters] -->
```

### Comparing `speakeasy-client-sdk-python-5.6.9/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-5.7.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,29 +57,32 @@
 src/speakeasy/models/operations/getschemarevision.py
 src/speakeasy/models/operations/getschemas.py
 src/speakeasy/models/operations/gettags.py
 src/speakeasy/models/operations/getuser.py
 src/speakeasy/models/operations/getvalidembedaccesstokens.py
 src/speakeasy/models/operations/getversionmetadata.py
 src/speakeasy/models/operations/getworkspaceaccess.py
-src/speakeasy/models/operations/getworkspaceevents.py
+src/speakeasy/models/operations/getworkspaceeventsbytarget.py
 src/speakeasy/models/operations/getworkspacetargets.py
 src/speakeasy/models/operations/insertversionmetadata.py
+src/speakeasy/models/operations/posttags.py
 src/speakeasy/models/operations/postworkspaceevents.py
 src/speakeasy/models/operations/preflight.py
 src/speakeasy/models/operations/queryeventlog.py
 src/speakeasy/models/operations/registerschema.py
 src/speakeasy/models/operations/revokeembedaccesstoken.py
+src/speakeasy/models/operations/searchworkspaceevents.py
 src/speakeasy/models/operations/uploadreport.py
 src/speakeasy/models/operations/upsertapi.py
 src/speakeasy/models/operations/upsertapiendpoint.py
 src/speakeasy/models/operations/validateapikey.py
 src/speakeasy/models/shared/__init__.py
 src/speakeasy/models/shared/accessdetails.py
 src/speakeasy/models/shared/accesstoken.py
+src/speakeasy/models/shared/addtags.py
 src/speakeasy/models/shared/annotations.py
 src/speakeasy/models/shared/api.py
 src/speakeasy/models/shared/api_input.py
 src/speakeasy/models/shared/apiendpoint.py
 src/speakeasy/models/shared/apiendpoint_input.py
 src/speakeasy/models/shared/apikeydetails.py
 src/speakeasy/models/shared/boundedrequest.py
```

