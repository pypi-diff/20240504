# Comparing `tmp/cpac-1.8.6.post1.dev1.tar.gz` & `tmp/cpac-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpac-1.8.6.post1.dev1.tar", max compression
+gzip compressed data, was "cpac-1.8.7.tar", max compression
```

## Comparing `cpac-1.8.6.post1.dev1.tar` & `cpac-1.8.7.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0      117 2024-03-28 16:41:13.623795 cpac-1.8.6.post1.dev1/AUTHORS.rst
--rw-r--r--   0        0        0     1117 2024-03-28 16:41:13.623795 cpac-1.8.6.post1.dev1/LICENSE.txt
--rw-r--r--   0        0        0     7559 2024-03-28 16:41:13.623795 cpac-1.8.6.post1.dev1/README.rst
--rw-r--r--   0        0        0     2774 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/pyproject.toml
--rw-r--r--   0        0        0      331 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/__init__.py
--rw-r--r--   0        0        0    14435 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/__main__.py
--rw-r--r--   0        0        0      594 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/backends/__init__.py
--rw-r--r--   0        0        0     7784 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/backends/docker.py
--rw-r--r--   0        0        0    16628 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/backends/platform.py
--rw-r--r--   0        0        0     7276 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/backends/singularity.py
--rw-r--r--   0        0        0     1416 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/helpers/__init__.py
--rwxr-xr-x   0        0        0     3870 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/helpers/cpac_parse_resources.py
--rwxr-xr-x   0        0        0     1826 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/helpers/cpac_read_crash.py
--rw-r--r--   0        0        0      224 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/utils/__init__.py
--rw-r--r--   0        0        0      899 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/utils/checks.py
--rw-r--r--   0        0        0     8877 2024-03-28 16:41:13.627795 cpac-1.8.6.post1.dev1/src/cpac/utils/utils.py
--rw-r--r--   0        0        0     9430 1970-01-01 00:00:00.000000 cpac-1.8.6.post1.dev1/PKG-INFO
+-rw-r--r--   0        0        0      117 2024-05-04 06:11:00.083567 cpac-1.8.7/AUTHORS.rst
+-rw-r--r--   0        0        0     1122 2024-05-04 06:11:00.083567 cpac-1.8.7/LICENSE.txt
+-rw-r--r--   0        0        0     8434 2024-05-04 06:11:00.083567 cpac-1.8.7/README.rst
+-rw-r--r--   0        0        0     3974 2024-05-04 06:11:00.083567 cpac-1.8.7/pyproject.toml
+-rw-r--r--   0        0        0      331 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/__init__.py
+-rw-r--r--   0        0        0    16725 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/__main__.py
+-rw-r--r--   0        0        0      346 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/backends/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/backends/apptainer/__init__.py
+-rw-r--r--   0        0        0      778 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/backends/apptainer/apptainer.py
+-rw-r--r--   0        0        0     1279 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/backends/apptainer/spython.py
+-rw-r--r--   0        0        0     7671 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/backends/docker.py
+-rw-r--r--   0        0        0    17964 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/backends/platform.py
+-rw-r--r--   0        0        0     7703 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/backends/singularity.py
+-rw-r--r--   0        0        0     1416 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/helpers/__init__.py
+-rwxr-xr-x   0        0        0     3870 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/helpers/cpac_parse_resources.py
+-rwxr-xr-x   0        0        0     1826 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/helpers/cpac_read_crash.py
+-rw-r--r--   0        0        0      329 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/utils/__init__.py
+-rw-r--r--   0        0        0     9785 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/utils/bare_wrap.py
+-rw-r--r--   0        0        0      899 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/utils/checks.py
+-rw-r--r--   0        0        0     9100 2024-05-04 06:11:00.083567 cpac-1.8.7/src/cpac/utils/utils.py
+-rw-r--r--   0        0        0    10654 1970-01-01 00:00:00.000000 cpac-1.8.7/PKG-INFO
```

### Comparing `cpac-1.8.6.post1.dev1/LICENSE.txt` & `cpac-1.8.7/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright © 2020 Child Mind Institute
+Copyright © 2020-2024 Child Mind Institute
 Copyright (c) 2019 anibalsolon
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `cpac-1.8.6.post1.dev1/README.rst` & `cpac-1.8.7/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -15,33 +15,36 @@
 .. admonition:: Note about cpac versioning
 
     This package's versioning scheme changed in version 1.8.5 to match C-PAC's versioning. From cpac v1.8.5 forward, the version of cpac indicates the newest supported version of C-PAC.
 
 Dependencies
 ============
 
-* `Python <https://www.python.org>`_ ≥ 3.8
+* `Python <https://www.python.org>`_ ≥ 3.10
 * `pip <https://pip.pypa.io>`_
 * At least one of:
 
   * `Docker <https://www.docker.com>`_
-  * **`Singularity <https://sylabs.io/singularity>`_ ≥ 2.5 \< 3.0** (this is different than the main release of ``cpac``!)
+  * `Apptainer <https://apptainer.org/documentation/>`_ ≥ 1.0
+  * `Singularity <https://sylabs.io/singularity>`_ ≥ 3.0 [*]_
+
+.. [*] ``cpac`` *may* work with older versions of Singularity, but `Singularity Python <https://singularityhub.github.io/singularity-cli/>`_ dropped support for Singularity < 3.0 in version 0.3.0. If you're running an older version of Singularity, you can try maually downgrading Singularity Python (:code:`pip install "spython<0.3.0"`) or try `running C-PAC in Singuliarty without this commandline wrapper <https://fcp-indi.github.io/docs/latest/user/singularity>`_
 
 Usage
 =====
 
 .. BEGIN USAGE
 
 .. code-block:: shell
 
     cpac --help
     usage: cpac [-h] [--version] [-o OPT] [-B CUSTOM_BINDING]
