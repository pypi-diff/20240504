# Comparing `tmp/aedev_git_repo_manager-0.3.76.tar.gz` & `tmp/aedev_git_repo_manager-0.3.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aedev_git_repo_manager-0.3.76.tar", last modified: Tue Apr 30 12:49:45 2024, max compression
+gzip compressed data, was "aedev_git_repo_manager-0.3.77.tar", last modified: Fri May  3 15:17:36 2024, max compression
```

## Comparing `aedev_git_repo_manager-0.3.76.tar` & `aedev_git_repo_manager-0.3.77.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.639560 aedev_git_repo_manager-0.3.76/
--rw-rw-rw-   0 root         (0) root         (0)    35002 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     6549 2024-04-30 12:49:45.639560 aedev_git_repo_manager-0.3.76/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3543 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.632560 aedev_git_repo_manager-0.3.76/aedev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.633560 aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1879 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   187688 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.636560 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6549 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      449 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      543 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 12:49:45.639560 aedev_git_repo_manager-0.3.76/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.635560 aedev_git_repo_manager-0.3.76/tests/
--rw-rw-rw-   0 root         (0) root         (0)   157998 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/tests/test_git_repo_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:36.440763 aedev_git_repo_manager-0.3.77/
+-rw-rw-rw-   0 root         (0) root         (0)    35002 2024-05-03 15:17:24.000000 aedev_git_repo_manager-0.3.77/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     6549 2024-05-03 15:17:36.440763 aedev_git_repo_manager-0.3.77/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2024-05-03 15:17:24.000000 aedev_git_repo_manager-0.3.77/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:36.433763 aedev_git_repo_manager-0.3.77/aedev/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:36.434763 aedev_git_repo_manager-0.3.77/aedev/git_repo_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2024-05-03 15:17:24.000000 aedev_git_repo_manager-0.3.77/aedev/git_repo_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   188195 2024-05-03 15:17:24.000000 aedev_git_repo_manager-0.3.77/aedev/git_repo_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:36.437763 aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6549 2024-05-03 15:17:36.000000 aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-03 15:17:36.000000 aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 15:17:36.000000 aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-03 15:17:36.000000 aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      543 2024-05-03 15:17:36.000000 aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-03 15:17:36.000000 aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 15:17:36.000000 aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 15:17:36.440763 aedev_git_repo_manager-0.3.77/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-05-03 15:17:24.000000 aedev_git_repo_manager-0.3.77/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:17:36.436763 aedev_git_repo_manager-0.3.77/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   157998 2024-05-03 15:17:24.000000 aedev_git_repo_manager-0.3.77/tests/test_git_repo_manager.py
```

### Comparing `aedev_git_repo_manager-0.3.76/LICENSE.md` & `aedev_git_repo_manager-0.3.77/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.76/PKG-INFO` & `aedev_git_repo_manager-0.3.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.76
+Version: 0.3.77
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -72,25 +72,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.76
+# git_repo_manager 0.3.77
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.75?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.75)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.76?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.76)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.76.
+>aedev_git_repo_manager package 0.3.77.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.76/README.md` & `aedev_git_repo_manager-0.3.77/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.76
+# git_repo_manager 0.3.77
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.75?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.75)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.76?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.76)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.76.
+>aedev_git_repo_manager package 0.3.77.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/__init__.py` & `aedev_git_repo_manager-0.3.77/aedev/git_repo_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 
 in conjunction with the template projects of the `aedev` namespace (like e.g. :mod:`aedev.tpl_project`) any common
 portions file (even the ``setup.py`` file) can be created/maintained as a template in a single place, and then
 requested and updated individually for each portion project.
 """
 
 
-__version__ = '0.3.76'
+__version__ = '0.3.77'
```

### Comparing `aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/__main__.py` & `aedev_git_repo_manager-0.3.77/aedev/git_repo_manager/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Sequence, Set, Tuple, Union, cast)
 
 from dotenv import find_dotenv, load_dotenv
 
 from github import Github
 from gitlab import Gitlab, GitlabCreateError, GitlabError, GitlabHttpError
 from gitlab.const import MAINTAINER_ACCESS
-from gitlab.v4.objects import Group, Project, User
+from gitlab.v4.objects import Group, Project, ProjectManager, User, UserProjectManager
 
 from packaging.version import Version
 from PIL import Image
 
 import ae.base                                                                          # type: ignore # for patching
 from ae.base import (
     PY_EXT, PY_INIT, TEMPLATES_FOLDER, UNSET, UnsetType,
@@ -2457,40 +2457,70 @@
                 self.connection.enable_debug()
             self.connection.auth()          # authenticate and create user attribute
         except (Exception, ) as ex:
             cae.po(f"****  Gitlab connection exception: {ex}")
             return False
         return True
 
-    def owner_from_pdv(self, ini_pdv: PdvType) -> Union[Group, User]:
-        """ convert group/user specified in pdv to remote repo group/user object instance.
+    def create_project(self, ini_pdv: PdvType):
+        """ create group/user project specified in ini_pdv or quit with error if group/user not found.
 
         :param ini_pdv:         project dev vars.
-        :return:                gitlab owner object/instance (group or user) or quit with error if not found.
         """
         domain = _get_host_domain(ini_pdv)
