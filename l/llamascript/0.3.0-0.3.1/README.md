# Comparing `tmp/llamascript-0.3.0.tar.gz` & `tmp/llamascript-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamascript-0.3.0.tar", last modified: Thu May  2 00:27:19 2024, max compression
+gzip compressed data, was "llamascript-0.3.1.tar", last modified: Sat May  4 18:56:33 2024, max compression
```

## Comparing `llamascript-0.3.0.tar` & `llamascript-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:27:19.718314 llamascript-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-02 00:27:11.000000 llamascript-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-02 00:27:19.718314 llamascript-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-02 00:27:11.000000 llamascript-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:27:19.718314 llamascript-0.3.0/llamascript/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-02 00:27:11.000000 llamascript-0.3.0/llamascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-02 00:27:11.000000 llamascript-0.3.0/llamascript/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:27:19.718314 llamascript-0.3.0/llamascript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-02 00:27:19.000000 llamascript-0.3.0/llamascript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-02 00:27:19.000000 llamascript-0.3.0/llamascript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:27:19.000000 llamascript-0.3.0/llamascript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 00:27:19.000000 llamascript-0.3.0/llamascript.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 00:27:19.000000 llamascript-0.3.0/llamascript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 00:27:19.000000 llamascript-0.3.0/llamascript.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:27:19.718314 llamascript-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-02 00:27:11.000000 llamascript-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:56:33.883068 llamascript-0.3.1/
+-rw-rw-rw-   0        0        0    11525 2024-04-30 21:46:58.000000 llamascript-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2783 2024-05-04 18:56:33.882068 llamascript-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2327 2024-05-04 18:33:32.000000 llamascript-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 18:56:33.852428 llamascript-0.3.1/llamascript/
+-rw-rw-rw-   0        0        0     4511 2024-05-04 18:33:38.000000 llamascript-0.3.1/llamascript/__init__.py
+-rw-rw-rw-   0        0        0     1191 2024-05-01 21:23:13.000000 llamascript-0.3.1/llamascript/test.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:56:33.880066 llamascript-0.3.1/llamascript.egg-info/
+-rw-rw-rw-   0        0        0     2783 2024-05-04 18:56:33.000000 llamascript-0.3.1/llamascript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-04 18:56:33.000000 llamascript-0.3.1/llamascript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 18:56:33.000000 llamascript-0.3.1/llamascript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-04 18:56:33.000000 llamascript-0.3.1/llamascript.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 18:56:33.000000 llamascript-0.3.1/llamascript.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-04 18:56:33.000000 llamascript-0.3.1/llamascript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 18:56:33.884064 llamascript-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      764 2024-05-04 18:56:28.000000 llamascript-0.3.1/setup.py
```

### Comparing `llamascript-0.3.0/LICENSE` & `llamascript-0.3.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `llamascript-0.3.0/PKG-INFO` & `llamascript-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,53 @@
-Metadata-Version: 2.1
-Name: llamascript
-Version: 0.3.0
-Summary: No-code AI chatbot using Ollama.
-Home-page: https://github.com/WolfTheDeveloper/llamascript
-Author: WolfTheDev
-Author-email: wolfthedev@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ollama
-
-# LlamaScript
-
-[![Black Format](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml)
-[![Upload to PyPi](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml)
-[![CodeQL](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql)
-[![Tests](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml)
-
-LlamaScript is a no-code AI chatbot using Ollama.
-
-## Installation
-
-You can install LlamaScript using pip:
-
-```bash
-pip install llamascript
-```
-
-## Usage
-To use LlamaScript, create a llama file (no file extension) with the following commands:
-
-```llamascript
-IGNORE: Use this before the CHAT command to supress the welcome message.
-USE <model>: This command loads the specified model.
-SYSTEM <message>: This command sets the system prompt.
-PROMPT <message>: This command sets the message to be sent to the chatbot.
-CHAT: This command sends the message to the chatbot and prints the response.
-```
-
-Here's an example:
-
-```llamascript
-IGNORE
-USE llama3
-PROMPT Hello, how are you?
-CHAT
-```
-
-You can then run LlamaScript with the following command:
-
-```bash
-llamascript
-```
-
-## License
-LlamaScript is licensed under the Apache 2.0 License.
+# LlamaScript
+
+[Medium Post](https://medium.com/@wolfthedev/llamascript-simple-ai-builder-74442dc9b090)
+
+[![Black Format](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml)
+[![Upload to PyPi](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml)
+[![CodeQL](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql)
+[![Tests](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml)
+
+[![VS Code Extension Downloads](https://img.shields.io/visual-studio-marketplace/d/WolfTheDev.llamascript?label=VS-Code%20Downloads)](https://marketplace.visualstudio.com/items?itemName=WolfTheDev.llamascript)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/WolfTheDeveloper/llamascript?label=Commits)
+![GitHub License](https://img.shields.io/github/license/WolfTheDeveloper/llamascript?label=License)
+
+LlamaScript is a no-code AI chatbot using Ollama.
+
+## Installation
+
+You can install LlamaScript using pip:
+
+```bash
+pip install llamascript
+```
+
+## Usage
+To use LlamaScript, create a llama file (no file extension) with the following commands:
+
+```llamascript
+IGNORE: Use this before the CHAT command to supress the welcome message.
+USE <model>: This command loads the specified model.
+SYSTEM <message>: This command sets the system prompt.
+PROMPT <message>: This command sets the message to be sent to the chatbot.
+CHAT: This command sends the message to the chatbot and prints the response.
+```
+
+Here's an example:
+
+```llamascript
+IGNORE
+USE llama3
+PROMPT Hello, how are you?
+CHAT
+```
+
+You can then run LlamaScript with the following command:
+
+```bash
+llamascript
+```
+
+LlamaScript usually has a file extension of `.llama`, but if it is ran as a main script, it is usually `llama` (no file extension).
+
+## License
+LlamaScript is licensed under the Apache 2.0 License.
```