-                [--platform {docker,singularity}] [--image IMAGE] [--tag TAG]
-                [--working_dir PATH] [-v] [-vv]
-                {run,utils,version,group,pull,upgrade,enter,bash,shell,parse-resources,parse_resources,crash}
+                [--platform {docker,singularity,apptainer}] [--image IMAGE]
+                [--tag TAG] [--working_dir PATH] [-v] [-vv]
+                {run,utils,version,group,gradients,tsconcat,pull,upgrade,enter,bash,shell,parse-resources,parse_resources,crash}
                 ...
     
     cpac: a Python package that simplifies using C-PAC <http://fcp-indi.github.io> containerized images. 
     
     This commandline interface package is designed to minimize repetition.
     As such, nearly all arguments are optional.
     
@@ -68,25 +71,29 @@
         1. `docker ps` to list the containers
       For each C-PAC conatainer that persists, run
         2. `docker attach <container_name>`
         3. `exit`
     - https://github.com/FCP-INDI/cpac/issues
     
     positional arguments:
-      {run,utils,version,group,pull,upgrade,enter,bash,shell,parse-resources,parse_resources,crash}
+      {run,utils,version,group,gradients,tsconcat,pull,upgrade,enter,bash,shell,parse-resources,parse_resources,crash}
         run                 Run C-PAC. See
-                            "cpac [--platform {docker,singularity}] [--image IMAGE] [--tag TAG] run --help"
+                            "cpac [--platform {docker,apptainer,singularity}] [--image IMAGE] [--tag TAG] run --help"
                             for more information.
         utils               Run C-PAC commandline utilities. See
-                            "cpac [--platform {docker,singularity}] [--image IMAGE] [--tag TAG] utils --help"
+                            "cpac [--platform {docker,apptainer,singularity}] [--image IMAGE] [--tag TAG] utils --help"
                             for more information.
         version             Print the version of C-PAC that cpac is using.
         group               Run a group level analysis in C-PAC. See
-                            "cpac [--platform {docker,singularity}] [--image IMAGE] [--tag TAG] group --help"
+                            "cpac [--platform {docker,apptainer,singularity}] [--image IMAGE] [--tag TAG] group --help"
+                            for more information.
+        gradients           Run ba_timeseries_gradients. See
+                            "cpac [--platform "{docker,singularity}] gradients --help" 
                             for more information.
+        tsconcat            Run ba-tsconcat (<0.2.0,>=0.1.2)
         pull (upgrade)      Upgrade your local C-PAC version to the latest version
                             by pulling from Docker Hub or other repository.
                             Use with "--image" and/or "--tag" to specify an image
                             other than the default "fcpindi/c-pac:latest" to pull.
         enter (bash, shell)
                             Enter a new C-PAC container via BASH.
         parse-resources (parse_resources)
@@ -99,15 +106,15 @@
                             "parse-resources" is intended to be run outside a C-PAC container.
                             See "cpac parse-resources --help" for more information.
         crash               Convert a crash pickle to plain text (C-PAC < 1.8.0).
     
     options:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
-      -o OPT, --container_option OPT
+      -o OPT, --container_option OPT, --container_options OPT
                             parameters and flags to pass through to Docker or Singularity
                             
                             This flag can take multiple arguments so cannot be
                             the final argument before the command argument (i.e.,
                             run or any other command that does not start with - or --)
       -B CUSTOM_BINDING, --custom_binding CUSTOM_BINDING
                             directories to bind with a different path in
@@ -116,22 +123,22 @@
                             	real_path:container_path
                             (eg, /home/C-PAC/run5/outputs:/outputs).
                             Use absolute paths for both paths.
                             
                             This flag can take multiple arguments so cannot be
                             the final argument before the command argument (i.e.,
                             run or any other command that does not start with - or --)
-      --platform {docker,singularity}
+      --platform {docker,singularity,apptainer}
                             If neither platform nor image is specified,
                             cpac will try Docker first, then try
-                            Singularity if Docker fails.
-      --image IMAGE         path to Singularity image file OR name of Docker image (eg, "fcpindi/c-pac").
+                            Apptainer/Singularity if Docker fails.
+      --image IMAGE         path to Apptainer/Singularity image file OR name of Docker image (eg, "fcpindi/c-pac").
                             Will attempt to pull from Singularity Hub or Docker Hub if not provided.
                             If image is specified but platform is not, platform is
-                            assumed to be Singularity if image is a path or 
+                            assumed to be Apptainer/Singularity if image is a path or 
                             Docker if image is an image name.
       --tag TAG             tag of the Docker image to use (eg, "latest" or "nightly").
       --working_dir PATH    working directory
       -v, --verbose         set loglevel to INFO
       -vv, --very-verbose   set loglevel to DEBUG
 
 .. END USAGE
```

### Comparing `cpac-1.8.6.post1.dev1/src/cpac/__main__.py` & `cpac-1.8.7/src/cpac/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 import sys
 
 from docker.errors import DockerException, NotFound
 
 from cpac import __version__
 from cpac.backends import Backends
 from cpac.helpers import cpac_parse_resources as parse_resources, TODOs