-
         group_name = _get_host_group(ini_pdv, domain)
-        try:
-            return self.connection.groups.get(group_name)
-        except GitlabError:
-            groups = self.connection.groups.list(search=group_name)
-            if groups:
-                return groups[0]                                    # type: ignore
-
         user_name = _get_host_user_name(ini_pdv, domain)
-        try:
-            return self.connection.users.get(user_name)
-        except GitlabError:
-            users = self.connection.users.list(search=user_name)
-            if users:
-                return users[0]                                     # type: ignore
 
-        _exit_error(37, f"neither group '{group_name}' nor user '{user_name}' found on repository host '{domain}'")
-        return                                                      # type: ignore
+        owner_obj: Optional[Union[Group, User]] = None
+        if group_name == user_name:             # repo_group == repo_user -> personal project
+            try:
+                owner_obj = self.connection.users.get(user_name)
+            except GitlabError:
+                users = self.connection.users.list(username=user_name)
+                if users:
+                    owner_obj = users[0]  # type: ignore
+        else:
+            try:
+                owner_obj = self.connection.groups.get(group_name)
+            except GitlabError:
+                groups = self.connection.groups.list(search=group_name)
+                if groups:
+                    owner_obj = groups[0]                               # type: ignore
+        if owner_obj is None:
+            _exit_error(37, f"neither group '{group_name}' nor user '{user_name}' found on repo host '{domain}'")
+            return                  # never executed but needed by mypy for owner_obj type checking
+
+        project_name = _get_prj_name(ini_pdv)
+        project_properties = {
+            'name': project_name,
+            'description': pdv_str(ini_pdv, 'project_desc'),
+            'default_branch': MAIN_BRANCH,
+            'visibility': 'public',
+        }
+        owner_projects: Union[ProjectManager, UserProjectManager]
+        if group_name == user_name:
+            project_properties['user_id'] = owner_obj.id
+            owner_projects = cast(User, owner_obj).projects
+        else:
+            project_properties['namespace_id'] = owner_obj.id
+            owner_projects = self.connection.projects
+        cae.vpo(f"    - remote project properties of new package {project_name}: {PPF(project_properties)}")
+
+        project = cast(Project, owner_projects.create(project_properties))
+        cae.po(f"   == created new project for user/group '{owner_obj.name}'; attributes: {PPF(project.attributes)}")
+
+        _wait()
+
+        for branch_mask in (MAIN_BRANCH, 'release*'):
+            protected_branch_properties = {'name': branch_mask,
+                                           'merge_access_level': MAINTAINER_ACCESS,
+                                           'push_access_level': MAINTAINER_ACCESS}
+            cae.vpo(f"    - {branch_mask} protected branch properties: {protected_branch_properties}")
+            project.protectedbranches.create(protected_branch_properties)
+        cae.po(f"   == created 2 protected branches: '{MAIN_BRANCH}', 'release*'")
 
     def project_from_name(self, err_code: int, err_msg: str, project_name: str, owned: bool = True) -> Project:
         """ convert group/project_name or an endswith-fragment of it to a Project instance of the remote repo api.
 
         :param err_code:        error code, pass 0 to not exit on error.
         :param err_msg:         error message to display on error with optional {name} to be automatically substituted
                                 with the project name from the :paramref:`~project_from_name.project_name` argument.
@@ -2633,36 +2663,15 @@
         project_name = _get_prj_name(ini_pdv)
 
         changed = _git_uncommitted(ini_pdv)
         _chk_if(76, not changed, f"{project_name} has {len(changed)} uncommitted files: {changed}")
 
         push_refs = []
         if not self.project_from_name(0, "", project_name):
-            owner_obj = self.owner_from_pdv(ini_pdv)                # get group/user object or quit
-            project_properties = {
-                'name': project_name,
-                'namespace_id': owner_obj.id,
-                'description': pdv_str(ini_pdv, 'project_desc'),
-                'default_branch': MAIN_BRANCH,
-                'visibility': 'public',
-            }
-            cae.vpo(f"    - remote project properties of new package {project_name}: {PPF(project_properties)}")
-            project = cast(Project, self.connection.projects.create(project_properties))
-
-            cae.po(f"   == created new project {PPF(project.attributes)} under remote user/group {owner_obj.name}")
-            _wait()
-
-            for branch_mask in (MAIN_BRANCH, 'release*'):
-                protected_branch_properties = {'name': branch_mask,
-                                               'merge_access_level': MAINTAINER_ACCESS,
-                                               'push_access_level': MAINTAINER_ACCESS}
-                cae.vpo(f"    - {branch_mask} protected branch properties: {protected_branch_properties}")
-                project.protectedbranches.create(protected_branch_properties)
-            cae.po(f"   == protected branches {MAIN_BRANCH} and release*")
-
+            self.create_project(ini_pdv)
             push_refs.append(MAIN_BRANCH)
 
         branch_name = branch_name or _get_branch(ini_pdv)
         if branch_name and branch_name not in push_refs:
             push_refs.append(branch_name)
 
         pkg_version = _git_project_version(ini_pdv, increment_part=cae.get_option('versionIncrementPart'))
@@ -2788,25 +2797,23 @@
         action = "requested merge"
         if cae.get_option('force') and user_name == group_name:
             _wait()  # wait for created un-forked/direct maintainer merge request (with --force --user=group_name)
             merge_req.merge(merge_commit_message=read_file(_check_commit_msg_file(ini_pdv)))
             action = "auto-merged un-forked and forced merge request"
         cae.po(f" ==== {action} of branch {branch} from fork/origin ({src_prj.id}) into upstream ({tgt_prj.id})")
 
-    @_action()
-    def search_repos(self, ini_pdv: PdvType):
-        """ search remote repositories via group/package name fragment. """
-        group_name = _get_host_group(ini_pdv, _get_host_domain(ini_pdv))
-        project_name = _get_prj_name(ini_pdv)
-        fragment = f"{group_name}/{project_name}" if group_name and project_name else group_name or project_name
-        repos = self.connection.projects.list(search=fragment, owned=True)
-        cae.po(f"----  found {len(repos)} project repositories containing {fragment}:")
+    @_action(arg_names=((), ('fragment', ), ))
+    def search_repos(self, ini_pdv: PdvType, fragment: str = ""):
+        """ search remote repositories via a text fragment in its project name/description. """
+        fragment = fragment or _get_prj_name(ini_pdv)
+        repos = self.connection.projects.list(search=fragment, get_all=True)
+        cae.po(f"----  found {len(repos)} repos containing '{fragment}' in its name project name or description:")
         for repo in repos:
-            cae.po(PPF(repo))
-        cae.po(f" ==== searched {pdv_str(ini_pdv, 'project_desc')}")
+            cae.po(f"    - {PPF(repo)}")
+        cae.po(f" ==== searched all repos at {_get_host_domain(ini_pdv)} for '{fragment}'")
 
     @_action(PARENT_PRJ, ROOT_PRJ)
     def show_children_repos(self, ini_pdv: PdvType, *children_pdv: PdvType):
         """ display remote properties of parent/root children repos. """
         for chi_pdv in children_pdv:
             self.show_repo(chi_pdv)
         cae.po(f"===== dumped info of {_children_desc(ini_pdv, children_pdv)}")
@@ -3583,16 +3590,16 @@
     cae.po(f" ==== updated {pdv_str(ini_pdv, 'project_desc')}")
     return errors
 
 
 # ----------------------- main ----------------------------------------------------------------------------------------
 
 
-def main():                                                                                 # pragma: no cover
-    """ main app script """
+def prepare_and_run_main():                                                                # pragma: no cover
+    """ prepare and run app """
     cae.add_argument('action', help="action to execute (run `grm -v show_actions` to display all available actions)")
     cae.add_argument('arguments',
                      help="additional arguments and optional flags, depending on specified action, e.g. all children"
                           " actions expecting either a list of package/portion names or an expression using one of the"
                           " preset children sets like all|editable|modified|develop|filterBranch|filterExpression",
                      nargs='*')
     cae.add_option('branch', "branch or version-tag to checkout/filter-/work-on", "")
@@ -3624,13 +3631,18 @@
 
     global TEMP_CONTEXT
     if TEMP_CONTEXT:
         TEMP_CONTEXT.cleanup()
         TEMP_CONTEXT = None
 
 
-if __name__ == '__main__':                                                                      # pragma: no cover
+def main():                                                                                 # pragma: no cover
+    """ main app script """
     try:
-        main()
+        prepare_and_run_main()
     except Exception as main_ex:
         debug_info = f":{os.linesep}{format_exc()}" if _debug_or_verbose() else ""
         _exit_error(99, f"unexpected exception {main_ex} raised{debug_info}")
+
+
+if __name__ == '__main__':                                                                  # pragma: no cover
+    main()
```

### Comparing `aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/PKG-INFO` & `aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.76
+Version: 0.3.77
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -72,25 +72,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.76
+# git_repo_manager 0.3.77
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.75?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.75)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.76?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.76)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.76.
+>aedev_git_repo_manager package 0.3.77.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/requires.txt` & `aedev_git_repo_manager-0.3.77/aedev_git_repo_manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.76/setup.py` & `aedev_git_repo_manager-0.3.77/setup.py`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.76/tests/test_git_repo_manager.py` & `aedev_git_repo_manager-0.3.77/tests/test_git_repo_manager.py`

 * *Files identical despite different names*