### Comparing `llamascript-0.3.0/llamascript/__init__.py` & `llamascript-0.3.1/llamascript/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,117 @@
-import asyncio
-import ollama
-import logging
-
-# Set up logging
-logging.basicConfig(level=logging.WARNING)
-
-
-class llama:
-    def __init__(self):
-        self.model = ""
-        self.data = ""
-        self.system = []
-        self.ignore = False
-
-    def USE(self, line):
-        if line.split(" ")[0] == "USE":
-            self.model = line.split(" ")[1].strip()
-        else:
-            raise ValueError("Invalid model")
-
-    def PROMPT(self, line="", p=""):
-        if p != "":
-            self.data = p
-        else:
-            split_line = line.split(" ", 1)
-            self.data = split_line[1] if len(split_line) > 1 else ""
-
-    def SYSTEM(self, line="", p=""):
-        if p != "":
-            self.system = [{"role": "system", "content": p}]
-        else:
-            split_line = line.split(" ", 1)
-            prompt = split_line[1] if len(split_line) > 1 else ""
-            self.system = [{"role": "system", "content": prompt}]
-
-    def CHAT(self, stream: bool = False):
-        for _ in range(3):
-            try:
-                response = ollama.chat(
-                    model=self.model,
-                    messages=self.system + [{"role": "user", "content": self.data}],
-                    stream=stream,
-                )
-                if stream:
-                    for message in response:
-                        print(message["message"]["content"], end="")
-                    print()
-                else:
-                    print(response["message"]["content"])
-                break
-            except Exception as e:
-                logging.error("Error using model: %s", e)
-                print("Model not loaded. Trying to load model...")
-                ollama.pull(self.model)
-                print("Model loaded. Trying again...")
-        else:
-            raise ValueError(
-                "Model does not exist or could not be loaded. Please try again."
-            )
-
-    def INPUT(self, command):
-        if command == "SYSTEM":
-            self.SYSTEM(p=input("Enter system prompt: "))
-        elif command == "PROMPT":
-            self.PROMPT(p=input("Enter prompt: "))
-        else:
-            raise ValueError("Invalid command for INPUT")
-
-    async def read(self, filename):
-        try:
-            with open(filename, "r") as file:
-                for line in file:
-                    line = line.strip()
-                    if not line:
-                        continue
-                    command = line.split(" ")
-                    if command[0] == "IGNORE":
-                        self.ignore = True
-                    elif command[0] == "USE":
-                        self.USE(line)
-                    elif len(command) > 1 and command[1] == "INPUT":
-                        self.INPUT(command[0])
-                    elif command[0] == "SYSTEM":
-                        self.SYSTEM(line=line)
-                    elif command[0] == "PROMPT":
-                        self.PROMPT(line=line)
-                    elif command[0] == "CHAT" and command[1] == "STREAM":
-                        stream = command[1] == True if len(command) > 1 else False
-                        if not self.ignore:
-                            print(
-                                '=================\nThanks for using llama, a no-code AI chatbot. Please ensure Ollama (https://ollama.com) is running. To get started, type "USE" followed by the model you want to use. Then, type "PROMPT" followed by the prompt you want to use. Finally, type "CHAT" to chat with the AI. To run a script, type "llamascript" to run your script. To ignore this message, add "IGNORE" to the beginning of your llama file.\n================='
-                            )
-                            self.ignore = True
-                        self.CHAT(stream=stream)
-                    else:
-                        raise ValueError("Invalid command")
-        except FileNotFoundError:
-            logging.error("File %s not found.", filename)
-            print(f"File {filename} not found.")
-
-import argparse
-
-def run():
-    parser = argparse.ArgumentParser(description='Run llama script.')
-    parser.add_argument('file_name', type=str, help='The name of the file to run')
-
-    args = parser.parse_args()
-
-    try:
-        l = llama()
-        asyncio.run(l.read(args.file_name))
-    except KeyboardInterrupt:
-        pass
+import asyncio
+import ollama
+import logging
+
+# Set up logging
+logging.basicConfig(level=logging.WARNING)
+
+
+class llama:
+    def __init__(self):
+        self.model = ""
+        self.data = ""
+        self.system = []
+        self.ignore = False
+
+    def USE(self, line):
+        if line.split(" ")[0] == "USE":
+            self.model = line.split(" ")[1].strip()
+        else:
+            raise ValueError("Invalid model")
+
+    def PROMPT(self, line="", p=""):
+        if p != "":
+            self.data = p
+        else:
+            split_line = line.split(" ", 1)
+            self.data = split_line[1] if len(split_line) > 1 else ""
+
+    def SYSTEM(self, line="", p=""):
+        if p != "":
+            self.system = [{"role": "system", "content": p}]
+        else:
+            split_line = line.split(" ", 1)
+            prompt = split_line[1] if len(split_line) > 1 else ""
+            self.system = [{"role": "system", "content": prompt}]
+
+    def CHAT(self, stream: bool = False):
+        for _ in range(3):
+            try:
+                response = ollama.chat(
+                    model=self.model,
+                    messages=self.system + [{"role": "user", "content": self.data}],
+                    stream=stream,
+                )
+                if stream:
+                    for message in response:
+                        print(message["message"]["content"], end="")
+                    print()
+                else:
+                    print(response["message"]["content"])
+                break
+            except Exception as e:
+                logging.error("Error using model: %s", e)
+                print("Model not loaded. Trying to load model...")
+                ollama.pull(self.model)
+                print("Model loaded. Trying again...")
+        else:
+            raise ValueError(
+                "Model does not exist or could not be loaded. Please try again."
+            )
+
+    def INPUT(self, command):
+        if command == "SYSTEM":
+            self.SYSTEM(p=input("Enter system prompt: "))
+        elif command == "PROMPT":
+            self.PROMPT(p=input("Enter prompt: "))
+        else:
+            raise ValueError("Invalid command for INPUT")
+
+    async def read(self, filename):
+        try:
+            with open(filename, "r") as file:
+                for line in file:
+                    line = line.strip()
+                    if not line:
+                        continue
+                    command = line.split(" ")
+                    if command[0] == "IGNORE":
+                        self.ignore = True
+                    elif command[0] == "USE":
+                        self.USE(line)
+                    elif len(command) > 1 and command[1] == "INPUT":
+                        self.INPUT(command[0])
+                    elif command[0] == "SYSTEM":
+                        self.SYSTEM(line=line)
+                    elif command[0] == "PROMPT":
+                        self.PROMPT(line=line)
+                    elif command[0] == "CHAT":
+                        if len(command) > 1 and command[1] == "STREAM":
+                            stream = command[1] == True if len(command) > 1 else False
+                        if not self.ignore:
+                            print(
+                                '=================\nThanks for using llama, a no-code AI chatbot. Please ensure Ollama (https://ollama.com) is running. To get started, type "USE" followed by the model you want to use. Then, type "PROMPT" followed by the prompt you want to use. Finally, type "CHAT" to chat with the AI. To run a script, type "llamascript" to run your script. To ignore this message, add "IGNORE" to the beginning of your llama file.\n================='
+                            )
+                            self.ignore = True
+                        self.CHAT(stream=stream)
+                    else:
+                        raise ValueError("Invalid command")
+        except FileNotFoundError:
+            logging.error("File %s not found.", filename)
+            print(f"File {filename} not found.")
+
+
+import argparse
+
+
+def run():
+    parser = argparse.ArgumentParser(description="Run llama script.")
+    parser.add_argument("file_name", type=str, help="The name of the file to run")
+
+    args = parser.parse_args()
+
+    try:
+        l = llama()
+        asyncio.run(l.read(args.file_name))
+    except KeyboardInterrupt:
+        pass
```

### Comparing `llamascript-0.3.0/llamascript/test.py` & `llamascript-0.3.1/llamascript/test.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import unittest
-from unittest.mock import patch
-from llamascript import llama
-
-
-class TestLlama(unittest.TestCase):
-    def setUp(self):
-        self.llama = llama()
-
-    def test_USE(self):
-        self.llama.USE("USE llama3")
-        self.assertEqual(self.llama.model, "llama3")
-
-    def test_PROMPT(self):
-        self.llama.PROMPT("PROMPT prompt1")
-        self.assertEqual(self.llama.data, "prompt1")
-
-    def test_SYSTEM(self):
-        self.llama.SYSTEM("SYSTEM system1")
-        self.assertEqual(self.llama.system, [{"role": "system", "content": "system1"}])
-
-    def test_INPUT_SYSTEM(self):
-        with patch("builtins.input", return_value="system1"):
-            self.llama.INPUT("SYSTEM")
-        self.assertEqual(self.llama.system, [{"role": "system", "content": "system1"}])
-
-    def test_INPUT_PROMPT(self):
-        with patch("builtins.input", return_value="prompt1"):
-            self.llama.INPUT("PROMPT")
-        self.assertEqual(self.llama.data, "prompt1")
-
-    def test_INPUT_invalid_command(self):
-        with self.assertRaises(ValueError):
-            self.llama.INPUT("INVALID")
-
-
-if __name__ == "__main__":
-    unittest.main()
+import unittest
+from unittest.mock import patch
+from llamascript import llama
+
+
+class TestLlama(unittest.TestCase):
+    def setUp(self):
+        self.llama = llama()
+
+    def test_USE(self):
+        self.llama.USE("USE llama3")
+        self.assertEqual(self.llama.model, "llama3")
+
+    def test_PROMPT(self):
+        self.llama.PROMPT("PROMPT prompt1")
+        self.assertEqual(self.llama.data, "prompt1")
+
+    def test_SYSTEM(self):
+        self.llama.SYSTEM("SYSTEM system1")
+        self.assertEqual(self.llama.system, [{"role": "system", "content": "system1"}])
+
+    def test_INPUT_SYSTEM(self):
+        with patch("builtins.input", return_value="system1"):
+            self.llama.INPUT("SYSTEM")
+        self.assertEqual(self.llama.system, [{"role": "system", "content": "system1"}])
+
+    def test_INPUT_PROMPT(self):
+        with patch("builtins.input", return_value="prompt1"):
+            self.llama.INPUT("PROMPT")
+        self.assertEqual(self.llama.data, "prompt1")
+
+    def test_INPUT_invalid_command(self):
+        with self.assertRaises(ValueError):
+            self.llama.INPUT("INVALID")
+
+
+if __name__ == "__main__":
+    unittest.main()
```