+from cpac.utils.bare_wrap import add_bare_wrapper, call, WRAPPED
 
 _logger = logging.getLogger(__name__)
 _CLARGS: set = {"group", "utils"}
 """commandline arguments to pass into container after `--`"""
 
 
 class ExtendAction(argparse.Action):
+    """Flatten commandline arguments for argparse."""
+
     def __call__(self, parser, namespace, values, option_string=None):
+        """Set flattened attributes on the namespace."""
         items = (getattr(namespace, self.dest) or []) + values
         items = [x for n, x in enumerate(items) if x not in items[:n]]
         setattr(namespace, self.dest, items)
 
 
 def address(str_addy):
+    """Split address into string and int components."""
     addr, port = str_addy.split(":")
     port = int(port)
     return addr, port
 
 
 def help_call(argument_list: list) -> bool:
     """Check if the helpstring is being called."""
@@ -82,15 +87,16 @@
         "`--platform`, `--image`, `--tag`) that you would use "
         "while running".format(ver=__version__),
     )
 
     parser.add_argument(
         "-o",
         "--container_option",
-        dest="container_option",
+        "--container_options",
+        dest="container_options",
         action="append",
         help="parameters and flags to pass through to Docker or Singularity\n"
         "\nThis flag can take multiple arguments so cannot "
         "be\nthe final argument before the command argument (i.e.,\nrun "
         "or any other command that does not start with - or --)\n",
         metavar="OPT",
     )
@@ -107,25 +113,25 @@
         "both paths.\n\nThis flag can take multiple arguments so cannot "
         "be\nthe final argument before the command argument (i.e.,\nrun "
         "or any other command that does not start with - or --)\n",
     )
 
     parser.add_argument(
         "--platform",
-        choices=["docker", "singularity"],
+        choices=["docker", "singularity", "apptainer"],
         help="If neither platform nor image is specified,\ncpac will try "
-        "Docker first, then try\nSingularity if Docker fails.",
+        "Docker first, then try\nApptainer/Singularity if Docker fails.",
     )
 
     parser.add_argument(
         "--image",
-        help="path to Singularity image file OR name of Docker image (eg, "
+        help="path to Apptainer/Singularity image file OR name of Docker image (eg, "
         '"fcpindi/c-pac").\nWill attempt to pull from Singularity Hub or '
         "Docker Hub if not provided.\nIf image is specified but platform "
-        "is not, platform is\nassumed to be Singularity if image is a "
+        "is not, platform is\nassumed to be Apptainer/Singularity if image is a "
         "path or \nDocker if image is an image name.",
     )
 
     parser.add_argument(
         "--tag", help='tag of the Docker image to use (eg, "latest" or "nightly").'
     )
 
@@ -152,25 +158,25 @@
     )
 
     subparsers = parser.add_subparsers(dest="command")
 
     run_parser = subparsers.add_parser(
         "run",
         add_help=False,
-        help='Run C-PAC. See\n"cpac [--platform {docker,singularity}] '
+        help='Run C-PAC. See\n"cpac [--platform {docker,apptainer,singularity}] '
         '[--image IMAGE] [--tag TAG] run --help"\nfor more '
         "information.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     utils_parser = subparsers.add_parser(
         "utils",
         add_help=False,
         help='Run C-PAC commandline utilities. See\n"cpac [--platform '
-        "{docker,singularity}] [--image IMAGE] [--tag TAG] utils "
+        "{docker,apptainer,singularity}] [--image IMAGE] [--tag TAG] utils "
         '--help"\nfor more information.',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     version_parser = subparsers.add_parser(
         "version", add_help=True, help="Print the version of C-PAC that cpac is using."
     )
@@ -188,19 +194,40 @@
     run_parser.add_argument("--data_config_file", metavar="PATH")
     run_parser.add_argument("extra_args", nargs=argparse.REMAINDER)
 
     group_parser = subparsers.add_parser(
         "group",
         add_help=False,
         help='Run a group level analysis in C-PAC. See\n"cpac [--platform '
-        "{docker,singularity}] [--image IMAGE] [--tag TAG] group "
+        "{docker,apptainer,singularity}] [--image IMAGE] [--tag TAG] group "
         '--help"\nfor more information.',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
+    gradients_parser = subparsers.add_parser(
+        "gradients",
+        add_help=False,
+        help='Run ba_timeseries_gradients. See\n"cpac [--platform '
+        '"{docker,singularity}] gradients --help" \nfor more information.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
+
+    if not help_call(sys.argv):
+        # These positional arguments are required unless we're just getting
+        # the helpstring
+        gradients_parser.add_argument("bids_dir")
+        gradients_parser.add_argument(
+            "output_dir", default=os.path.join(cwd, "outputs")
+        )
+        gradients_parser.add_argument("level_of_analysis", choices=["group"])
+    gradients_parser.add_argument("extra_args", nargs=argparse.REMAINDER)
+
+    for bare_package in ["tsconcat"]:
+        add_bare_wrapper(subparsers, bare_package)
+
     subparsers.add_parser(
         "pull",
         add_help=True,
         help="Upgrade your local C-PAC version to the latest version\n"
         "by pulling from Docker Hub or other repository.\nUse with "
         '"--image" and/or "--tag" to specify an image\nother than '
         'the default "fcpindi/c-pac:latest" to pull.',
@@ -247,14 +274,15 @@
     )
 
     for subparser in [
         crash_parser,
         enter_parser,
         group_parser,
         run_parser,
+        gradients_parser,
         utils_parser,
         version_parser,
     ]:
         subparser.register("action", "extend", ExtendAction)
 
     return parser
 
@@ -277,15 +305,27 @@
         *(parsed.extra_args if hasattr(parsed, "extra_args") else []),
         *extras,
     ]
 
     return parsed
 
 
+def setup_help(arg_vars: dict, level_of_analysis: str) -> dict:
+    """Supply necessary positional arguments to get helpstring from container."""
+    pwd = os.getcwd()
+    for arg in ["output_dir", "bids_dir"]:
+        if arg_vars.get(arg) is None or arg_vars.get(arg) is arg:
+            arg_vars[arg] = pwd
+    if level_of_analysis is None:
+        arg_vars["level_of_analysis"] = level_of_analysis
+    return arg_vars
+
+
 def setup_logging(loglevel):
+    """Set up logging."""
     logformat = "[%(asctime)s] %(levelname)s:%(name)s:%(message)s"
     logging.basicConfig(
         level=loglevel, stream=sys.stdout, format=logformat, datefmt="%Y-%m-%d %H:%M:%S"
     )
 
 
 def main(args):
@@ -334,20 +374,36 @@
             [
                 "--help" in arg_vars,
                 "-h" in arg_vars,
                 "--help" in args.extra_args,
                 "-h" in args.extra_args,
             ]
         ):
-            pwd = os.getcwd()
-            if arg_vars.get("level_of_analysis") is None:
-                arg_vars["level_of_analysis"] = "participant"
-            for arg in ["output_dir", "bids_dir"]:
-                if arg_vars.get(arg) is None:
-                    arg_vars[arg] = pwd
+            arg_vars = setup_help(arg_vars, "participant")
+        Backends(**arg_vars).run(flags=args.extra_args, **arg_vars)
+
+    if args.command == "gradients":
+        arg_vars.update(
+            {
+                "image": "ghcr.io/childmindresearch/ba-timeseries-gradients",
+                "tag": "main",
+            }
+        )
+        if any(
+            [
+                "--help" in arg_vars,
+                "-h" in arg_vars,
+                "--help" in args.extra_args,
+                "-h" in args.extra_args,
+            ]
+        ):
+            arg_vars = setup_help(arg_vars, "group")
+            if "--help" in args.extra_args:
+                args.extra_args.remove("--help")
+                args.extra_args.append("-h")
         Backends(**arg_vars).run(flags=args.extra_args, **arg_vars)
 
     elif args.command in ["enter", "version"]:
         Backends(**arg_vars).run(
             run_type=args.command, flags=args.extra_args, **arg_vars
         )
 
@@ -367,15 +423,15 @@
 
     elif args.command == "parse-resources":
         parse_resources.main(args)
 
 
 def run():
     """
-    Try Docker first and fall back on Singularity if Docker fails if --platform is not specified.
+    Try Docker first and fall back on Apptainer/Singularity if Docker fails if --platform is not specified.
 
     Parameters
     ----------
     None
 
     Returns
     -------
@@ -400,21 +456,25 @@
     )
     options = set(
         chain.from_iterable([o.option_strings for o in parser._get_optional_actions()])
     )
     # keep help option with specific command
     for option in ("-h", "--help"):
         options.discard(option)
-    for cmd in commands:
-        if command is None and cmd in args:
+    for cmd in args:
+        if command is None and cmd in commands:
             command_index = args.index(cmd)
             command = args.pop(command_index)
     if command is None:
         parser.print_help()
         parser.exit()
+    if command in WRAPPED:
+        if not help_call(args):
+            # directly call external package and exit on completion or failure
+            call(command, args)
     reordered_args = []
     option_value_setting = False
     for i, arg in enumerate(args.copy()):
         if i == command_index:
             option_value_setting = False
         if arg in options:
             reordered_args.append(args.pop(args.index(arg)))
```

### Comparing `cpac-1.8.6.post1.dev1/src/cpac/backends/docker.py` & `cpac-1.8.7/src/cpac/backends/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from typing import Optional
 
 import docker
 from docker.errors import ImageNotFound
 import dockerpty
 
 from cpac.backends.platform import Backend, PlatformMeta
 
@@ -84,25 +85,18 @@
             for k in layer
             if k in {"id", "status", "progress"}
         ]
 
     def _read_crash(self, read_crash_command, **kwargs):
         return self._execute(command=read_crash_command, run_type="exec", **kwargs)
 
-    def run(self, flags=[], **kwargs):
-        kwargs["command"] = [
-            i
-            for i in [
-                kwargs.get("bids_dir"),
-                kwargs.get("output_dir"),
-                kwargs.get("level_of_analysis"),
-                *flags,
-            ]
-            if (i is not None and len(i))
-        ]
+    def run(self, flags: Optional[list] = None, **kwargs):
+        if not flags:
+            flags = []
+        kwargs["command"] = self.drop_missing_positional_arguments(kwargs, flags)
         return self._execute(**kwargs)
 
     def clarg(self, clcommand, flags=None, **kwargs):
         """Run a commandline command.
 
         Parameters
         ----------
```

### Comparing `cpac-1.8.6.post1.dev1/src/cpac/backends/platform.py` & `cpac-1.8.7/src/cpac/backends/platform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Base classes for platform-specific implementations."""
+
 import atexit
 from collections import namedtuple
 from contextlib import redirect_stderr
 from io import StringIO
 import os
 import pwd
 import tempfile
 import textwrap
-from typing import overload
+from typing import Union
 from warnings import warn
 
 from docker import errors as docker_errors
 import pandas as pd
 from tabulate import tabulate
 import yaml
 
@@ -28,14 +29,15 @@
     def __init__(self, backend):
         self.versions = namedtuple("versions", "cpac CPAC")
         self.versions.cpac = cpac_version
         self.versions.CPAC = backend.get_response("cat /code/version").rstrip()
         self.platform = backend.platform
 
     def __str__(self):
+        """Return string representation of CpacVersion."""
         return (
             f"cpac (convenience wrapper) version {self.versions.cpac}\n"
             f"C-PAC version {self.versions.CPAC} running on "
             f"{self.platform.name} version {self.platform.version}"
         )
 
 
@@ -60,19 +62,29 @@
 
     # pylint: disable=too-few-public-methods
     def __init__(self, name, symbol):
         self.name = name
         self.symbol = symbol
         self.version = "unknown"
 
+    def __repr__(self):
+        """Return reproducible string reprensentation of platform metadata."""
+        return f"PlatformMeta({self.name}, {self.symbol})"
+
     def __str__(self):
-        return f"{self.symbol} {self.name}"
+        """Return string representation of platform metadata."""
+        _str = f"{self.symbol} {self.name}"
+        if self.version != "unknown":
+            _str += f" {self.version}"
+        return _str
 
 
 class Backend:
+    """Generic class for container backends."""
+
     def __init__(self, **kwargs):
         self.pipeline_config = None
         if "extra_args" in kwargs and isinstance(kwargs["extra_args"], list):
             pipeline_config = get_extra_arg_value(kwargs["extra_args"], "pipeline_file")
             if pipeline_config is not None:
                 self.pipeline_config = yaml.safe_load(pipeline_config)
             else:
@@ -101,24 +113,38 @@
                     "--tracking_opt-out and C-PAC >= "
                     "1.8.4"
                 )
         # initilizing these for overriding on load
         self.bindings = {}
         self.container = None
         self.image = None
-        self.platform = None
         self._run = None
         self.uid = 0
         self.username = "root"
         self.working_dir = kwargs.get("working_dir", os.getcwd())
         atexit.register(self._cleanup)
 
     def __del__(self):
+        """Clean up container when finished."""
         self._cleanup()
 
+    @staticmethod
+    def drop_missing_positional_arguments(kwargs: dict, flags: list) -> list:
+        """Return ordered list of positional args and flags without placeholders."""
+        return [
+            i
+            for i in [
+                kwargs.get("bids_dir"),
+                kwargs.get("output_dir"),
+                kwargs.get("level_of_analysis"),
+                *flags,
+            ]
+            if (i is not None and len(i))
+        ]
+
     def read_crash(self, crashfile, flags=None, **kwargs):
         """
         Decode a crashfile into plain text.
 
         For C-PAC < 1.8.0. Since C-PAC 1.8.0, crashfiles are stored as plain text.
 
         Parameters
@@ -306,15 +332,15 @@
         print(version)
         return version
 
     def _load_logging(self):
         table = pd.DataFrame(
             [
                 (volume.local, volume.bind, volume.mode)
-                for volume in self.bindings["volumes"]
+                for volume in self.bindings.get("volumes", [])
             ]
         )
         if not table.empty:
             table.columns = ["local", self.platform.name, "mode"]
             self._print_loading_with_symbol(
                 " ".join(
                     [
@@ -338,14 +364,27 @@
                     "  ",
                 )
             )
             print(
                 f"Logging messages will refer to the {self.platform.name} " "paths.\n"
             )
 
+    @property
+    def platform(self):
+        """Platform metadata."""
+        try:
+            return self._platform
+        except AttributeError:
+            return None
+
+    @platform.setter
+    def platform(self, value):
+        """Set platform metadata."""
+        self._platform = value
+
     def _prep_binding(self, volume: Volume, second_try: bool = False) -> Volume:
         """Prepare a volume binding for the container.
 
         Parameters
         ----------
         volume : Volume
             Volume to bind.
@@ -377,27 +416,18 @@
         if prefix is not None:
             print(prefix, end=" ")
         try:
             print(" ".join([self.platform.symbol, message]))
         except UnicodeEncodeError:
             print(message)
 
-    @overload
-    def __setattr__(self, name: str, value: Volume) -> None:
-        ...
-
-    @overload
-    def __setattr__(self, name: str, value: list) -> None:
-        ...
-
-    @overload
-    def __setattr__(self, name: str, value: Volumes) -> None:
-        ...
-
-    def __setattr__(self, name, value):
+    def __setattr__(self, name: str, value: Union[list, Volume, Volumes]) -> None:
+        """Coerce self.volumes to be a Volumes instance."""
+        if name == "platform":
+            super().__setattr__(name, value)
         if name == "volumes":
             if isinstance(value, Volumes):
                 self.__dict__[name] = value
             else:
                 self.__dict__[name] = Volumes(value)
         else:
             self.__dict__[name] = value
@@ -459,39 +489,47 @@
         with tempfile.TemporaryDirectory() as temp_dir:
             self._bind_volume(Volume(temp_dir, "/out", "rw"))
         helper = cpac_read_crash.__file__
         self._bind_volume(Volume(helper, mode="ro"))
 
 
 class Result:
+    """Yield result."""
+
     mime = None
 
     def __init__(self, name, value):
         self.name = name
         self.value = value
 
     def __call__(self):
+        """Yield result."""
         yield self.value
 
     @property
     def description(self):
+        """Return dict of {'type': 'object'}."""
         return {"type": "object"}
 
 
 class FileResult(Result):
+    """Yield a file."""
+
     def __init__(self, name, value, mime):
         self.name = name
         self.value = value
         self.mime = mime
 
     def __call__(self):
+        """Yeild file."""
         with open(self.value, "rb") as f:
             while True:
                 piece = f.read(1024)
                 if piece:
                     yield piece
                 else:
                     return
 
     @property
     def description(self):
+        """Return dict of 'type' and 'mime' for file."""
         return {"type": "file", "mime": self.mime}
```

### Comparing `cpac-1.8.6.post1.dev1/src/cpac/backends/singularity.py` & `cpac-1.8.7/src/cpac/backends/singularity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-from itertools import chain
+"""Backend for Singularity images."""
+
 import os
 
 from spython.image import Image
 from spython.main import Client
 
 from cpac.backends.platform import Backend, PlatformMeta
 
 BINDING_MODES = {"ro": "ro", "w": "rw", "rw": "rw"}
 
 
 class Singularity(Backend):
+    """Backend for Singularity images."""
+
+    @Backend.platform.setter  # type: ignore[attr-defined]
+    def platform(self, value):
+        """Set metadata for Singularity platform."""
+        self._platform = value
+        self._platform.version = Client.version().split(" ")[-1]
+
+    def _set_platform(self):
+        """Set metadata for Apptainer platform."""
+        self.platform = PlatformMeta("Singularity", "Ⓢ")
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.container = None
-        self.platform = PlatformMeta("Singularity", "Ⓢ")
-        self.platform.version = Client.version().split(" ")[-1]
+        self._set_platform()
         self._print_loading_with_symbol(self.platform.name)
+        container_options = kwargs.get("container_options")
+        self.options = container_options if isinstance(container_options, list) else []
         self.pull(**kwargs, force=False)
-        self.options = (
-            list(chain.from_iterable(kwargs["container_options"]))
-            if bool(kwargs.get("container_options"))
-            else []
-        )
         if isinstance(self.pipeline_config, str):
             self.config = Client.execute(
                 image=self.image,
                 command=f"cat {self.pipeline_config}",
                 return_result=False,
             )
         else:
@@ -53,46 +62,51 @@
             self.options.remove("-B")
         enter_options["singularity_options"] = self.options
         return enter_options
 
     def _pull(self, img, force, pull_folder):
         """Try to pull image gracefully."""
         try:
-            self.image = Client.pull(img, force=force, pull_folder=pull_folder)
+            self.image = Client.pull(
+                img,
+                force=force,
+                pull_folder=pull_folder,
+                singularity_options=self.options,
+            )
         except ValueError as value_error:
             if "closed file" in str(value_error):
                 # pylint: disable=protected-access
                 self.image = Image(Client._get_filename(img))
 
     def pull(self, force=False, **kwargs):
+        """Pull a Singularity container."""
         image = kwargs["image"] if kwargs.get("image") is not None else "fcpindi/c-pac"
         tag = kwargs.get("tag")
         pwd = os.getcwd()
         if kwargs.get("working_dir") is not None:
             pwd = kwargs["working_dir"]
             os.chdir(pwd)
         image_path = Client._get_filename(  # pylint: disable=protected-access
             image if tag is None else ":".join([image, tag])
         )
-        if (
-            not force
-            and image
-            and isinstance(image, str)
-            and os.path.exists(image_path)
-        ):
-            self.image = image_path
-        elif tag and isinstance(tag, str):  # pragma: no cover
-            self._pull(f"docker://{image}:{tag}", force=force, pull_folder=pwd)
+        if image:
+            if not force and isinstance(image, str) and os.path.exists(image_path):
+                self.image = image_path
+            elif tag and isinstance(tag, str):  # pragma: no cover
+                self._pull(f"docker://{image}:{tag}", force=force, pull_folder=pwd)
+            else:
+                self._pull(f"docker://{image}", force=force, pull_folder=pwd)
         else:  # pragma: no cover
             try:
                 self._pull(
                     "docker://fcpindi/c-pac:latest", force=force, pull_folder=pwd
                 )
             except Exception as exception:
-                raise OSError("Could not connect to Singularity") from exception
+                msg = f"Could not connect to {self.platform.name}"
+                raise OSError(msg) from exception
 
     def get_response(self, command, **kwargs):
         """
         Return the response of running a command in the Singularity container.
 
         Parameters
         ----------
@@ -109,15 +123,15 @@
             full_response.append(response)
         return "".join(full_response)
 
     def _try_to_stream(self, args, stream_command="run", silent=False, **kwargs):
         self._bindings_as_option()
         if stream_command == "run":
             self.container = Client.run(
-                Client.instance(self.image),
+                self.image,
                 args=args,
                 options=self.options,
                 stream=not silent,
                 return_result=True,
                 **kwargs,
             )
         else:
@@ -153,29 +167,25 @@
 
     def _read_crash(self, read_crash_command, **kwargs):
         return self._try_to_stream(
             args={"command": read_crash_command}, stream_command="execute", **kwargs
         )
 
     def run(self, flags=None, run_type="run", **kwargs):
+        """Run a Singularity container."""
         # pylint: disable=expression-not-assigned
         if flags is None:
             flags = []
         self._load_logging()
         if run_type == "run":
             [
                 print(o, end="")
                 for o in self._try_to_stream(
                     args=" ".join(
-                        [
-                            kwargs["bids_dir"],
-                            kwargs["output_dir"],
-                            kwargs["level_of_analysis"],
-                            *flags,
-                        ]
+                        self.drop_missing_positional_arguments(kwargs, flags)
                     ).strip(" ")
                 )
             ]
         elif run_type == "version":
             return self.get_version()
         else:
             for o in self._try_to_stream(
```

### Comparing `cpac-1.8.6.post1.dev1/src/cpac/helpers/__init__.py` & `cpac-1.8.7/src/cpac/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `cpac-1.8.6.post1.dev1/src/cpac/helpers/cpac_parse_resources.py` & `cpac-1.8.7/src/cpac/helpers/cpac_parse_resources.py`

 * *Files identical despite different names*

### Comparing `cpac-1.8.6.post1.dev1/src/cpac/helpers/cpac_read_crash.py` & `cpac-1.8.7/src/cpac/helpers/cpac_read_crash.py`

 * *Files identical despite different names*

### Comparing `cpac-1.8.6.post1.dev1/src/cpac/utils/checks.py` & `cpac-1.8.7/src/cpac/utils/checks.py`

 * *Files identical despite different names*

### Comparing `cpac-1.8.6.post1.dev1/src/cpac/utils/utils.py` & `cpac-1.8.7/src/cpac/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from typing import ClassVar, Iterator, Optional, Set, Union
 from warnings import warn
 
 import yaml
 
 from cpac import DIST_NAME
 
+INTERVAL_CHECKS = {"[": "__ge__", "]": "__le__", "(": "__gt__", ")": "__lt__"}
+
 
 class LocalsToBind:
     """Class to collect local directories to bind to containers."""
 
     def __init__(self):
         self.locals = set()
 
@@ -22,16 +24,16 @@
     def __str__(self):
         return str(self.locals)
 
     def from_config_file(self, config_path):
         """
         Add local bindings from a configuration file.
 
-        Paramter.
-        --------
+        Parameters
+        ----------
         config_path : str
             path to data config file
         """
         with open(config_path, "r") as config_yml:
             config_dict = yaml.safe_load(config_yml)
         self._add_locals(config_dict)
 
@@ -184,14 +186,19 @@
                  ])}""",
                 UserWarning,
             )
             return True
         return False
 
 
+def version_tuple(version: str) -> tuple:
+    """Convert version string to tuple."""
+    return tuple(int(v) for v in version.split("."))
+
+
 class Volume:
     """Class to store bind volume information."""
 
     def __init__(
         self,
         local: str,
         bind: Optional[str] = None,
```

### Comparing `cpac-1.8.6.post1.dev1/PKG-INFO` & `cpac-1.8.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: cpac
-Version: 1.8.6.post1.dev1
+Version: 1.8.7
 Summary: C-PAC Python Package
 Home-page: https://github.com/FCP-INDI/cpac
 License: MIT
 Author: C-PAC developers
 Author-email: cpac@cnl.childmind.org
-Requires-Python: >=3.8
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: dev
+Provides-Extra: gradients
 Provides-Extra: testing
+Provides-Extra: tsconcat
 Requires-Dist: alabaster ; extra == "testing"
+Requires-Dist: ba-tsconcat (>=0.1.2,<0.2.0) ; (python_version >= "3.11" and python_version < "4.0") and (extra == "tsconcat")
+Requires-Dist: bids2table (==0.1.0b0) ; extra == "tsconcat"
 Requires-Dist: coveralls ; extra == "dev"
 Requires-Dist: docker (>=4.2.1)
 Requires-Dist: docker-pycreds
 Requires-Dist: dockerpty
+Requires-Dist: elbow (==0.1.1) ; extra == "tsconcat"
 Requires-Dist: imagesize ; extra == "testing"
-Requires-Dist: importlib_metadata ; python_version < "3.8"
+Requires-Dist: nibabel (==5.2.1) ; extra == "tsconcat"
+Requires-Dist: pandas (==2.2.2) ; python_version >= "3.11" and python_version < "4.0" and extra == "tsconcat"
 Requires-Dist: pandas (>=0.23.4)
-Requires-Dist: poetry
+Requires-Dist: poetry (>=1.8.2)
+Requires-Dist: pyarrow (==16.0.0) ; extra == "tsconcat"
 Requires-Dist: pytest ; extra == "dev" or extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
 Requires-Dist: pytest-remotedata (>=0.3.2) ; extra == "dev"
 Requires-Dist: pytest-runner ; extra == "dev" or extra == "testing"
 Requires-Dist: pyyaml
 Requires-Dist: rich
 Requires-Dist: semver
 Requires-Dist: sphinx ; extra == "dev" or extra == "testing"
-Requires-Dist: spython (>=0.0.81,<0.3.0)
+Requires-Dist: spython (>=0.3.0)
 Requires-Dist: tabulate (>=0.8.6)
 Requires-Dist: tornado
 Requires-Dist: websocket-client
 Project-URL: Documentation, https://fcp-indi.github.io/docs/latest/user/cpac
 Project-URL: Repository, https://github.com/FCP-INDI/cpac
 Description-Content-Type: text/x-rst
 
@@ -63,33 +68,36 @@
 .. admonition:: Note about cpac versioning
 
     This package's versioning scheme changed in version 1.8.5 to match C-PAC's versioning. From cpac v1.8.5 forward, the version of cpac indicates the newest supported version of C-PAC.
 
 Dependencies
 ============
 
-* `Python <https://www.python.org>`_ ≥ 3.8
+* `Python <https://www.python.org>`_ ≥ 3.10
 * `pip <https://pip.pypa.io>`_
 * At least one of:
 
   * `Docker <https://www.docker.com>`_
-  * **`Singularity <https://sylabs.io/singularity>`_ ≥ 2.5 \< 3.0** (this is different than the main release of ``cpac``!)
+  * `Apptainer <https://apptainer.org/documentation/>`_ ≥ 1.0
+  * `Singularity <https://sylabs.io/singularity>`_ ≥ 3.0 [*]_
+
+.. [*] ``cpac`` *may* work with older versions of Singularity, but `Singularity Python <https://singularityhub.github.io/singularity-cli/>`_ dropped support for Singularity < 3.0 in version 0.3.0. If you're running an older version of Singularity, you can try maually downgrading Singularity Python (:code:`pip install "spython<0.3.0"`) or try `running C-PAC in Singuliarty without this commandline wrapper <https://fcp-indi.github.io/docs/latest/user/singularity>`_
 
 Usage
 =====
 
 .. BEGIN USAGE
 
 .. code-block:: shell
 
     cpac --help
     usage: cpac [-h] [--version] [-o OPT] [-B CUSTOM_BINDING]
-                [--platform {docker,singularity}] [--image IMAGE] [--tag TAG]
-                [--working_dir PATH] [-v] [-vv]
-                {run,utils,version,group,pull,upgrade,enter,bash,shell,parse-resources,parse_resources,crash}
+                [--platform {docker,singularity,apptainer}] [--image IMAGE]
+                [--tag TAG] [--working_dir PATH] [-v] [-vv]
+                {run,utils,version,group,gradients,tsconcat,pull,upgrade,enter,bash,shell,parse-resources,parse_resources,crash}
                 ...
     
     cpac: a Python package that simplifies using C-PAC <http://fcp-indi.github.io> containerized images. 
     
     This commandline interface package is designed to minimize repetition.
     As such, nearly all arguments are optional.
     
@@ -116,25 +124,29 @@
         1. `docker ps` to list the containers
       For each C-PAC conatainer that persists, run
         2. `docker attach <container_name>`
         3. `exit`
     - https://github.com/FCP-INDI/cpac/issues
     
     positional arguments:
-      {run,utils,version,group,pull,upgrade,enter,bash,shell,parse-resources,parse_resources,crash}
+      {run,utils,version,group,gradients,tsconcat,pull,upgrade,enter,bash,shell,parse-resources,parse_resources,crash}
         run                 Run C-PAC. See
-                            "cpac [--platform {docker,singularity}] [--image IMAGE] [--tag TAG] run --help"
+                            "cpac [--platform {docker,apptainer,singularity}] [--image IMAGE] [--tag TAG] run --help"
                             for more information.
         utils               Run C-PAC commandline utilities. See
-                            "cpac [--platform {docker,singularity}] [--image IMAGE] [--tag TAG] utils --help"
+                            "cpac [--platform {docker,apptainer,singularity}] [--image IMAGE] [--tag TAG] utils --help"
                             for more information.
         version             Print the version of C-PAC that cpac is using.
         group               Run a group level analysis in C-PAC. See
-                            "cpac [--platform {docker,singularity}] [--image IMAGE] [--tag TAG] group --help"
+                            "cpac [--platform {docker,apptainer,singularity}] [--image IMAGE] [--tag TAG] group --help"
+                            for more information.
+        gradients           Run ba_timeseries_gradients. See
+                            "cpac [--platform "{docker,singularity}] gradients --help" 
                             for more information.
+        tsconcat            Run ba-tsconcat (<0.2.0,>=0.1.2)
         pull (upgrade)      Upgrade your local C-PAC version to the latest version
                             by pulling from Docker Hub or other repository.
                             Use with "--image" and/or "--tag" to specify an image
                             other than the default "fcpindi/c-pac:latest" to pull.
         enter (bash, shell)
                             Enter a new C-PAC container via BASH.
         parse-resources (parse_resources)
@@ -147,15 +159,15 @@
                             "parse-resources" is intended to be run outside a C-PAC container.
                             See "cpac parse-resources --help" for more information.
         crash               Convert a crash pickle to plain text (C-PAC < 1.8.0).
     
     options:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
-      -o OPT, --container_option OPT
+      -o OPT, --container_option OPT, --container_options OPT
                             parameters and flags to pass through to Docker or Singularity
                             
                             This flag can take multiple arguments so cannot be
                             the final argument before the command argument (i.e.,
                             run or any other command that does not start with - or --)
       -B CUSTOM_BINDING, --custom_binding CUSTOM_BINDING
                             directories to bind with a different path in
@@ -164,22 +176,22 @@
                             	real_path:container_path
                             (eg, /home/C-PAC/run5/outputs:/outputs).
                             Use absolute paths for both paths.
                             
                             This flag can take multiple arguments so cannot be
                             the final argument before the command argument (i.e.,
                             run or any other command that does not start with - or --)
-      --platform {docker,singularity}
+      --platform {docker,singularity,apptainer}
                             If neither platform nor image is specified,
                             cpac will try Docker first, then try
-                            Singularity if Docker fails.
-      --image IMAGE         path to Singularity image file OR name of Docker image (eg, "fcpindi/c-pac").
+                            Apptainer/Singularity if Docker fails.
+      --image IMAGE         path to Apptainer/Singularity image file OR name of Docker image (eg, "fcpindi/c-pac").
                             Will attempt to pull from Singularity Hub or Docker Hub if not provided.
                             If image is specified but platform is not, platform is
-                            assumed to be Singularity if image is a path or 
+                            assumed to be Apptainer/Singularity if image is a path or 
                             Docker if image is an image name.
       --tag TAG             tag of the Docker image to use (eg, "latest" or "nightly").
       --working_dir PATH    working directory
       -v, --verbose         set loglevel to INFO
       -vv, --very-verbose   set loglevel to DEBUG
 
 .. END USAGE
```

