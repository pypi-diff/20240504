# Comparing `tmp/identitychain-0.0.1.tar.gz` & `tmp/identitychain-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "identitychain-0.0.1.tar", last modified: Tue Oct 10 10:19:09 2023, max compression
+gzip compressed data, was "identitychain-0.1.0.tar", last modified: Sat May  4 05:24:12 2024, max compression
```

## Comparing `identitychain-0.0.1.tar` & `identitychain-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-10-10 10:19:09.878325 identitychain-0.0.1/
--rw-rw-rw-   0        0        0      315 2023-10-10 09:30:57.000000 identitychain-0.0.1/.bumpversion.cfg
--rw-rw-rw-   0        0        0    11558 2023-07-13 18:02:22.000000 identitychain-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      589 2023-10-10 09:31:10.000000 identitychain-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2817 2023-10-10 09:31:10.000000 identitychain-0.0.1/Makefile
--rw-rw-rw-   0        0        0    18817 2023-10-10 10:19:09.876320 identitychain-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4910 2023-10-10 10:07:12.000000 identitychain-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-10-10 10:19:09.835326 identitychain-0.0.1/examples/
--rw-rw-rw-   0        0        0     1888 2023-10-10 09:31:10.000000 identitychain-0.0.1/examples/run_identity_chain.sh
--rw-rw-rw-   0        0        0    32024 2023-10-10 09:31:10.000000 identitychain-0.0.1/examples/run_identity_chain_huggingface.py
--rw-rw-rw-   0        0        0    14735 2023-10-10 09:31:10.000000 identitychain-0.0.1/examples/run_identity_chain_openai.py
-drwxrwxrwx   0        0        0        0 2023-10-10 10:19:09.847332 identitychain-0.0.1/identitychain/
--rw-rw-rw-   0        0        0      247 2023-10-10 09:30:57.000000 identitychain-0.0.1/identitychain/__init__.py
--rw-rw-rw-   0        0        0    11808 2023-10-10 09:31:10.000000 identitychain-0.0.1/identitychain/dialogue.py
--rw-rw-rw-   0        0        0     8081 2023-10-10 09:30:57.000000 identitychain-0.0.1/identitychain/executor.py
--rw-rw-rw-   0        0        0    20684 2023-10-10 09:31:10.000000 identitychain-0.0.1/identitychain/identity_chain.py
-drwxrwxrwx   0        0        0        0 2023-10-10 10:19:09.858325 identitychain-0.0.1/identitychain/tests/
--rw-rw-rw-   0        0        0    16350 2023-10-10 09:30:57.000000 identitychain-0.0.1/identitychain/tests/test_executor.py
--rw-rw-rw-   0        0        0      569 2023-10-10 09:30:57.000000 identitychain-0.0.1/identitychain/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-10 10:19:09.856323 identitychain-0.0.1/identitychain.egg-info/
--rw-rw-rw-   0        0        0    18817 2023-10-10 10:19:09.000000 identitychain-0.0.1/identitychain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      815 2023-10-10 10:19:09.000000 identitychain-0.0.1/identitychain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-10 10:19:09.000000 identitychain-0.0.1/identitychain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      358 2023-10-10 10:19:09.000000 identitychain-0.0.1/identitychain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-10-10 10:19:09.000000 identitychain-0.0.1/identitychain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2594 2023-10-10 09:31:10.000000 identitychain-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      188 2023-10-10 09:31:10.000000 identitychain-0.0.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-10-10 10:19:09.868332 identitychain-0.0.1/scripts/
--rw-rw-rw-   0        0        0    15463 2023-10-10 09:31:10.000000 identitychain-0.0.1/scripts/analyze_results.py
--rw-rw-rw-   0        0        0     2073 2023-10-10 09:31:10.000000 identitychain-0.0.1/scripts/browse_results.py
-drwxrwxrwx   0        0        0        0 2023-10-10 10:19:09.875325 identitychain-0.0.1/scripts/human_judge/
--rw-rw-rw-   0        0        0    10761 2023-10-10 09:31:10.000000 identitychain-0.0.1/scripts/human_judge/analyze_results_hj.py
--rw-rw-rw-   0        0        0     2202 2023-10-10 09:31:10.000000 identitychain-0.0.1/scripts/human_judge/browse_samples.py
--rw-rw-rw-   0        0        0    10261 2023-10-10 09:31:10.000000 identitychain-0.0.1/scripts/human_judge/compute_correlation.py
--rw-rw-rw-   0        0        0     9087 2023-10-10 09:31:10.000000 identitychain-0.0.1/scripts/reformat_EvalPlus.py
--rw-rw-rw-   0        0        0    12555 2023-10-10 09:31:10.000000 identitychain-0.0.1/scripts/reformat_MBPP-S.py
--rw-rw-rw-   0        0        0       83 2023-10-10 09:30:57.000000 identitychain-0.0.1/scripts/run_tests.sh
--rw-rw-rw-   0        0        0       42 2023-10-10 10:19:09.878325 identitychain-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-07-13 17:46:35.000000 identitychain-0.0.1/setup.py
+drwx--S---   0 jm5025   (19193) arise      (509)        0 2024-05-04 05:24:12.040558 identitychain-0.1.0/
+-rw-------   0 jm5025   (19193) arise      (509)      303 2024-05-04 05:17:48.000000 identitychain-0.1.0/.bumpversion.cfg
+-rw-------   0 jm5025   (19193) arise      (509)    11357 2023-12-19 16:00:34.000000 identitychain-0.1.0/LICENSE
+-rw-------   0 jm5025   (19193) arise      (509)      587 2024-02-25 11:31:56.000000 identitychain-0.1.0/MANIFEST.in
+-rw-------   0 jm5025   (19193) arise      (509)     2704 2023-12-19 16:00:34.000000 identitychain-0.1.0/Makefile
+-rw-------   0 jm5025   (19193) arise      (509)    20193 2024-05-04 05:24:12.040558 identitychain-0.1.0/PKG-INFO
+-rw-------   0 jm5025   (19193) arise      (509)     6456 2024-05-04 05:17:48.000000 identitychain-0.1.0/README.md
+drwx--S---   0 jm5025   (19193) arise      (509)        0 2024-05-04 05:24:11.952558 identitychain-0.1.0/examples/
+-rw-------   0 jm5025   (19193) arise      (509)     1982 2024-05-04 05:17:48.000000 identitychain-0.1.0/examples/run_identity_chain.sh
+-rw-------   0 jm5025   (19193) arise      (509)    16112 2024-02-26 06:35:56.000000 identitychain-0.1.0/examples/run_identity_chain_google.py
+-rw-------   0 jm5025   (19193) arise      (509)    36057 2024-05-04 05:17:48.000000 identitychain-0.1.0/examples/run_identity_chain_huggingface.py
+-rw-------   0 jm5025   (19193) arise      (509)    15020 2024-02-25 11:31:56.000000 identitychain-0.1.0/examples/run_identity_chain_openai.py
+drwx--S---   0 jm5025   (19193) arise      (509)        0 2024-05-04 05:24:11.964558 identitychain-0.1.0/identitychain/
+-rw-------   0 jm5025   (19193) arise      (509)      319 2024-05-04 05:17:48.000000 identitychain-0.1.0/identitychain/__init__.py
+-rw-------   0 jm5025   (19193) arise      (509)    11545 2023-12-19 16:00:34.000000 identitychain-0.1.0/identitychain/dialogue.py
+-rw-------   0 jm5025   (19193) arise      (509)     7825 2023-12-19 16:00:34.000000 identitychain-0.1.0/identitychain/executor.py
+-rw-------   0 jm5025   (19193) arise      (509)    20908 2024-05-04 05:17:48.000000 identitychain-0.1.0/identitychain/identity_chain.py
+drwx--S---   0 jm5025   (19193) arise      (509)        0 2024-05-04 05:24:11.976558 identitychain-0.1.0/identitychain/tests/
+-rw-------   0 jm5025   (19193) arise      (509)    16009 2023-12-19 16:00:34.000000 identitychain-0.1.0/identitychain/tests/test_executor.py
+-rw-------   0 jm5025   (19193) arise      (509)      549 2023-12-19 16:00:34.000000 identitychain-0.1.0/identitychain/utils.py
+drwx--S---   0 jm5025   (19193) arise      (509)        0 2024-05-04 05:24:11.972558 identitychain-0.1.0/identitychain.egg-info/
+-rw-r--r--   0 jm5025   (19193) arise      (509)    20193 2024-05-04 05:24:11.000000 identitychain-0.1.0/identitychain.egg-info/PKG-INFO
+-rw-------   0 jm5025   (19193) arise      (509)      869 2024-05-04 05:24:11.000000 identitychain-0.1.0/identitychain.egg-info/SOURCES.txt
+-rw-------   0 jm5025   (19193) arise      (509)        1 2024-05-04 05:24:11.000000 identitychain-0.1.0/identitychain.egg-info/dependency_links.txt
+-rw-------   0 jm5025   (19193) arise      (509)      358 2024-05-04 05:24:11.000000 identitychain-0.1.0/identitychain.egg-info/requires.txt
+-rw-------   0 jm5025   (19193) arise      (509)       14 2024-05-04 05:24:11.000000 identitychain-0.1.0/identitychain.egg-info/top_level.txt
+drwx--S---   0 jm5025   (19193) arise      (509)        0 2024-05-04 05:24:11.976558 identitychain-0.1.0/images/
+-rw-------   0 jm5025   (19193) arise      (509)   864344 2024-02-25 11:31:56.000000 identitychain-0.1.0/images/main.png
+-rw-------   0 jm5025   (19193) arise      (509)     2519 2024-05-04 05:17:48.000000 identitychain-0.1.0/pyproject.toml
+-rw-------   0 jm5025   (19193) arise      (509)      172 2023-12-19 16:00:34.000000 identitychain-0.1.0/requirements.txt
+drwx--S---   0 jm5025   (19193) arise      (509)        0 2024-05-04 05:24:12.032559 identitychain-0.1.0/scripts/
+-rw-------   0 jm5025   (19193) arise      (509)    15110 2024-04-06 02:49:15.000000 identitychain-0.1.0/scripts/analyze_results.py
+-rw-------   0 jm5025   (19193) arise      (509)     2020 2023-12-19 16:00:34.000000 identitychain-0.1.0/scripts/browse_results.py
+drwx--S---   0 jm5025   (19193) arise      (509)        0 2024-05-04 05:24:12.036558 identitychain-0.1.0/scripts/human_judge/
+-rw-------   0 jm5025   (19193) arise      (509)    10491 2023-12-19 16:00:34.000000 identitychain-0.1.0/scripts/human_judge/analyze_results_hj.py
+-rw-------   0 jm5025   (19193) arise      (509)     2146 2023-12-19 16:00:34.000000 identitychain-0.1.0/scripts/human_judge/browse_samples.py
+-rw-------   0 jm5025   (19193) arise      (509)    10065 2023-12-19 16:00:34.000000 identitychain-0.1.0/scripts/human_judge/compute_correlation.py
+-rw-------   0 jm5025   (19193) arise      (509)    10717 2024-05-04 05:17:48.000000 identitychain-0.1.0/scripts/reformat_EvalPlus.py
+-rw-------   0 jm5025   (19193) arise      (509)    12282 2023-12-19 16:00:34.000000 identitychain-0.1.0/scripts/reformat_MBPP-S.py
+-rw-------   0 jm5025   (19193) arise      (509)       77 2023-12-19 16:00:34.000000 identitychain-0.1.0/scripts/run_tests.sh
+-rw-------   0 jm5025   (19193) arise      (509)       38 2024-05-04 05:24:12.040558 identitychain-0.1.0/setup.cfg
+-rw-------   0 jm5025   (19193) arise      (509)       39 2023-12-19 16:00:34.000000 identitychain-0.1.0/setup.py
```

### Comparing `identitychain-0.0.1/LICENSE` & `identitychain-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
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
+                                 Apache License
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

### Comparing `identitychain-0.0.1/Makefile` & `identitychain-0.1.0/Makefile`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-#########
-# BUILD #
-#########
-develop:  ## install dependencies and the library
-	python -m pip install -e .[develop]
-
-build:  ## build the python library
-	python setup.py build build_ext --inplace
-
-install:  ## install library
-	python -m pip install .
-
-
-#########
-# LINTS #
-#########
-lint:  ## run static analysis with black, flake8, and pylint, 	python -m pylint --disable=C0301,R1720,C0114,C0103,W1114 identitychain
-	python -m black --check identitychain scripts examples
-	python -m flake8 --max-line-length=150 --extend-ignore=E203 identitychain scripts examples
-
-# Alias
-lints: lint
-
-format:  ## run autoformatting with black
-	python -m black identitychain/ scripts/ examples/
-
-# Alias
-fix: format
-
-check:  ## check assets for packaging
-	check-manifest -v
-
-# Alias
-checks: check
-
-annotate:  ## run type checking
-	python -m mypy ./identitychain ./scripts
-
-# Alias
-type: annotate
-
-
-#########
-# TESTS #
-#########
-test:  ## clean and run unit tests, python -m pytest -vv identitychain/tests
-	bash scripts/run_tests.sh
-
-# Alias
-tests: test
-
-coverage:  ## clean and run unit tests with coverage
-	python -m pytest -v identitychain/tests --cov=identitychain --cov-branch --cov-fail-under=100 --junitxml=python_junit.xml --cov-report term-missing
-
-# Alias
-cov: coverage
-
-
-###########
-# VERSION #
-###########
-show-version:  ## doesn't work on Windows
-	bump2version --dry-run --allow-dirty setup.py --list | grep current | awk -F= '{print $2}'
-
-patch:
-	bump2version patch
-
-minor:
-	bump2version minor
-
-major:
-	bump2version major
-
-
-########
-# DIST #
-########
-dist-build:  ## build python dist, can also add bdist_wheel
-	python setup.py sdist
-
-dist-check:
-	python -m twine check dist/*
-
-dist: deep-clean check dist-build dist-check  ## build dists
-
-publish:  ## upload python assets
-	echo "would usually run python -m twine upload dist/* --skip-existing"
-
-# Alias
-pub: publish
-
-
-#########
-# CLEAN #
-#########
-deep-clean:  ## clean everything untracked from the repository
-	git clean -fdx
-
-clean:  ## clean the repository, doesn't work on Windows
-	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache .mypy_cache identitychain/__pycache__ identitychain/tests/__pycache__
-
-
-############################################################################################
-
-
-.DEFAULT_GOAL := help
-help:  ## doesn't work on Windows
-	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
-
-print-%:
-	@echo '$*=$($*)'
-
-.PHONY: develop build install lint lints format fix check checks annotate type test tests coverage cov show-version patch minor major dist-build dist-check dist publish pub deep-clean clean help
+#########
+# BUILD #
+#########
+develop:  ## install dependencies and the library
+	python -m pip install -e .[develop]
+
+build:  ## build the python library
+	python setup.py build build_ext --inplace
+
+install:  ## install library
+	python -m pip install .
+
+
+#########
+# LINTS #
+#########
+lint:  ## run static analysis with black, flake8, and pylint, 	python -m pylint --disable=C0301,R1720,C0114,C0103,W1114 identitychain
+	python -m black --check identitychain scripts examples
+	python -m flake8 --max-line-length=150 --extend-ignore=E203 identitychain scripts examples
+
+# Alias
+lints: lint
+
+format:  ## run autoformatting with black
+	python -m black identitychain/ scripts/ examples/
+
+# Alias
+fix: format
+
+check:  ## check assets for packaging
+	check-manifest -v
+
+# Alias
+checks: check
+
+annotate:  ## run type checking
+	python -m mypy ./identitychain ./scripts
+
+# Alias
+type: annotate
+
+
+#########
+# TESTS #
+#########
+test:  ## clean and run unit tests, python -m pytest -vv identitychain/tests
+	bash scripts/run_tests.sh
+
+# Alias
+tests: test
+
+coverage:  ## clean and run unit tests with coverage
+	python -m pytest -v identitychain/tests --cov=identitychain --cov-branch --cov-fail-under=100 --junitxml=python_junit.xml --cov-report term-missing
+
+# Alias
+cov: coverage
+
+
+###########
+# VERSION #
+###########
+show-version:  ## doesn't work on Windows
+	bump2version --dry-run --allow-dirty setup.py --list | grep current | awk -F= '{print $2}'
+
+patch:
+	bump2version patch
+
+minor:
+	bump2version minor
+
+major:
+	bump2version major
+
+
+########
+# DIST #
+########
+dist-build:  ## build python dist, can also add bdist_wheel
+	python setup.py sdist
+
+dist-check:
+	python -m twine check dist/*
+
+dist: deep-clean check dist-build dist-check  ## build dists
+
+publish:  ## upload python assets
+	echo "would usually run python -m twine upload dist/* --skip-existing"
+
+# Alias
+pub: publish
+
+
+#########
+# CLEAN #
+#########
+deep-clean:  ## clean everything untracked from the repository
+	git clean -fdx
+
+clean:  ## clean the repository, doesn't work on Windows
+	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache .mypy_cache identitychain/__pycache__ identitychain/tests/__pycache__
+
+
+############################################################################################
+
+
+.DEFAULT_GOAL := help
+help:  ## doesn't work on Windows
+	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
+
+print-%:
+	@echo '$*=$($*)'
+
+.PHONY: develop build install lint lints format fix check checks annotate type test tests coverage cov show-version patch minor major dist-build dist-check dist publish pub deep-clean clean help
```

### Comparing `identitychain-0.0.1/PKG-INFO` & `identitychain-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,322 +1,337 @@
-Metadata-Version: 2.1
-Name: identitychain
-Version: 0.0.1
-Summary: Code Model Trust Evaluation
-Author-email: "marcusm117, Robin-Y-Ding" <authors@gmail.com>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: repository, https://github.com/marcusm117/
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
-# IdentityChain
-
-## Installation
-
-Create and Activate a Conda Environment.
-
-   ``` bash
-   conda create -n idchain python=3.10
-   conda activate idchain
-   ```
-
-Clone this Repository to your Local Environment.
-
-   ``` bash
-   git clone https://github.com/marcusm117/IdentityChain.git
-   ```
-
-Install the Library with all Dependencies.
-
-   ``` bash
-   cd IdentityChain
-   make develop
-   ```
-
-## Usage
-
-Before the self-consistency evaluation, you need to make sure that one of the followings is satisfied:
-
-1. Your model is an Instruction-tuned Code LLM, and it's trained on both NL-to-PL and PL-to-NL tasks.
-2. Your model is a Foundation Code LLM, and it's trained on both completion and fill-in-the-middle tasks.
-
-To evaluate your model using IdentityChain, you need to prepare the followings:
-
-1. An evaluation dataset in the format of one of the followings (you can also use these two directly):
-   - [EvalPlus-Mini-v0.1.6_reformatted.jsonl](./data/EvalPlus-Mini-v0.1.6_reformatted.jsonl.gz)
-   - [MBPP-S_test_reformatted.jsonl](./data/MBPP-S_test_reformatted.jsonl.gz)
-2. An NL-to-PL prompt for your model
-3. A PL-to-NL prompt for your model
-4. An NL-to-PL generation function for your model
-5. A PL-to-NL generation function for your model
-
-See [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) for an example of how to use IdentityChain to evaluate OpenAI models.
-
-See [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py) for an example of how to use IdentityChain to evaluate HuggingFace open-source models. This example script already includes the following models:
-
-1. CodeLlama-Instruct-hf (7B, 13B, 34B)
-2. CodeLlama-hf (7B, 13B, 34B)
-3. starchat-beta
-4. starcoder
-5. starcoderplus
-6. starcoderbase (1B, 3B, 7B, 15B)
-
-## Example
-
-Use [run_identity_chain.sh](./examples/run_identity_chain.sh) to execute scripts [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) or [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py), which conducts several IdentityChain evaluation in a batch. Make sure that you modify the followings before running the script:
-
-1. `export CUDA_VISIBLE_DEVICES=0` to specify the local GPU device you want to use
-2. `export HF_HOME=YOUR_OWN_PATH/huggingface` to specify your own huggingface home path, where the model checkpoints will be cached
-3. `export IDENTITY_CHAIN_HOME=YOUR_OWN_PATH/IdentityChain` to your own IdentityChain home path
-4. other parameters in the script for your own needs
-
-Then run the script:
-
-``` bash
-cd examples
-bash run_identity_chain.sh
-```
-
-This script will create a temporary folder `tmp` under your IdentityChain home path, and store the results of IdentityChain evaluation in this folder, which will be a `jsonl` file. For example, `tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl`.
-
-Use [analyze_results.py](./scripts/analyze_results.py) to analyze the results of IdentityChain evaluation. It will geneartes an `xlsx` file, which contains the following information:
-
-1. The SC (Self-Consistency) and SSC (Strong Self-Consistency) scores of the model at each self-iteration step. Note that SSC_0 is just Pass@1
-2. The aggregated TOM score (also BLEU and CodeBLEU) information at each step for the following 4 types of resulsts: Pass-Pass, Pass-Fail, Fail-Fail, Fail-Pass
-3. The TOM score (also BLEU and CodeBLEU) trajectory at each self-iteration step for each sample in the eavluation set.
-4. The raw test case outputs at each self-iteration step
-
-``` bash
-cd ../scripts
-python analyze_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5
-```
-
-The analyzed results will give you a sense of the model's overall performance, and the TOM score trajectory will help you pinpoint the exact step where the model makes a mistake.
-
-Use [browse_results.py](./scripts/browse_results.py) to browse the results of IdentityChain evaluation. You can use this script to manually examine and study the mistakes made by the model for specific samples.
-
-``` bash
-cd ../scripts
-python browse_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5 --start 0
-```
-
-## Linting & Testing
-
-We use a `Makefile` as a command registry:
-
-- `make format`: autoformat  this library with `black`
-- `make lint`: perform static analysis of this library with `black` and `flake8`
-- `make annotate`: run type checking using `mypy`
-- `make test`: run automated tests
-- `make check`: check assets for packaging
-
-Make sure that `make lint`, `make test`, and `make check` all pass locally before submitting a Pull Request.
+Metadata-Version: 2.1
+Name: identitychain
+Version: 0.1.0
+Summary: Evaluation Framework for Code Large Language Models (Code LLMs)
+Author-email: "marcusm117, Robin-Y-Ding" <authors@gmail.com>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: repository, https://github.com/marcusm117/IdentityChain/
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+License-File: LICENSE
+
+# IdentityChain
+
+[![PyPI](https://img.shields.io/pypi/v/identitychain?color=blue&label=PyPI)](https://pypi.org/project/identitychain/) [![CI](https://github.com/marcusm117/IdentityChain/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/marcusm117/IdentityChain/actions/workflows/build.yml) [![License](https://img.shields.io/badge/License-Apache_2.0-green)](https://github.com/marcusm117/IdentityChain/blob/main/LICENSE) [![Issues](https://img.shields.io/github/issues/marcusm117/IdentityChain?color=red&label=Issues)](https://github.com/marcusm117/IdentityChain/issues)
+
+The IdentityChain Framework for Code Large Language Models (Code LLMs) Evaluation. Official implementation of the ICLR 2024 paper [Beyond Accuracy: Evaluating Self-Consistency of Code Large Language Models with IdentityChain](https://arxiv.org/abs/2310.14053).
+
+The IdentityChain Framework evaluates the NL-to-PL (Code Generation) Accuracy, PL-to-NL (Code Summurization) Accuracy, and the Self-Consistency across the two tasks. It also provides a fine-grained analysis of the model's performance so that you can pinpoint the exact step and problem where the model makes a self-inconsistency violation.
+
+<img src="./images/main.png" alt="image" width="800" height="auto">
+
+## Installation
+
+Create and Activate a Conda Environment.
+
+   ``` bash
+   conda create -n idchain python=3.10
+   conda activate idchain
+   ```
+
+Install from PyPI with all Dependencies.
+
+   ``` bash
+   pip3 install identitychain
+   pip3 install -r requirements.txt
+   ```
+
+Install from Source with all Dependencies.
+
+   ``` bash
+   git clone https://github.com/marcusm117/IdentityChain.git
+   cd IdentityChain
+   make develop
+   ```
+
+## Usage
+
+Before the self-consistency evaluation, you need to make sure that one of the followings is satisfied:
+
+1. Your model is an Instruction-tuned Code LLM, and it's trained on both NL-to-PL and PL-to-NL tasks.
+2. Your model is a Foundation Code LLM, and it's trained on both completion and fill-in-the-middle tasks.
+
+To evaluate your model using IdentityChain, you need to prepare the followings:
+
+1. An evaluation dataset from one of the followings (or one of your own in the same format):
+   - [EvalPlus-Mini-v0.1.6_reformatted.jsonl](./data/EvalPlus-Mini-v0.1.6_reformatted.jsonl.gz)
+   - [EvalPlus-Mini-v0.1.10_reformatted.jsonl](./data/EvalPlus-Mini-v0.1.10_reformatted.jsonl.gz)
+   - [MBPP-S_test_reformatted.jsonl](./data/MBPP-S_test_reformatted.jsonl.gz)
+2. An NL-to-PL prompt for your model
+3. A PL-to-NL prompt for your model
+4. An NL-to-PL generation function for your model
+5. A PL-to-NL generation function for your model
+
+See [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) for an example of how to use IdentityChain to evaluate OpenAI models.
+
+See [run_identity_chain_google.py](./examples/run_identity_chain_google.py) for an example of how to use IdentityChain to evaluate Google models.
+
+See [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py) for an example of how to use IdentityChain to evaluate HuggingFace open-source models. This example script already includes the following models:
+
+1. CodeLlama-Instruct-hf (7B, 13B, 34B, 70B)
+2. CodeLlama-hf (7B, 13B, 34B, 70B)
+3. StarChat-Beta
+4. StarCoder
+5. StarCoderPlus
+6. StarCoderBase (1B, 3B, 7B, 15B)
+7. DeepSeekCoder-Instruct (1.3B, 6.7B, 33B, 7B-v1.5)
+8. DeepSeekCoder (1.3B, 6.7B, 33B, 7B-v1.5)
+
+## Example
+
+Use [run_identity_chain.sh](./examples/run_identity_chain.sh) to execute scripts [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) or [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py), which conducts several IdentityChain evaluation in a batch. Make sure that you modify the followings before running the script:
+
+1. `export CUDA_VISIBLE_DEVICES=0` to specify the local GPU device you want to use
+2. `export HF_HOME=YOUR_OWN_PATH/huggingface` to specify your own huggingface home path, where the model checkpoints will be cached
+3. `export IDENTITY_CHAIN_HOME=YOUR_OWN_PATH/IdentityChain` to your own IdentityChain home path
+4. other parameters in the script for your own needs
+
+Then run the script:
+
+``` bash
+cd examples
+bash run_identity_chain.sh
+```
+
+This script will create a temporary folder `tmp` under your IdentityChain home path, and store the results of IdentityChain evaluation in this folder, which will be a `jsonl` file. For example, `tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl`.
+
+Use [analyze_results.py](./scripts/analyze_results.py) to analyze the results of IdentityChain evaluation. It will geneartes an `xlsx` file, which contains the following information:
+
+1. The SC (Self-Consistency) and SSC (Strong Self-Consistency) scores of the model at each self-iteration step. Note that SSC_0 is just Pass@1
+2. The aggregated TOM score (also BLEU and CodeBLEU) information at each step for the following 4 types of resulsts: Pass-Pass, Pass-Fail, Fail-Fail, Fail-Pass
+3. The TOM score (also BLEU and CodeBLEU) trajectory at each self-iteration step for each sample in the eavluation set.
+4. The raw test case outputs at each self-iteration step
+
+``` bash
+cd ../scripts
+python analyze_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5
+```
+
+The analyzed results will give you a sense of the model's overall performance, and the TOM score trajectory will help you pinpoint the exact step where the model makes a mistake.
+
+Use [browse_results.py](./scripts/browse_results.py) to browse the results of IdentityChain evaluation. You can use this script to manually examine and study the mistakes made by the model for specific samples.
+
+``` bash
+cd ../scripts
+python browse_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5 --start 0
+```
+
+## Linting & Testing
+
+We use a `Makefile` as a command registry:
+
+- `make format`: autoformat  this library with `black`
+- `make lint`: perform static analysis of this library with `black` and `flake8`
+- `make annotate`: run type checking using `mypy`
+- `make test`: run automated tests
+- `make check`: check assets for packaging
+
+Make sure that `make lint`, `make test`, and `make check` all pass locally before submitting a Pull Request.
```

### Comparing `identitychain-0.0.1/README.md` & `identitychain-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,117 @@
-# IdentityChain
-
-## Installation
-
-Create and Activate a Conda Environment.
-
-   ``` bash
-   conda create -n idchain python=3.10
-   conda activate idchain
-   ```
-
-Clone this Repository to your Local Environment.
-
-   ``` bash
-   git clone https://github.com/marcusm117/IdentityChain.git
-   ```
-
-Install the Library with all Dependencies.
-
-   ``` bash
-   cd IdentityChain
-   make develop
-   ```
-
-## Usage
-
-Before the self-consistency evaluation, you need to make sure that one of the followings is satisfied:
-
-1. Your model is an Instruction-tuned Code LLM, and it's trained on both NL-to-PL and PL-to-NL tasks.
-2. Your model is a Foundation Code LLM, and it's trained on both completion and fill-in-the-middle tasks.
-
-To evaluate your model using IdentityChain, you need to prepare the followings:
-
-1. An evaluation dataset in the format of one of the followings (you can also use these two directly):
-   - [EvalPlus-Mini-v0.1.6_reformatted.jsonl](./data/EvalPlus-Mini-v0.1.6_reformatted.jsonl.gz)
-   - [MBPP-S_test_reformatted.jsonl](./data/MBPP-S_test_reformatted.jsonl.gz)
-2. An NL-to-PL prompt for your model
-3. A PL-to-NL prompt for your model
-4. An NL-to-PL generation function for your model
-5. A PL-to-NL generation function for your model
-
-See [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) for an example of how to use IdentityChain to evaluate OpenAI models.
-
-See [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py) for an example of how to use IdentityChain to evaluate HuggingFace open-source models. This example script already includes the following models:
-
-1. CodeLlama-Instruct-hf (7B, 13B, 34B)
-2. CodeLlama-hf (7B, 13B, 34B)
-3. starchat-beta
-4. starcoder
-5. starcoderplus
-6. starcoderbase (1B, 3B, 7B, 15B)
-
-## Example
-
-Use [run_identity_chain.sh](./examples/run_identity_chain.sh) to execute scripts [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) or [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py), which conducts several IdentityChain evaluation in a batch. Make sure that you modify the followings before running the script:
-
-1. `export CUDA_VISIBLE_DEVICES=0` to specify the local GPU device you want to use
-2. `export HF_HOME=YOUR_OWN_PATH/huggingface` to specify your own huggingface home path, where the model checkpoints will be cached
-3. `export IDENTITY_CHAIN_HOME=YOUR_OWN_PATH/IdentityChain` to your own IdentityChain home path
-4. other parameters in the script for your own needs
-
-Then run the script:
-
-``` bash
-cd examples
-bash run_identity_chain.sh
-```
-
-This script will create a temporary folder `tmp` under your IdentityChain home path, and store the results of IdentityChain evaluation in this folder, which will be a `jsonl` file. For example, `tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl`.
-
-Use [analyze_results.py](./scripts/analyze_results.py) to analyze the results of IdentityChain evaluation. It will geneartes an `xlsx` file, which contains the following information:
-
-1. The SC (Self-Consistency) and SSC (Strong Self-Consistency) scores of the model at each self-iteration step. Note that SSC_0 is just Pass@1
-2. The aggregated TOM score (also BLEU and CodeBLEU) information at each step for the following 4 types of resulsts: Pass-Pass, Pass-Fail, Fail-Fail, Fail-Pass
-3. The TOM score (also BLEU and CodeBLEU) trajectory at each self-iteration step for each sample in the eavluation set.
-4. The raw test case outputs at each self-iteration step
-
-``` bash
-cd ../scripts
-python analyze_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5
-```
-
-The analyzed results will give you a sense of the model's overall performance, and the TOM score trajectory will help you pinpoint the exact step where the model makes a mistake.
-
-Use [browse_results.py](./scripts/browse_results.py) to browse the results of IdentityChain evaluation. You can use this script to manually examine and study the mistakes made by the model for specific samples.
-
-``` bash
-cd ../scripts
-python browse_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5 --start 0
-```
-
-## Linting & Testing
-
-We use a `Makefile` as a command registry:
-
-- `make format`: autoformat  this library with `black`
-- `make lint`: perform static analysis of this library with `black` and `flake8`
-- `make annotate`: run type checking using `mypy`
-- `make test`: run automated tests
-- `make check`: check assets for packaging
-
-Make sure that `make lint`, `make test`, and `make check` all pass locally before submitting a Pull Request.
+# IdentityChain
+
+[![PyPI](https://img.shields.io/pypi/v/identitychain?color=blue&label=PyPI)](https://pypi.org/project/identitychain/) [![CI](https://github.com/marcusm117/IdentityChain/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/marcusm117/IdentityChain/actions/workflows/build.yml) [![License](https://img.shields.io/badge/License-Apache_2.0-green)](https://github.com/marcusm117/IdentityChain/blob/main/LICENSE) [![Issues](https://img.shields.io/github/issues/marcusm117/IdentityChain?color=red&label=Issues)](https://github.com/marcusm117/IdentityChain/issues)
+
+The IdentityChain Framework for Code Large Language Models (Code LLMs) Evaluation. Official implementation of the ICLR 2024 paper [Beyond Accuracy: Evaluating Self-Consistency of Code Large Language Models with IdentityChain](https://arxiv.org/abs/2310.14053).
+
+The IdentityChain Framework evaluates the NL-to-PL (Code Generation) Accuracy, PL-to-NL (Code Summurization) Accuracy, and the Self-Consistency across the two tasks. It also provides a fine-grained analysis of the model's performance so that you can pinpoint the exact step and problem where the model makes a self-inconsistency violation.
+
+<img src="./images/main.png" alt="image" width="800" height="auto">
+
+## Installation
+
+Create and Activate a Conda Environment.
+
+   ``` bash
+   conda create -n idchain python=3.10
+   conda activate idchain
+   ```
+
+Install from PyPI with all Dependencies.
+
+   ``` bash
+   pip3 install identitychain
+   pip3 install -r requirements.txt
+   ```
+
+Install from Source with all Dependencies.
+
+   ``` bash
+   git clone https://github.com/marcusm117/IdentityChain.git
+   cd IdentityChain
+   make develop
+   ```
+
+## Usage
+
+Before the self-consistency evaluation, you need to make sure that one of the followings is satisfied:
+
+1. Your model is an Instruction-tuned Code LLM, and it's trained on both NL-to-PL and PL-to-NL tasks.
+2. Your model is a Foundation Code LLM, and it's trained on both completion and fill-in-the-middle tasks.
+
+To evaluate your model using IdentityChain, you need to prepare the followings:
+
+1. An evaluation dataset from one of the followings (or one of your own in the same format):
+   - [EvalPlus-Mini-v0.1.6_reformatted.jsonl](./data/EvalPlus-Mini-v0.1.6_reformatted.jsonl.gz)
+   - [EvalPlus-Mini-v0.1.10_reformatted.jsonl](./data/EvalPlus-Mini-v0.1.10_reformatted.jsonl.gz)
+   - [MBPP-S_test_reformatted.jsonl](./data/MBPP-S_test_reformatted.jsonl.gz)
+2. An NL-to-PL prompt for your model
+3. A PL-to-NL prompt for your model
+4. An NL-to-PL generation function for your model
+5. A PL-to-NL generation function for your model
+
+See [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) for an example of how to use IdentityChain to evaluate OpenAI models.
+
+See [run_identity_chain_google.py](./examples/run_identity_chain_google.py) for an example of how to use IdentityChain to evaluate Google models.
+
+See [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py) for an example of how to use IdentityChain to evaluate HuggingFace open-source models. This example script already includes the following models:
+
+1. CodeLlama-Instruct-hf (7B, 13B, 34B, 70B)
+2. CodeLlama-hf (7B, 13B, 34B, 70B)
+3. StarChat-Beta
+4. StarCoder
+5. StarCoderPlus
+6. StarCoderBase (1B, 3B, 7B, 15B)
+7. DeepSeekCoder-Instruct (1.3B, 6.7B, 33B, 7B-v1.5)
+8. DeepSeekCoder (1.3B, 6.7B, 33B, 7B-v1.5)
+
+## Example
+
+Use [run_identity_chain.sh](./examples/run_identity_chain.sh) to execute scripts [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) or [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py), which conducts several IdentityChain evaluation in a batch. Make sure that you modify the followings before running the script:
+
+1. `export CUDA_VISIBLE_DEVICES=0` to specify the local GPU device you want to use
+2. `export HF_HOME=YOUR_OWN_PATH/huggingface` to specify your own huggingface home path, where the model checkpoints will be cached
+3. `export IDENTITY_CHAIN_HOME=YOUR_OWN_PATH/IdentityChain` to your own IdentityChain home path
+4. other parameters in the script for your own needs
+
+Then run the script:
+
+``` bash
+cd examples
+bash run_identity_chain.sh
+```
+
+This script will create a temporary folder `tmp` under your IdentityChain home path, and store the results of IdentityChain evaluation in this folder, which will be a `jsonl` file. For example, `tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl`.
+
+Use [analyze_results.py](./scripts/analyze_results.py) to analyze the results of IdentityChain evaluation. It will geneartes an `xlsx` file, which contains the following information:
+
+1. The SC (Self-Consistency) and SSC (Strong Self-Consistency) scores of the model at each self-iteration step. Note that SSC_0 is just Pass@1
+2. The aggregated TOM score (also BLEU and CodeBLEU) information at each step for the following 4 types of resulsts: Pass-Pass, Pass-Fail, Fail-Fail, Fail-Pass
+3. The TOM score (also BLEU and CodeBLEU) trajectory at each self-iteration step for each sample in the eavluation set.
+4. The raw test case outputs at each self-iteration step
+
+``` bash
+cd ../scripts
+python analyze_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5
+```
+
+The analyzed results will give you a sense of the model's overall performance, and the TOM score trajectory will help you pinpoint the exact step where the model makes a mistake.
+
+Use [browse_results.py](./scripts/browse_results.py) to browse the results of IdentityChain evaluation. You can use this script to manually examine and study the mistakes made by the model for specific samples.
+
+``` bash
+cd ../scripts
+python browse_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5 --start 0
+```
+
+## Linting & Testing
+
+We use a `Makefile` as a command registry:
+
+- `make format`: autoformat  this library with `black`
+- `make lint`: perform static analysis of this library with `black` and `flake8`
+- `make annotate`: run type checking using `mypy`
+- `make test`: run automated tests
+- `make check`: check assets for packaging
+
+Make sure that `make lint`, `make test`, and `make check` all pass locally before submitting a Pull Request.
```

### Comparing `identitychain-0.0.1/examples/run_identity_chain.sh` & `identitychain-0.1.0/examples/run_identity_chain.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-# set your GPU device id
-export CUDA_VISIBLE_DEVICES=0
-
-# set your HuggingFace home path and your IdentityChain home path
-export HF_HOME=YOUR_OWN_PATH/huggingface
-export IDENTITY_CHAIN_HOME=YOUR_OWN_PATH/IdentityChain  # no / at the end
-
-# the folloiwng parameters
-# --seq_length 1536,
-# --gen_len 512,
-# --chain_length 5
-# are only for experiments in the paper, feel free use smaller values to save time
-# however, the results may be different from what we report in the paper
-
-# for open-source models from HuggingFace, when using greedy, add the flag --greedy_early_stop to accelerate
-# for OpenAI models, don't use --greedy_early_stop!!! temperature = 0 is NOT greedy!!!
-# for HumanEvalPlus-Mini-v0.1.6_reformatted.jsonl, use --resume_task_bs 1, since HumanEval/0 is used for prompt
-# for MBPP-S_test_reformatted.jsonl, use --resume_task_bs 0, since there's a separate prompt split
-
-for MODEL in "bigcode/starcoderbase-1b"  # feel free to add other supported models
-do
-	for DATASET in "EvalPlus-Mini-v0.1.6_reformatted.jsonl"  # feel free add other supported datasets
-	do
-		for TMP in 0  # feel free to add other temperatures, add the flag --do_sample to use temperature sampling
-		do
-			MODEL_NAME=$(basename $MODEL)
-			OUTPUT_DIR=${IDENTITY_CHAIN_HOME}/tmp/${MODEL_NAME}
-			mkdir -p $OUTPUT_DIR
-			# change this to python run_identity_chain_openai.py if you are evaluating OpenAI models
-			python run_identity_chain_huggingface.py \
-				--model_name_or_path $MODEL \
-				--hf_dir $HF_HOME \
-				--input_path ${IDENTITY_CHAIN_HOME}/tmp/${DATASET} \
-				--output_dir $OUTPUT_DIR \
-				--seq_length 1536 \
-				--gen_len 512 \
-				--greedy_early_stop \
-				--chain_length 5 \
-				--use_fp16 \
-				--mask_func_name \
-				--bootstrap_method problem \
-				--resume_task_bs 1 \
-				--resume_task_run 0 \
-				--temperature $TMP
-		done
-	done
+# set your GPU device id
+export CUDA_VISIBLE_DEVICES=0
+
+# set your HuggingFace home path and your IdentityChain home path
+export HF_HOME=YOUR_OWN_PATH/huggingface
+export IDENTITY_CHAIN_HOME=YOUR_OWN_PATH/IdentityChain  # no / at the end
+
+# the folloiwng parameters
+# --seq_length 1536,
+# --gen_len 512,
+# --chain_length 5
+# are only for experiments in the paper, feel free use smaller values to save time
+# however, the results may be different from what we report in the paper
+
+# for open-source models from HuggingFace, when using greedy, add the flag --greedy_early_stop to accelerate
+# for OpenAI models, don't use --greedy_early_stop!!! temperature = 0 is NOT greedy!!!
+# for EvalPlus-Mini-v0.1.6_reformatted.jsonl (or other versions), use --resume_task_bs 1, since HumanEval/0 is used for prompt
+# for MBPP-S_test_reformatted.jsonl, use --resume_task_bs 0, since there's a separate prompt split
+
+for MODEL in "bigcode/starcoderbase-1b"  # feel free to add other supported models
+do
+	for DATASET in "EvalPlus-Mini-v0.1.6_reformatted.jsonl"  # feel free add other supported datasets
+	do
+		for TMP in 0  # feel free to add other temperatures, add the flag --do_sample to use temperature sampling
+		do
+			MODEL_NAME=$(basename $MODEL)
+			OUTPUT_DIR=${IDENTITY_CHAIN_HOME}/tmp/${MODEL_NAME}
+			mkdir -p $OUTPUT_DIR
+			# change this to python run_identity_chain_openai.py if you are evaluating OpenAI models
+			# change this to python run_identity_chain_google.py if you are evaluating Google models
+			python ${IDENTITY_CHAIN_HOME}/examples/run_identity_chain_huggingface.py \
+				--model_name_or_path $MODEL \
+				--hf_dir $HF_HOME \
+				--input_path ${IDENTITY_CHAIN_HOME}/data/${DATASET} \
+				--output_dir $OUTPUT_DIR \
+				--seq_length 1536 \
+				--gen_len 512 \
+				--greedy_early_stop \
+				--chain_length 5 \
+				--use_fp16 \
+				--mask_func_name \
+				--bootstrap_method problem \
+				--resume_task_bs 1 \
+				--resume_task_run 0 \
+				--temperature $TMP
+		done
+	done
 done
```

### Comparing `identitychain-0.0.1/examples/run_identity_chain_huggingface.py` & `identitychain-0.1.0/examples/run_identity_chain_huggingface.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,707 +1,837 @@
-# Authors: Robin-Y-Ding, marcusm117
-# License: Apache 2.0
-
-
-# Standard Library Modules
-import argparse
-import os
-
-# External Modules
-import torch
-from transformers import AutoModelForCausalLM, AutoTokenizer, set_seed
-
-# Internal Modules
-from identitychain import IdentityChain
-from identitychain.dialogue import (
-    DialogueTemplate,
-    get_dialogue_template,
-    B_INST_CLLAMA,
-    E_INST_CLLAMA,
-)
-from identitychain.utils import g_unzip
-
-
-# set random seed
-set_seed(42)
-
-
-# Instruction-tuned Models and Foundation Models have different nl_2_pl/pl_2_nl prompts and functions
-INSTRUCTION_MODELS = [
-    "codellama/CodeLlama-7b-Instruct-hf",
-    "codellama/CodeLlama-13b-Instruct-hf",
-    "codellama/CodeLlama-34b-Instruct-hf",
-    "HuggingFaceH4/starchat-beta",
-]
-FOUNDATION_MODELS = [
-    "bigcode/starcoder",
-    "bigcode/starcoderplus",
-    "bigcode/starcoderbase",
-    "bigcode/starcoderbase-7b",
-    "bigcode/starcoderbase-3b",
-    "bigcode/starcoderbase-1b",
-    "codellama/CodeLlama-7b-hf",
-    "codellama/CodeLlama-13b-hf",
-    "codellama/CodeLlama-34b-hf",
-]
-
-
-# prompt settings
-NL_2_PL_HUMANEVAL = [
-    {  # Instructions
-        "role": "system",
-        "content": "Solve a coding problem in Python. "
-        + "Given the function signature and the problem description in the docstring, "
-        + "you only need to continue to complete the function body. "
-        + "Please strictly follow the format of the example below! "
-        + "Don't write down any thought processes! "
-        + "Don't copy the problem description! "
-        + "You must use correct indentation! "
-        + "Make sure your return statement is always inside the function! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "Output an indentation of 4 spaces first before you write anything else! "
-        + "You’d better be sure. \n\n",
-    },
-    {  # One-Shot Example: user input = function signature + problem description in docstring format
-        "role": "user",
-        "content": 'from typing import List\n\n\ndef has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
-        + '"""Check if in given list of numbers, are any two numbers closer to each other than\n    given threshold.\n    '
-        + '>>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    '
-        + '>>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    True\n    """\n',
-    },
-    {  # One-Shot Example: model output = solution
-        "role": "assistant",
-        "content": '    sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
-        + 'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n',
-    },
-    {  # Instructions to emphasize the format
-        "role": "system",
-        "content": "\nPlease strictly follow the format of the example above! "
-        + "You must use correct indentation! "
-        + "Make sure your return statement is always inside the function! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "Output an indentation of 4 spaces first before you write anything else! "
-        + "You’d better be sure. \n\n",
-    },
-]
-
-PL_2_NL_HUMANEVAL = [
-    {  # Instructions
-        "role": "system",
-        "content": "Given a Python solution to a coding problem, "
-        + "write an accurate problem description for it in the format of Python docstring without 'Args' and 'Returns'. "
-        + "Please strictly follow the format of the example below!"
-        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
-        + "Make sure to give a few examples of inputs and outputs in the docstring! "
-        + "Make sure the docstring has no 'Args' and no 'Returns'! "
-        + "You can only write a text desciption with a few examples as shown in the example below!  "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "You’d better be sure. \n\n",
-    },
-    {  # One-Shot Example: user input = function signature + candidate solution
-        "role": "user",
-        "content": 'from typing import List\n\n\ndef has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
-        + 'sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
-        + 'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n',
-    },
-    {  # One-Shot Example: model output = problem description in docstring format
-        "role": "assistant",
-        "content": '    """Check if in given list of numbers, are any two numbers closer to each other than\n    '
-        + 'given threshold.\n    >>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    '
-        + '>>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    True\n    """\n',
-    },
-    {  # Instructions to emphasize the format
-        "role": "system",
-        "content": "\nPlease strictly follow the format of the example above! "
-        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
-        + "Make sure to give a few examples of inputs and outputs in the docstring! "
-        + "Make sure the docstring has no 'Args' and no 'Returns'! "
-        + "You can only write a text desciption with a few examples as shown in the example above!  "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "You’d better be sure. \n\n",
-    },
-]
-
-NL_2_PL_MBPP = [
-    {  # Instructions
-        "role": "system",
-        "content": "Solve a coding problem in Python. "
-        + "Given the function signature and the problem description in the docstring, you only need to continue to complete the function body. "
-        + "Please strictly follow the format of the example below! "
-        + "Don't write down any thought processes! "
-        + "Don't copy the problem description! "
-        + "You must use correct indentation! "
-        + "Make sure your return statement is always inside the function! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "Output an indentation of 4 spaces first before you write anything else! "
-        + "You’d better be sure. \n\n",
-    },
-    {  # One-Shot Example: user input = function signature + problem description in docstring format
-        "role": "user",
-        "content": 'def similar_elements(test_tup1, test_tup2):\n    '
-        + '""" Write a function to find the shared elements from the given two lists.\n    """\n',
-    },
-    {  # One-Shot Example: model output = solution
-        "role": "assistant",
-        "content": '    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n',
-    },
-    {  # Instructions to emphasize the format
-        "role": "system",
-        "content": "\nPlease strictly follow the format of the example above! "
-        + "You must use correct indentation! "
-        + "Make sure your return statement is always inside the function! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "Output an indentation of 4 spaces first before you write anything else! "
-        + "You’d better be sure. \n\n",
-    },
-]
-
-PL_2_NL_MBPP = [
-    {  # Instructions
-        "role": "system",
-        "content": "Given a Python solution to a coding problem, write an accurate problem description for it in the format of Python docstring"
-        + "Please strictly follow the format of the example below!"
-        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
-        + "Make sure the docstring has no 'Args', no 'Returns', and no 'Examples'! "
-        + "You can only write a plain text desciption as shown in the example below! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "You’d better be sure. \n\n",
-    },
-    {  # One-Shot Example: user input = function signature + candidate solution
-        "role": "user",
-        "content": 'def similar_elements(test_tup1, test_tup2):\n    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n',
-    },
-    {  # One-Shot Example: model output = problem description in docstring format
-        "role": "assistant",
-        "content": '    """ Write a function to find the shared elements from the given two lists.\n    """\n',
-    },
-    {  # Instructions to emphasize the format
-        "role": "system",
-        "content": "\nPlease strictly follow the format of the example above! "
-        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
-        + "Make sure the docstring has no 'Args', no 'Returns', and no 'Examples'! "
-        + "You can only write a plain text desciption as shown in the example above! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "You’d better be sure. \n\n",
-    },
-]
-
-ONE_SHOT_HUMANEVAL = (
-    'def has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
-    + '"""Check if in given list of numbers, are any two numbers closer to each other than\n    given threshold.\n    '
-    + '>>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    >>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    '
-    + 'True\n    """\n    sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
-    + 'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n'
-)
-
-ONE_SHOT_MBPP = (
-    'def similar_elements(test_tup1, test_tup2):\n    """ Write a function to find the shared elements from the given two lists.\n    '
-    + '"""\n    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n'
-)
-
-
-def generate_text(model, tokenizer, prompt_text, args, eos_token_id=None):
-    if eos_token_id is None:
-        eos_token_id = tokenizer.eos_token_id
-    model_inputs = tokenizer(prompt_text, padding=False, add_special_tokens=False, return_tensors="pt")
-    model_inputs["prompt_text"] = prompt_text
-    input_ids = model_inputs["input_ids"]
-    attention_mask = model_inputs.get("attention_mask", None)
-    # Allow empty prompts
-    if input_ids.shape[1] == 0:
-        input_ids = None
-        attention_mask = None
-        in_b = 1
-    else:
-        in_b = input_ids.shape[0]
-    # BS x SL
-    if args.gen_length is None:
-        max_length = args.seq_length
-    else:
-        max_length = input_ids.shape[1] + args.gen_length
-    print("Generating text...")
-    generated_sequence = model.generate(
-        input_ids=input_ids.to(model.device),
-        attention_mask=attention_mask.to(model.device),
-        temperature=args.temperature,
-        top_k=args.top_k,
-        top_p=args.top_p,
-        max_length=max_length,
-        do_sample=args.do_sample,
-        num_beams=args.num_beams,
-        num_return_sequences=args.num_return_sequences,
-        pad_token_id=tokenizer.pad_token_id,
-        eos_token_id=eos_token_id,
-    )
-    out_b = generated_sequence.shape[0]
-    generated_sequence = generated_sequence.reshape(in_b, out_b // in_b, *generated_sequence.shape[1:])
-    generated_sequence = generated_sequence[0].cpu().numpy().tolist()
-    records = []
-    print("Decoding text...")
-    for sequence in generated_sequence:
-        text = tokenizer.decode(sequence, skip_special_tokens=True)
-        prompt_length = len(tokenizer.decode(input_ids[0], skip_special_tokens=True))
-        all_text = text[prompt_length:]
-        record = {"generated_text": all_text}
-        records.append(record)
-    return records
-
-
-def get_completion_starchat_nl_to_pl(prompt, user_input, model, tokenizer, args):
-    # select the correct in-context learning prompt based on the task
-    messages = prompt + [{"role": "user", "content": user_input}]
-    try:
-        dialogue_template = DialogueTemplate.from_pretrained(args.model_name_or_path)
-    except Exception:
-        print("No dialogue template found in model repo. Defaulting to the `no_system` template.")
-        dialogue_template = get_dialogue_template("no_system")
-    dialogue_template.messages = messages
-    formatted_prompt = dialogue_template.get_inference_prompt_nl_to_pl()
-    # Debug
-    # print(formatted_prompt)
-    # get completion from code lm
-    output = generate_text(
-        model,
-        tokenizer,
-        formatted_prompt,
-        args,
-        eos_token_id=tokenizer.convert_tokens_to_ids(dialogue_template.end_token),
-    )
-    completion = output[0]["generated_text"]
-    # post-processing
-    completion_lines = completion.split("\n")
-    processed_completion = ""
-    for line in completion_lines:
-        if line.startswith("    "):
-            processed_completion += line + "\n"
-    # remove extra docstring
-    # find all occurrences of three consecutive double quotes
-    res = [i for i in range(len(processed_completion)) if processed_completion.startswith('"""', i)]
-    # if res is empty, check for both single quotes
-    if not res:
-        res = [i for i in range(len(processed_completion)) if processed_completion.startswith("'''", i)]
-    # if found an extra docstring, remove it
-    if res:
-        # get end position of the extra docstring, remove everything before it
-        try:
-            end_position = res[1] + 3
-            processed_completion = processed_completion[end_position:]
-            if processed_completion.startswith("\n"):
-                processed_completion = processed_completion[1:]
-        except IndexError:
-            pass
-
-    # Debug
-    print(processed_completion)
-    return processed_completion
-
-
-def get_completion_starchat_pl_to_nl(prompt, user_input, model, tokenizer, args):
-    # select the correct in-context learning prompt based on the task
-    messages = prompt + [{"role": "user", "content": user_input}]
-    try:
-        dialogue_template = DialogueTemplate.from_pretrained(args.model_name_or_path)
-    except Exception:
-        print("No dialogue template found in model repo. Defaulting to the `no_system` template.")
-        dialogue_template = get_dialogue_template("no_system")
-    dialogue_template.messages = messages
-    formatted_prompt = dialogue_template.get_inference_prompt_pl_to_nl()
-    # Debug
-    # print(formatted_prompt)
-    # get completion from code lm
-    output = generate_text(
-        model,
-        tokenizer,
-        formatted_prompt,
-        args,
-        eos_token_id=tokenizer.convert_tokens_to_ids(dialogue_template.end_token),
-    )
-    completion = output[0]["generated_text"]
-    # post-processing: extract the docstring
-    completion = completion.replace("python", "")
-    completion_parts = completion.split("```")
-    if len(completion_parts) > 1:
-        completion = completion_parts[1]
-    completion_parts = completion.split('"""')
-    if len(completion_parts) > 1:
-        completion = completion_parts[1]
-    completion_parts = completion.split("'''")
-    if len(completion_parts) > 1:
-        completion = completion_parts[1]
-
-    # double check
-    if not completion.startswith('"""'):
-        completion = '"""' + completion
-    if not completion.endswith('"""'):
-        completion = completion + '\n"""'
-    completion_lines = completion.split("\n")
-    for idx, line in enumerate(completion_lines):
-        if not line.startswith("    "):
-            completion_lines[idx] = "    " + line
-    completion = "\n".join(completion_lines)
-    # Debug
-    print(completion)
-    return completion
-
-
-def get_completion_codellama_instruct_nl_to_pl(
-    prompt, user_input, model, tokenizer, args
-):  # reference: https://github.com/facebookresearch/codellama/blob/main/llama/generation.py
-    # select the correct in-context learning prompt based on the task
-    messages = prompt + [{"role": "user", "content": user_input}]
-    formatted_prompt = ""
-    for msg in messages:
-        if msg["role"] == "user":
-            content = msg["content"].strip()
-            formatted_prompt += tokenizer.bos_token + f"{B_INST_CLLAMA} " + content + f" {E_INST_CLLAMA} "
-        elif msg["role"] == "assistant":
-            formatted_prompt += " " + msg["content"].strip() + " " + tokenizer.eos_token
-        # system prompt doesn't work well for Code Llama-Instructs
-        # elif msg["role"] == "system":
-        #     formatted_prompt += f"{B_SYS_CLLAMA}" + msg["content"] + f"{E_SYS_CLLAMA}"
-    # Debug
-    # print(formatted_prompt)
-    output = generate_text(model, tokenizer, formatted_prompt, args)
-    completion = output[0]["generated_text"]
-
-    # post-processing
-    completion_lines = completion.split("\n")
-    processed_completion = ""
-    for line in completion_lines:
-        if line.startswith("    "):
-            processed_completion += line + "\n"
-
-    # remove extra docstring
-    # find all occurrences of three consecutive double quotes
-    res = [i for i in range(len(processed_completion)) if processed_completion.startswith('"""', i)]
-    # if res is empty, check for both single quotes
-    if not res:
-        res = [i for i in range(len(processed_completion)) if processed_completion.startswith("'''", i)]
-    # if found an extra docstring, remove it
-    if res:
-        # get end position of the extra docstring, remove everything before it
-        try:
-            end_position = res[1] + 3
-            processed_completion = processed_completion[end_position:]
-            if processed_completion.startswith("\n"):
-                processed_completion = processed_completion[1:]
-        except IndexError:
-            pass
-
-    # Debug
-    print(processed_completion)
-    return processed_completion
-
-
-def get_completion_codellama_instruct_pl_to_nl(prompt, user_input, model, tokenizer, args):
-    # select the correct in-context learning prompt based on the task
-    messages = prompt + [{"role": "user", "content": user_input}]
-    formatted_prompt = ""
-    for msg in messages:
-        if msg["role"] == "user":
-            if args.input_path.endswith("EvalPlus-Mini-v0.1.6_reformatted.jsonl"):
-                content = (
-                    msg["content"]
-                    + "\n\nWhat should be the docstring of the above function? Please only write down the docstring with some examples."
-                )
-            elif args.input_path.endswith("MBPP-S_test_reformatted.jsonl"):
-                content = (
-                    msg["content"]
-                    + "\n\nWhat should be the docstring of the above function? Please write down the docstring only in words without any examples!"
-                )
-            else:
-                raise ValueError(f"Input file {args.input_path} not supported")
-            formatted_prompt += tokenizer.bos_token + "[INST] " + content + " [/INST] "
-        elif msg["role"] == "assistant":
-            formatted_prompt += " " + msg["content"].strip() + " " + tokenizer.eos_token
-    # Debug
-    # print(formatted_prompt)
-    output = generate_text(model, tokenizer, formatted_prompt, args)
-    completion = output[0]["generated_text"]
-    # post-processing
-    completion_lines = completion.split("\n")
-    for idx, line in enumerate(completion_lines):
-        if not line.startswith("    "):
-            completion_lines[idx] = "    " + line.lstrip()
-    completion = "\n".join(completion_lines)
-    # add docstring guards if not present
-    if completion.startswith('    """') and not completion.endswith('"""'):
-        completion = completion + '"""'
-    elif completion.startswith("    '''") and not completion.endswith("'''"):
-        completion = completion + "'''"
-    # Debug
-    print(completion)
-    return completion
-
-
-def get_completion_codellama(
-    prompt, user_input, model, tokenizer, args
-):  # prompt is ONE_SHOT_HUMANEVAL or ONE_SHOT_MBPP
-    user_input = prompt + user_input
-    output = generate_text(model, tokenizer, user_input, args)
-    completion = output[0]["generated_text"]
-    # post-processing: extract the function body
-    processed_completion = ""
-    completion_lines = completion.split("\n")
-    for line in completion_lines:
-        if line.startswith("    "):
-            processed_completion += line + "\n"
-        else:
-            break
-    # Debug
-    print(processed_completion)
-    return processed_completion
-
-
-def get_completion_codellama_fim(
-    prompt, function_signature, function_body, model, tokenizer, args
-):  # prompt is ONE_SHOT_HUMANEVAL or ONE_SHOT_MBPP
-    function_signature = prompt + function_signature
-    fim_prompt = ""
-    # check indent
-    fim_prompt += (
-        " <PRE>" + function_signature + "    \"\"\"\n    " + " <SUF>" + "    \"\"\"\n" + function_body + " <MID>"
-    )
-    # Debug
-    # print(fim_prompt)
-    output = generate_text(model, tokenizer, fim_prompt, args)
-    completion = output[0]["generated_text"]
-    completion = "    \"\"\"\n    " + completion + "    \"\"\"\n"
-    # Debug
-    print(completion)
-    return completion
-
-
-def get_completion_starcoder(
-    prompt, user_input, model, tokenizer, args
-):  # prompt is ONE_SHOT_HUMANEVAL or ONE_SHOT_MBPP
-    user_input = prompt + user_input
-    output = generate_text(model, tokenizer, user_input.strip(), args)
-    completion = output[0]["generated_text"]
-    # post-processing: extract the function body
-    processed_completion = ""
-    completion_lines = completion.split("\n")
-    start = False
-    for line in completion_lines:
-        if line.startswith("    "):
-            start = True
-            processed_completion += line + "\n"
-        else:
-            if start:
-                break
-    # Debug
-    print(processed_completion)
-    return processed_completion
-
-
-def get_completion_starcoder_fim(
-    prompt, function_signature, function_body, model, tokenizer, args
-):  # prompt is ONE_SHOT_HUMANEVAL or ONE_SHOT_MBPP
-    function_signature = prompt + function_signature
-    fim_prompt = ""
-    # TODO check indent
-    fim_prompt += (
-        "<fim_prefix>"
-        + function_signature
-        + "    \"\"\""
-        + "<fim_suffix>"
-        + "\"\"\"\n"
-        + function_body
-        + "<fim_middle>"
-    )
-    output = generate_text(model, tokenizer, fim_prompt, args)
-    completion = output[0]["generated_text"]
-    completion = "    \"\"\"" + completion + "\"\"\"\n"
-    # Debug
-    print(completion)
-    return completion
-
-
-# EXAMPLE USAGE:
-# python run_identity_chain_huggingface.py
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--model_name_or_path', type=str, help='Path to the model')
-    parser.add_argument('--hf_dir', type=str, help='Path to the huggingface cache directory')
-    parser.add_argument('--input_path', type=str, help='Path to the input file')
-    parser.add_argument('--output_dir', type=str, help='Path to the output directory')
-    parser.add_argument('--chain_length', type=int, default=5, help='Number of steps in the Identity Chain')
-    parser.add_argument('--seq_length', type=int, default=2048, help='max length of the sequence')
-    parser.add_argument('--gen_length', type=int, default=None, help='max length of the generated sequence')
-    parser.add_argument('--do_sample', action='store_true', help='whether to do sampling')
-    parser.add_argument('--greedy_early_stop', action='store_true', help='whether to stop inference when fixed point')
-    parser.add_argument('--temperature', type=float, default=0, help='temperature for sampling')
-    parser.add_argument('--top_k', type=int, default=0, help='top k for sampling')
-    parser.add_argument('--top_p', type=float, default=1, help='top p for sampling')
-    parser.add_argument('--num_return_sequences', type=int, default=1, help='number of return sequences')
-    parser.add_argument('--num_beams', type=int, default=1, help='number of beams for beam search')
-    parser.add_argument('--use_int8', action='store_true', help='whether to use int8 quantization')
-    parser.add_argument('--use_fp16', action='store_true', help='whether to use fp16 precision')
-    parser.add_argument('--pass_only', action='store_true', help='whether to only pass the input to the next step')
-    parser.add_argument('--mask_func_name', action='store_true', help='whether to mask the function name')
-    parser.add_argument('--bootstrap_method', type=str, default='problem', help='method to bootstrap the chain')
-    parser.add_argument('--resume_task_bs', type=int, default=0, help='task to resume at when bootstrapping')
-    parser.add_argument('--resume_task_run', type=int, default=0, help='task to resume at')
-    parser.add_argument('--skip_bootstrap', action='store_true', help='whether to skip the bootstrap stage')
-    parser.add_argument('--version', type=str, default='v1', help='version of the identity chain')
-    args = parser.parse_args()
-
-    # set huggingface cache directory
-    HF_HOME = args.hf_dir
-    print("Loading model...")
-    # if specified, use int8 quantization
-    if args.use_int8:
-        print("**********************************")
-        print("**** Using 8-bit quantization ****")
-        print("**********************************")
-        model = AutoModelForCausalLM.from_pretrained(
-            args.model_name_or_path,
-            load_in_8bit=True,
-            device_map="auto",
-            cache_dir=HF_HOME,
-        )
-    # if specified, use fp16 precision
-    elif args.use_fp16:
-        print("**********************************")
-        print("****** Using fp16 precision ******")
-        print("**********************************")
-        model = AutoModelForCausalLM.from_pretrained(
-            args.model_name_or_path,
-            device_map="auto",
-            torch_dtype=torch.float16,
-            cache_dir=HF_HOME,
-        )
-    # otherwise, use default precision
-    else:
-        model = AutoModelForCausalLM.from_pretrained(
-            args.model_name_or_path,
-            device_map="auto",
-            cache_dir=HF_HOME,
-        )
-
-    # configure tokenizer
-    tokenizer = AutoTokenizer.from_pretrained(
-        args.model_name_or_path,
-        model_max_length=args.seq_length,
-        padding_side="right",
-        use_fast=False,
-        trust_remote_code=True,
-        cache_dir=HF_HOME,
-    )
-
-    # create output directory if not exists
-    if not os.path.exists("../tmp"):
-        os.makedirs("../tmp", exist_ok=True)
-    if not os.path.exists(args.output_dir):
-        os.makedirs(args.output_dir, exist_ok=True)
-
-    # unzip input file
-    input_path = args.input_path
-    input_file = input_path.split("/")[-1]
-    g_unzip(f"../data/{input_file}.gz", input_path)
-
-    # for output path naming
-    model_name = args.model_name_or_path.split("/")[-1]
-    tmp = args.temperature
-    len = args.chain_length
-    bootstrap = "pb" if args.bootstrap_method == "problem" else "cb"
-    pass_only = "po" if args.pass_only else "all"
-    mask_name = "m" if args.mask_func_name else "um"
-    greedy = "g" if args.greedy_early_stop else ""
-    version = args.version
-
-    # define the output path
-    output_path = f"{args.output_dir}/IDChain_{model_name}_tmp{tmp}{greedy}_len{len}_{bootstrap}_{pass_only}_{mask_name}_{version}_{input_file}"
-
-    # configure nl_2_pl/pl_2_nl functions based on the model
-    # configure functions for starchat-beta
-    if args.model_name_or_path == "HuggingFaceH4/starchat-beta":
-        nl_2_pl_function = get_completion_starchat_nl_to_pl
-        pl_2_nl_function = get_completion_starchat_pl_to_nl
-    # configure functions for starcoder completion models
-    elif args.model_name_or_path.startswith("bigcode/starcoder"):
-        nl_2_pl_function = get_completion_starcoder
-        pl_2_nl_function = get_completion_starcoder_fim
-    # configure functions for codellama models
-    elif "CodeLlama" in args.model_name_or_path:
-        # configure functions for codellama-instruct chat models
-        if "Instruct" in args.model_name_or_path:
-            nl_2_pl_function = get_completion_codellama_instruct_nl_to_pl
-            pl_2_nl_function = get_completion_codellama_instruct_pl_to_nl
-        # configure functions for codellama completion models
-        else:
-            nl_2_pl_function = get_completion_codellama
-            pl_2_nl_function = get_completion_codellama_fim
-    else:
-        raise ValueError(f"Model {args.model_name_or_path} not supported")
-
-    # configure nl_2_pl/pl_2_nl prompts based on the model and input dataset
-    # configure prompts for HumanEvalPlus-Mini-v0.1.6
-    if args.input_path.endswith("EvalPlus-Mini-v0.1.6_reformatted.jsonl"):
-        # configure prompt for supported chat models
-        if args.model_name_or_path in INSTRUCTION_MODELS:
-            nl_2_pl_prompt = NL_2_PL_HUMANEVAL
-            pl_2_nl_prompt = PL_2_NL_HUMANEVAL
-        # configure prompt for supported completion models
-        elif args.model_name_or_path in FOUNDATION_MODELS:
-            # both nl_2_pl and pl_2_nl prompts are the same for completion models
-            nl_2_pl_prompt = ONE_SHOT_HUMANEVAL
-            pl_2_nl_prompt = ONE_SHOT_HUMANEVAL
-        else:
-            raise ValueError(f"Model {args.model_name_or_path} not supported")
-    # configure prompts for MBPP-S_test
-    elif args.input_path.endswith("MBPP-S_test_reformatted.jsonl"):
-        # configure prompt for supported chat models
-        if args.model_name_or_path in INSTRUCTION_MODELS:
-            nl_2_pl_prompt = NL_2_PL_MBPP
-            pl_2_nl_prompt = PL_2_NL_MBPP
-        # configure prompt for supported completion models
-        elif args.model_name_or_path in FOUNDATION_MODELS:
-            # both nl_2_pl and pl_2_nl prompts are the same for completion models
-            nl_2_pl_prompt = ONE_SHOT_MBPP
-            pl_2_nl_prompt = ONE_SHOT_MBPP
-        else:
-            raise ValueError(f"Model {args.model_name_or_path} not supported")
-    else:
-        raise ValueError(f"Input file {args.input_path} not supported")
-
-    # for debugging
-    print("--------- Prompt Configuration -----------")
-    print(nl_2_pl_prompt)
-    print(pl_2_nl_prompt)
-    print("-----------------------------------------")
-
-    # create the identity chain
-    my_chain = IdentityChain(
-        model=model,
-        tokenizer=tokenizer,
-        args=args,
-        input_path=input_path,
-        output_path=output_path,
-        get_model_response_NL_to_PL=nl_2_pl_function,
-        get_model_response_PL_to_NL=pl_2_nl_function,
-        prompt_NL_to_PL=nl_2_pl_prompt,
-        prompt_PL_to_NL=pl_2_nl_prompt,
-        bootstrap_method="problem",
-        length=args.chain_length,
-    )
-    print("-----------------------------------------")
-    print(f"Input Path: {input_path}")
-    print(f"Output Path: {output_path}")
-    print("-----------------------------------------")
-    input("Please Confirm the Identity Chain Setup. Press 'Enter' to Continue...")
-
-    # if resume_task_run != 0 or skip_bootstrap == True, then we don't need to bootstrap
-    if (args.resume_task_run == 0) and (not args.skip_bootstrap):
-        my_chain.bootstrap(resume_task=args.resume_task_bs)
-
-    my_chain.run(
-        resume_task=args.resume_task_run,
-        resume_step=1,
-        pass_only=args.pass_only,
-        mask_func_name=args.mask_func_name,
-        greedy_early_stop=args.greedy_early_stop,
-    )
-
-
-if __name__ == "__main__":
-    main()
+# Authors: Robin-Y-Ding, marcusm117
+# License: Apache 2.0
+
+
+# Standard Library Modules
+import argparse
+import os
+
+# External Modules
+import torch
+from transformers import AutoModelForCausalLM, AutoTokenizer, set_seed
+
+# Internal Modules
+from identitychain import IdentityChain, INSTRUCTION_MODELS, FOUNDATION_MODELS
+from identitychain.dialogue import (
+    DialogueTemplate,
+    get_dialogue_template,
+    B_INST_CLLAMA,
+    E_INST_CLLAMA,
+)
+from identitychain.utils import g_unzip
+
+
+# set random seed
+set_seed(42)
+
+
+# prompt settings
+NL_2_PL_HUMANEVAL = [
+    {  # Instructions
+        "role": "system",
+        "content": "Solve a coding problem in Python. "
+        + "Given the function signature and the problem description in the docstring, "
+        + "you only need to continue to complete the function body. "
+        + "Please strictly follow the format of the example below! "
+        + "Don't write down any thought processes! "
+        + "Don't copy the problem description! "
+        + "You must use correct indentation! "
+        + "Make sure your return statement is always inside the function! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "Output an indentation of 4 spaces first before you write anything else! "
+        + "You’d better be sure. \n\n",
+    },
+    {  # One-Shot Example: user input = function signature + problem description in docstring format
+        "role": "user",
+        "content": 'from typing import List\n\n\ndef has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
+        + '"""Check if in given list of numbers, are any two numbers closer to each other than\n    given threshold.\n    '
+        + '>>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    '
+        + '>>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    True\n    """\n',
+    },
+    {  # One-Shot Example: model output = solution
+        "role": "assistant",
+        "content": '    sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
+        + 'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n',
+    },
+    {  # Instructions to emphasize the format
+        "role": "system",
+        "content": "\nPlease strictly follow the format of the example above! "
+        + "You must use correct indentation! "
+        + "Make sure your return statement is always inside the function! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "Output an indentation of 4 spaces first before you write anything else! "
+        + "You’d better be sure. \n\n",
+    },
+]
+
+PL_2_NL_HUMANEVAL = [
+    {  # Instructions
+        "role": "system",
+        "content": "Given a Python solution to a coding problem, "
+        + "write an accurate problem description for it in the format of Python docstring without 'Args' and 'Returns'. "
+        + "Please strictly follow the format of the example below!"
+        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
+        + "Make sure to give a few examples of inputs and outputs in the docstring! "
+        + "Make sure the docstring has no 'Args' and no 'Returns'! "
+        + "You can only write a text desciption with a few examples as shown in the example below!  "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "You’d better be sure. \n\n",
+    },
+    {  # One-Shot Example: user input = function signature + candidate solution
+        "role": "user",
+        "content": 'from typing import List\n\n\ndef has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
+        + 'sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
+        + 'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n',
+    },
+    {  # One-Shot Example: model output = problem description in docstring format
+        "role": "assistant",
+        "content": '    """Check if in given list of numbers, are any two numbers closer to each other than\n    '
+        + 'given threshold.\n    >>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    '
+        + '>>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    True\n    """\n',
+    },
+    {  # Instructions to emphasize the format
+        "role": "system",
+        "content": "\nPlease strictly follow the format of the example above! "
+        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
+        + "Make sure to give a few examples of inputs and outputs in the docstring! "
+        + "Make sure the docstring has no 'Args' and no 'Returns'! "
+        + "You can only write a text desciption with a few examples as shown in the example above!  "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "You’d better be sure. \n\n",
+    },
+]
+
+NL_2_PL_MBPP = [
+    {  # Instructions
+        "role": "system",
+        "content": "Solve a coding problem in Python. "
+        + "Given the function signature and the problem description in the docstring, you only need to continue to complete the function body. "
+        + "Please strictly follow the format of the example below! "
+        + "Don't write down any thought processes! "
+        + "Don't copy the problem description! "
+        + "You must use correct indentation! "
+        + "Make sure your return statement is always inside the function! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "Output an indentation of 4 spaces first before you write anything else! "
+        + "You’d better be sure. \n\n",
+    },
+    {  # One-Shot Example: user input = function signature + problem description in docstring format
+        "role": "user",
+        "content": 'def similar_elements(test_tup1, test_tup2):\n    '
+        + '""" Write a function to find the shared elements from the given two lists.\n    """\n',
+    },
+    {  # One-Shot Example: model output = solution
+        "role": "assistant",
+        "content": '    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n',
+    },
+    {  # Instructions to emphasize the format
+        "role": "system",
+        "content": "\nPlease strictly follow the format of the example above! "
+        + "You must use correct indentation! "
+        + "Make sure your return statement is always inside the function! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "Output an indentation of 4 spaces first before you write anything else! "
+        + "You’d better be sure. \n\n",
+    },
+]
+
+PL_2_NL_MBPP = [
+    {  # Instructions
+        "role": "system",
+        "content": "Given a Python solution to a coding problem, write an accurate problem description for it in the format of Python docstring"
+        + "Please strictly follow the format of the example below!"
+        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
+        + "Make sure the docstring has no 'Args', no 'Returns', and no 'Examples'! "
+        + "You can only write a plain text desciption as shown in the example below! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "You’d better be sure. \n\n",
+    },
+    {  # One-Shot Example: user input = function signature + candidate solution
+        "role": "user",
+        "content": 'def similar_elements(test_tup1, test_tup2):\n    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n',
+    },
+    {  # One-Shot Example: model output = problem description in docstring format
+        "role": "assistant",
+        "content": '    """ Write a function to find the shared elements from the given two lists.\n    """\n',
+    },
+    {  # Instructions to emphasize the format
+        "role": "system",
+        "content": "\nPlease strictly follow the format of the example above! "
+        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
+        + "Make sure the docstring has no 'Args', no 'Returns', and no 'Examples'! "
+        + "You can only write a plain text desciption as shown in the example above! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "You’d better be sure. \n\n",
+    },
+]
+
+ONE_SHOT_HUMANEVAL = (
+    'def has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
+    '"""Check if in given list of numbers, are any two numbers closer to each other than\n    given threshold.\n    '
+    '>>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    >>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    '
+    'True\n    """\n    sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
+    'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n'
+)
+
+ONE_SHOT_FIM_HUMANEVAL = (
+    '<pre_token>def has_close_elements(numbers: List[float], threshold: float) -> bool:\n    """\n'
+    '<suf_token>    """\n    sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
+    'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n'
+    '<mid_token>'
+    'Check if in given list of numbers, are any two numbers closer to each other than\n    given threshold.\n    '
+    '>>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    >>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    True\n'
+)
+
+ONE_SHOT_MBPP = (
+    'def similar_elements(test_tup1, test_tup2):\n    """ Write a function to find the shared elements from the given two lists.\n    '
+    '"""\n    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n'
+)
+
+ONE_SHOT_FIM_MBPP = (
+    '<pre_token>def similar_elements(test_tup1, test_tup2):\n    """\n'
+    '<suf_token>    """\n    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n'
+    '<mid_token>Write a function to find the shared elements from the given two lists.\n'
+)
+
+
+def generate_text(model, tokenizer, prompt_text, args, eos_token_id=None):
+    if eos_token_id is None:
+        eos_token_id = tokenizer.eos_token_id
+    model_inputs = tokenizer(prompt_text, padding=False, add_special_tokens=False, return_tensors="pt")
+    model_inputs["prompt_text"] = prompt_text
+    input_ids = model_inputs["input_ids"]
+    attention_mask = model_inputs.get("attention_mask", None)
+    # Allow empty prompts
+    if input_ids.shape[1] == 0:
+        input_ids = None
+        attention_mask = None
+        in_b = 1
+    else:
+        in_b = input_ids.shape[0]
+    # BS x SL
+    if args.gen_length is None:
+        max_length = args.seq_length
+    else:
+        max_length = input_ids.shape[1] + args.gen_length
+    print("Generating Text...")
+    generated_sequence = model.generate(
+        input_ids=input_ids.to(model.device),
+        attention_mask=attention_mask.to(model.device),
+        temperature=args.temperature,
+        top_k=args.top_k,
+        top_p=args.top_p,
+        max_length=max_length,
+        do_sample=args.do_sample,
+        num_beams=args.num_beams,
+        num_return_sequences=args.num_return_sequences,
+        pad_token_id=tokenizer.pad_token_id,
+        eos_token_id=eos_token_id,
+    )
+    out_b = generated_sequence.shape[0]
+    generated_sequence = generated_sequence.reshape(in_b, out_b // in_b, *generated_sequence.shape[1:])
+    generated_sequence = generated_sequence[0].cpu().numpy().tolist()
+    records = []
+    print("Decoding Text...")
+    for sequence in generated_sequence:
+        text = tokenizer.decode(sequence, skip_special_tokens=True)
+        prompt_length = len(tokenizer.decode(input_ids[0], skip_special_tokens=True))
+        all_text = text[prompt_length:]
+        record = {"generated_text": all_text}
+        records.append(record)
+    return records
+
+
+def post_processing_nl_to_pl(completion):
+    # DEBUG
+    print(completion)
+    print("Post-Processing Text...")
+
+    # separate the completion into lines
+    completion_lines = completion.split("\n")
+    processed_completion = ""
+    for idx, line in enumerate(completion_lines):
+        if line.startswith("    "):
+            processed_completion += line + "\n"
+        # omit everything after the end of the first function body
+        if line.startswith("    return "):
+            break
+        if "return" in line:
+            # if the next line is non-empty, then discard all docstrings + anything without an indentation
+            if idx < len(completion_lines) - 1 and completion_lines[idx + 1] != "":
+                if (
+                    completion_lines[idx + 1].startswith("    \"\"\"")
+                    or completion_lines[idx + 1].startswith("    '''")
+                    or not completion_lines[idx + 1].startswith("    ")
+                ):
+                    break
+            # if the next line is empty, check the line after it
+            if idx < len(completion_lines) - 2 and completion_lines[idx + 1] == "":
+                if (
+                    completion_lines[idx + 2].startswith("    \"\"\"")
+                    or completion_lines[idx + 2].startswith("    '''")
+                    or not completion_lines[idx + 2].startswith("    ")
+                ):
+                    break
+
+    # remove extra docstring
+    # find all occurrences of three consecutive double quotes
+    res = [i for i in range(len(processed_completion)) if processed_completion.startswith('"""', i)]
+    # if res is empty, check for both single quotes
+    if not res:
+        res = [i for i in range(len(processed_completion)) if processed_completion.startswith("'''", i)]
+    # if found an extra docstring, remove it
+    if res:
+        # get end position of the extra docstring, remove everything before it
+        try:
+            end_position = res[1] + 3
+            processed_completion = processed_completion[end_position:]
+            if processed_completion.startswith("\n"):
+                processed_completion = processed_completion[1:]
+        except IndexError:
+            pass
+
+    # DEBUG
+    print(processed_completion)
+    return processed_completion
+
+
+def post_processing_pl_to_nl(completion):
+    # DEBUG
+    print(completion)
+    print("Post-Processing Text...")
+
+    # extract the docstring
+    completion = completion.replace("python", "")
+    completion_parts = completion.split("```")
+    if len(completion_parts) > 1:
+        completion = completion_parts[1]
+    completion_parts = completion.split('"""')
+    if len(completion_parts) > 1:
+        completion = completion_parts[1]
+    completion_parts = completion.split("'''")
+    if len(completion_parts) > 1:
+        completion = completion_parts[1]
+
+    # double check
+    if not completion.startswith('"""'):
+        completion = '"""' + completion
+    if not completion.endswith('"""'):
+        completion = completion.rstrip() + '\n"""'
+
+    # add indentation if missing
+    completion_lines = completion.split("\n")
+    for idx, line in enumerate(completion_lines):
+        if not line.startswith("    "):
+            completion_lines[idx] = "    " + line.lstrip()
+    processed_completion = "\n".join(completion_lines)
+
+    # add docstring guards if not present
+    if processed_completion.startswith('    """') and not processed_completion.endswith('"""'):
+        processed_completion = processed_completion + '"""'
+    elif processed_completion.startswith("    '''") and not processed_completion.endswith("'''"):
+        processed_completion = processed_completion + "'''"
+
+    # DEBUG
+    print(processed_completion)
+    return processed_completion
+
+
+def fill_in_middle(
+    prompt,
+    function_signature,
+    function_body,
+    model,
+    tokenizer,
+    args,
+    pre_token,
+    suf_token,
+    mid_token,
+):
+    # custimize the one-shot example by replacing the string "<pre-token>" with the actual pre-token etc.
+    prompt = (
+        prompt.replace("<pre_token>", pre_token).replace("<suf_token>", suf_token).replace("<mid_token>", mid_token)
+    )
+    fim_prompt = ""
+
+    # construct the fill-in-the-middle prompt
+    fim_prompt += (
+        prompt
+        + pre_token
+        + function_signature
+        + "    \"\"\"\n    "
+        + suf_token
+        + "    \"\"\"\n"
+        + function_body
+        + mid_token
+    )
+
+    # DEBUG
+    # print(fim_prompt)
+
+    output = generate_text(model, tokenizer, fim_prompt, args)
+    completion = output[0]["generated_text"]
+    completion = "    \"\"\"\n    " + completion + "    \"\"\"\n"
+
+    # DEBUG
+    print(completion)
+    return completion
+
+
+def get_completion_starchat_nl_to_pl(prompt, user_input, model, tokenizer, args):
+    # select the correct in-context learning prompt based on the task
+    messages = prompt + [{"role": "user", "content": user_input}]
+    try:
+        dialogue_template = DialogueTemplate.from_pretrained(args.model_name_or_path)
+    except Exception:
+        print("No dialogue template found in model repo. Defaulting to the `no_system` template.")
+        dialogue_template = get_dialogue_template("no_system")
+    dialogue_template.messages = messages
+    formatted_prompt = dialogue_template.get_inference_prompt_nl_to_pl()
+
+    # DEBUG
+    # print(formatted_prompt)
+    # get completion from code lm
+    output = generate_text(
+        model,
+        tokenizer,
+        formatted_prompt,
+        args,
+        eos_token_id=tokenizer.convert_tokens_to_ids(dialogue_template.end_token),
+    )
+    completion = output[0]["generated_text"]
+
+    # post-processing
+    processed_completion = post_processing_nl_to_pl(completion)
+    return processed_completion
+
+
+def get_completion_starchat_pl_to_nl(prompt, user_input, model, tokenizer, args):
+    # select the correct in-context learning prompt based on the task
+    messages = prompt + [{"role": "user", "content": user_input}]
+    try:
+        dialogue_template = DialogueTemplate.from_pretrained(args.model_name_or_path)
+    except Exception:
+        print("No dialogue template found in model repo. Defaulting to the `no_system` template.")
+        dialogue_template = get_dialogue_template("no_system")
+    dialogue_template.messages = messages
+    formatted_prompt = dialogue_template.get_inference_prompt_pl_to_nl()
+
+    # DEBUG
+    # print(formatted_prompt)
+    # get completion from code lm
+    output = generate_text(
+        model,
+        tokenizer,
+        formatted_prompt,
+        args,
+        eos_token_id=tokenizer.convert_tokens_to_ids(dialogue_template.end_token),
+    )
+    completion = output[0]["generated_text"]
+
+    # post-processing
+    processed_completion = post_processing_pl_to_nl(completion)
+    return processed_completion
+
+
+def get_completion_codellama_instruct_nl_to_pl(
+    prompt, user_input, model, tokenizer, args
+):  # reference: https://github.com/facebookresearch/codellama/blob/main/llama/generation.py
+    # select the correct in-context learning prompt based on the task
+    messages = prompt + [{"role": "user", "content": user_input}]
+    formatted_prompt = ""
+    for msg in messages:
+        if msg["role"] == "user":
+            content = msg["content"].strip()
+            formatted_prompt += tokenizer.bos_token + f"{B_INST_CLLAMA} " + content + f" {E_INST_CLLAMA} "
+        elif msg["role"] == "assistant":
+            formatted_prompt += " " + msg["content"].strip() + " " + tokenizer.eos_token
+        # system prompt doesn't work well for Code Llama-Instructs
+        # elif msg["role"] == "system":
+        #     formatted_prompt += f"{B_SYS_CLLAMA}" + msg["content"] + f"{E_SYS_CLLAMA}"
+
+    # DEBUG
+    # print(formatted_prompt)
+    output = generate_text(model, tokenizer, formatted_prompt, args)
+    completion = output[0]["generated_text"]
+
+    # post-processing
+    processed_completion = post_processing_nl_to_pl(completion)
+    return processed_completion
+
+
+def get_completion_codellama_instruct_pl_to_nl(prompt, user_input, model, tokenizer, args):
+    # select the correct in-context learning prompt based on the task
+    messages = prompt + [{"role": "user", "content": user_input}]
+    formatted_prompt = ""
+    for msg in messages:
+        if msg["role"] == "user":
+            if args.input_path.endswith("EvalPlus-Mini-v0.1.6_reformatted.jsonl"):
+                content = (
+                    msg["content"]
+                    + "\n\nWhat should be the docstring of the above function? Please only write down the docstring with some examples."
+                )
+            elif args.input_path.endswith("MBPP-S_test_reformatted.jsonl"):
+                content = (
+                    msg["content"]
+                    + "\n\nWhat should be the docstring of the above function? Please write down the docstring only in words without any examples!"
+                )
+            else:
+                raise ValueError(f"Input file {args.input_path} not supported")
+            formatted_prompt += tokenizer.bos_token + "[INST] " + content + " [/INST] "
+        elif msg["role"] == "assistant":
+            formatted_prompt += " " + msg["content"].strip() + " " + tokenizer.eos_token
+    # DEBUG
+    # print(formatted_prompt)
+    output = generate_text(model, tokenizer, formatted_prompt, args)
+    completion = output[0]["generated_text"]
+
+    # post-processing
+    processed_completion = post_processing_pl_to_nl(completion)
+    return processed_completion
+
+
+def get_completion_deepseek_instruct_nl_to_pl(
+    prompt, user_input, model, tokenizer, args
+):  # reference: https://github.com/deepseek-ai/DeepSeek-Coder/blob/main/README.md
+    # select the correct in-context learning prompt based on the task
+    # remove the last system prompt
+    messages = prompt[:-1] + [{"role": "user", "content": user_input}]
+
+    input_ids = tokenizer.apply_chat_template(messages, add_generation_prompt=True, return_tensors="pt").to(
+        model.device
+    )
+    print("Generating Text...")
+    generated_sequence = model.generate(
+        input_ids=input_ids,
+        max_length=args.seq_length,
+        do_sample=args.do_sample,
+        num_beams=args.num_beams,
+        temperature=args.temperature,
+        top_k=args.top_k,
+        top_p=args.top_p,
+        num_return_sequences=args.num_return_sequences,
+        pad_token_id=tokenizer.pad_token_id,
+        eos_token_id=tokenizer.eos_token_id,
+    )
+    print("Decoding Text...")
+    completion = tokenizer.decode(generated_sequence[0][len(input_ids[0]) :], skip_special_tokens=True)
+
+    # post-processing
+    processed_completion = post_processing_nl_to_pl(completion)
+    return processed_completion
+
+
+def get_completion_deepseek_instruct_pl_to_nl(
+    prompt, user_input, model, tokenizer, args
+):  # reference: https://github.com/deepseek-ai/DeepSeek-Coder/blob/main/README.md
+    # select the correct in-context learning prompt based on the task
+    # remove the last system prompt
+    messages = prompt[:-1] + [{"role": "user", "content": user_input}]
+
+    input_ids = tokenizer.apply_chat_template(messages, add_generation_prompt=True, return_tensors="pt").to(
+        model.device
+    )
+    print("Generating Text...")
+    generated_sequence = model.generate(
+        input_ids=input_ids,
+        max_length=args.seq_length,
+        do_sample=args.do_sample,
+        num_beams=args.num_beams,
+        temperature=args.temperature,
+        top_k=args.top_k,
+        top_p=args.top_p,
+        num_return_sequences=args.num_return_sequences,
+        pad_token_id=tokenizer.pad_token_id,
+        eos_token_id=tokenizer.eos_token_id,
+    )
+    print("Decoding Text...")
+    completion = tokenizer.decode(generated_sequence[0][len(input_ids[0]) :], skip_special_tokens=True)
+
+    # post-processing
+    processed_completion = post_processing_pl_to_nl(completion)
+    return processed_completion
+
+
+def get_completion_codellama(
+    prompt, user_input, model, tokenizer, args
+):  # prompt is ONE_SHOT_HUMANEVAL or ONE_SHOT_MBPP
+    user_input = prompt + user_input
+    output = generate_text(model, tokenizer, user_input, args)
+    completion = output[0]["generated_text"]
+
+    # post-processing
+    processed_completion = post_processing_nl_to_pl(completion)
+    return processed_completion
+
+
+def get_completion_codellama_fim(
+    prompt, function_signature, function_body, model, tokenizer, args
+):  # prompt is ONE_SHOT_FIM_HUMANEVAL or ONE_SHOT_FIM_MBPP
+    return fill_in_middle(
+        prompt=prompt,
+        function_signature=function_signature,
+        function_body=function_body,
+        model=model,
+        tokenizer=tokenizer,
+        args=args,
+        pre_token=" <PRE>",
+        suf_token=" <SUF>",
+        mid_token=" <MID>",
+    )
+
+
+def get_completion_starcoder(
+    prompt, user_input, model, tokenizer, args
+):  # prompt is ONE_SHOT_HUMANEVAL or ONE_SHOT_MBPP
+    user_input = prompt + user_input
+    output = generate_text(model, tokenizer, user_input.strip(), args)
+    completion = output[0]["generated_text"]
+
+    # post-processing
+    processed_completion = post_processing_nl_to_pl(completion)
+    return processed_completion
+
+
+def get_completion_starcoder_fim(
+    prompt, function_signature, function_body, model, tokenizer, args
+):  # prompt is ONE_SHOT_FIM_HUMANEVAL or ONE_SHOT_FIM_MBPP
+    return fill_in_middle(
+        prompt=prompt,
+        function_signature=function_signature,
+        function_body=function_body,
+        model=model,
+        tokenizer=tokenizer,
+        args=args,
+        pre_token="<fim_prefix>",
+        suf_token="<fim_suffix>",
+        mid_token="<fim_middle>",
+    )
+
+
+def get_completion_deepseek(
+    prompt, user_input, model, tokenizer, args
+):  # prompt is ONE_SHOT_HUMANEVAL or ONE_SHOT_MBPP
+    user_input = prompt + user_input
+    output = generate_text(model, tokenizer, user_input.strip(), args)
+    completion = output[0]["generated_text"]
+
+    # post-processing
+    processed_completion = post_processing_nl_to_pl(completion)
+    return processed_completion
+
+
+def get_completion_deepseek_fim(
+    prompt, function_signature, function_body, model, tokenizer, args
+):  # prompt is ONE_SHOT_FIM_HUMANEVAL or ONE_SHOT_FIM_MBPP
+    return fill_in_middle(
+        prompt=prompt,
+        function_signature=function_signature,
+        function_body=function_body,
+        model=model,
+        tokenizer=tokenizer,
+        args=args,
+        pre_token="<｜fim▁begin｜>",
+        suf_token="<｜fim▁hole｜>",
+        mid_token="<｜fim▁end｜>",
+    )
+
+
+# EXAMPLE USAGE:
+# python run_identity_chain_huggingface.py
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--model_name_or_path', type=str, help='Path to the model')
+    parser.add_argument('--hf_dir', type=str, help='Path to the huggingface cache directory')
+    parser.add_argument('--input_path', type=str, help='Path to the input file')
+    parser.add_argument('--output_dir', type=str, help='Path to the output directory')
+    parser.add_argument('--chain_length', type=int, default=5, help='Number of steps in the Identity Chain')
+    parser.add_argument('--seq_length', type=int, default=2048, help='max length of the sequence')
+    parser.add_argument('--gen_length', type=int, default=None, help='max length of the generated sequence')
+    parser.add_argument('--do_sample', action='store_true', help='whether to do sampling')
+    parser.add_argument('--greedy_early_stop', action='store_true', help='whether to stop inference when fixed point')
+    parser.add_argument('--temperature', type=float, default=0, help='temperature for sampling')
+    parser.add_argument('--top_k', type=int, default=0, help='top k for sampling')
+    parser.add_argument('--top_p', type=float, default=1, help='top p for sampling')
+    parser.add_argument('--num_return_sequences', type=int, default=1, help='number of return sequences')
+    parser.add_argument('--num_beams', type=int, default=1, help='number of beams for beam search')
+    parser.add_argument('--use_int8', action='store_true', help='whether to use int8 quantization')
+    parser.add_argument('--use_fp16', action='store_true', help='whether to use fp16 precision')
+    parser.add_argument('--pass_only', action='store_true', help='whether to only pass the input to the next step')
+    parser.add_argument('--mask_func_name', action='store_true', help='whether to mask the function name')
+    parser.add_argument('--bootstrap_method', type=str, default='problem', help='method to bootstrap the chain')
+    parser.add_argument('--resume_task_bs', type=int, default=0, help='task to resume at when bootstrapping')
+    parser.add_argument('--resume_task_run', type=int, default=0, help='task to resume at')
+    parser.add_argument('--skip_bootstrap', action='store_true', help='whether to skip the bootstrap stage')
+    parser.add_argument('--version', type=str, default='v1', help='version of the identity chain')
+    args = parser.parse_args()
+
+    # set huggingface cache directory
+    HF_HOME = args.hf_dir
+    print("Loading model...")
+    # if specified, use int8 quantization
+    if args.use_int8:
+        print("**********************************")
+        print("**** Using 8-bit quantization ****")
+        print("**********************************")
+        model = AutoModelForCausalLM.from_pretrained(
+            args.model_name_or_path,
+            load_in_8bit=True,
+            device_map="auto",
+            cache_dir=HF_HOME,
+        )
+    # if specified, use fp16 precision
+    elif args.use_fp16:
+        print("**********************************")
+        print("****** Using fp16 precision ******")
+        print("**********************************")
+        model = AutoModelForCausalLM.from_pretrained(
+            args.model_name_or_path,
+            device_map="auto",
+            torch_dtype=torch.float16,
+            cache_dir=HF_HOME,
+        )
+    # otherwise, use default precision
+    else:
+        model = AutoModelForCausalLM.from_pretrained(
+            args.model_name_or_path,
+            device_map="auto",
+            cache_dir=HF_HOME,
+        )
+
+    # configure tokenizer
+    tokenizer = AutoTokenizer.from_pretrained(
+        args.model_name_or_path,
+        model_max_length=args.seq_length,
+        padding_side="right",
+        use_fast=False,
+        trust_remote_code=True,
+        cache_dir=HF_HOME,
+    )
+
+    # create output directory if not exists
+    if not os.path.exists("../tmp"):
+        os.makedirs("../tmp", exist_ok=True)
+    if not os.path.exists(args.output_dir):
+        os.makedirs(args.output_dir, exist_ok=True)
+
+    # unzip input file
+    input_path = args.input_path
+    input_file = input_path.split("/")[-1]
+    g_unzip(f"{input_path}.gz", input_path)
+
+    # for output path naming
+    model_name = args.model_name_or_path.split("/")[-1]
+    tmp = args.temperature
+    len = args.chain_length
+    bootstrap = "pb" if args.bootstrap_method == "problem" else "cb"
+    pass_only = "po" if args.pass_only else "all"
+    mask_name = "m" if args.mask_func_name else "um"
+    greedy = "g" if args.greedy_early_stop else ""
+    version = args.version
+
+    # define the output path
+    output_path = f"{args.output_dir}/IDChain_{model_name}_tmp{tmp}{greedy}_len{len}_{bootstrap}_{pass_only}_{mask_name}_{version}_{input_file}"
+
+    # configure nl_2_pl/pl_2_nl functions based on the model
+    # configure functions for starchat-beta
+    if args.model_name_or_path == "HuggingFaceH4/starchat-beta":
+        nl_2_pl_function = get_completion_starchat_nl_to_pl
+        pl_2_nl_function = get_completion_starchat_pl_to_nl
+    # configure functions for starcoder completion models
+    elif args.model_name_or_path.startswith("bigcode/starcoder"):
+        nl_2_pl_function = get_completion_starcoder
+        pl_2_nl_function = get_completion_starcoder_fim
+    # configure functions for codellama models
+    elif "CodeLlama" in args.model_name_or_path:
+        # configure functions for codellama-instruct chat models
+        if "Instruct" in args.model_name_or_path:
+            nl_2_pl_function = get_completion_codellama_instruct_nl_to_pl
+            pl_2_nl_function = get_completion_codellama_instruct_pl_to_nl
+        # configure functions for codellama completion models
+        else:
+            nl_2_pl_function = get_completion_codellama
+            pl_2_nl_function = get_completion_codellama_fim
+    # configure function for deepseekcoder models
+    elif "deepseek-ai" in args.model_name_or_path:
+        # configure functions for deepseekcoder chat models
+        if "instruct" in args.model_name_or_path:
+            nl_2_pl_function = get_completion_deepseek_instruct_nl_to_pl
+            pl_2_nl_function = get_completion_deepseek_instruct_pl_to_nl
+        # configure functions for deepseekcoder completion models
+        else:
+            nl_2_pl_function = get_completion_deepseek
+            pl_2_nl_function = get_completion_deepseek_fim
+    else:
+        raise ValueError(f"Model {args.model_name_or_path} not supported")
+
+    # configure nl_2_pl/pl_2_nl prompts based on the model and input dataset
+    # configure prompts for HumanEvalPlus-Mini-v0.1.6 or v0.1.9
+    if "EvalPlus-Mini" in args.input_path:
+        # configure prompt for supported chat models
+        if args.model_name_or_path in INSTRUCTION_MODELS:
+            nl_2_pl_prompt = NL_2_PL_HUMANEVAL
+            pl_2_nl_prompt = PL_2_NL_HUMANEVAL
+        # configure prompt for supported completion models
+        elif args.model_name_or_path in FOUNDATION_MODELS:
+            # both nl_2_pl and pl_2_nl prompts are the same for completion models
+            nl_2_pl_prompt = ONE_SHOT_HUMANEVAL
+            pl_2_nl_prompt = ONE_SHOT_FIM_HUMANEVAL
+        else:
+            raise ValueError(f"Model {args.model_name_or_path} not supported")
+    # configure prompts for MBPP-S_test
+    elif args.input_path.endswith("MBPP-S_test_reformatted.jsonl"):
+        # configure prompt for supported chat models
+        if args.model_name_or_path in INSTRUCTION_MODELS:
+            nl_2_pl_prompt = NL_2_PL_MBPP
+            pl_2_nl_prompt = PL_2_NL_MBPP
+        # configure prompt for supported completion models
+        elif args.model_name_or_path in FOUNDATION_MODELS:
+            # both nl_2_pl and pl_2_nl prompts are the same for completion models
+            nl_2_pl_prompt = ONE_SHOT_MBPP
+            pl_2_nl_prompt = ONE_SHOT_FIM_MBPP
+        else:
+            raise ValueError(f"Model {args.model_name_or_path} not supported")
+    else:
+        raise ValueError(f"Input file {args.input_path} not supported")
+
+    # for DEBUGging
+    print("--------- Prompt Configuration -----------")
+    print(nl_2_pl_prompt)
+    print(pl_2_nl_prompt)
+    print("-----------------------------------------")
+
+    # create the identity chain
+    my_chain = IdentityChain(
+        model=model,
+        tokenizer=tokenizer,
+        args=args,
+        input_path=input_path,
+        output_path=output_path,
+        get_model_response_NL_to_PL=nl_2_pl_function,
+        get_model_response_PL_to_NL=pl_2_nl_function,
+        prompt_NL_to_PL=nl_2_pl_prompt,
+        prompt_PL_to_NL=pl_2_nl_prompt,
+        bootstrap_method="problem",
+        length=args.chain_length,
+    )
+    print("-----------------------------------------")
+    print(f"Input Path: {input_path}")
+    print(f"Output Path: {output_path}")
+    print("-----------------------------------------")
+    input("Please Confirm the Identity Chain Setup. Press 'Enter' to Continue...")
+
+    # if resume_task_run != 0 or skip_bootstrap == True, then we don't need to bootstrap
+    if (args.resume_task_run == 0) and (not args.skip_bootstrap):
+        my_chain.bootstrap(resume_task=args.resume_task_bs)
+
+    my_chain.run(
+        resume_task=args.resume_task_run,
+        resume_step=1,
+        pass_only=args.pass_only,
+        mask_func_name=args.mask_func_name,
+        greedy_early_stop=args.greedy_early_stop,
+    )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `identitychain-0.0.1/examples/run_identity_chain_openai.py` & `identitychain-0.1.0/examples/run_identity_chain_google.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,291 +1,347 @@
-# Authors: marcusm117
-# License: Apache 2.0
-
-
-# Standard Library Modules
-import argparse
-import os
-import time
-
-# External Modules
-import openai
-
-# Internal Modules
-from identitychain import IdentityChain
-from identitychain.utils import g_unzip
-
-
-# add your OpenAI API key here
-openai.api_key = ""
-
-
-# prompt settings
-NL_2_PL_HUMANEVAL = [
-    {  # Instructions
-        "role": "system",
-        "content": "Solve a coding problem in Python. "
-        + "Given the function signature and the problem description in the docstring, "
-        + "you only need to continue to complete the function body. "
-        + "Please strictly follow the format of the example below! "
-        + "Don't write down any thought processes! "
-        + "Don't copy the problem description! "
-        + "You must use correct indentation! "
-        + "Make sure your return statement is always inside the function! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "Output an indentation of 4 spaces first before you write anything else! "
-        + "You’d better be sure. \n\n",
-    },
-    {  # One-Shot Example: user input = function signature + problem description in docstring format
-        "role": "user",
-        "content": 'from typing import List\n\n\ndef has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
-        + '"""Check if in given list of numbers, are any two numbers closer to each other than\n    given threshold.\n    '
-        + '>>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    '
-        + '>>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    True\n    """\n',
-    },
-    {  # One-Shot Example: model output = solution
-        "role": "assistant",
-        "content": '    sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
-        + 'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n',
-    },
-    {  # Instructions to emphasize the format
-        "role": "system",
-        "content": "\nPlease strictly follow the format of the example above! "
-        + "You must use correct indentation! "
-        + "Make sure your return statement is always inside the function! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "Output an indentation of 4 spaces first before you write anything else! "
-        + "You’d better be sure. \n\n",
-    },
-]
-
-PL_2_NL_HUMANEVAL = [
-    {  # Instructions
-        "role": "system",
-        "content": "Given a Python solution to a coding problem, "
-        + "write an accurate problem description for it in the format of Python docstring without 'Args' and 'Returns'. "
-        + "Please strictly follow the format of the example below!"
-        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
-        + "Make sure to give a few examples of inputs and outputs in the docstring! "
-        + "Make sure the docstring has no 'Args' and no 'Returns'! "
-        + "You can only write a text desciption with a few examples as shown in the example below!  "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "You’d better be sure. \n\n",
-    },
-    {  # One-Shot Example: user input = function signature + candidate solution
-        "role": "user",
-        "content": 'from typing import List\n\n\ndef has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
-        + 'sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
-        + 'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n',
-    },
-    {  # One-Shot Example: model output = problem description in docstring format
-        "role": "assistant",
-        "content": '    """Check if in given list of numbers, are any two numbers closer to each other than\n    '
-        + 'given threshold.\n    >>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    '
-        + '>>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    True\n    """\n',
-    },
-    {  # Instructions to emphasize the format
-        "role": "system",
-        "content": "\nPlease strictly follow the format of the example above! "
-        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
-        + "Make sure to give a few examples of inputs and outputs in the docstring! "
-        + "Make sure the docstring has no 'Args' and no 'Returns'! "
-        + "You can only write a text desciption with a few examples as shown in the example above!  "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "You’d better be sure. \n\n",
-    },
-]
-
-NL_2_PL_MBPP = [
-    {  # Instructions
-        "role": "system",
-        "content": "Solve a coding problem in Python. "
-        + "Given the function signature and the problem description in the docstring, you only need to continue to complete the function body. "
-        + "Please strictly follow the format of the example below! "
-        + "Don't write down any thought processes! "
-        + "Don't copy the problem description! "
-        + "You must use correct indentation! "
-        + "Make sure your return statement is always inside the function! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "Output an indentation of 4 spaces first before you write anything else! "
-        + "You’d better be sure. \n\n",
-    },
-    {  # One-Shot Example: user input = function signature + problem description in docstring format
-        "role": "user",
-        "content": 'def similar_elements(test_tup1, test_tup2):\n    '
-        + '""" Write a function to find the shared elements from the given two lists.\n    """\n',
-    },
-    {  # One-Shot Example: model output = solution
-        "role": "assistant",
-        "content": '    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n',
-    },
-    {  # Instructions to emphasize the format
-        "role": "system",
-        "content": "\nPlease strictly follow the format of the example above! "
-        + "You must use correct indentation! "
-        + "Make sure your return statement is always inside the function! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "Output an indentation of 4 spaces first before you write anything else! "
-        + "You’d better be sure. \n\n",
-    },
-]
-
-PL_2_NL_MBPP = [
-    {  # Instructions
-        "role": "system",
-        "content": "Given a Python solution to a coding problem, write an accurate problem description for it in the format of Python docstring"
-        + "Please strictly follow the format of the example below!"
-        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
-        + "Make sure the docstring has no 'Args', no 'Returns', and no 'Examples'! "
-        + "You can only write a plain text desciption as shown in the example below! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "You’d better be sure. \n\n",
-    },
-    {  # One-Shot Example: user input = function signature + candidate solution
-        "role": "user",
-        "content": 'def similar_elements(test_tup1, test_tup2):\n    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n',
-    },
-    {  # One-Shot Example: model output = problem description in docstring format
-        "role": "assistant",
-        "content": '    """ Write a function to find the shared elements from the given two lists.\n    """\n',
-    },
-    {  # Instructions to emphasize the format
-        "role": "system",
-        "content": "\nPlease strictly follow the format of the example above! "
-        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
-        + "Make sure the docstring has no 'Args', no 'Returns', and no 'Examples'! "
-        + "You can only write a plain text desciption as shown in the example above! "
-        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
-        + "You’d better be sure. \n\n",
-    },
-]
-
-
-# get completion from an OpenAI chat model
-def get_openai_chat(
-    prompt,
-    user_input,
-    model,
-    tokenizer,
-    args,
-):
-    # select the correct in-context learning prompt based on the task
-    messages = prompt + [{"role": "user", "content": user_input}]
-
-    # get response from OpenAI
-    try:
-        response = openai.ChatCompletion.create(
-            model=model,
-            temperature=args.temperature,
-            max_tokens=args.gen_length,
-            messages=messages,
-        )
-        response_content = response["choices"][0]["message"]["content"]
-        # if the API is unstable, consider sleeping for a short period of time after each request
-        # time.sleep(0.2)
-        return response_content
-
-    # when encounter RateLimit or Connection Error, sleep for 5 or specified seconds and try again
-    except (openai.error.RateLimitError, openai.error.Timeout, openai.error.APIConnectionError) as error:
-        retry_time = error.retry_after if hasattr(error, "retry_after") else 5
-        print(f"Rate Limit or Connection Error. Sleeping for {retry_time} seconds ...")
-        time.sleep(retry_time)
-        return get_openai_chat(
-            prompt,
-            user_input,
-            model,
-            tokenizer,
-            args,
-        )
-
-
-# EXAMPLE USAGE:
-# python run_identity_chain_openai.py
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--model_name_or_path', type=str, help='Path to the model')
-    parser.add_argument('--hf_dir', type=str, help='Path to the huggingface cache directory')
-    parser.add_argument('--input_path', type=str, help='Path to the input file')
-    parser.add_argument('--output_dir', type=str, help='Path to the output directory')
-    parser.add_argument('--chain_length', type=int, default=5, help='Number of steps in the Identity Chain')
-    parser.add_argument('--seq_length', type=int, default=2048, help='max length of the sequence')
-    parser.add_argument('--gen_length', type=int, default=None, help='max length of the generated sequence')
-    parser.add_argument('--do_sample', action='store_true', help='whether to do sampling')
-    parser.add_argument('--greedy_early_stop', action='store_true', help='whether to stop inference when fixed point')
-    parser.add_argument('--temperature', type=float, default=0, help='temperature for sampling')
-    parser.add_argument('--top_k', type=int, default=0, help='top k for sampling')
-    parser.add_argument('--top_p', type=float, default=1, help='top p for sampling')
-    parser.add_argument('--num_return_sequences', type=int, default=1, help='number of return sequences')
-    parser.add_argument('--num_beams', type=int, default=1, help='number of beams for beam search')
-    parser.add_argument('--use_int8', action='store_true', help='whether to use int8 quantization')
-    parser.add_argument('--use_fp16', action='store_true', help='whether to use fp16 precision')
-    parser.add_argument('--pass_only', action='store_true', help='whether to only pass the input to the next step')
-    parser.add_argument('--mask_func_name', action='store_true', help='whether to mask the function name')
-    parser.add_argument('--bootstrap_method', type=str, default='problem', help='method to bootstrap the chain')
-    parser.add_argument('--resume_task_bs', type=int, default=0, help='task to resume at when bootstrapping')
-    parser.add_argument('--resume_task_run', type=int, default=0, help='task to resume at')
-    parser.add_argument('--skip_bootstrap', action='store_true', help='whether to skip the bootstrap stage')
-    parser.add_argument('--version', type=str, default='v1', help='version of the identity chain')
-    args = parser.parse_args()
-
-    # create output directory if not exists
-    if not os.path.exists("../tmp"):
-        os.makedirs("../tmp", exist_ok=True)
-    if not os.path.exists(args.output_dir):
-        os.makedirs(args.output_dir, exist_ok=True)
-
-    # unzip input file
-    input_path = args.input_path
-    input_file = input_path.split("/")[-1]
-    g_unzip(f"../data/{input_file}.gz", input_path)
-
-    # for output path naming
-    model_name = args.model_name_or_path.split("/")[-1]
-    tmp = args.temperature
-    len = args.chain_length
-    bootstrap = "pb" if args.bootstrap_method == "problem" else "cb"
-    pass_only = "po" if args.pass_only else "all"
-    mask_name = "m" if args.mask_func_name else "um"
-    greedy = "g" if args.greedy_early_stop else ""
-    version = args.version
-
-    # define the output path
-    output_path = f"{args.output_dir}/IDChain_{model_name}_tmp{tmp}{greedy}_len{len}_{bootstrap}_{pass_only}_{mask_name}_{version}_{input_file}"
-
-    # create an Identity Chain
-    my_chain = IdentityChain(
-        model=args.model_name_or_path,
-        tokenizer=None,
-        args=args,
-        input_path=input_path,
-        output_path=output_path,
-        get_model_response_NL_to_PL=get_openai_chat,
-        get_model_response_PL_to_NL=get_openai_chat,
-        prompt_NL_to_PL=NL_2_PL_HUMANEVAL,
-        prompt_PL_to_NL=PL_2_NL_HUMANEVAL,
-        bootstrap_method=args.bootstrap_method,
-        length=args.chain_length,
-    )
-    print("-----------------------------------------")
-    print(f"Input Path: {input_path}")
-    print(f"Output Path: {output_path}")
-    print("-----------------------------------------")
-    input("Please Confirm the Identity Chain Setup. Press 'Enter' to Continue...")
-
-    # uncomment the code below to bootstrap the chain
-    # if resume_task_run != 0 or skip_bootstrap == True, then we don't need to bootstrap
-    if (args.resume_task_run == 0) and (not args.skip_bootstrap):
-        my_chain.bootstrap(resume_task=args.resume_task_bs)
-
-    # if you already have a bootstraped chain, ignore the line above
-    # the following line will resume the chain from your specified task and step
-    my_chain.run(
-        resume_task=args.resume_task_run,
-        resume_step=1,
-        pass_only=args.pass_only,
-        mask_func_name=args.mask_func_name,
-        greedy_early_stop=args.greedy_early_stop,
-    )
-
-
-if __name__ == "__main__":
-    main()
+# Authors: marcusm117
+# License: Apache 2.0
+
+
+# Standard Library Modules
+import argparse
+import os
+import time
+
+# External Modules
+import google.generativeai as genai
+
+# Internal Modules
+from identitychain import IdentityChain
+from identitychain.utils import g_unzip
+
+
+# add your OpenAI API key here
+genai.configure(api_key="YOUR_API_KEY")
+
+
+# prompt settings
+NL_2_PL_HUMANEVAL = [
+    {  # Instructions
+        "role": "system",
+        "content": "Solve a coding problem in Python. "
+        + "Given the function signature and the problem description in the docstring, "
+        + "you only need to continue to complete the function body. "
+        + "Please strictly follow the format of the example below! "
+        + "Don't write down any thought processes! "
+        + "Don't copy the problem description! "
+        + "You must use correct indentation! "
+        + "Make sure your return statement is always inside the function! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "Output an indentation of 4 spaces first before you write anything else! "
+        + "You’d better be sure. \n\n",
+    },
+    {  # One-Shot Example: user input = function signature + problem description in docstring format
+        "role": "user",
+        "content": 'from typing import List\n\n\ndef has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
+        + '"""Check if in given list of numbers, are any two numbers closer to each other than\n    given threshold.\n    '
+        + '>>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    '
+        + '>>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    True\n    """\n',
+    },
+    {  # One-Shot Example: model output = solution
+        "role": "assistant",
+        "content": '    sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
+        + 'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n',
+    },
+    {  # Instructions to emphasize the format
+        "role": "system",
+        "content": "\nPlease strictly follow the format of the example above! "
+        + "You must use correct indentation! "
+        + "Make sure your return statement is always inside the function! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "Output an indentation of 4 spaces first before you write anything else! "
+        + "You’d better be sure. \n\n",
+    },
+]
+
+PL_2_NL_HUMANEVAL = [
+    {  # Instructions
+        "role": "system",
+        "content": "Given a Python solution to a coding problem, "
+        + "write an accurate problem description for it in the format of Python docstring without 'Args' and 'Returns'. "
+        + "Please strictly follow the format of the example below!"
+        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
+        + "Make sure to give a few examples of inputs and outputs in the docstring! "
+        + "Make sure the docstring has no 'Args' and no 'Returns'! "
+        + "You can only write a text desciption with a few examples as shown in the example below!  "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "You’d better be sure. \n\n",
+    },
+    {  # One-Shot Example: user input = function signature + candidate solution
+        "role": "user",
+        "content": 'from typing import List\n\n\ndef has_close_elements(numbers: List[float], threshold: float) -> bool:\n    '
+        + 'sorted_numbers = sorted(numbers)\n    for i in range(len(sorted_numbers) - 1):\n        '
+        + 'if sorted_numbers[i + 1] - sorted_numbers[i] < threshold:\n            return True\n    return False\n\n',
+    },
+    {  # One-Shot Example: model output = problem description in docstring format
+        "role": "assistant",
+        "content": '    """Check if in given list of numbers, are any two numbers closer to each other than\n    '
+        + 'given threshold.\n    >>> has_close_elements([1.0, 2.0, 3.0], 0.5)\n    False\n    '
+        + '>>> has_close_elements([1.0, 2.8, 3.0, 4.0, 5.0, 2.0], 0.3)\n    True\n    """\n',
+    },
+    {  # Instructions to emphasize the format
+        "role": "system",
+        "content": "\nPlease strictly follow the format of the example above! "
+        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
+        + "Make sure to give a few examples of inputs and outputs in the docstring! "
+        + "Make sure the docstring has no 'Args' and no 'Returns'! "
+        + "You can only write a text desciption with a few examples as shown in the example above!  "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "You’d better be sure. \n\n",
+    },
+]
+
+NL_2_PL_MBPP = [
+    {  # Instructions
+        "role": "system",
+        "content": "Solve a coding problem in Python. "
+        + "Given the function signature and the problem description in the docstring, you only need to continue to complete the function body. "
+        + "Please strictly follow the format of the example below! "
+        + "Don't write down any thought processes! "
+        + "Don't copy the problem description! "
+        + "You must use correct indentation! "
+        + "Make sure your return statement is always inside the function! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "Output an indentation of 4 spaces first before you write anything else! "
+        + "You’d better be sure. \n\n",
+    },
+    {  # One-Shot Example: user input = function signature + problem description in docstring format
+        "role": "user",
+        "content": 'def similar_elements(test_tup1, test_tup2):\n    '
+        + '""" Write a function to find the shared elements from the given two lists.\n    """\n',
+    },
+    {  # One-Shot Example: model output = solution
+        "role": "assistant",
+        "content": '    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n',
+    },
+    {  # Instructions to emphasize the format
+        "role": "system",
+        "content": "\nPlease strictly follow the format of the example above! "
+        + "You must use correct indentation! "
+        + "Make sure your return statement is always inside the function! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "Output an indentation of 4 spaces first before you write anything else! "
+        + "You’d better be sure. \n\n",
+    },
+]
+
+PL_2_NL_MBPP = [
+    {  # Instructions
+        "role": "system",
+        "content": "Given a Python solution to a coding problem, write an accurate problem description for it in the format of Python docstring"
+        + "Please strictly follow the format of the example below!"
+        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
+        + "Make sure the docstring has no 'Args', no 'Returns', and no 'Examples'! "
+        + "You can only write a plain text desciption as shown in the example below! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "You’d better be sure. \n\n",
+    },
+    {  # One-Shot Example: user input = function signature + candidate solution
+        "role": "user",
+        "content": 'def similar_elements(test_tup1, test_tup2):\n    res = tuple(set(test_tup1) & set(test_tup2))\n    return (res)\n\n',
+    },
+    {  # One-Shot Example: model output = problem description in docstring format
+        "role": "assistant",
+        "content": '    """ Write a function to find the shared elements from the given two lists.\n    """\n',
+    },
+    {  # Instructions to emphasize the format
+        "role": "system",
+        "content": "\nPlease strictly follow the format of the example above! "
+        + "Provide all necessary details to accurately describe the problem, but in a concise way! "
+        + "Make sure the docstring has no 'Args', no 'Returns', and no 'Examples'! "
+        + "You can only write a plain text desciption as shown in the example above! "
+        + "Make sure your output always starts with an indentation of exactly 4 spaces! "
+        + "You’d better be sure. \n\n",
+    },
+]
+
+
+# convert the structured prompts to strings
+NL_2_PL_HUMANEVAL_STR = (
+    NL_2_PL_HUMANEVAL[0]["content"]
+    + "User Input:\n"
+    + NL_2_PL_HUMANEVAL[1]["content"]
+    + "Your Output:\n"
+    + NL_2_PL_HUMANEVAL[2]["content"]
+    + NL_2_PL_HUMANEVAL[3]["content"]
+)
+
+PL_2_NL_HUMANEVAL_STR = (
+    PL_2_NL_HUMANEVAL[0]["content"]
+    + "User Input:\n"
+    + PL_2_NL_HUMANEVAL[1]["content"]
+    + "Your Output:\n"
+    + PL_2_NL_HUMANEVAL[2]["content"]
+    + PL_2_NL_HUMANEVAL[3]["content"]
+)
+
+NL_2_PL_MBPP_STR = (
+    NL_2_PL_MBPP[0]["content"]
+    + "User Input:\n"
+    + NL_2_PL_MBPP[1]["content"]
+    + "Your Output:\n"
+    + NL_2_PL_MBPP[2]["content"]
+    + NL_2_PL_MBPP[3]["content"]
+)
+
+PL_2_NL_MBPP_STR = (
+    PL_2_NL_MBPP[0]["content"]
+    + "User Input:\n"
+    + PL_2_NL_MBPP[1]["content"]
+    + "Your Output:\n"
+    + PL_2_NL_MBPP[2]["content"]
+    + PL_2_NL_MBPP[3]["content"]
+)
+
+
+# get completion from a Google model
+def get_google_model_chat(
+    prompt,
+    user_input,
+    model,
+    tokenizer,
+    args,
+):
+    # select the correct in-context learning prompt based on the task
+    messages = prompt + user_input
+
+    # get response from OpenAI
+    try:
+        # get the response
+        response = model.generate_content(messages)
+        # print(response.candidates)
+        # extract the response text content
+        response_content = response.candidates[0].content.parts[0].text
+        # if the API is unstable, consider sleeping for a short period of time after each request
+        time.sleep(0.5)
+        return response_content
+
+    # when encounter APIError, sleep for 5 or specified seconds and try again
+    except Exception as error:
+        retry_time = error.retry_after if hasattr(error, "retry_after") else 5
+        print(f"{error}. Sleeping for {retry_time} seconds ...")
+        time.sleep(retry_time)
+        return get_google_model_chat(prompt, user_input, model, tokenizer, args)
+
+
+# EXAMPLE USAGE:
+# python run_identity_chain_google.py
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--model_name_or_path', type=str, help='Path to the model')
+    parser.add_argument('--hf_dir', type=str, help='Path to the huggingface cache directory')
+    parser.add_argument('--input_path', type=str, help='Path to the input file')
+    parser.add_argument('--output_dir', type=str, help='Path to the output directory')
+    parser.add_argument('--chain_length', type=int, default=5, help='Number of steps in the Identity Chain')
+    parser.add_argument('--seq_length', type=int, default=2048, help='max length of the sequence')
+    parser.add_argument('--gen_length', type=int, default=None, help='max length of the generated sequence')
+    parser.add_argument('--do_sample', action='store_true', help='whether to do sampling')
+    parser.add_argument('--greedy_early_stop', action='store_true', help='whether to stop inference when fixed point')
+    parser.add_argument('--temperature', type=float, default=0, help='temperature for sampling')
+    parser.add_argument('--top_k', type=int, default=0, help='top k for sampling')
+    parser.add_argument('--top_p', type=float, default=1, help='top p for sampling')
+    parser.add_argument('--num_return_sequences', type=int, default=1, help='number of return sequences')
+    parser.add_argument('--num_beams', type=int, default=1, help='number of beams for beam search')
+    parser.add_argument('--use_int8', action='store_true', help='whether to use int8 quantization')
+    parser.add_argument('--use_fp16', action='store_true', help='whether to use fp16 precision')
+    parser.add_argument('--pass_only', action='store_true', help='whether to only pass the input to the next step')
+    parser.add_argument('--mask_func_name', action='store_true', help='whether to mask the function name')
+    parser.add_argument('--bootstrap_method', type=str, default='problem', help='method to bootstrap the chain')
+    parser.add_argument('--resume_task_bs', type=int, default=0, help='task to resume at when bootstrapping')
+    parser.add_argument('--resume_task_run', type=int, default=0, help='task to resume at')
+    parser.add_argument('--skip_bootstrap', action='store_true', help='whether to skip the bootstrap stage')
+    parser.add_argument('--version', type=str, default='v1', help='version of the identity chain')
+    args = parser.parse_args()
+
+    # create output directory if not exists
+    if not os.path.exists("../tmp"):
+        os.makedirs("../tmp", exist_ok=True)
+    if not os.path.exists(args.output_dir):
+        os.makedirs(args.output_dir, exist_ok=True)
+
+    # unzip input file
+    input_path = args.input_path
+    input_file = input_path.split("/")[-1]
+    g_unzip(f"{input_path}.gz", input_path)
+
+    # for output path naming
+    model_name = args.model_name_or_path.split("/")[-1]
+    tmp = args.temperature
+    len = args.chain_length
+    bootstrap = "pb" if args.bootstrap_method == "problem" else "cb"
+    pass_only = "po" if args.pass_only else "all"
+    mask_name = "m" if args.mask_func_name else "um"
+    greedy = "g" if args.greedy_early_stop else ""
+    version = args.version
+
+    # define the output path
+    output_path = f"{args.output_dir}/IDChain_{model_name}_tmp{tmp}{greedy}_len{len}_{bootstrap}_{pass_only}_{mask_name}_{version}_{input_file}"
+
+    # configure prompts for HumanEvalPlus-Mini-v0.1.6
+    if args.input_path.endswith("EvalPlus-Mini-v0.1.6_reformatted.jsonl"):
+        nl_2_pl_prompt = NL_2_PL_HUMANEVAL_STR
+        pl_2_nl_prompt = PL_2_NL_HUMANEVAL_STR
+    # configure prompts for MBPP-S_test
+    elif args.input_path.endswith("MBPP-S_test_reformatted.jsonl"):
+        nl_2_pl_prompt = NL_2_PL_MBPP_STR
+        pl_2_nl_prompt = PL_2_NL_MBPP_STR
+    else:
+        raise ValueError(f"Input file {args.input_path} not supported")
+
+    # for debugging
+    print("--------- Prompt Configuration -----------")
+    print(nl_2_pl_prompt)
+    print(pl_2_nl_prompt)
+    print("-----------------------------------------")
+
+    # create generation config
+    generation_config = genai.GenerationConfig(
+        candidate_count=1,
+        max_output_tokens=args.gen_length,
+        temperature=args.temperature,
+    )
+    # creat the model object
+    model_obj = genai.GenerativeModel(args.model_name_or_path, generation_config=generation_config)
+
+    # create an Identity Chain
+    my_chain = IdentityChain(
+        model=model_obj,
+        tokenizer=None,
+        args=args,
+        input_path=input_path,
+        output_path=output_path,
+        get_model_response_NL_to_PL=get_google_model_chat,
+        get_model_response_PL_to_NL=get_google_model_chat,
+        prompt_NL_to_PL=nl_2_pl_prompt,
+        prompt_PL_to_NL=pl_2_nl_prompt,
+        bootstrap_method=args.bootstrap_method,
+        length=args.chain_length,
+    )
+    print("-----------------------------------------")
+    print(f"Input Path: {input_path}")
+    print(f"Output Path: {output_path}")
+    print("-----------------------------------------")
+    input("Please Confirm the Identity Chain Setup. Press 'Enter' to Continue...")
+
+    # uncomment the code below to bootstrap the chain
+    # if resume_task_run != 0 or skip_bootstrap == True, then we don't need to bootstrap
+    if (args.resume_task_run == 0) and (not args.skip_bootstrap):
+        my_chain.bootstrap(resume_task=args.resume_task_bs)
+
+    # if you already have a bootstraped chain, ignore the line above
+    # the following line will resume the chain from your specified task and step
+    my_chain.run(
+        resume_task=args.resume_task_run,
+        resume_step=1,
+        pass_only=args.pass_only,
+        mask_func_name=args.mask_func_name,
+        greedy_early_stop=args.greedy_early_stop,
+    )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `identitychain-0.0.1/identitychain/dialogue.py` & `identitychain-0.1.0/identitychain/dialogue.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,263 +1,263 @@
-# Authors: Robin-Y-Ding, marcusm117
-# License: Apache 2.0
-
-
-# Standard Library Modules
-from dataclasses import asdict, dataclass
-import json
-import os
-from pathlib import Path
-from typing import Any, Dict, List, Optional, Type, TypeVar, Union
-
-# External Modules
-from huggingface_hub import ModelHubMixin, hf_hub_download
-
-
-# Generic variable that is either ModelHubMixin or a subclass thereof
-T = TypeVar("T", bound="ModelHubMixin")
-
-TEMPLATE_FILENAME = "dialogue_template.json"
-IGNORE_INDEX = -100
-
-B_INST_CLLAMA, E_INST_CLLAMA = "[INST]", "[/INST]"
-B_SYS_CLLAMA, E_SYS_CLLAMA = "<<SYS>>\n", "\n<</SYS>>\n\n"
-
-
-@dataclass
-class DialogueTemplate(ModelHubMixin):
-    """Converts all turns of a dialogue between a user and assistant to a standardized format.
-
-    Adapted from OpenAI's ChatML (https://github.com/openai/openai-python/blob/main/chatml.md) and
-    Vicuna (https://github.com/lm-sys/FastChat/blob/main/fastchat/conversation.py)
-    """
-
-    system: str
-    messages: List[Dict[str, str]] = None
-    system_token: str = "<|system|>"
-    user_token: str = "<|user|>"
-    assistant_token: str = "<|assistant|>"
-    end_token: str = "<|end|>"
-
-    def get_inference_prompt_nl_to_pl(self) -> str:
-        prompt = ""
-        if self.messages is None:
-            raise ValueError("Dialogue template must have at least one message.")
-        for message in self.messages:
-            if message["role"] == "user":
-                content = message["content"] + "\n" if not message["content"].endswith("\n") else message["content"]
-                # content = message["content"] + "\n\nWhat should be the function body of the above prompt?
-                # Please only write down the function body starting with exactly four spaces.\n\n"
-                prompt += self.user_token + "\n" + content + self.end_token + "\n"
-            elif message["role"] == "assistant":
-                content = message["content"] + "\n" if not message["content"].endswith("\n") else message["content"]
-                prompt += self.assistant_token + "\n" + content + self.end_token + "\n"
-            # elif message["role"] == "system":
-            #     prompt += self.system_token + "\n" + message["content"] + self.end_token + "\n"
-            # else:
-            #     raise ValueError(f"Invalid role {message['role']}")
-        # Add a final system token to indicate the end of the dialogue
-        prompt += self.assistant_token
-        return prompt
-
-    def get_inference_prompt_pl_to_nl(self) -> str:
-        prompt = ""
-        if self.messages is None:
-            raise ValueError("Dialogue template must have at least one message.")
-        for message in self.messages:
-            if message["role"] == "user":
-                prompt += (
-                    self.user_token
-                    + "\n"
-                    + message["content"]
-                    + "\n\nWhat should be the docstring of the above function? Please only write down the docstring with some examples.\n\n"
-                    + self.end_token
-                    + "\n"
-                )
-            elif message["role"] == "assistant":
-                content = message["content"]
-                prompt += self.assistant_token + "\n" + content + self.end_token + "\n"
-            # elif message["role"] == "system":
-            #     prompt += self.system_token + "\n" + message["content"] + self.end_token + "\n"
-            # else:
-            #     raise ValueError(f"Invalid role {message['role']}")
-        # Add a final system token to indicate the end of the dialogue
-        prompt += self.assistant_token
-        return prompt
-
-    def get_dialogue(self):
-        """Helper function to format the messages as an easy-to-read dialogue."""
-        prompt = ""
-        if self.messages is None:
-            raise ValueError("Dialogue template must have at least one message.")
-        for message in self.messages:
-            if message["role"] == "user":
-                prompt += "\n\nHuman: " + message["content"]
-            else:
-                prompt += "\n\nAssistant: " + message["content"]
-        return prompt
-
-    def get_special_tokens(self) -> List[str]:
-        return [self.system_token, self.user_token, self.assistant_token, self.end_token]
-
-    def copy(self):
-        return DialogueTemplate(
-            system=self.system,
-            messages=self.messages,
-            system_token=self.system_token,
-            user_token=self.user_token,
-            assistant_token=self.assistant_token,
-            end_token=self.end_token,
-        )
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {k: v for k, v in asdict(self).items()}
-
-    @classmethod
-    def from_dict(cls, data):
-        return DialogueTemplate(
-            system=data["system"] if "system" in data else "",
-            messages=data["messages"] if "messages" in data else None,
-            system_token=data["system_token"] if "system_token" in data else "<|system|>",
-            user_token=data["user_token"] if "user_token" in data else "<|user|>",
-            assistant_token=data["assistant_token"] if "assistant_token" in data else "<|assistant|>",
-            end_token=data["end_token"] if "end_token" in data else "<|end|>",
-        )
-
-    def _save_pretrained(self, save_directory: Union[str, Path]) -> None:
-        save_directory = Path(save_directory)
-        save_directory.mkdir(exist_ok=True)
-        with open(save_directory / "dialogue_template.json", "w") as f:
-            json.dump(self.to_dict(), f, indent=2)
-
-    @classmethod
-    def _from_pretrained(
-        cls: Type[T],
-        *,
-        model_id: str,
-        revision: Optional[str],
-        cache_dir: Optional[Union[str, Path]],
-        force_download: bool,
-        proxies: Optional[Dict],
-        resume_download: bool,
-        local_files_only: bool,
-        token: Optional[Union[str, bool]],
-        **model_kwargs,
-    ) -> T:
-        """Loads the dialogue template from a local directory or the Huggingface Hub.
-
-        Args:
-            model_id (`str`):
-                ID of the model to load from the Huggingface Hub (e.g. `bigscience/bloom`).
-            revision (`str`, *optional*):
-                Revision of the model on the Hub. Can be a branch name, a git tag or any commit id. Defaults to the
-                latest commit on `main` branch.
-            force_download (`bool`, *optional*, defaults to `False`):
-                Whether to force (re-)downloading the model weights and configuration files from the Hub, overriding
-                the existing cache.
-            resume_download (`bool`, *optional*, defaults to `False`):
-                Whether to delete incompletely received files. Will attempt to resume the download if such a file exists.
-            proxies (`Dict[str, str]`, *optional*):
-                A dictionary of proxy servers to use by protocol or endpoint (e.g., `{'http': 'foo.bar:3128',
-                'http://hostname': 'foo.bar:4012'}`).
-            token (`str` or `bool`, *optional*):
-                The token to use as HTTP bearer authorization for remote files. By default, it will use the token
-                cached when running `huggingface-cli login`.
-            cache_dir (`str`, `Path`, *optional*):
-                Path to the folder where cached files are stored.
-            local_files_only (`bool`, *optional*, defaults to `False`):
-                If `True`, avoid downloading the file and return the path to the local cached file if it exists.
-            model_kwargs:
-                Additional keyword arguments passed along to the [`~ModelHubMixin._from_pretrained`] method.
-        """
-        if os.path.isdir(model_id):  # Can either be a local directory
-            print("Loading dialogue template from local directory")
-            template_file = os.path.join(model_id, TEMPLATE_FILENAME)
-        else:  # Or a template on the Hub
-            template_file = hf_hub_download(  # Download from the hub, passing same input args
-                repo_id=model_id,
-                filename=TEMPLATE_FILENAME,
-                revision=revision,
-                cache_dir=cache_dir,
-                force_download=force_download,
-                proxies=proxies,
-                resume_download=resume_download,
-                token=token,
-                local_files_only=local_files_only,
-            )
-
-        # Load template
-        with open(template_file, "r") as f:
-            data = json.load(f)
-        return cls.from_dict(data=data)
-
-
-# A shortened version of the system message in Anthropic's HHH prompt:
-# https://gist.github.com/jareddk/2509330f8ef3d787fc5aaac67aab5f11#file-hhh_prompt-txt
-default_template = DialogueTemplate(
-    system="Below is a dialogue between a human user and an AI assistant. "
-    + "The assistant is happy to help with almost anything, and will do its best to understand exactly what is needed.",
-)
-
-# OpenAI and OpenAssistant train on few to no system messages.
-# TODO: consider defining this as the `default` template
-no_system_template = DialogueTemplate(
-    system="",
-)
-
-alpaca_template = DialogueTemplate(
-    system="Below is an instruction that describes a task. Write a response that appropriately completes the request.",
-    user_token="### Instruction:",
-    assistant_token="### Response:",
-)
-
-SUPPORTED_DIALOGUE_TEMPLATES = {
-    "default": default_template,
-    "no_system": no_system_template,
-    "alpaca": alpaca_template,
-}
-
-
-def get_dialogue_template(template: str) -> DialogueTemplate:
-    if template not in SUPPORTED_DIALOGUE_TEMPLATES.keys():
-        raise ValueError(f"Template {template} is not supported!")
-    return SUPPORTED_DIALOGUE_TEMPLATES[template].copy()
-
-
-def prepare_dialogue(example, dialogue_template, is_train=True):
-    """Format example to single- or multi-turn dialogue."""
-    # TODO: make this simpler by just ensuring every dataset has a messages column
-    if "messages" in example.keys() and example["messages"] is not None:
-        dialogue_template.messages = example["messages"]
-    elif all(k in example.keys() for k in ("prompt", "completion")):
-        # Construct single-turn dialogue from prompt and completion
-        dialogue_template.messages = [
-            {"role": "user", "content": example["prompt"]},
-            {"role": "assistant", "content": example["completion"]},
-        ]
-    elif "prompt" in example.keys():
-        # Construct single-turn dialogue from prompt (inference only)
-        dialogue_template.messages = [
-            {"role": "user", "content": example["prompt"]},
-        ]
-    else:
-        raise ValueError(
-            "Could not format example as dialogue! "
-            + f"Require either `messages` or `[prompt, completion]` or `[prompt]` keys but found {list(example.keys())}"
-        )
-    if is_train:
-        example["text"] = dialogue_template.get_training_prompt()
-    else:
-        example["text"] = dialogue_template.get_inference_prompt()
-    return example
-
-
-def mask_user_labels(tokenizer, dialogue_template, labels):
-    """Masks the user turns of a dialogue from the loss"""
-    user_token_id = tokenizer.convert_tokens_to_ids(dialogue_template.user_token)
-    assistant_token_id = tokenizer.convert_tokens_to_ids(dialogue_template.assistant_token)
-    for idx, label_id in enumerate(labels):
-        if label_id == user_token_id:
-            current_idx = idx
-            while labels[current_idx] != assistant_token_id and current_idx < len(labels):
-                labels[current_idx] = IGNORE_INDEX
-                current_idx += 1
+# Authors: Robin-Y-Ding, marcusm117
+# License: Apache 2.0
+
+
+# Standard Library Modules
+from dataclasses import asdict, dataclass
+import json
+import os
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
+
+# External Modules
+from huggingface_hub import ModelHubMixin, hf_hub_download
+
+
+# Generic variable that is either ModelHubMixin or a subclass thereof
+T = TypeVar("T", bound="ModelHubMixin")
+
+TEMPLATE_FILENAME = "dialogue_template.json"
+IGNORE_INDEX = -100
+
+B_INST_CLLAMA, E_INST_CLLAMA = "[INST]", "[/INST]"
+B_SYS_CLLAMA, E_SYS_CLLAMA = "<<SYS>>\n", "\n<</SYS>>\n\n"
+
+
+@dataclass
+class DialogueTemplate(ModelHubMixin):
+    """Converts all turns of a dialogue between a user and assistant to a standardized format.
+
+    Adapted from OpenAI's ChatML (https://github.com/openai/openai-python/blob/main/chatml.md) and
+    Vicuna (https://github.com/lm-sys/FastChat/blob/main/fastchat/conversation.py)
+    """
+
+    system: str
+    messages: List[Dict[str, str]] = None
+    system_token: str = "<|system|>"
+    user_token: str = "<|user|>"
+    assistant_token: str = "<|assistant|>"
+    end_token: str = "<|end|>"
+
+    def get_inference_prompt_nl_to_pl(self) -> str:
+        prompt = ""
+        if self.messages is None:
+            raise ValueError("Dialogue template must have at least one message.")
+        for message in self.messages:
+            if message["role"] == "user":
+                content = message["content"] + "\n" if not message["content"].endswith("\n") else message["content"]
+                # content = message["content"] + "\n\nWhat should be the function body of the above prompt?
+                # Please only write down the function body starting with exactly four spaces.\n\n"
+                prompt += self.user_token + "\n" + content + self.end_token + "\n"
+            elif message["role"] == "assistant":
+                content = message["content"] + "\n" if not message["content"].endswith("\n") else message["content"]
+                prompt += self.assistant_token + "\n" + content + self.end_token + "\n"
+            # elif message["role"] == "system":
+            #     prompt += self.system_token + "\n" + message["content"] + self.end_token + "\n"
+            # else:
+            #     raise ValueError(f"Invalid role {message['role']}")
+        # Add a final system token to indicate the end of the dialogue
+        prompt += self.assistant_token
+        return prompt
+
+    def get_inference_prompt_pl_to_nl(self) -> str:
+        prompt = ""
+        if self.messages is None:
+            raise ValueError("Dialogue template must have at least one message.")
+        for message in self.messages:
+            if message["role"] == "user":
+                prompt += (
+                    self.user_token
+                    + "\n"
+                    + message["content"]
+                    + "\n\nWhat should be the docstring of the above function? Please only write down the docstring with some examples.\n\n"
+                    + self.end_token
+                    + "\n"
+                )
+            elif message["role"] == "assistant":
+                content = message["content"]
+                prompt += self.assistant_token + "\n" + content + self.end_token + "\n"
+            # elif message["role"] == "system":
+            #     prompt += self.system_token + "\n" + message["content"] + self.end_token + "\n"
+            # else:
+            #     raise ValueError(f"Invalid role {message['role']}")
+        # Add a final system token to indicate the end of the dialogue
+        prompt += self.assistant_token
+        return prompt
+
+    def get_dialogue(self):
+        """Helper function to format the messages as an easy-to-read dialogue."""
+        prompt = ""
+        if self.messages is None:
+            raise ValueError("Dialogue template must have at least one message.")
+        for message in self.messages:
+            if message["role"] == "user":
+                prompt += "\n\nHuman: " + message["content"]
+            else:
+                prompt += "\n\nAssistant: " + message["content"]
+        return prompt
+
+    def get_special_tokens(self) -> List[str]:
+        return [self.system_token, self.user_token, self.assistant_token, self.end_token]
+
+    def copy(self):
+        return DialogueTemplate(
+            system=self.system,
+            messages=self.messages,
+            system_token=self.system_token,
+            user_token=self.user_token,
+            assistant_token=self.assistant_token,
+            end_token=self.end_token,
+        )
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {k: v for k, v in asdict(self).items()}
+
+    @classmethod
+    def from_dict(cls, data):
+        return DialogueTemplate(
+            system=data["system"] if "system" in data else "",
+            messages=data["messages"] if "messages" in data else None,
+            system_token=data["system_token"] if "system_token" in data else "<|system|>",
+            user_token=data["user_token"] if "user_token" in data else "<|user|>",
+            assistant_token=data["assistant_token"] if "assistant_token" in data else "<|assistant|>",
+            end_token=data["end_token"] if "end_token" in data else "<|end|>",
+        )
+
+    def _save_pretrained(self, save_directory: Union[str, Path]) -> None:
+        save_directory = Path(save_directory)
+        save_directory.mkdir(exist_ok=True)
+        with open(save_directory / "dialogue_template.json", "w") as f:
+            json.dump(self.to_dict(), f, indent=2)
+
+    @classmethod
+    def _from_pretrained(
+        cls: Type[T],
+        *,
+        model_id: str,
+        revision: Optional[str],
+        cache_dir: Optional[Union[str, Path]],
+        force_download: bool,
+        proxies: Optional[Dict],
+        resume_download: bool,
+        local_files_only: bool,
+        token: Optional[Union[str, bool]],
+        **model_kwargs,
+    ) -> T:
+        """Loads the dialogue template from a local directory or the Huggingface Hub.
+
+        Args:
+            model_id (`str`):
+                ID of the model to load from the Huggingface Hub (e.g. `bigscience/bloom`).
+            revision (`str`, *optional*):
+                Revision of the model on the Hub. Can be a branch name, a git tag or any commit id. Defaults to the
+                latest commit on `main` branch.
+            force_download (`bool`, *optional*, defaults to `False`):
+                Whether to force (re-)downloading the model weights and configuration files from the Hub, overriding
+                the existing cache.
+            resume_download (`bool`, *optional*, defaults to `False`):
+                Whether to delete incompletely received files. Will attempt to resume the download if such a file exists.
+            proxies (`Dict[str, str]`, *optional*):
+                A dictionary of proxy servers to use by protocol or endpoint (e.g., `{'http': 'foo.bar:3128',
+                'http://hostname': 'foo.bar:4012'}`).
+            token (`str` or `bool`, *optional*):
+                The token to use as HTTP bearer authorization for remote files. By default, it will use the token
+                cached when running `huggingface-cli login`.
+            cache_dir (`str`, `Path`, *optional*):
+                Path to the folder where cached files are stored.
+            local_files_only (`bool`, *optional*, defaults to `False`):
+                If `True`, avoid downloading the file and return the path to the local cached file if it exists.
+            model_kwargs:
+                Additional keyword arguments passed along to the [`~ModelHubMixin._from_pretrained`] method.
+        """
+        if os.path.isdir(model_id):  # Can either be a local directory
+            print("Loading dialogue template from local directory")
+            template_file = os.path.join(model_id, TEMPLATE_FILENAME)
+        else:  # Or a template on the Hub
+            template_file = hf_hub_download(  # Download from the hub, passing same input args
+                repo_id=model_id,
+                filename=TEMPLATE_FILENAME,
+                revision=revision,
+                cache_dir=cache_dir,
+                force_download=force_download,
+                proxies=proxies,
+                resume_download=resume_download,
+                token=token,
+                local_files_only=local_files_only,
+            )
+
+        # Load template
+        with open(template_file, "r") as f:
+            data = json.load(f)
+        return cls.from_dict(data=data)
+
+
+# A shortened version of the system message in Anthropic's HHH prompt:
+# https://gist.github.com/jareddk/2509330f8ef3d787fc5aaac67aab5f11#file-hhh_prompt-txt
+default_template = DialogueTemplate(
+    system="Below is a dialogue between a human user and an AI assistant. "
+    + "The assistant is happy to help with almost anything, and will do its best to understand exactly what is needed.",
+)
+
+# OpenAI and OpenAssistant train on few to no system messages.
+# TODO: consider defining this as the `default` template
+no_system_template = DialogueTemplate(
+    system="",
+)
+
+alpaca_template = DialogueTemplate(
+    system="Below is an instruction that describes a task. Write a response that appropriately completes the request.",
+    user_token="### Instruction:",
+    assistant_token="### Response:",
+)
+
+SUPPORTED_DIALOGUE_TEMPLATES = {
+    "default": default_template,
+    "no_system": no_system_template,
+    "alpaca": alpaca_template,
+}
+
+
+def get_dialogue_template(template: str) -> DialogueTemplate:
+    if template not in SUPPORTED_DIALOGUE_TEMPLATES.keys():
+        raise ValueError(f"Template {template} is not supported!")
+    return SUPPORTED_DIALOGUE_TEMPLATES[template].copy()
+
+
+def prepare_dialogue(example, dialogue_template, is_train=True):
+    """Format example to single- or multi-turn dialogue."""
+    # TODO: make this simpler by just ensuring every dataset has a messages column
+    if "messages" in example.keys() and example["messages"] is not None:
+        dialogue_template.messages = example["messages"]
+    elif all(k in example.keys() for k in ("prompt", "completion")):
+        # Construct single-turn dialogue from prompt and completion
+        dialogue_template.messages = [
+            {"role": "user", "content": example["prompt"]},
+            {"role": "assistant", "content": example["completion"]},
+        ]
+    elif "prompt" in example.keys():
+        # Construct single-turn dialogue from prompt (inference only)
+        dialogue_template.messages = [
+            {"role": "user", "content": example["prompt"]},
+        ]
+    else:
+        raise ValueError(
+            "Could not format example as dialogue! "
+            + f"Require either `messages` or `[prompt, completion]` or `[prompt]` keys but found {list(example.keys())}"
+        )
+    if is_train:
+        example["text"] = dialogue_template.get_training_prompt()
+    else:
+        example["text"] = dialogue_template.get_inference_prompt()
+    return example
+
+
+def mask_user_labels(tokenizer, dialogue_template, labels):
+    """Masks the user turns of a dialogue from the loss"""
+    user_token_id = tokenizer.convert_tokens_to_ids(dialogue_template.user_token)
+    assistant_token_id = tokenizer.convert_tokens_to_ids(dialogue_template.assistant_token)
+    for idx, label_id in enumerate(labels):
+        if label_id == user_token_id:
+            current_idx = idx
+            while labels[current_idx] != assistant_token_id and current_idx < len(labels):
+                labels[current_idx] = IGNORE_INDEX
+                current_idx += 1
```

### Comparing `identitychain-0.0.1/identitychain/executor.py` & `identitychain-0.1.0/identitychain/executor.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-# Authors: marcusm117
-# License: Apache 2.0
-
-# Code is adapted from OpenAI's original script
-# https://github.com/openai/human-eval/blob/master/human_eval/execution.py
-# and a patch provided by davide221 in the following issue:
-# https://github.com/openai/human-eval/issues/18
-
-
-from typing import List, Dict, Optional
-import contextlib
-import faulthandler
-import io
-import os
-import platform
-import signal
-import threading
-import tempfile
-
-
-def unsafe_execute(task: Dict, mask_func_name: bool, timeout: float = 0.5) -> List[str]:
-    """Please read the WARNING below! Execute untrusted model-generated code with test cases.
-
-    WARNING from OpenAI's original script:
-    # This program exists to execute untrusted model-generated code. Although
-    # it is highly unlikely that model-generated code will do something overtly
-    # malicious in response to this test suite, model-generated code may act
-    # destructively due to a lack of model capability or alignment.
-    # Users are strongly encouraged to sandbox this evaluation suite so that it
-    # does not perform destructive actions on their host or network. For more
-    # information on how OpenAI sandboxes its code, see the accompanying paper.
-
-    Args:
-        task: a dictionary with keys: prompt, contract, function_name, model_solution, tests, atol
-        mask_func_name: whether the function name is replaced by a generic "func" in the function signature
-        timeout: maximum time to run each test case
-
-    Returns:
-        a list of strings representing the result of each test case
-    """
-    # disable functionalities that can make destructive changes to the test
-    reliability_guard()
-
-    # construct the program to be tested
-    program = "\n" + task["problem"] + task["contract"] + "\n" + task["model_solution"] + "\n\n\n"
-
-    # initialize the results list
-    results = []
-
-    # run program for each test case
-    for test in task["tests"]:
-        # Test Case Format 1: a dict of input and output (HumanEvalPlus-reformatted Style)
-        if isinstance(test, dict):
-            # mask the function name if necessary
-            if mask_func_name:
-                task["function_name"] = "func"
-            # capture the output, will assert it later
-            capture_output = f"test_out = {task['function_name']}({test['input']})"
-            # if atol is not 0, assert using the atol provided
-            if task["atol"]:
-                atol = task["atol"]
-                assertion_stmt = f"\nassert abs(test_out - {test['output']}) <= {atol}" + r", f'outputs {test_out}'"
-            else:
-                # otherwise, assert equality
-                assertion_stmt = f"\nassert test_out == {test['output']}" + r", f'outputs {test_out}'"
-            # concatenate the program with assertion statement
-            program_w_test = program + capture_output + assertion_stmt
-
-        # Test Case Format 2: a string of assertion statement (MBPP Style)
-        elif isinstance(test, str):
-            # mask the function name if necessary
-            if mask_func_name:
-                test = test.replace(task["function_name"], "func")
-            # concatenate the program with test case
-            program_w_test = program + test
-
-        # we currently don't support other formats
-        else:
-            raise ValueError("Invalid Test Case Format!")
-
-        # for debugging, uncomment the following line
-        # print(program_w_test)
-
-        try:
-            exec_globals = {}
-            with swallow_io():
-                # change <time_limit> to <time_limit_windows> if you're on Windows
-                with time_limit(timeout):
-                    # please read the WARNING above in the docstring
-                    exec(program_w_test, exec_globals)
-            results.append("Passed")
-        except TimeoutException:
-            results.append("Time Out")
-        except BaseException as error:
-            results.append(f"{type(error).__name__}: {str(error)}")
-
-    return results
-
-
-@contextlib.contextmanager
-def swallow_io():
-    stream = WriteOnlyStringIO()
-    with contextlib.redirect_stdout(stream):
-        with contextlib.redirect_stderr(stream):
-            with redirect_stdin(stream):
-                yield
-
-
-@contextlib.contextmanager
-def create_tempdir():
-    with tempfile.TemporaryDirectory() as dirname:
-        with chdir(dirname):
-            yield dirname
-
-
-class TimeoutException(Exception):
-    pass
-
-
-@contextlib.contextmanager
-def time_limit_windows(seconds: float):
-    timer = threading.Timer(seconds, lambda: (_ for _ in ()).throw(TimeoutException("Timed out!")))
-    timer.start()
-    try:
-        yield
-    finally:
-        timer.cancel()
-
-
-@contextlib.contextmanager
-def time_limit(seconds: float):
-    def signal_handler(signum, frame):
-        raise TimeoutException("Timed out!")
-
-    # only works on Unix-based systems, not Windows
-    signal.setitimer(signal.ITIMER_REAL, seconds)
-    signal.signal(signal.SIGALRM, signal_handler)
-    try:
-        yield
-    finally:
-        signal.setitimer(signal.ITIMER_REAL, 0)
-
-
-class WriteOnlyStringIO(io.StringIO):
-    """StringIO that throws an exception when it's read from"""
-
-    def read(self, *args, **kwargs):
-        raise IOError
-
-    def readline(self, *args, **kwargs):
-        raise IOError
-
-    def readlines(self, *args, **kwargs):
-        raise IOError
-
-    def readable(self, *args, **kwargs):
-        """Returns True if the IO object can be read."""
-        return False
-
-
-class redirect_stdin(contextlib._RedirectStream):  # type: ignore
-    _stream = "stdin"
-
-
-@contextlib.contextmanager
-def chdir(root):
-    if root == ".":
-        yield
-        return
-    cwd = os.getcwd()
-    os.chdir(root)
-    try:
-        yield
-    except BaseException as exc:
-        raise exc
-    finally:
-        os.chdir(cwd)
-
-
-def reliability_guard(maximum_memory_bytes: Optional[int] = None):
-    """
-    This disables various destructive functions and prevents the generated code
-    from interfering with the test (e.g. fork bomb, killing other processes,
-    removing filesystem files, etc.)
-
-    WARNING
-    This function is NOT a security sandbox. Untrusted code, including, model-
-    generated code, should not be blindly executed outside of one. See the
-    Codex paper for more information about OpenAI's code sandbox, and proceed
-    with caution.
-    """
-
-    if maximum_memory_bytes is not None:
-        import resource
-
-        resource.setrlimit(resource.RLIMIT_AS, (maximum_memory_bytes, maximum_memory_bytes))
-        resource.setrlimit(resource.RLIMIT_DATA, (maximum_memory_bytes, maximum_memory_bytes))
-        if not platform.uname().system == "Darwin":
-            resource.setrlimit(resource.RLIMIT_STACK, (maximum_memory_bytes, maximum_memory_bytes))
-
-    faulthandler.disable()
-
-    import builtins
-
-    builtins.exit = None
-    builtins.quit = None
-
-    import os
-
-    os.kill = None
-    os.system = None
-    os.putenv = None
-    os.remove = None
-    os.removedirs = None
-    os.rmdir = None
-    os.fchdir = None
-    os.setuid = None
-    os.fork = None
-    os.forkpty = None
-    os.killpg = None
-    os.rename = None
-    os.renames = None
-    os.truncate = None
-    os.replace = None
-    os.unlink = None
-    os.fchmod = None
-    os.fchown = None
-    os.chmod = None
-    os.chown = None
-    os.chroot = None
-    os.fchdir = None
-    os.lchflags = None
-    os.lchmod = None
-    os.lchown = None
-    os.getcwd = None
-    os.chdir = None
-
-    import shutil
-
-    shutil.rmtree = None
-    shutil.move = None
-    shutil.chown = None
-
-    import subprocess
-
-    subprocess.Popen = None  # type: ignore
-
-    __builtins__["help"] = None
-
-    import sys
-
-    sys.modules["ipdb"] = None
-    sys.modules["joblib"] = None
-    sys.modules["resource"] = None
-    sys.modules["psutil"] = None
-    sys.modules["tkinter"] = None
+# Authors: marcusm117
+# License: Apache 2.0
+
+# Code is adapted from OpenAI's original script
+# https://github.com/openai/human-eval/blob/master/human_eval/execution.py
+# and a patch provided by davide221 in the following issue:
+# https://github.com/openai/human-eval/issues/18
+
+
+from typing import List, Dict, Optional
+import contextlib
+import faulthandler
+import io
+import os
+import platform
+import signal
+import threading
+import tempfile
+
+
+def unsafe_execute(task: Dict, mask_func_name: bool, timeout: float = 0.5) -> List[str]:
+    """Please read the WARNING below! Execute untrusted model-generated code with test cases.
+
+    WARNING from OpenAI's original script:
+    # This program exists to execute untrusted model-generated code. Although
+    # it is highly unlikely that model-generated code will do something overtly
+    # malicious in response to this test suite, model-generated code may act
+    # destructively due to a lack of model capability or alignment.
+    # Users are strongly encouraged to sandbox this evaluation suite so that it
+    # does not perform destructive actions on their host or network. For more
+    # information on how OpenAI sandboxes its code, see the accompanying paper.
+
+    Args:
+        task: a dictionary with keys: prompt, contract, function_name, model_solution, tests, atol
+        mask_func_name: whether the function name is replaced by a generic "func" in the function signature
+        timeout: maximum time to run each test case
+
+    Returns:
+        a list of strings representing the result of each test case
+    """
+    # disable functionalities that can make destructive changes to the test
+    reliability_guard()
+
+    # construct the program to be tested
+    program = "\n" + task["problem"] + task["contract"] + "\n" + task["model_solution"] + "\n\n\n"
+
+    # initialize the results list
+    results = []
+
+    # run program for each test case
+    for test in task["tests"]:
+        # Test Case Format 1: a dict of input and output (HumanEvalPlus-reformatted Style)
+        if isinstance(test, dict):
+            # mask the function name if necessary
+            if mask_func_name:
+                task["function_name"] = "func"
+            # capture the output, will assert it later
+            capture_output = f"test_out = {task['function_name']}({test['input']})"
+            # if atol is not 0, assert using the atol provided
+            if task["atol"]:
+                atol = task["atol"]
+                assertion_stmt = f"\nassert abs(test_out - {test['output']}) <= {atol}" + r", f'outputs {test_out}'"
+            else:
+                # otherwise, assert equality
+                assertion_stmt = f"\nassert test_out == {test['output']}" + r", f'outputs {test_out}'"
+            # concatenate the program with assertion statement
+            program_w_test = program + capture_output + assertion_stmt
+
+        # Test Case Format 2: a string of assertion statement (MBPP Style)
+        elif isinstance(test, str):
+            # mask the function name if necessary
+            if mask_func_name:
+                test = test.replace(task["function_name"], "func")
+            # concatenate the program with test case
+            program_w_test = program + test
+
+        # we currently don't support other formats
+        else:
+            raise ValueError("Invalid Test Case Format!")
+
+        # for debugging, uncomment the following line
+        # print(program_w_test)
+
+        try:
+            exec_globals = {}
+            with swallow_io():
+                # change <time_limit> to <time_limit_windows> if you're on Windows
+                with time_limit(timeout):
+                    # please read the WARNING above in the docstring
+                    exec(program_w_test, exec_globals)
+            results.append("Passed")
+        except TimeoutException:
+            results.append("Time Out")
+        except BaseException as error:
+            results.append(f"{type(error).__name__}: {str(error)}")
+
+    return results
+
+
+@contextlib.contextmanager
+def swallow_io():
+    stream = WriteOnlyStringIO()
+    with contextlib.redirect_stdout(stream):
+        with contextlib.redirect_stderr(stream):
+            with redirect_stdin(stream):
+                yield
+
+
+@contextlib.contextmanager
+def create_tempdir():
+    with tempfile.TemporaryDirectory() as dirname:
+        with chdir(dirname):
+            yield dirname
+
+
+class TimeoutException(Exception):
+    pass
+
+
+@contextlib.contextmanager
+def time_limit_windows(seconds: float):
+    timer = threading.Timer(seconds, lambda: (_ for _ in ()).throw(TimeoutException("Timed out!")))
+    timer.start()
+    try:
+        yield
+    finally:
+        timer.cancel()
+
+
+@contextlib.contextmanager
+def time_limit(seconds: float):
+    def signal_handler(signum, frame):
+        raise TimeoutException("Timed out!")
+
+    # only works on Unix-based systems, not Windows
+    signal.setitimer(signal.ITIMER_REAL, seconds)
+    signal.signal(signal.SIGALRM, signal_handler)
+    try:
+        yield
+    finally:
+        signal.setitimer(signal.ITIMER_REAL, 0)
+
+
+class WriteOnlyStringIO(io.StringIO):
+    """StringIO that throws an exception when it's read from"""
+
+    def read(self, *args, **kwargs):
+        raise IOError
+
+    def readline(self, *args, **kwargs):
+        raise IOError
+
+    def readlines(self, *args, **kwargs):
+        raise IOError
+
+    def readable(self, *args, **kwargs):
+        """Returns True if the IO object can be read."""
+        return False
+
+
+class redirect_stdin(contextlib._RedirectStream):  # type: ignore
+    _stream = "stdin"
+
+
+@contextlib.contextmanager
+def chdir(root):
+    if root == ".":
+        yield
+        return
+    cwd = os.getcwd()
+    os.chdir(root)
+    try:
+        yield
+    except BaseException as exc:
+        raise exc
+    finally:
+        os.chdir(cwd)
+
+
+def reliability_guard(maximum_memory_bytes: Optional[int] = None):
+    """
+    This disables various destructive functions and prevents the generated code
+    from interfering with the test (e.g. fork bomb, killing other processes,
+    removing filesystem files, etc.)
+
+    WARNING
+    This function is NOT a security sandbox. Untrusted code, including, model-
+    generated code, should not be blindly executed outside of one. See the
+    Codex paper for more information about OpenAI's code sandbox, and proceed
+    with caution.
+    """
+
+    if maximum_memory_bytes is not None:
+        import resource
+
+        resource.setrlimit(resource.RLIMIT_AS, (maximum_memory_bytes, maximum_memory_bytes))
+        resource.setrlimit(resource.RLIMIT_DATA, (maximum_memory_bytes, maximum_memory_bytes))
+        if not platform.uname().system == "Darwin":
+            resource.setrlimit(resource.RLIMIT_STACK, (maximum_memory_bytes, maximum_memory_bytes))
+
+    faulthandler.disable()
+
+    import builtins
+
+    builtins.exit = None
+    builtins.quit = None
+
+    import os
+
+    os.kill = None
+    os.system = None
+    os.putenv = None
+    os.remove = None
+    os.removedirs = None
+    os.rmdir = None
+    os.fchdir = None
+    os.setuid = None
+    os.fork = None
+    os.forkpty = None
+    os.killpg = None
+    os.rename = None
+    os.renames = None
+    os.truncate = None
+    os.replace = None
+    os.unlink = None
+    os.fchmod = None
+    os.fchown = None
+    os.chmod = None
+    os.chown = None
+    os.chroot = None
+    os.fchdir = None
+    os.lchflags = None
+    os.lchmod = None
+    os.lchown = None
+    os.getcwd = None
+    os.chdir = None
+
+    import shutil
+
+    shutil.rmtree = None
+    shutil.move = None
+    shutil.chown = None
+
+    import subprocess
+
+    subprocess.Popen = None  # type: ignore
+
+    __builtins__["help"] = None
+
+    import sys
+
+    sys.modules["ipdb"] = None
+    sys.modules["joblib"] = None
+    sys.modules["resource"] = None
+    sys.modules["psutil"] = None
+    sys.modules["tkinter"] = None
```

### Comparing `identitychain-0.0.1/identitychain/identity_chain.py` & `identitychain-0.1.0/identitychain/identity_chain.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,462 +1,481 @@
-# Authors: marcusm117, Robin-Y-Ding
-# License: Apache 2.0
-
-
-# Standard Library Modules
-import json
-from typing import Any, Callable, Dict, List
-
-# External Modules
-from tqdm import tqdm
-
-# Internal Modules
-from identitychain import unsafe_execute
-
-
-# a list of supported Foundation Models
-# PL-2-NL generation for Foundation Model is Fill-In-the-Middle (FIM)
-FOUNDATION_MODELS = [
-    "bigcode/starcoder",
-    "bigcode/starcoderplus",
-    "bigcode/starcoderbase",
-    "bigcode/starcoderbase-7b",
-    "bigcode/starcoderbase-3b",
-    "bigcode/starcoderbase-1b",
-    "codellama/CodeLlama-7b-hf",
-    "codellama/CodeLlama-13b-hf",
-    "codellama/CodeLlama-34b-hf",
-]
-
-
-class IdentityChainError(Exception):
-    """Exceptions raised by methods related to class IdentityChain."""
-
-
-class IdentityChain:
-    """A class that performs a chain of Identity Transformations, to wholistically evluate a Code LM.
-
-    Given a problem description, NL_0, prompt the model to generate a solution, PL_0, and run test cases on PL_0.
-    Prompt the model to backtranslate/summarize PL_0 into a new problem description, NL_1,
-    prompt the model to generate a solution, PL_1, and run test cases on PL_1.
-
-    Denote the semantics of PL and NL as sem(PL) and sem(NL),
-    I() is the Identity Transformation in the Semantics Space.
-    then we have:
-
-    sem ∘ NL-2-PL ∘ PL-2-NL(PL_0) = sem ∘ NL-2-PL(NL_1) = sem(PL_1) = I^2(sem(PL_0))
-
-    We expect semantics, thus the test outputs, of PL_1 to be exactly the same as PL_0.
-    In general, we want to see:
-
-    sem ∘ (NL-2-PL ∘ PL-2-NL)^n (PL_0) = I^(2n)(sem(PL_0))
-
-    where n is the number of Identity Transformations performed, which is also the length of the Chain.
-
-
-    Attributes:
-        input_path (str): a string representing the path to the input file
-        output_path (str): a string representing the path to the output file
-        get_model_response_NL_to_PL (callable): a function that takes in a prompt and a problem description,
-            and returns the Model's solution to the problem description
-        get_model_response_PL_to_NL (callable): a function that takes in a prompt and a code solution,
-            and returns the Model's summarization of the code solution
-        prompt_NL_to_PL: a prompt to get the Model's solution to a Natural Langauge problem description,
-            will be used by self.get_model_response_NL_to_PL
-        prompt_PL_to_NL: a prompt to get the Model's summarization of a Programming Language code solution,
-            will be used by self.get_model_response_PL_to_NL
-        length (int): the length of the Identity Chain
-        bootstrap_method (str): either "problem" or "canonical_solution"
-
-    """
-
-    def __init__(
-        self,
-        model,
-        tokenizer,
-        args,
-        input_path,
-        output_path,
-        get_model_response_NL_to_PL,
-        get_model_response_PL_to_NL,
-        prompt_NL_to_PL,
-        prompt_PL_to_NL,
-        length=5,
-        bootstrap_method="problem",
-    ):
-        self.model = model  # model is either a string (for APIs) or a HuggingFace AutoModelForCausalLM object
-        self.tokenizer = tokenizer  # tokenizer is either None (for APIs) or a HuggingFace AutoTokenizer object
-        self.args = args  # args is a argparse.Namespace object to store hyperparameters for model inference
-        self.input_path = input_path
-        self.output_path = output_path
-        self.get_model_response_NL_to_PL = get_model_response_NL_to_PL
-        self.get_model_response_PL_to_NL = get_model_response_PL_to_NL
-        self.prompt_NL_to_PL = prompt_NL_to_PL
-        self.prompt_PL_to_NL = prompt_PL_to_NL
-        self.set_length(length)
-        self.set_bootstrap_method(bootstrap_method)
-
-    def set_model(self, model: Any):
-        """Set the model.
-
-        Args:
-            model: either a string (for APIs) or a HuggingFace AutoModelForCausalLM object
-
-        """
-        self.model = model
-
-    def set_tokenizer(self, tokenizer: Any):
-        """Set the tokenizer.
-
-        Args:
-            tokenizer: either None (for APIs) or a HuggingFace AutoTokenizer object
-
-        """
-        self.tokenizer = tokenizer
-
-    def set_args(self, args: Any):
-        """Set the args.
-
-        Args:
-            args: a argparse.Namespace object to store hyperparameters for model inference
-
-        """
-        self.args = args
-
-    def set_input_path(self, input_path: str):
-        """Set the path to the input file.
-
-        Args:
-            input_path: a string representing the path to the input file
-
-        """
-        self.input_path = input_path
-
-    def set_output_path(self, output_path: str):
-        """Set the path to the output file.
-
-        Args:
-            output_path: a string representing the path to the output file
-
-        """
-        self.output_path = output_path
-
-    def set_get_model_response_NL_to_PL(self, get_model_response_NL_to_PL: Callable):
-        """Set the function to get the Model's solution to a Natural Langauge problem description.
-
-        Args:
-            get_model_response_NL_to_PL: a function that takes in a prompt and a problem description,
-                and returns the Model's solution to the problem description
-
-        """
-        self.get_model_response_NL_to_PL = get_model_response_NL_to_PL
-
-    def set_get_model_response_PL_to_NL(self, get_model_response_PL_to_NL: Callable):
-        """Set the function to get the Model's summarization of a Programming Language code solution.
-
-        Args:
-            get_model_response_PL_to_NL: a function that takes in a prompt and a code solution,
-                and returns the Model's summarization of the code solution
-
-        Note:
-            If the Model have PL-2-NL generation ability i.e.
-            the ability to summarize a code solution into a problem description,
-            then this function should be the same as self.get_model_response_NL_to_PL.
-            If not, this function should be different.
-
-        """
-        self.get_model_response_PL_to_NL = get_model_response_PL_to_NL
-
-    def set_prompt_NL_to_PL(self, prompt_NL_to_PL: str | List[Dict[str, str]]):
-        """Set the prompt to get the Model's solution to a Natural Langauge problem description.
-
-        Args:
-            prompt_NL_to_PL: a prompt to get the Model's solution to a Natural Langauge problem description,
-                will be used by self.get_model_response_NL_to_PL
-
-        """
-        self.prompt_NL_to_PL = prompt_NL_to_PL
-
-    def set_prompt_PL_to_NL(self, prompt_PL_to_NL: str | List[Dict[str, str]]):
-        """Set the prompt to get the Model's summarization of a Programming Language code solution.
-
-        Args:
-            prompt_PL_to_NL: a prompt to get the Model's summarization of a Programming Language code solution,
-                will be used by self.get_model_response_PL_to_NL
-
-        """
-        self.prompt_PL_to_NL = prompt_PL_to_NL
-
-    def set_length(self, length: int):
-        """Set the length of the Identity Chain.
-
-        Args:
-            length: the length of the Identity Chain
-
-        Raises:
-            IdentityChainError: if length is not a positive integer
-            IdentityChainError: if user does not confirm to run an Identity Chain of length > 5
-
-        Note:
-            lenght = 5 is usually enough to get a good estimate of the model's performance.
-            If you are using a very large evaluation set, you may want to set length to 4 or even 3.
-
-        """
-        if length < 1:
-            raise IdentityChainError("length must be a positive integer")
-        if length > 5:
-            answer = input("WARNING: length > 5 may take a long time to run. Continue? (y/n) ")
-            if answer != "y" and answer != "Y":
-                raise IdentityChainError("enter 'y' or 'Y' to confirm an Identity Chain of length > 5")
-        self.length = length
-
-    def set_bootstrap_method(self, bootstrap_method: str):
-        """Set the method to bootstrap the Identity Chain.
-
-        We can either use the problem description as NL_0, and use the model's generated solution PL_0,
-        or if the dataset includes the canonical solution, we can use it as PL_0 directly.
-
-        Args:
-            bootstrap_method: either "problem" or "canonical_solution"
-
-        Raises:
-            IdentityChainError: if bootstrap_method is not "problem" or "canonical_solution"
-
-        """
-        if bootstrap_method not in ["problem", "canonical_solution"]:
-            raise IdentityChainError("bootstrap_method must be either 'problem' or 'canonical_solution'")
-        self.bootstrap_method = bootstrap_method
-
-    def bootstrap(self, resume_task: int = 1):
-        """Bootstrap the Identity Chain to get PL_0.
-
-        Args:
-            resume_task: the task to resume from. Defaults to 1, since tasks[0] can used for in-context prompting.
-
-        Raises:
-            IdentityChainError: if resume_task is a negative integer
-
-        """
-        # check for invalid input
-        if resume_task < 0:
-            raise IdentityChainError("resume_task must be a non-negative integer")
-
-        # read in all the tasks
-        with open(self.input_path, "r", encoding="utf-8") as reader:
-            tasks = reader.readlines()
-
-        # bootstrap the Identity Chain for each task
-        with open(self.output_path, "a", encoding="utf-8") as writer:
-            for input_task in tqdm(tasks[resume_task:]):
-                input_task = json.loads(input_task)
-
-                # get the Original Problem Description NL_0, and other invariant fields
-                NL_0 = input_task["problem"]
-                task_id = input_task["task_id"]
-                contract = input_task["contract"]
-                function_name = input_task["function_name"]
-                function_signature = input_task["function_signature"]
-                tests = input_task["tests"]
-                atol = input_task["atol"]
-
-                # bootstrap PL_0, it can be either the Model Solution or the Canonical Solution
-                if self.bootstrap_method == "problem":
-                    # prompt the model to generate a solution PL_0 given the problem description NL_0
-                    # the prompt we are using is "self.prompt_NL_to_PL"
-                    PL_0 = self.get_model_response_NL_to_PL(
-                        self.prompt_NL_to_PL, NL_0, self.model, self.tokenizer, self.args
-                    )
-                else:
-                    PL_0 = input_task["canonical_solution"]
-
-                # run test cases on PL_0
-                test_task = {
-                    "problem": NL_0,
-                    "contract": contract,
-                    "function_name": function_name,
-                    "model_solution": PL_0,
-                    "tests": tests,
-                    "atol": atol,
-                }
-                # no need to mask the function name when bootstrapping
-                results = unsafe_execute(test_task, mask_func_name=False, timeout=0.5)
-
-                # write to output file
-                output_task = {
-                    "task_id": task_id,
-                    "NL_0": NL_0,
-                    "contract": contract,
-                    "function_name": function_name,
-                    "function_signature": function_signature,
-                    "tests": tests,
-                    "atol": atol,
-                    "PL_0": PL_0,
-                    "PL_0_results": results,
-                }
-                writer.write(json.dumps(output_task) + "\n")
-                writer.flush()
-
-                # for debugging
-                # print(output_task)
-
-    def run(
-        self,
-        resume_task: int = 0,
-        resume_step: int = 1,
-        pass_only: bool = False,
-        mask_func_name: bool = True,
-        greedy_early_stop: bool = False,
-    ):
-        """Run the Identity Chain to get PL_1 to PL_n.
-
-        Args:
-            resume_task: the task to resume from
-            resume_step: the step to resume from. Defaults to 1, since Step 0 is the bootstrap step.
-            pass_only: whether to only run on tasks that passed all tests in the previous step
-            mask_func_name: whether to replace the function name with a generic "func",
-                to avoid conflict when a wrong solution/problem description that doesn't match the function name
-            greedy_early_stop: when using greedy decoding, whether to stop the model generation when
-                PL_i is exactly the same as PL_{i-1} or NL_i is exactly the same as NL_{i-1}.
-                The Identity Chain keeps running by just copying the previous step's solution/problem description.
-                !!!WARNING!!! This should only be set to True when the model is set to do greedy decoding!!!
-
-        Raises:
-            IdentityChainError: if resume_task is a negative integer
-            IdentityChainError: if resume_step is not in the closed interval [1, self.length]
-            IdentityChainError: if greedy_early_stop is True and the user does not confirm
-
-        """
-        # check for invalid input
-        if resume_task < 0:
-            raise IdentityChainError("resume_task must be a non-negative integer")
-        if resume_step > self.length or resume_step < 1:
-            raise IdentityChainError("resume_step must be in [1, self.length]")
-
-        # double check if using greedy decoding
-        if greedy_early_stop:
-            answer = input(
-                "WARNING: greedy_early_stop is True. This should only be set to True when doing greedy decoding. Continue? (y/n) "
-            )
-            if answer != "y" and answer != "Y":
-                raise IdentityChainError("enter 'y' or 'Y' to confirm setting greedy_early_stop to True")
-
-        # read in all the tasks, from the bootstrapped output file
-        with open(self.output_path, "r", encoding="utf-8") as reader:
-            tasks = reader.readlines()
-
-        # run the Identity Chain for each task
-        for idx, task in enumerate(tqdm(tasks[resume_task:])):
-            task = json.loads(task)
-            # if greedy_early_stop is set to True, we use this flag to indicate if we have reached a fixed point
-            # so that we don't waste time generating the exact same solutions/problem descriptions again
-            fixed_point = False
-
-            # run Identity Transformation for each step in the Chain
-            for i in range(resume_step, self.length + 1):
-                # if pass_only option is False,
-                # check if PL_{i-1} is defined and passed all test cases,
-                # where PL_{i-1} is the Model Solution from the previous step,
-                # if undefined or passed, stop running the Identity Chain for this task
-                if pass_only and (f"PL_{i-1}_results" not in task or "Error" in "".join(task[f"PL_{i-1}_results"])):
-                    task[f"NL_{i}"] = "NA"
-                    task[f"PL_{i}"] = "NA"
-                    task[f"PL_{i}_results"] = "NA"
-
-                # if pass_only option is False, run the Identity Chain on every task regardless
-                else:
-                    # get invariant fields
-                    contract = task["contract"]
-                    function_name = task["function_name"]
-                    function_signature = task["function_signature"]
-                    tests = task["tests"]
-                    atol = task["atol"]
-
-                    # if mask_func_name option is True, repalce the function name with a generic "func" in the function signature
-                    masked_function_signature = function_signature
-                    if mask_func_name:
-                        masked_function_signature = function_signature.replace(function_name, "func")
-
-                    # get PL_{i-1}, the Model Solution from the previous step
-                    PL_i_minus_1 = task[f"PL_{i-1}"]
-                    # if mask_func_name option is True, repalce the function name with a generic "func" in PL_0, as it might be recursive
-                    # if PL_0 is recursive and we don't replace, then the original function name in PL_0 will be an undefined name
-                    if mask_func_name and i == 1:
-                        PL_i_minus_1 = PL_i_minus_1.replace(function_name, "func")
-
-                    # prompt the Code Model to summarize a new problem description NL_i given PL_{i-1}
-                    # the prompt we are using is self.PL_to_NL
-                    # if we have reached a fixed point, copy the problem description from the previous step
-                    if fixed_point:
-                        NL_i = task[f"NL_{i-1}"]
-                    else:
-                        if self.args.model_name_or_path in FOUNDATION_MODELS:
-                            NL_i = self.get_model_response_PL_to_NL(
-                                self.prompt_PL_to_NL,
-                                masked_function_signature,
-                                PL_i_minus_1,
-                                self.model,
-                                self.tokenizer,
-                                self.args,
-                            )
-                        else:
-                            NL_i = self.get_model_response_PL_to_NL(
-                                self.prompt_PL_to_NL,
-                                masked_function_signature.rstrip('\n') + '\n' + PL_i_minus_1.lstrip('\n'),
-                                self.model,
-                                self.tokenizer,
-                                self.args,
-                            )
-
-                    # if NL_i = NL_{i-1} and we're using greedy decoding, then we have reached a fixed point
-                    if greedy_early_stop and NL_i == task[f"NL_{i-1}"]:
-                        # for debugging
-                        print("Reached a Fixed Point! Stop Model Inference.")
-                        fixed_point = True
-
-                    # prompt the Code Model to generate a solution PL_i given the problem description NL_i
-                    # the prompt we are using is "self.NL_to_PL"
-                    # if we have reached a fixed point, copy the solution from the previous step
-                    if fixed_point:
-                        PL_i = task[f"PL_{i-1}"]
-                    else:
-                        PL_i = self.get_model_response_NL_to_PL(
-                            self.prompt_NL_to_PL,
-                            masked_function_signature + NL_i,
-                            self.model,
-                            self.tokenizer,
-                            self.args,
-                        )
-
-                    # if PL_i = PL_{i-1} and we're using greedy decoding, then we have reached a fixed point
-                    if greedy_early_stop and PL_i == task[f"PL_{i-1}"]:
-                        # for debugging
-                        print("Reached a Fixed Point! Stop Model Inference.")
-                        fixed_point = True
-
-                    # run test cases on PL_i
-                    # if we have reached a fixed point, copy the results from the previous step
-                    if fixed_point:
-                        results = task[f"PL_{i-1}_results"]
-                    else:
-                        test_task = {
-                            "problem": masked_function_signature + NL_i,
-                            "contract": contract,
-                            "function_name": function_name,
-                            "model_solution": PL_i,
-                            "tests": tests,
-                            "atol": atol,
-                        }
-                        results = unsafe_execute(test_task, mask_func_name, timeout=0.5)
-
-                    # update new fields
-                    task[f"NL_{i}"] = NL_i
-                    task[f"PL_{i}"] = PL_i
-                    task[f"PL_{i}_results"] = results
-
-                # write to output file
-                tasks[idx + resume_task] = json.dumps(task) + "\n"
-                with open(self.output_path, "w", encoding="utf-8") as writer:
-                    writer.writelines(tasks)
-                    writer.flush()
-
-                # for debugging
-                print(tasks[idx + resume_task])
+# Authors: marcusm117, Robin-Y-Ding
+# License: Apache 2.0
+
+
+# Standard Library Modules
+import json
+from typing import Any, Callable, Dict, List
+
+# External Modules
+from tqdm import tqdm
+
+# Internal Modules
+from identitychain import unsafe_execute
+
+
+# a list of supported Foundation Models
+# PL-2-NL generation for Foundation Model is Fill-In-the-Middle (FIM)
+FOUNDATION_MODELS = [
+    "codellama/CodeLlama-7b-hf",
+    "codellama/CodeLlama-13b-hf",
+    "codellama/CodeLlama-34b-hf",
+    "codellama/CodeLlama-70b-hf",
+    "bigcode/starcoderbase-1b",
+    "bigcode/starcoderbase-3b",
+    "bigcode/starcoderbase-7b",
+    "bigcode/starcoderbase",
+    "bigcode/starcoderplus",
+    "bigcode/starcoder",
+    "deepseek-ai/deepseek-coder-1.3b-base",
+    "deepseek-ai/deepseek-coder-6.7b-base",
+    "deepseek-ai/deepseek-coder-33b-base",
+    "deepseek-ai/deepseek-coder-7b-base-v1.5",
+]
+
+
+# a list of supported Instruction-Tuned Models
+INSTRUCTION_MODELS = [
+    "codellama/CodeLlama-7b-Instruct-hf",
+    "codellama/CodeLlama-13b-Instruct-hf",
+    "codellama/CodeLlama-34b-Instruct-hf",
+    "codellama/CodeLlama-70b-Instruct-hf",
+    "HuggingFaceH4/starchat-beta",
+    "deepseek-ai/deepseek-coder-1.3b-instruct",
+    "deepseek-ai/deepseek-coder-6.7b-instruct",
+    "deepseek-ai/deepseek-coder-33b-instruct",
+    "deepseek-ai/deepseek-coder-7b-instruct-v1.5",
+]
+
+
+class IdentityChainError(Exception):
+    """Exceptions raised by methods related to class IdentityChain."""
+
+
+class IdentityChain:
+    """A class that performs a chain of Identity Transformations, to wholistically evluate a Code LM.
+
+    Given a problem description, NL_0, prompt the model to generate a solution, PL_0, and run test cases on PL_0.
+    Prompt the model to backtranslate/summarize PL_0 into a new problem description, NL_1,
+    prompt the model to generate a solution, PL_1, and run test cases on PL_1.
+
+    Denote the semantics of PL and NL as sem(PL) and sem(NL),
+    I() is the Identity Transformation in the Semantics Space.
+    then we have:
+
+    sem ∘ NL-2-PL ∘ PL-2-NL(PL_0) = sem ∘ NL-2-PL(NL_1) = sem(PL_1) = I^2(sem(PL_0))
+
+    We expect semantics, thus the test outputs, of PL_1 to be exactly the same as PL_0.
+    In general, we want to see:
+
+    sem ∘ (NL-2-PL ∘ PL-2-NL)^n (PL_0) = I^(2n)(sem(PL_0))
+
+    where n is the number of Identity Transformations performed, which is also the length of the Chain.
+
+
+    Attributes:
+        input_path (str): a string representing the path to the input file
+        output_path (str): a string representing the path to the output file
+        get_model_response_NL_to_PL (callable): a function that takes in a prompt and a problem description,
+            and returns the Model's solution to the problem description
+        get_model_response_PL_to_NL (callable): a function that takes in a prompt and a code solution,
+            and returns the Model's summarization of the code solution
+        prompt_NL_to_PL: a prompt to get the Model's solution to a Natural Langauge problem description,
+            will be used by self.get_model_response_NL_to_PL
+        prompt_PL_to_NL: a prompt to get the Model's summarization of a Programming Language code solution,
+            will be used by self.get_model_response_PL_to_NL
+        length (int): the length of the Identity Chain
+        bootstrap_method (str): either "problem" or "canonical_solution"
+
+    """
+
+    def __init__(
+        self,
+        model,
+        tokenizer,
+        args,
+        input_path,
+        output_path,
+        get_model_response_NL_to_PL,
+        get_model_response_PL_to_NL,
+        prompt_NL_to_PL,
+        prompt_PL_to_NL,
+        length=5,
+        bootstrap_method="problem",
+    ):
+        self.model = model  # model is either a string (for APIs) or a HuggingFace AutoModelForCausalLM object
+        self.tokenizer = tokenizer  # tokenizer is either None (for APIs) or a HuggingFace AutoTokenizer object
+        self.args = args  # args is a argparse.Namespace object to store hyperparameters for model inference
+        self.input_path = input_path
+        self.output_path = output_path
+        self.get_model_response_NL_to_PL = get_model_response_NL_to_PL
+        self.get_model_response_PL_to_NL = get_model_response_PL_to_NL
+        self.prompt_NL_to_PL = prompt_NL_to_PL
+        self.prompt_PL_to_NL = prompt_PL_to_NL
+        self.set_length(length)
+        self.set_bootstrap_method(bootstrap_method)
+
+    def set_model(self, model: Any):
+        """Set the model.
+
+        Args:
+            model: either a string (for APIs) or a HuggingFace AutoModelForCausalLM object
+
+        """
+        self.model = model
+
+    def set_tokenizer(self, tokenizer: Any):
+        """Set the tokenizer.
+
+        Args:
+            tokenizer: either None (for APIs) or a HuggingFace AutoTokenizer object
+
+        """
+        self.tokenizer = tokenizer
+
+    def set_args(self, args: Any):
+        """Set the args.
+
+        Args:
+            args: a argparse.Namespace object to store hyperparameters for model inference
+
+        """
+        self.args = args
+
+    def set_input_path(self, input_path: str):
+        """Set the path to the input file.
+
+        Args:
+            input_path: a string representing the path to the input file
+
+        """
+        self.input_path = input_path
+
+    def set_output_path(self, output_path: str):
+        """Set the path to the output file.
+
+        Args:
+            output_path: a string representing the path to the output file
+
+        """
+        self.output_path = output_path
+
+    def set_get_model_response_NL_to_PL(self, get_model_response_NL_to_PL: Callable):
+        """Set the function to get the Model's solution to a Natural Langauge problem description.
+
+        Args:
+            get_model_response_NL_to_PL: a function that takes in a prompt and a problem description,
+                and returns the Model's solution to the problem description
+
+        """
+        self.get_model_response_NL_to_PL = get_model_response_NL_to_PL
+
+    def set_get_model_response_PL_to_NL(self, get_model_response_PL_to_NL: Callable):
+        """Set the function to get the Model's summarization of a Programming Language code solution.
+
+        Args:
+            get_model_response_PL_to_NL: a function that takes in a prompt and a code solution,
+                and returns the Model's summarization of the code solution
+
+        Note:
+            If the Model have PL-2-NL generation ability i.e.
+            the ability to summarize a code solution into a problem description,
+            then this function should be the same as self.get_model_response_NL_to_PL.
+            If not, this function should be different.
+
+        """
+        self.get_model_response_PL_to_NL = get_model_response_PL_to_NL
+
+    def set_prompt_NL_to_PL(self, prompt_NL_to_PL: str | List[Dict[str, str]]):
+        """Set the prompt to get the Model's solution to a Natural Langauge problem description.
+
+        Args:
+            prompt_NL_to_PL: a prompt to get the Model's solution to a Natural Langauge problem description,
+                will be used by self.get_model_response_NL_to_PL
+
+        """
+        self.prompt_NL_to_PL = prompt_NL_to_PL
+
+    def set_prompt_PL_to_NL(self, prompt_PL_to_NL: str | List[Dict[str, str]]):
+        """Set the prompt to get the Model's summarization of a Programming Language code solution.
+
+        Args:
+            prompt_PL_to_NL: a prompt to get the Model's summarization of a Programming Language code solution,
+                will be used by self.get_model_response_PL_to_NL
+
+        """
+        self.prompt_PL_to_NL = prompt_PL_to_NL
+
+    def set_length(self, length: int):
+        """Set the length of the Identity Chain.
+
+        Args:
+            length: the length of the Identity Chain
+
+        Raises:
+            IdentityChainError: if length is not a positive integer
+            IdentityChainError: if user does not confirm to run an Identity Chain of length > 5
+
+        Note:
+            lenght = 5 is usually enough to get a good estimate of the model's performance.
+            If you are using a very large evaluation set, you may want to set length to 4 or even 3.
+
+        """
+        if length < 1:
+            raise IdentityChainError("length must be a positive integer")
+        if length > 5:
+            answer = input("WARNING: length > 5 may take a long time to run. Continue? (y/n) ")
+            if answer != "y" and answer != "Y":
+                raise IdentityChainError("enter 'y' or 'Y' to confirm an Identity Chain of length > 5")
+        self.length = length
+
+    def set_bootstrap_method(self, bootstrap_method: str):
+        """Set the method to bootstrap the Identity Chain.
+
+        We can either use the problem description as NL_0, and use the model's generated solution PL_0,
+        or if the dataset includes the canonical solution, we can use it as PL_0 directly.
+
+        Args:
+            bootstrap_method: either "problem" or "canonical_solution"
+
+        Raises:
+            IdentityChainError: if bootstrap_method is not "problem" or "canonical_solution"
+
+        """
+        if bootstrap_method not in ["problem", "canonical_solution"]:
+            raise IdentityChainError("bootstrap_method must be either 'problem' or 'canonical_solution'")
+        self.bootstrap_method = bootstrap_method
+
+    def bootstrap(self, resume_task: int = 1):
+        """Bootstrap the Identity Chain to get PL_0.
+
+        Args:
+            resume_task: the task to resume from. Defaults to 1, since tasks[0] can used for in-context prompting.
+
+        Raises:
+            IdentityChainError: if resume_task is a negative integer
+
+        """
+        # check for invalid input
+        if resume_task < 0:
+            raise IdentityChainError("resume_task must be a non-negative integer")
+
+        # read in all the tasks
+        with open(self.input_path, "r", encoding="utf-8") as reader:
+            tasks = reader.readlines()
+
+        # bootstrap the Identity Chain for each task
+        with open(self.output_path, "a", encoding="utf-8") as writer:
+            for input_task in tqdm(tasks[resume_task:]):
+                input_task = json.loads(input_task)
+
+                # get the Original Problem Description NL_0, and other invariant fields
+                NL_0 = input_task["problem"]
+                task_id = input_task["task_id"]
+                contract = input_task["contract"]
+                function_name = input_task["function_name"]
+                function_signature = input_task["function_signature"]
+                tests = input_task["tests"]
+                atol = input_task["atol"]
+
+                # bootstrap PL_0, it can be either the Model Solution or the Canonical Solution
+                if self.bootstrap_method == "problem":
+                    # prompt the model to generate a solution PL_0 given the problem description NL_0
+                    # the prompt we are using is "self.prompt_NL_to_PL"
+                    PL_0 = self.get_model_response_NL_to_PL(
+                        self.prompt_NL_to_PL, NL_0, self.model, self.tokenizer, self.args
+                    )
+                else:
+                    PL_0 = input_task["canonical_solution"]
+
+                # run test cases on PL_0
+                test_task = {
+                    "problem": NL_0,
+                    "contract": contract,
+                    "function_name": function_name,
+                    "model_solution": PL_0,
+                    "tests": tests,
+                    "atol": atol,
+                }
+                # no need to mask the function name when bootstrapping
+                results = unsafe_execute(test_task, mask_func_name=False, timeout=0.5)
+
+                # write to output file
+                output_task = {
+                    "task_id": task_id,
+                    "NL_0": NL_0,
+                    "contract": contract,
+                    "function_name": function_name,
+                    "function_signature": function_signature,
+                    "tests": tests,
+                    "atol": atol,
+                    "PL_0": PL_0,
+                    "PL_0_results": results,
+                }
+                writer.write(json.dumps(output_task) + "\n")
+                writer.flush()
+
+                # for debugging
+                # print(output_task)
+
+    def run(
+        self,
+        resume_task: int = 0,
+        resume_step: int = 1,
+        pass_only: bool = False,
+        mask_func_name: bool = True,
+        greedy_early_stop: bool = False,
+    ):
+        """Run the Identity Chain to get PL_1 to PL_n.
+
+        Args:
+            resume_task: the task to resume from
+            resume_step: the step to resume from. Defaults to 1, since Step 0 is the bootstrap step.
+            pass_only: whether to only run on tasks that passed all tests in the previous step
+            mask_func_name: whether to replace the function name with a generic "func",
+                to avoid conflict when a wrong solution/problem description that doesn't match the function name
+            greedy_early_stop: when using greedy decoding, whether to stop the model generation when
+                PL_i is exactly the same as PL_{i-1} or NL_i is exactly the same as NL_{i-1}.
+                The Identity Chain keeps running by just copying the previous step's solution/problem description.
+                !!!WARNING!!! This should only be set to True when the model is set to do greedy decoding!!!
+
+        Raises:
+            IdentityChainError: if resume_task is a negative integer
+            IdentityChainError: if resume_step is not in the closed interval [1, self.length]
+            IdentityChainError: if greedy_early_stop is True and the user does not confirm
+
+        """
+        # check for invalid input
+        if resume_task < 0:
+            raise IdentityChainError("resume_task must be a non-negative integer")
+        if resume_step > self.length or resume_step < 1:
+            raise IdentityChainError("resume_step must be in [1, self.length]")
+
+        # double check if using greedy decoding
+        if greedy_early_stop:
+            answer = input(
+                "WARNING: greedy_early_stop is True. This should only be set to True when doing greedy decoding. Continue? (y/n) "
+            )
+            if answer != "y" and answer != "Y":
+                raise IdentityChainError("enter 'y' or 'Y' to confirm setting greedy_early_stop to True")
+
+        # read in all the tasks, from the bootstrapped output file
+        with open(self.output_path, "r", encoding="utf-8") as reader:
+            tasks = reader.readlines()
+
+        # run the Identity Chain for each task
+        for idx, task in enumerate(tqdm(tasks[resume_task:])):
+            task = json.loads(task)
+            # if greedy_early_stop is set to True, we use this flag to indicate if we have reached a fixed point
+            # so that we don't waste time generating the exact same solutions/problem descriptions again
+            fixed_point = False
+
+            # run Identity Transformation for each step in the Chain
+            for i in range(resume_step, self.length + 1):
+                # if pass_only option is False,
+                # check if PL_{i-1} is defined and passed all test cases,
+                # where PL_{i-1} is the Model Solution from the previous step,
+                # if undefined or passed, stop running the Identity Chain for this task
+                if pass_only and (f"PL_{i-1}_results" not in task or "Error" in "".join(task[f"PL_{i-1}_results"])):
+                    task[f"NL_{i}"] = "NA"
+                    task[f"PL_{i}"] = "NA"
+                    task[f"PL_{i}_results"] = "NA"
+
+                # if pass_only option is False, run the Identity Chain on every task regardless
+                else:
+                    # get invariant fields
+                    contract = task["contract"]
+                    function_name = task["function_name"]
+                    function_signature = task["function_signature"]
+                    tests = task["tests"]
+                    atol = task["atol"]
+
+                    # if mask_func_name option is True, repalce the function name with a generic "func" in the function signature
+                    masked_function_signature = function_signature
+                    if mask_func_name:
+                        masked_function_signature = function_signature.replace(function_name, "func")
+
+                    # get PL_{i-1}, the Model Solution from the previous step
+                    PL_i_minus_1 = task[f"PL_{i-1}"]
+                    # if mask_func_name option is True, repalce the function name with a generic "func" in PL_0, as it might be recursive
+                    # if PL_0 is recursive and we don't replace, then the original function name in PL_0 will be an undefined name
+                    if mask_func_name and i == 1:
+                        PL_i_minus_1 = PL_i_minus_1.replace(function_name, "func")
+
+                    # prompt the Code Model to summarize a new problem description NL_i given PL_{i-1}
+                    # the prompt we are using is self.PL_to_NL
+                    # if we have reached a fixed point, copy the problem description from the previous step
+                    if fixed_point:
+                        NL_i = task[f"NL_{i-1}"]
+                    else:
+                        if self.args.model_name_or_path in FOUNDATION_MODELS:
+                            NL_i = self.get_model_response_PL_to_NL(
+                                self.prompt_PL_to_NL,
+                                masked_function_signature,
+                                PL_i_minus_1,
+                                self.model,
+                                self.tokenizer,
+                                self.args,
+                            )
+                        else:
+                            NL_i = self.get_model_response_PL_to_NL(
+                                self.prompt_PL_to_NL,
+                                masked_function_signature.rstrip('\n') + '\n' + PL_i_minus_1.lstrip('\n'),
+                                self.model,
+                                self.tokenizer,
+                                self.args,
+                            )
+
+                    # if NL_i = NL_{i-1} and we're using greedy decoding, then we have reached a fixed point
+                    if greedy_early_stop and NL_i == task[f"NL_{i-1}"]:
+                        # for debugging
+                        print("Reached a Fixed Point! Stop Model Inference.")
+                        fixed_point = True
+
+                    # prompt the Code Model to generate a solution PL_i given the problem description NL_i
+                    # the prompt we are using is "self.NL_to_PL"
+                    # if we have reached a fixed point, copy the solution from the previous step
+                    if fixed_point:
+                        PL_i = task[f"PL_{i-1}"]
+                    else:
+                        PL_i = self.get_model_response_NL_to_PL(
+                            self.prompt_NL_to_PL,
+                            masked_function_signature + NL_i,
+                            self.model,
+                            self.tokenizer,
+                            self.args,
+                        )
+
+                    # if PL_i = PL_{i-1} and we're using greedy decoding, then we have reached a fixed point
+                    if greedy_early_stop and PL_i == task[f"PL_{i-1}"]:
+                        # for debugging
+                        print("Reached a Fixed Point! Stop Model Inference.")
+                        fixed_point = True
+
+                    # run test cases on PL_i
+                    # if we have reached a fixed point, copy the results from the previous step
+                    if fixed_point:
+                        results = task[f"PL_{i-1}_results"]
+                    else:
+                        test_task = {
+                            "problem": masked_function_signature + NL_i,
+                            "contract": contract,
+                            "function_name": function_name,
+                            "model_solution": PL_i,
+                            "tests": tests,
+                            "atol": atol,
+                        }
+                        results = unsafe_execute(test_task, mask_func_name, timeout=0.5)
+
+                    # update new fields
+                    task[f"NL_{i}"] = NL_i
+                    task[f"PL_{i}"] = PL_i
+                    task[f"PL_{i}_results"] = results
+
+                # write to output file
+                tasks[idx + resume_task] = json.dumps(task) + "\n"
+                with open(self.output_path, "w", encoding="utf-8") as writer:
+                    writer.writelines(tasks)
+                    writer.flush()
+
+                # for debugging
+                print(tasks[idx + resume_task])
```

### Comparing `identitychain-0.0.1/identitychain/tests/test_executor.py` & `identitychain-0.1.0/identitychain/tests/test_executor.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,341 +1,341 @@
-# Authors: marcusm117
-# License: Apache 2.0
-
-
-# Standard Library Modules
-import json
-import os
-
-# Internal Modules
-from identitychain.utils import g_unzip
-
-# Internal Modules to be tested
-from identitychain import unsafe_execute
-
-
-def test_unsafe_execute():
-    task = {
-        "problem": "from typing import List\n\n\ndef separate_paren_groups(paren_string: str) -> List[str]:\n    \"\"\" Input to this function is a string containing multiple groups of nested parentheses. Your goal is to\n    separate those group into separate strings and return the list of those.\n    Separate groups are balanced (each open brace is properly closed) and not nested within each other\n    Ignore any spaces in the input string.\n    >>> separate_paren_groups('( ) (( )) (( )( ))')\n    ['()', '(())', '(()())']\n    \"\"\"\n",
-        "contract": "\n    assert type(paren_string) == str, \"invalid inputs\" # $_CONTRACT_$\n    cnt = 0 # $_CONTRACT_$\n    for ch in paren_string: # $_CONTRACT_$\n        assert ch in [\"(\", \")\", \" \"], \"invalid inputs\"  # $_CONTRACT_$\n        if ch == \"(\": cnt += 1 # $_CONTRACT_$\n        if ch == \")\": cnt -= 1 # $_CONTRACT_$\n        assert cnt >= 0, \"invalid inputs\" # $_CONTRACT_$\n",
-        "function_name": "separate_paren_groups",
-        "model_solution": "\n\n    cnt, group, results = 0, \"\", []\n    for ch in paren_string:\n        if ch == \"(\": cnt += 1\n        if ch == \")\": cnt -= 1\n        if ch != \" \": group += ch\n        if cnt == 0:\n            if group != \"\": results.append(group)\n            group = \"\"\n    return results\n\n",
-        "tests": [
-            {
-                "input": "'(()()) ((())) () ((())()())'",
-                "output": "['(()())', '((()))', '()', '((())()())']",
-            },
-            {
-                "input": "'() (()) ((())) (((())))'",
-                "output": "['()', '(())', '((()))', '(((())))']",
-            },
-        ],
-        "atol": 0,
-    }
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == ["Passed", "Passed"]
-
-    task["model_solution"] = "    return []"
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == [
-        "AssertionError: outputs []",
-        "AssertionError: outputs []",
-    ]
-
-    task["model_solution"] = "    return ['(()())', '((()))', '()', '((())()())']"
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == ["Passed", "AssertionError: outputs ['(()())', '((()))', '()', '((())()())']"]
-
-    # print results
-    print("++ All tests passed for test_unsafe_execute() ++")
-
-
-# test executing functions with float ouputs
-def test_unsafe_execute_atol():
-    task = {
-        "problem": "def truncate_number(number: float) -> float:\n    \"\"\" Given a positive floating point number, it can be decomposed into\n    and integer part (largest integer smaller than given number) and decimals\n    (leftover part always smaller than 1).\n\n    Return the decimal part of the number.\n    >>> truncate_number(3.5)\n    0.5\n    \"\"\"\n",
-        "contract": "\n    assert number > 0, \"invalid inputs\" # $_CONTRACT_$\n    assert isinstance(number, float), \"invalid inputs\" # $_CONTRACT_$\n",
-        "function_name": "truncate_number",
-        "model_solution": "\n\n    return number - int(number)\n\n",
-        "tests": [
-            {"input": "3.5", "output": "0.5"},
-            {"input": "1.33", "output": "0.33000000000000007"},
-            {"input": "123.456", "output": "0.45600000000000307"},
-            {"input": "999.99999", "output": "0.9999900000000252"},
-            {"input": "0.04320870526393539", "output": "0.04320870526393539"},
-            {"input": "1.0", "output": "0.0"},
-            {"input": "1e-323", "output": "1e-323"},
-            {"input": "1000000000.0", "output": "0.0"},
-        ],
-        "atol": 1e-06,
-    }
-
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == ["Passed", "Passed", "Passed", "Passed", "Passed", "Passed", "Passed", "Passed"]
-
-    task["model_solution"] = "    return 0.0"
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == [
-        "AssertionError: outputs 0.0",
-        "AssertionError: outputs 0.0",
-        "AssertionError: outputs 0.0",
-        "AssertionError: outputs 0.0",
-        "AssertionError: outputs 0.0",
-        "Passed",
-        "Passed",
-        "Passed",
-    ]
-
-    task["model_solution"] = "    return 0.5"
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == [
-        "Passed",
-        "AssertionError: outputs 0.5",
-        "AssertionError: outputs 0.5",
-        "AssertionError: outputs 0.5",
-        "AssertionError: outputs 0.5",
-        "AssertionError: outputs 0.5",
-        "AssertionError: outputs 0.5",
-        "AssertionError: outputs 0.5",
-    ]
-
-    # print results
-    print("++ All tests passed for test_unsafe_execute_atol() ++")
-
-
-# test executing functions with multiple def
-def test_unsafe_execute_multiple_def():
-    task = {
-        "problem": "def is_palindrome(string: str) -> bool:\n    \"\"\" Test if given string is a palindrome \"\"\"\n    return string == string[::-1]\n\n\ndef make_palindrome(string: str) -> str:\n    \"\"\" Find the shortest palindrome that begins with a supplied string.\n    Algorithm idea is simple:\n    - Find the longest postfix of supplied string that is a palindrome.\n    - Append to the end of the string reverse of a string prefix that comes before the palindromic suffix.\n    >>> make_palindrome('')\n    ''\n    >>> make_palindrome('cat')\n    'catac'\n    >>> make_palindrome('cata')\n    'catac'\n    \"\"\"\n",
-        "contract": "\n    assert type(string) == str, \"invalid inputs\" # $_CONTRACT_$\n",
-        "function_name": "make_palindrome",
-        "model_solution": "\n    if is_palindrome(string):\n        return string\n    for i in range(len(string)):\n        if is_palindrome(string[i:]):\n            return string + string[i-1::-1]\n\n",
-        "tests": [
-            {"input": "''", "output": "''"},
-            {"input": "'x'", "output": "'x'"},
-            {"input": "'xyz'", "output": "'xyzyx'"},
-            {"input": "'xyx'", "output": "'xyx'"},
-            {"input": "'jerry'", "output": "'jerryrrej'"},
-            {"input": "'race'", "output": "'racecar'"},
-            {"input": "'level'", "output": "'level'"},
-            {"input": "'raracece'", "output": "'raracececarar'"},
-            {"input": "'raceredder'", "output": "'raceredderecar'"},
-            {"input": "'abacabacaba'", "output": "'abacabacaba'"},
-            {"input": "'rrefrerace'", "output": "'rrefreracecarerferr'"},
-            {"input": "''", "output": "''"},
-        ],
-        "atol": 0,
-    }
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == [
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-    ]
-
-    # print results
-    print("++ All tests passed for test_unsafe_execute_multiple_def() ++")
-
-
-# test executing functions with escape characters in outputs
-def test_unsafe_execute_escape():
-    task = {
-        "problem": "def remove_vowels(text):\n    \"\"\"\n    remove_vowels is a function that takes string and returns string without vowels.\n    >>> remove_vowels('')\n    ''\n    >>> remove_vowels(\"abcdef\\nghijklm\")\n    'bcdf\\nghjklm'\n    >>> remove_vowels('abcdef')\n    'bcdf'\n    >>> remove_vowels('aaaaa')\n    ''\n    >>> remove_vowels('aaBAA')\n    'B'\n    >>> remove_vowels('zbcd')\n    'zbcd'\n    \"\"\"\n",
-        "contract": "\n    assert type(text) == str, \"invalid inputs\" # $_CONTRACT_$\n",
-        "function_name": "remove_vowels",
-        "model_solution": "\n    return \"\".join(list(filter(lambda ch: ch not in \"aeiouAEIOU\", text)))\n\n",
-        "tests": [
-            {"input": "''", "output": "''"},
-            {"input": "'abcdef\\nghijklm'", "output": "'bcdf\\nghjklm'"},
-            {"input": "'fedcba'", "output": "'fdcb'"},
-            {"input": "'eeeee'", "output": "''"},
-            {"input": "'acBAA'", "output": "'cB'"},
-            {"input": "'EcBOO'", "output": "'cB'"},
-            {"input": "'ybcd'", "output": "'ybcd'"},
-            {"input": "'hello'", "output": "'hll'"},
-            {"input": "'CX'", "output": "'CX'"},
-            {"input": "'AEEIayoubcd\\n\\n\\r\\t'", "output": "'ybcd\\n\\n\\r\\t'"},
-            {"input": "'\\n'", "output": "'\\n'"},
-            {"input": "'a'", "output": "''"},
-        ],
-        "atol": 0,
-    }
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == [
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-    ]
-
-    # print results
-    print("++ All tests passed for test_unsafe_execute_escape() ++")
-
-
-# test executing functions that will reulst in a timeout
-def test_unsafe_execute_timeout():
-    task = {
-        "problem": "def fib(n: int):\n    \"\"\"Return n-th Fibonacci number.\n    >>> fib(10)\n    55\n    >>> fib(1)\n    1\n    >>> fib(8)\n    21\n    \"\"\"\n",
-        "contract": "\n    assert n >= 0, \"invalid inputs\" # $_CONTRACT_$\n    assert isinstance(n, int), \"invalid inputs\" # $_CONTRACT_$\n",
-        "function_name": "fib",
-        "model_solution": "    if n <= 0:\n        return 0\n    elif n == 1:\n        return 1\n    else:\n        return fib(n-1) + fib(n-2)",
-        "tests": [
-            {"input": "10", "output": "55"},
-            {"input": "1", "output": "1"},
-            {"input": "8", "output": "21"},
-            {"input": "11", "output": "89"},
-            {"input": "12", "output": "144"},
-            {"input": "16", "output": "987"},
-            {"input": "0", "output": "0"},
-            {"input": "1", "output": "1"},
-            {"input": "3", "output": "2"},
-            {"input": "63", "output": "6557470319842"},
-            {"input": "2", "output": "1"},
-        ],
-        "atol": 0,
-    }
-
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == [
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Passed",
-        "Time Out",
-        "Passed",
-    ]
-
-    # print results
-    print("++ All tests passed for test_unsafe_execute_timeout() ++")
-
-
-# test executing functions with MBPP-reformatted Style test case format
-def test_unsafe_execute_MBPP():
-    task = {
-        "problem": "def first_repeated_char(str1):\n    \"\"\" Write a python function to find the first repeated character in a given string.\n    \"\"\"\n",
-        "contract": "",
-        "function_name": "first_repeated_char",
-        "model_solution": "    return 'a'",
-        "tests": [
-            "test_out = first_repeated_char(\"abcabc\")\nassert test_out == \"a\", f'outputs {test_out}'",
-            "test_out = first_repeated_char(\"abc\")\nassert test_out == None, f'outputs {test_out}'",
-            "test_out = first_repeated_char(\"123123\")\nassert test_out == \"1\", f'outputs {test_out}'",
-        ],
-        "atol": 0,
-    }
-    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
-    assert results == [
-        "Passed",
-        "AssertionError: outputs a",
-        "AssertionError: outputs a",
-    ]
-
-    os.makedirs("tmp", exist_ok=True)
-    g_unzip("data/MBPP-S_test_reformatted.jsonl.gz", "tmp/MBPP-S_test_reformatted.jsonl")
-    with open("tmp/MBPP-S_test_reformatted.jsonl", "r", encoding="utf-8") as reader:
-        tasks = reader.readlines()
-
-    for task in tasks:
-        task = json.loads(task)
-        test_task = {
-            "problem": task["problem"],
-            "contract": task["contract"],
-            "function_name": task["function_name"],
-            "model_solution": task["canonical_solution"],
-            "tests": task["tests"],
-            "atol": task["atol"],
-        }
-        results = unsafe_execute(test_task, mask_func_name=False, timeout=10)
-        for result in results:
-            assert result == "Passed"
-
-    # print results
-    print("++ All tests passed for test_unsafe_execute_MBPP() ++")
-
-
-# test executing functions with name masked
-def test_unsafe_execute_name_masked():
-    # Test Case Format 1: a dict of input and output (HumanEvalPlus Style)
-    task = {
-        "problem": "from typing import List\n\n\ndef func(paren_string: str) -> List[str]:\n    \"\"\" Input to this function is a string containing multiple groups of nested parentheses. Your goal is to\n    separate those group into separate strings and return the list of those.\n    Separate groups are balanced (each open brace is properly closed) and not nested within each other\n    Ignore any spaces in the input string.\n    >>> separate_paren_groups('( ) (( )) (( )( ))')\n    ['()', '(())', '(()())']\n    \"\"\"\n",
-        "contract": "\n    assert type(paren_string) == str, \"invalid inputs\" # $_CONTRACT_$\n    cnt = 0 # $_CONTRACT_$\n    for ch in paren_string: # $_CONTRACT_$\n        assert ch in [\"(\", \")\", \" \"], \"invalid inputs\"  # $_CONTRACT_$\n        if ch == \"(\": cnt += 1 # $_CONTRACT_$\n        if ch == \")\": cnt -= 1 # $_CONTRACT_$\n        assert cnt >= 0, \"invalid inputs\" # $_CONTRACT_$\n",
-        "function_name": "separate_paren_groups",
-        "model_solution": "\n\n    cnt, group, results = 0, \"\", []\n    for ch in paren_string:\n        if ch == \"(\": cnt += 1\n        if ch == \")\": cnt -= 1\n        if ch != \" \": group += ch\n        if cnt == 0:\n            if group != \"\": results.append(group)\n            group = \"\"\n    return results\n\n",
-        "tests": [
-            {
-                "input": "'(()()) ((())) () ((())()())'",
-                "output": "['(()())', '((()))', '()', '((())()())']",
-            },
-            {
-                "input": "'() (()) ((())) (((())))'",
-                "output": "['()', '(())', '((()))', '(((())))']",
-            },
-        ],
-        "atol": 0,
-    }
-
-    results = unsafe_execute(task, mask_func_name=True, timeout=0.5)
-    assert results == ["Passed", "Passed"]
-
-    # Test Case Format 2: a string of assertion statement (MBBP Style)
-    os.makedirs("tmp", exist_ok=True)
-    g_unzip("data/MBPP-S_test_reformatted.jsonl.gz", "tmp/MBPP-S_test_reformatted.jsonl")
-    with open("tmp/MBPP-S_test_reformatted.jsonl", "r", encoding="utf-8") as reader:
-        tasks = reader.readlines()
-
-    task = json.loads(tasks[0])
-    test_task = {
-        "problem": task["problem"].replace(task["function_name"], "func"),
-        "contract": task["contract"],
-        "function_name": task["function_name"],
-        "model_solution": task["canonical_solution"].replace(task["function_name"], "func"),
-        "tests": task["tests"],
-        "atol": task["atol"],
-    }
-    results = unsafe_execute(test_task, mask_func_name=True, timeout=5)
-    for result in results:
-        assert result == "Passed"
-
-    # print results
-    print("++ All tests passed for test_unsafe_execute_name_masked() ++")
-
-
-def main():
-    print("***********************************************")
-    print("** Running tests for module <executor.py> **")
-    print("-----------------------------------------------")
-    test_unsafe_execute()
-    test_unsafe_execute_atol()
-    test_unsafe_execute_multiple_def()
-    test_unsafe_execute_escape()
-    test_unsafe_execute_timeout()
-    test_unsafe_execute_MBPP()
-    test_unsafe_execute_name_masked()
-    print("-----------------------------------------------")
-    print("** All tests passed for module <executor.py> **")
-    print("***********************************************")
-
-
-if __name__ == "__main__":
-    main()
+# Authors: marcusm117
+# License: Apache 2.0
+
+
+# Standard Library Modules
+import json
+import os
+
+# Internal Modules
+from identitychain.utils import g_unzip
+
+# Internal Modules to be tested
+from identitychain import unsafe_execute
+
+
+def test_unsafe_execute():
+    task = {
+        "problem": "from typing import List\n\n\ndef separate_paren_groups(paren_string: str) -> List[str]:\n    \"\"\" Input to this function is a string containing multiple groups of nested parentheses. Your goal is to\n    separate those group into separate strings and return the list of those.\n    Separate groups are balanced (each open brace is properly closed) and not nested within each other\n    Ignore any spaces in the input string.\n    >>> separate_paren_groups('( ) (( )) (( )( ))')\n    ['()', '(())', '(()())']\n    \"\"\"\n",
+        "contract": "\n    assert type(paren_string) == str, \"invalid inputs\" # $_CONTRACT_$\n    cnt = 0 # $_CONTRACT_$\n    for ch in paren_string: # $_CONTRACT_$\n        assert ch in [\"(\", \")\", \" \"], \"invalid inputs\"  # $_CONTRACT_$\n        if ch == \"(\": cnt += 1 # $_CONTRACT_$\n        if ch == \")\": cnt -= 1 # $_CONTRACT_$\n        assert cnt >= 0, \"invalid inputs\" # $_CONTRACT_$\n",
+        "function_name": "separate_paren_groups",
+        "model_solution": "\n\n    cnt, group, results = 0, \"\", []\n    for ch in paren_string:\n        if ch == \"(\": cnt += 1\n        if ch == \")\": cnt -= 1\n        if ch != \" \": group += ch\n        if cnt == 0:\n            if group != \"\": results.append(group)\n            group = \"\"\n    return results\n\n",
+        "tests": [
+            {
+                "input": "'(()()) ((())) () ((())()())'",
+                "output": "['(()())', '((()))', '()', '((())()())']",
+            },
+            {
+                "input": "'() (()) ((())) (((())))'",
+                "output": "['()', '(())', '((()))', '(((())))']",
+            },
+        ],
+        "atol": 0,
+    }
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == ["Passed", "Passed"]
+
+    task["model_solution"] = "    return []"
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == [
+        "AssertionError: outputs []",
+        "AssertionError: outputs []",
+    ]
+
+    task["model_solution"] = "    return ['(()())', '((()))', '()', '((())()())']"
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == ["Passed", "AssertionError: outputs ['(()())', '((()))', '()', '((())()())']"]
+
+    # print results
+    print("++ All tests passed for test_unsafe_execute() ++")
+
+
+# test executing functions with float ouputs
+def test_unsafe_execute_atol():
+    task = {
+        "problem": "def truncate_number(number: float) -> float:\n    \"\"\" Given a positive floating point number, it can be decomposed into\n    and integer part (largest integer smaller than given number) and decimals\n    (leftover part always smaller than 1).\n\n    Return the decimal part of the number.\n    >>> truncate_number(3.5)\n    0.5\n    \"\"\"\n",
+        "contract": "\n    assert number > 0, \"invalid inputs\" # $_CONTRACT_$\n    assert isinstance(number, float), \"invalid inputs\" # $_CONTRACT_$\n",
+        "function_name": "truncate_number",
+        "model_solution": "\n\n    return number - int(number)\n\n",
+        "tests": [
+            {"input": "3.5", "output": "0.5"},
+            {"input": "1.33", "output": "0.33000000000000007"},
+            {"input": "123.456", "output": "0.45600000000000307"},
+            {"input": "999.99999", "output": "0.9999900000000252"},
+            {"input": "0.04320870526393539", "output": "0.04320870526393539"},
+            {"input": "1.0", "output": "0.0"},
+            {"input": "1e-323", "output": "1e-323"},
+            {"input": "1000000000.0", "output": "0.0"},
+        ],
+        "atol": 1e-06,
+    }
+
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == ["Passed", "Passed", "Passed", "Passed", "Passed", "Passed", "Passed", "Passed"]
+
+    task["model_solution"] = "    return 0.0"
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == [
+        "AssertionError: outputs 0.0",
+        "AssertionError: outputs 0.0",
+        "AssertionError: outputs 0.0",
+        "AssertionError: outputs 0.0",
+        "AssertionError: outputs 0.0",
+        "Passed",
+        "Passed",
+        "Passed",
+    ]
+
+    task["model_solution"] = "    return 0.5"
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == [
+        "Passed",
+        "AssertionError: outputs 0.5",
+        "AssertionError: outputs 0.5",
+        "AssertionError: outputs 0.5",
+        "AssertionError: outputs 0.5",
+        "AssertionError: outputs 0.5",
+        "AssertionError: outputs 0.5",
+        "AssertionError: outputs 0.5",
+    ]
+
+    # print results
+    print("++ All tests passed for test_unsafe_execute_atol() ++")
+
+
+# test executing functions with multiple def
+def test_unsafe_execute_multiple_def():
+    task = {
+        "problem": "def is_palindrome(string: str) -> bool:\n    \"\"\" Test if given string is a palindrome \"\"\"\n    return string == string[::-1]\n\n\ndef make_palindrome(string: str) -> str:\n    \"\"\" Find the shortest palindrome that begins with a supplied string.\n    Algorithm idea is simple:\n    - Find the longest postfix of supplied string that is a palindrome.\n    - Append to the end of the string reverse of a string prefix that comes before the palindromic suffix.\n    >>> make_palindrome('')\n    ''\n    >>> make_palindrome('cat')\n    'catac'\n    >>> make_palindrome('cata')\n    'catac'\n    \"\"\"\n",
+        "contract": "\n    assert type(string) == str, \"invalid inputs\" # $_CONTRACT_$\n",
+        "function_name": "make_palindrome",
+        "model_solution": "\n    if is_palindrome(string):\n        return string\n    for i in range(len(string)):\n        if is_palindrome(string[i:]):\n            return string + string[i-1::-1]\n\n",
+        "tests": [
+            {"input": "''", "output": "''"},
+            {"input": "'x'", "output": "'x'"},
+            {"input": "'xyz'", "output": "'xyzyx'"},
+            {"input": "'xyx'", "output": "'xyx'"},
+            {"input": "'jerry'", "output": "'jerryrrej'"},
+            {"input": "'race'", "output": "'racecar'"},
+            {"input": "'level'", "output": "'level'"},
+            {"input": "'raracece'", "output": "'raracececarar'"},
+            {"input": "'raceredder'", "output": "'raceredderecar'"},
+            {"input": "'abacabacaba'", "output": "'abacabacaba'"},
+            {"input": "'rrefrerace'", "output": "'rrefreracecarerferr'"},
+            {"input": "''", "output": "''"},
+        ],
+        "atol": 0,
+    }
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == [
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+    ]
+
+    # print results
+    print("++ All tests passed for test_unsafe_execute_multiple_def() ++")
+
+
+# test executing functions with escape characters in outputs
+def test_unsafe_execute_escape():
+    task = {
+        "problem": "def remove_vowels(text):\n    \"\"\"\n    remove_vowels is a function that takes string and returns string without vowels.\n    >>> remove_vowels('')\n    ''\n    >>> remove_vowels(\"abcdef\\nghijklm\")\n    'bcdf\\nghjklm'\n    >>> remove_vowels('abcdef')\n    'bcdf'\n    >>> remove_vowels('aaaaa')\n    ''\n    >>> remove_vowels('aaBAA')\n    'B'\n    >>> remove_vowels('zbcd')\n    'zbcd'\n    \"\"\"\n",
+        "contract": "\n    assert type(text) == str, \"invalid inputs\" # $_CONTRACT_$\n",
+        "function_name": "remove_vowels",
+        "model_solution": "\n    return \"\".join(list(filter(lambda ch: ch not in \"aeiouAEIOU\", text)))\n\n",
+        "tests": [
+            {"input": "''", "output": "''"},
+            {"input": "'abcdef\\nghijklm'", "output": "'bcdf\\nghjklm'"},
+            {"input": "'fedcba'", "output": "'fdcb'"},
+            {"input": "'eeeee'", "output": "''"},
+            {"input": "'acBAA'", "output": "'cB'"},
+            {"input": "'EcBOO'", "output": "'cB'"},
+            {"input": "'ybcd'", "output": "'ybcd'"},
+            {"input": "'hello'", "output": "'hll'"},
+            {"input": "'CX'", "output": "'CX'"},
+            {"input": "'AEEIayoubcd\\n\\n\\r\\t'", "output": "'ybcd\\n\\n\\r\\t'"},
+            {"input": "'\\n'", "output": "'\\n'"},
+            {"input": "'a'", "output": "''"},
+        ],
+        "atol": 0,
+    }
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == [
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+    ]
+
+    # print results
+    print("++ All tests passed for test_unsafe_execute_escape() ++")
+
+
+# test executing functions that will reulst in a timeout
+def test_unsafe_execute_timeout():
+    task = {
+        "problem": "def fib(n: int):\n    \"\"\"Return n-th Fibonacci number.\n    >>> fib(10)\n    55\n    >>> fib(1)\n    1\n    >>> fib(8)\n    21\n    \"\"\"\n",
+        "contract": "\n    assert n >= 0, \"invalid inputs\" # $_CONTRACT_$\n    assert isinstance(n, int), \"invalid inputs\" # $_CONTRACT_$\n",
+        "function_name": "fib",
+        "model_solution": "    if n <= 0:\n        return 0\n    elif n == 1:\n        return 1\n    else:\n        return fib(n-1) + fib(n-2)",
+        "tests": [
+            {"input": "10", "output": "55"},
+            {"input": "1", "output": "1"},
+            {"input": "8", "output": "21"},
+            {"input": "11", "output": "89"},
+            {"input": "12", "output": "144"},
+            {"input": "16", "output": "987"},
+            {"input": "0", "output": "0"},
+            {"input": "1", "output": "1"},
+            {"input": "3", "output": "2"},
+            {"input": "63", "output": "6557470319842"},
+            {"input": "2", "output": "1"},
+        ],
+        "atol": 0,
+    }
+
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == [
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Passed",
+        "Time Out",
+        "Passed",
+    ]
+
+    # print results
+    print("++ All tests passed for test_unsafe_execute_timeout() ++")
+
+
+# test executing functions with MBPP-reformatted Style test case format
+def test_unsafe_execute_MBPP():
+    task = {
+        "problem": "def first_repeated_char(str1):\n    \"\"\" Write a python function to find the first repeated character in a given string.\n    \"\"\"\n",
+        "contract": "",
+        "function_name": "first_repeated_char",
+        "model_solution": "    return 'a'",
+        "tests": [
+            "test_out = first_repeated_char(\"abcabc\")\nassert test_out == \"a\", f'outputs {test_out}'",
+            "test_out = first_repeated_char(\"abc\")\nassert test_out == None, f'outputs {test_out}'",
+            "test_out = first_repeated_char(\"123123\")\nassert test_out == \"1\", f'outputs {test_out}'",
+        ],
+        "atol": 0,
+    }
+    results = unsafe_execute(task, mask_func_name=False, timeout=0.5)
+    assert results == [
+        "Passed",
+        "AssertionError: outputs a",
+        "AssertionError: outputs a",
+    ]
+
+    os.makedirs("tmp", exist_ok=True)
+    g_unzip("data/MBPP-S_test_reformatted.jsonl.gz", "tmp/MBPP-S_test_reformatted.jsonl")
+    with open("tmp/MBPP-S_test_reformatted.jsonl", "r", encoding="utf-8") as reader:
+        tasks = reader.readlines()
+
+    for task in tasks:
+        task = json.loads(task)
+        test_task = {
+            "problem": task["problem"],
+            "contract": task["contract"],
+            "function_name": task["function_name"],
+            "model_solution": task["canonical_solution"],
+            "tests": task["tests"],
+            "atol": task["atol"],
+        }
+        results = unsafe_execute(test_task, mask_func_name=False, timeout=10)
+        for result in results:
+            assert result == "Passed"
+
+    # print results
+    print("++ All tests passed for test_unsafe_execute_MBPP() ++")
+
+
+# test executing functions with name masked
+def test_unsafe_execute_name_masked():
+    # Test Case Format 1: a dict of input and output (HumanEvalPlus Style)
+    task = {
+        "problem": "from typing import List\n\n\ndef func(paren_string: str) -> List[str]:\n    \"\"\" Input to this function is a string containing multiple groups of nested parentheses. Your goal is to\n    separate those group into separate strings and return the list of those.\n    Separate groups are balanced (each open brace is properly closed) and not nested within each other\n    Ignore any spaces in the input string.\n    >>> separate_paren_groups('( ) (( )) (( )( ))')\n    ['()', '(())', '(()())']\n    \"\"\"\n",
+        "contract": "\n    assert type(paren_string) == str, \"invalid inputs\" # $_CONTRACT_$\n    cnt = 0 # $_CONTRACT_$\n    for ch in paren_string: # $_CONTRACT_$\n        assert ch in [\"(\", \")\", \" \"], \"invalid inputs\"  # $_CONTRACT_$\n        if ch == \"(\": cnt += 1 # $_CONTRACT_$\n        if ch == \")\": cnt -= 1 # $_CONTRACT_$\n        assert cnt >= 0, \"invalid inputs\" # $_CONTRACT_$\n",
+        "function_name": "separate_paren_groups",
+        "model_solution": "\n\n    cnt, group, results = 0, \"\", []\n    for ch in paren_string:\n        if ch == \"(\": cnt += 1\n        if ch == \")\": cnt -= 1\n        if ch != \" \": group += ch\n        if cnt == 0:\n            if group != \"\": results.append(group)\n            group = \"\"\n    return results\n\n",
+        "tests": [
+            {
+                "input": "'(()()) ((())) () ((())()())'",
+                "output": "['(()())', '((()))', '()', '((())()())']",
+            },
+            {
+                "input": "'() (()) ((())) (((())))'",
+                "output": "['()', '(())', '((()))', '(((())))']",
+            },
+        ],
+        "atol": 0,
+    }
+
+    results = unsafe_execute(task, mask_func_name=True, timeout=0.5)
+    assert results == ["Passed", "Passed"]
+
+    # Test Case Format 2: a string of assertion statement (MBBP Style)
+    os.makedirs("tmp", exist_ok=True)
+    g_unzip("data/MBPP-S_test_reformatted.jsonl.gz", "tmp/MBPP-S_test_reformatted.jsonl")
+    with open("tmp/MBPP-S_test_reformatted.jsonl", "r", encoding="utf-8") as reader:
+        tasks = reader.readlines()
+
+    task = json.loads(tasks[0])
+    test_task = {
+        "problem": task["problem"].replace(task["function_name"], "func"),
+        "contract": task["contract"],
+        "function_name": task["function_name"],
+        "model_solution": task["canonical_solution"].replace(task["function_name"], "func"),
+        "tests": task["tests"],
+        "atol": task["atol"],
+    }
+    results = unsafe_execute(test_task, mask_func_name=True, timeout=5)
+    for result in results:
+        assert result == "Passed"
+
+    # print results
+    print("++ All tests passed for test_unsafe_execute_name_masked() ++")
+
+
+def main():
+    print("***********************************************")
+    print("** Running tests for module <executor.py> **")
+    print("-----------------------------------------------")
+    test_unsafe_execute()
+    test_unsafe_execute_atol()
+    test_unsafe_execute_multiple_def()
+    test_unsafe_execute_escape()
+    test_unsafe_execute_timeout()
+    test_unsafe_execute_MBPP()
+    test_unsafe_execute_name_masked()
+    print("-----------------------------------------------")
+    print("** All tests passed for module <executor.py> **")
+    print("***********************************************")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `identitychain-0.0.1/identitychain.egg-info/PKG-INFO` & `identitychain-0.1.0/identitychain.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,322 +1,337 @@
-Metadata-Version: 2.1
-Name: identitychain
-Version: 0.0.1
-Summary: Code Model Trust Evaluation
-Author-email: "marcusm117, Robin-Y-Ding" <authors@gmail.com>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: repository, https://github.com/marcusm117/
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
-# IdentityChain
-
-## Installation
-
-Create and Activate a Conda Environment.
-
-   ``` bash
-   conda create -n idchain python=3.10
-   conda activate idchain
-   ```
-
-Clone this Repository to your Local Environment.
-
-   ``` bash
-   git clone https://github.com/marcusm117/IdentityChain.git
-   ```
-
-Install the Library with all Dependencies.
-
-   ``` bash
-   cd IdentityChain
-   make develop
-   ```
-
-## Usage
-
-Before the self-consistency evaluation, you need to make sure that one of the followings is satisfied:
-
-1. Your model is an Instruction-tuned Code LLM, and it's trained on both NL-to-PL and PL-to-NL tasks.
-2. Your model is a Foundation Code LLM, and it's trained on both completion and fill-in-the-middle tasks.
-
-To evaluate your model using IdentityChain, you need to prepare the followings:
-
-1. An evaluation dataset in the format of one of the followings (you can also use these two directly):
-   - [EvalPlus-Mini-v0.1.6_reformatted.jsonl](./data/EvalPlus-Mini-v0.1.6_reformatted.jsonl.gz)
-   - [MBPP-S_test_reformatted.jsonl](./data/MBPP-S_test_reformatted.jsonl.gz)
-2. An NL-to-PL prompt for your model
-3. A PL-to-NL prompt for your model
-4. An NL-to-PL generation function for your model
-5. A PL-to-NL generation function for your model
-
-See [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) for an example of how to use IdentityChain to evaluate OpenAI models.
-
-See [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py) for an example of how to use IdentityChain to evaluate HuggingFace open-source models. This example script already includes the following models:
-
-1. CodeLlama-Instruct-hf (7B, 13B, 34B)
-2. CodeLlama-hf (7B, 13B, 34B)
-3. starchat-beta
-4. starcoder
-5. starcoderplus
-6. starcoderbase (1B, 3B, 7B, 15B)
-
-## Example
-
-Use [run_identity_chain.sh](./examples/run_identity_chain.sh) to execute scripts [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) or [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py), which conducts several IdentityChain evaluation in a batch. Make sure that you modify the followings before running the script:
-
-1. `export CUDA_VISIBLE_DEVICES=0` to specify the local GPU device you want to use
-2. `export HF_HOME=YOUR_OWN_PATH/huggingface` to specify your own huggingface home path, where the model checkpoints will be cached
-3. `export IDENTITY_CHAIN_HOME=YOUR_OWN_PATH/IdentityChain` to your own IdentityChain home path
-4. other parameters in the script for your own needs
-
-Then run the script:
-
-``` bash
-cd examples
-bash run_identity_chain.sh
-```
-
-This script will create a temporary folder `tmp` under your IdentityChain home path, and store the results of IdentityChain evaluation in this folder, which will be a `jsonl` file. For example, `tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl`.
-
-Use [analyze_results.py](./scripts/analyze_results.py) to analyze the results of IdentityChain evaluation. It will geneartes an `xlsx` file, which contains the following information:
-
-1. The SC (Self-Consistency) and SSC (Strong Self-Consistency) scores of the model at each self-iteration step. Note that SSC_0 is just Pass@1
-2. The aggregated TOM score (also BLEU and CodeBLEU) information at each step for the following 4 types of resulsts: Pass-Pass, Pass-Fail, Fail-Fail, Fail-Pass
-3. The TOM score (also BLEU and CodeBLEU) trajectory at each self-iteration step for each sample in the eavluation set.
-4. The raw test case outputs at each self-iteration step
-
-``` bash
-cd ../scripts
-python analyze_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5
-```
-
-The analyzed results will give you a sense of the model's overall performance, and the TOM score trajectory will help you pinpoint the exact step where the model makes a mistake.
-
-Use [browse_results.py](./scripts/browse_results.py) to browse the results of IdentityChain evaluation. You can use this script to manually examine and study the mistakes made by the model for specific samples.
-
-``` bash
-cd ../scripts
-python browse_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5 --start 0
-```
-
-## Linting & Testing
-
-We use a `Makefile` as a command registry:
-
-- `make format`: autoformat  this library with `black`
-- `make lint`: perform static analysis of this library with `black` and `flake8`
-- `make annotate`: run type checking using `mypy`
-- `make test`: run automated tests
-- `make check`: check assets for packaging
-
-Make sure that `make lint`, `make test`, and `make check` all pass locally before submitting a Pull Request.
+Metadata-Version: 2.1
+Name: identitychain
+Version: 0.1.0
+Summary: Evaluation Framework for Code Large Language Models (Code LLMs)
+Author-email: "marcusm117, Robin-Y-Ding" <authors@gmail.com>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: repository, https://github.com/marcusm117/IdentityChain/
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+License-File: LICENSE
+
+# IdentityChain
+
+[![PyPI](https://img.shields.io/pypi/v/identitychain?color=blue&label=PyPI)](https://pypi.org/project/identitychain/) [![CI](https://github.com/marcusm117/IdentityChain/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/marcusm117/IdentityChain/actions/workflows/build.yml) [![License](https://img.shields.io/badge/License-Apache_2.0-green)](https://github.com/marcusm117/IdentityChain/blob/main/LICENSE) [![Issues](https://img.shields.io/github/issues/marcusm117/IdentityChain?color=red&label=Issues)](https://github.com/marcusm117/IdentityChain/issues)
+
+The IdentityChain Framework for Code Large Language Models (Code LLMs) Evaluation. Official implementation of the ICLR 2024 paper [Beyond Accuracy: Evaluating Self-Consistency of Code Large Language Models with IdentityChain](https://arxiv.org/abs/2310.14053).
+
+The IdentityChain Framework evaluates the NL-to-PL (Code Generation) Accuracy, PL-to-NL (Code Summurization) Accuracy, and the Self-Consistency across the two tasks. It also provides a fine-grained analysis of the model's performance so that you can pinpoint the exact step and problem where the model makes a self-inconsistency violation.
+
+<img src="./images/main.png" alt="image" width="800" height="auto">
+
+## Installation
+
+Create and Activate a Conda Environment.
+
+   ``` bash
+   conda create -n idchain python=3.10
+   conda activate idchain
+   ```
+
+Install from PyPI with all Dependencies.
+
+   ``` bash
+   pip3 install identitychain
+   pip3 install -r requirements.txt
+   ```
+
+Install from Source with all Dependencies.
+
+   ``` bash
+   git clone https://github.com/marcusm117/IdentityChain.git
+   cd IdentityChain
+   make develop
+   ```
+
+## Usage
+
+Before the self-consistency evaluation, you need to make sure that one of the followings is satisfied:
+
+1. Your model is an Instruction-tuned Code LLM, and it's trained on both NL-to-PL and PL-to-NL tasks.
+2. Your model is a Foundation Code LLM, and it's trained on both completion and fill-in-the-middle tasks.
+
+To evaluate your model using IdentityChain, you need to prepare the followings:
+
+1. An evaluation dataset from one of the followings (or one of your own in the same format):
+   - [EvalPlus-Mini-v0.1.6_reformatted.jsonl](./data/EvalPlus-Mini-v0.1.6_reformatted.jsonl.gz)
+   - [EvalPlus-Mini-v0.1.10_reformatted.jsonl](./data/EvalPlus-Mini-v0.1.10_reformatted.jsonl.gz)
+   - [MBPP-S_test_reformatted.jsonl](./data/MBPP-S_test_reformatted.jsonl.gz)
+2. An NL-to-PL prompt for your model
+3. A PL-to-NL prompt for your model
+4. An NL-to-PL generation function for your model
+5. A PL-to-NL generation function for your model
+
+See [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) for an example of how to use IdentityChain to evaluate OpenAI models.
+
+See [run_identity_chain_google.py](./examples/run_identity_chain_google.py) for an example of how to use IdentityChain to evaluate Google models.
+
+See [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py) for an example of how to use IdentityChain to evaluate HuggingFace open-source models. This example script already includes the following models:
+
+1. CodeLlama-Instruct-hf (7B, 13B, 34B, 70B)
+2. CodeLlama-hf (7B, 13B, 34B, 70B)
+3. StarChat-Beta
+4. StarCoder
+5. StarCoderPlus
+6. StarCoderBase (1B, 3B, 7B, 15B)
+7. DeepSeekCoder-Instruct (1.3B, 6.7B, 33B, 7B-v1.5)
+8. DeepSeekCoder (1.3B, 6.7B, 33B, 7B-v1.5)
+
+## Example
+
+Use [run_identity_chain.sh](./examples/run_identity_chain.sh) to execute scripts [run_identity_chain_openai.py](./examples/run_identity_chain_openai.py) or [run_identity_chain_huggingface.py](./examples/run_identity_chain_huggingface.py), which conducts several IdentityChain evaluation in a batch. Make sure that you modify the followings before running the script:
+
+1. `export CUDA_VISIBLE_DEVICES=0` to specify the local GPU device you want to use
+2. `export HF_HOME=YOUR_OWN_PATH/huggingface` to specify your own huggingface home path, where the model checkpoints will be cached
+3. `export IDENTITY_CHAIN_HOME=YOUR_OWN_PATH/IdentityChain` to your own IdentityChain home path
+4. other parameters in the script for your own needs
+
+Then run the script:
+
+``` bash
+cd examples
+bash run_identity_chain.sh
+```
+
+This script will create a temporary folder `tmp` under your IdentityChain home path, and store the results of IdentityChain evaluation in this folder, which will be a `jsonl` file. For example, `tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl`.
+
+Use [analyze_results.py](./scripts/analyze_results.py) to analyze the results of IdentityChain evaluation. It will geneartes an `xlsx` file, which contains the following information:
+
+1. The SC (Self-Consistency) and SSC (Strong Self-Consistency) scores of the model at each self-iteration step. Note that SSC_0 is just Pass@1
+2. The aggregated TOM score (also BLEU and CodeBLEU) information at each step for the following 4 types of resulsts: Pass-Pass, Pass-Fail, Fail-Fail, Fail-Pass
+3. The TOM score (also BLEU and CodeBLEU) trajectory at each self-iteration step for each sample in the eavluation set.
+4. The raw test case outputs at each self-iteration step
+
+``` bash
+cd ../scripts
+python analyze_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5
+```
+
+The analyzed results will give you a sense of the model's overall performance, and the TOM score trajectory will help you pinpoint the exact step where the model makes a mistake.
+
+Use [browse_results.py](./scripts/browse_results.py) to browse the results of IdentityChain evaluation. You can use this script to manually examine and study the mistakes made by the model for specific samples.
+
+``` bash
+cd ../scripts
+python browse_results.py --input_path ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl --chain_length 5 --start 0
+```
+
+## Linting & Testing
+
+We use a `Makefile` as a command registry:
+
+- `make format`: autoformat  this library with `black`
+- `make lint`: perform static analysis of this library with `black` and `flake8`
+- `make annotate`: run type checking using `mypy`
+- `make test`: run automated tests
+- `make check`: check assets for packaging
+
+Make sure that `make lint`, `make test`, and `make check` all pass locally before submitting a Pull Request.
```

### Comparing `identitychain-0.0.1/identitychain.egg-info/SOURCES.txt` & `identitychain-0.1.0/identitychain.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 examples/run_identity_chain.sh
+examples/run_identity_chain_google.py
 examples/run_identity_chain_huggingface.py
 examples/run_identity_chain_openai.py
 identitychain/__init__.py
 identitychain/dialogue.py
 identitychain/executor.py
 identitychain/identity_chain.py
 identitychain/utils.py
 identitychain.egg-info/PKG-INFO
 identitychain.egg-info/SOURCES.txt
 identitychain.egg-info/dependency_links.txt
 identitychain.egg-info/requires.txt
 identitychain.egg-info/top_level.txt
 identitychain/tests/test_executor.py
+images/main.png
 scripts/analyze_results.py
 scripts/browse_results.py
 scripts/reformat_EvalPlus.py
 scripts/reformat_MBPP-S.py
 scripts/run_tests.sh
 scripts/human_judge/analyze_results_hj.py
 scripts/human_judge/browse_samples.py
```

### Comparing `identitychain-0.0.1/scripts/browse_results.py` & `identitychain-0.1.0/scripts/browse_results.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# Authors: marcusm117
-# License: Apache 2.0
-
-
-# Standard Library Modules
-import argparse
-import json
-
-
-# EXAMPLE USAGE:
-# python browse_results.py --input_path
-# ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl
-# --chain_length 5 --start 0
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--input_path", type=str, required=True)
-    parser.add_argument("--start", type=int, default=0)
-    parser.add_argument("--chain_length", type=int, default=1)
-    args = parser.parse_args()
-
-    # read the Identity Chain results
-    with open(args.input_path, "r", encoding="utf-8") as reader:
-        tasks = reader.readlines()
-
-    for task in tasks[args.start :]:
-        input("Press Enter to continue...")
-        task = json.loads(task)
-        print("*****************************************")
-        print(f"Task: {task['task_id']}")
-        print("-----------------------------------------")
-        print(f"++ Description NL_0 & Solution PL_0 ++:\n\n{task['NL_0']}{task['contract']}\n{task['PL_0']}\n")
-        print("-----------------------------------------")
-        print(f"++ Tests ++:\n\n{task['tests']}")
-        print("-----------------------------------------")
-        print(f"++ Solution PL_0 Test Result ++:\n\n{task['PL_0_results']}\n")
-        for i in range(1, args.chain_length + 1):
-            if task[f"NL_{i}"] == "NA":
-                break
-            print("-----------------------------------------")
-            print(
-                f"++ Description NL_{i} & Solution PL_{i} ++:\n\n{task['function_signature']}"
-                + task[f"NL_{i}"]
-                + "\n"
-                + task[f"PL_{i}"]
-                + "\n"
-            )
-            print("-----------------------------------------")
-            print(f"++ Solution PL_{i} Test Result ++:\n\n" + str(task[f"PL_{i}_results"]) + "\n")
-        print("*****************************************")
-
-
-if __name__ == "__main__":
-    main()
+# Authors: marcusm117
+# License: Apache 2.0
+
+
+# Standard Library Modules
+import argparse
+import json
+
+
+# EXAMPLE USAGE:
+# python browse_results.py --input_path
+# ../tmp/starcoderbase-1b/IDChain_starcoderbase-1b_tmp0.0g_len5_pb_all_m_v1_EvalPlus-Mini-v0.1.6_reformatted.jsonl
+# --chain_length 5 --start 0
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--input_path", type=str, required=True)
+    parser.add_argument("--start", type=int, default=0)
+    parser.add_argument("--chain_length", type=int, default=1)
+    args = parser.parse_args()
+
+    # read the Identity Chain results
+    with open(args.input_path, "r", encoding="utf-8") as reader:
+        tasks = reader.readlines()
+
+    for task in tasks[args.start :]:
+        input("Press Enter to continue...")
+        task = json.loads(task)
+        print("*****************************************")
+        print(f"Task: {task['task_id']}")
+        print("-----------------------------------------")
+        print(f"++ Description NL_0 & Solution PL_0 ++:\n\n{task['NL_0']}{task['contract']}\n{task['PL_0']}\n")
+        print("-----------------------------------------")
+        print(f"++ Tests ++:\n\n{task['tests']}")
+        print("-----------------------------------------")
+        print(f"++ Solution PL_0 Test Result ++:\n\n{task['PL_0_results']}\n")
+        for i in range(1, args.chain_length + 1):
+            if task[f"NL_{i}"] == "NA":
+                break
+            print("-----------------------------------------")
+            print(
+                f"++ Description NL_{i} & Solution PL_{i} ++:\n\n{task['function_signature']}"
+                + task[f"NL_{i}"]
+                + "\n"
+                + task[f"PL_{i}"]
+                + "\n"
+            )
+            print("-----------------------------------------")
+            print(f"++ Solution PL_{i} Test Result ++:\n\n" + str(task[f"PL_{i}_results"]) + "\n")
+        print("*****************************************")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `identitychain-0.0.1/scripts/human_judge/browse_samples.py` & `identitychain-0.1.0/scripts/human_judge/browse_samples.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# Authors: marcusm117
-# License: Apache 2.0
-
-
-# Standard Library Modules
-import argparse
-import json
-import os
-
-# Internal Modules
-from identitychain.utils import g_unzip
-
-
-# EXAMPLE USAGE:
-# python browse_samples.py --start 0
-def main():
-    # unzip the raw experiment results to a temporary directory
-    tmp_dir = "../../tmp"
-    os.makedirs(tmp_dir, exist_ok=True)
-    input_file = "IDChain_gpt-3.5-turbo-0613_tmp0_len1_pb_all_m_human-judge_EvalPlus-Mini-v0.1.6_reformatted.jsonl"
-    input_path = f"{tmp_dir}/{input_file}"
-    g_unzip(f"../../data/experiments/{input_file}.gz", input_path)
-
-    # you can used this script to browse results of other Human Judgment experiments results
-    # for that purpose, you can specify the command line argument --input_path
-    # by default, we will browse the samples of the above experiment
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--input_path", type=str, default=input_path)
-    parser.add_argument("--start", type=int, default=0)
-    args = parser.parse_args()
-
-    # read the Identity Chain results
-    with open(input_path, "r", encoding="utf-8") as reader:
-        tasks = reader.readlines()
-
-    for task in tasks[args.start :]:
-        input("Press Enter to continue...")
-        task = json.loads(task)
-        function_name = task["function_name"]
-        function_signature = task["function_signature"]
-        masked_function_signature = function_signature.replace(function_name, "func")
-        print("*****************************************")
-        print(f"Task: {task['task_id']}")
-        print("-----------------------------------------")
-        print("++ PL, Implementation of a Function ++:")
-        print("-----------------------------------------")
-        print(f"\n{masked_function_signature}\n{task['PL_0']}\n")
-        print("-----------------------------------------")
-        print("++ NL, Docstring of a Function ++:")
-        print("-----------------------------------------")
-        print(f"\n{masked_function_signature}\n{task['NL_1']}\n")
-        print("*****************************************")
-
-
-if __name__ == "__main__":
-    main()
+# Authors: marcusm117
+# License: Apache 2.0
+
+
+# Standard Library Modules
+import argparse
+import json
+import os
+
+# Internal Modules
+from identitychain.utils import g_unzip
+
+
+# EXAMPLE USAGE:
+# python browse_samples.py --start 0
+def main():
+    # unzip the raw experiment results to a temporary directory
+    tmp_dir = "../../tmp"
+    os.makedirs(tmp_dir, exist_ok=True)
+    input_file = "IDChain_gpt-3.5-turbo-0613_tmp0_len1_pb_all_m_human-judge_EvalPlus-Mini-v0.1.6_reformatted.jsonl"
+    input_path = f"{tmp_dir}/{input_file}"
+    g_unzip(f"../../data/experiments/{input_file}.gz", input_path)
+
+    # you can used this script to browse results of other Human Judgment experiments results
+    # for that purpose, you can specify the command line argument --input_path
+    # by default, we will browse the samples of the above experiment
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--input_path", type=str, default=input_path)
+    parser.add_argument("--start", type=int, default=0)
+    args = parser.parse_args()
+
+    # read the Identity Chain results
+    with open(input_path, "r", encoding="utf-8") as reader:
+        tasks = reader.readlines()
+
+    for task in tasks[args.start :]:
+        input("Press Enter to continue...")
+        task = json.loads(task)
+        function_name = task["function_name"]
+        function_signature = task["function_signature"]
+        masked_function_signature = function_signature.replace(function_name, "func")
+        print("*****************************************")
+        print(f"Task: {task['task_id']}")
+        print("-----------------------------------------")
+        print("++ PL, Implementation of a Function ++:")
+        print("-----------------------------------------")
+        print(f"\n{masked_function_signature}\n{task['PL_0']}\n")
+        print("-----------------------------------------")
+        print("++ NL, Docstring of a Function ++:")
+        print("-----------------------------------------")
+        print(f"\n{masked_function_signature}\n{task['NL_1']}\n")
+        print("*****************************************")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `identitychain-0.0.1/scripts/human_judge/compute_correlation.py` & `identitychain-0.1.0/scripts/human_judge/compute_correlation.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-# Authors: marcusm117
-# License: Apache 2.0
-
-
-# Standard Library Modules
-import argparse
-
-# External Modules
-import pandas as pd
-import scipy.stats
-
-
-# calculate Pearson, Spearman, and Kendall-Tau correlations
-def calculate_correlation(x, y):
-    pearson_cor = scipy.stats.pearsonr(x, y)  # Pearson's r
-    spearman_cor = scipy.stats.spearmanr(x, y)  # Spearman's rho
-    kendall_tau_cor = scipy.stats.kendalltau(x, y)  # Kendall's tau
-    return pearson_cor, spearman_cor, kendall_tau_cor
-
-
-# EXAMPLE USAGE:
-# python compute_correlation.py --gt_path ../../tmp/Human_Judge_GT.xlsx
-# --metric_path ../../tmp/IDChain_gpt-3.5-turbo-0613_tmp0_len1_pb_all_m_human-judge_EvalPlus-Mini-v0.1.6_reformatted.jsonl.xlsx
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--gt_path", type=str, required=True)
-    parser.add_argument("--metric_path", type=str, required=True)
-    parser.add_argument("--output_path", type=str, default=None)
-    args = parser.parse_args()
-
-    # load the GT and analyzed results for various metrics
-    gt_df = pd.read_excel(args.gt_path, sheet_name="gt", header=1)
-    metric_df = pd.read_excel(args.metric_path, sheet_name="traj", header=1)
-
-    # if PL0 pass, NL0 can seen as a Ground Truth reference for NL1, we can evaluate NL1 in both NL and PL space
-    # otherwise, NL1 doesn't have a Ground Truth reference, we can only evaluate NL1 in PL space
-    # therefore, we handle the above 2 case separately
-    # create filter conditions
-    filter_condition1 = metric_df["Summary"] == "Pass-Pass"
-    filter_condition2 = metric_df["Summary"] == "Pass-Fail"
-    filter_condiiton3 = metric_df["Summary"] == "Fail-Pass"
-    filter_condition4 = metric_df["Summary"] == "Fail-Fail"
-    # we will calculate correlation separately for "PL0 Pass" and "PL0 Fail" samples
-    metric_df_pass = metric_df[filter_condition1 | filter_condition2]
-    gt_df_pass = gt_df[filter_condition1 | filter_condition2]
-    metric_df_fail = metric_df[filter_condiiton3 | filter_condition4]
-    gt_df_fail = gt_df[filter_condiiton3 | filter_condition4]
-
-    # sanity check
-    print(f"Number of PL0 Pass Samples: {len(metric_df_pass)}")
-    print(f"Number of PL0 Fail Samples: {len(metric_df_fail)}")
-
-    # creat DataFrames to store the correlation results
-    # we have Ground Truth (GT) and Relaxed Ground Truth (Relaxed GT)
-    # Relaxed GT means in the docstring, nl description is correct, but some of the examples wrong
-    cor_gt_pass = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
-    cor_relaxed_gt_pass = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
-    cor_gt_fail = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
-    cor_relaxed_gt_fail = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
-    cor_gt_all = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
-    cor_relaxed_gt_all = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
-
-    # correlation between GT and metrics
-    for case in ["Pass", "Fail", "All"]:
-        # if PL0 pass, we can see NL0 as the Ground Truth for PL1, we can evaluate in both NL and PL space
-        if case == "Pass":
-            gt = gt_df_pass["Ground Truth"].astype(float)
-            relaxed_gt = gt_df_pass["Relaxed GT"].astype(float)
-            # we have 6 NL space metrics
-            bleu_NL = metric_df_pass["BLEU-NL"].astype(float)
-            chrF_NL = metric_df_pass["chrF-NL"].astype(float)
-            rouge_1_NL = metric_df_pass["ROUGE-1-NL"].astype(float)
-            rouge_2_NL = metric_df_pass["ROUGE-2-NL"].astype(float)
-            rouge_L_NL = metric_df_pass["ROUGE-L-NL"].astype(float)
-            bertscore_NL = metric_df_pass["BERTScore-NL"].astype(float)
-            # we have 4 PL space metrics
-            em_PL = metric_df_pass["EM-PL"].astype(float)
-            codebleu = metric_df_pass["CodeBLEU"].astype(float)
-            pfm = metric_df_pass["P/FM"].astype(float)
-            tom = metric_df_pass["TOM"].astype(float)
-        # if PL0 fail, we have no Ground Truth for NL1, we can only evaluate in PL space
-        else:
-            # if case = "All", we will calculate correlation for samples that PL0 fails
-            if case == "Fail":
-                gt = gt_df_fail["Ground Truth"].astype(float)
-                relaxed_gt = gt_df_fail["Relaxed GT"].astype(float)
-                # we have 4 PL space metrics
-                em_PL = metric_df_fail["EM-PL"].astype(float)
-                codebleu = metric_df_fail["CodeBLEU"].astype(float)
-                pfm = metric_df_fail["P/FM"].astype(float)
-                tom = metric_df_fail["TOM"].astype(float)
-            # if case = "All", we will calculate correlation for all samples
-            else:
-                gt = gt_df["Ground Truth"].astype(float)
-                relaxed_gt = gt_df["Relaxed GT"].astype(float)
-                # we have 4 PL space metrics
-                em_PL = metric_df["EM-PL"].astype(float)
-                codebleu = metric_df["CodeBLEU"].astype(float)
-                pfm = metric_df["P/FM"].astype(float)
-                tom = metric_df["TOM"].astype(float)
-            # we don't have NL space metrics
-            bleu_NL = None
-            chrF_NL = None
-            rouge_1_NL = None
-            rouge_2_NL = None
-            rouge_L_NL = None
-            bertscore_NL = None
-
-        # we have Ground Truth (GT) and Relaxed Ground Truth (Relaxed GT)
-        # Relaxed GT means in the docstring, nl description is correct, but some of the examples wrong
-        for gt_type in ["GT", "Relaxed GT"]:
-            # list lout all the metrics we want to compute correlation with
-            if case == "Pass":
-                metrics = {
-                    "BLEU-NL": bleu_NL,
-                    "chrF-NL": chrF_NL,
-                    "ROUGE-1-NL": rouge_1_NL,
-                    "ROUGE-2-NL": rouge_2_NL,
-                    "ROUGE-L-NL": rouge_L_NL,
-                    "BERTScore-NL": bertscore_NL,
-                    "EM-PL": em_PL,
-                    "CodeBLEU": codebleu,
-                    "P/FM": pfm,
-                    "TOM": tom,
-                }
-            # if PL0 fail, we don't have NL space metrics
-            else:
-                metrics = {
-                    "EM-PL": em_PL,
-                    "CodeBLEU": codebleu,
-                    "P/FM": pfm,
-                    "TOM": tom,
-                }
-
-            # for each metric, calculate correlation with GT or Relaxed GT
-            for metric_name, metric_result in metrics.items():
-                print("==========================================")
-                print(f"Correlation between {gt_type} and {metric_name}:")
-                if gt_type == "GT":
-                    pearson_cor, spearman_cor, kendall_tau_cor = calculate_correlation(gt, metric_result)
-                else:
-                    pearson_cor, spearman_cor, kendall_tau_cor = calculate_correlation(relaxed_gt, metric_result)
-
-                print("-----------------------------------------")
-                print(f"Pearson's r: {pearson_cor}")
-                print(f"Spearman's rho: {spearman_cor}")
-                print(f"Kendall's tau: {kendall_tau_cor}")
-                print("==========================================")
-                # add row to the corresponding DataFrame
-                row = {
-                    "Metric": metric_name,
-                    "Pearson's r": pearson_cor[0],
-                    "Spearman's rho": spearman_cor[0],
-                    "Kendall's tau": kendall_tau_cor[0],
-                }
-                if gt_type == "GT":
-                    if case == "Pass":
-                        cor_gt_pass = pd.concat([cor_gt_pass, pd.DataFrame([row])], ignore_index=True)
-                    elif case == "Fail":
-                        cor_gt_fail = pd.concat([cor_gt_fail, pd.DataFrame([row])], ignore_index=True)
-                    else:
-                        cor_gt_all = pd.concat([cor_gt_all, pd.DataFrame([row])], ignore_index=True)
-                else:
-                    if case == "Pass":
-                        cor_relaxed_gt_pass = pd.concat([cor_relaxed_gt_pass, pd.DataFrame([row])], ignore_index=True)
-                    elif case == "Fail":
-                        cor_relaxed_gt_fail = pd.concat([cor_relaxed_gt_fail, pd.DataFrame([row])], ignore_index=True)
-                    else:
-                        cor_relaxed_gt_all = pd.concat([cor_relaxed_gt_all, pd.DataFrame([row])], ignore_index=True)
-
-            print("\n**********************************************************************************\n")
-
-    # write correlation statistics to excel
-    if args.output_path is None:
-        output_path = "Human_Judge_Correlation.xlsx"
-    else:
-        output_path = args.output_path
-    with pd.ExcelWriter(output_path) as writer:
-        gt_df.to_excel(writer, sheet_name="gt", index=False, startrow=1, startcol=1, engine="xlsxwriter")
-        metric_df.to_excel(writer, sheet_name="traj", index=False, startrow=1, startcol=1, engine="xlsxwriter")
-        cor_gt_pass.to_excel(writer, sheet_name="cor_gt_pass", index=False, startrow=1, startcol=1, engine="xlsxwriter")
-        cor_relaxed_gt_pass.to_excel(
-            writer, sheet_name="cor_relaxed_gt_pass", index=False, startrow=1, startcol=1, engine="xlsxwriter"
-        )
-        cor_gt_fail.to_excel(writer, sheet_name="cor_gt_fail", index=False, startrow=1, startcol=1, engine="xlsxwriter")
-        cor_relaxed_gt_fail.to_excel(
-            writer, sheet_name="cor_relaxed_gt_fail", index=False, startrow=1, startcol=1, engine="xlsxwriter"
-        )
-        cor_gt_all.to_excel(writer, sheet_name="cor_gt_all", index=False, startrow=1, startcol=1, engine="xlsxwriter")
-        cor_relaxed_gt_all.to_excel(
-            writer, sheet_name="cor_relaxed_gt_all", index=False, startrow=1, startcol=1, engine="xlsxwriter"
-        )
-
-
-if __name__ == "__main__":
-    main()
+# Authors: marcusm117
+# License: Apache 2.0
+
+
+# Standard Library Modules
+import argparse
+
+# External Modules
+import pandas as pd
+import scipy.stats
+
+
+# calculate Pearson, Spearman, and Kendall-Tau correlations
+def calculate_correlation(x, y):
+    pearson_cor = scipy.stats.pearsonr(x, y)  # Pearson's r
+    spearman_cor = scipy.stats.spearmanr(x, y)  # Spearman's rho
+    kendall_tau_cor = scipy.stats.kendalltau(x, y)  # Kendall's tau
+    return pearson_cor, spearman_cor, kendall_tau_cor
+
+
+# EXAMPLE USAGE:
+# python compute_correlation.py --gt_path ../../tmp/Human_Judge_GT.xlsx
+# --metric_path ../../tmp/IDChain_gpt-3.5-turbo-0613_tmp0_len1_pb_all_m_human-judge_EvalPlus-Mini-v0.1.6_reformatted.jsonl.xlsx
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--gt_path", type=str, required=True)
+    parser.add_argument("--metric_path", type=str, required=True)
+    parser.add_argument("--output_path", type=str, default=None)
+    args = parser.parse_args()
+
+    # load the GT and analyzed results for various metrics
+    gt_df = pd.read_excel(args.gt_path, sheet_name="gt", header=1)
+    metric_df = pd.read_excel(args.metric_path, sheet_name="traj", header=1)
+
+    # if PL0 pass, NL0 can seen as a Ground Truth reference for NL1, we can evaluate NL1 in both NL and PL space
+    # otherwise, NL1 doesn't have a Ground Truth reference, we can only evaluate NL1 in PL space
+    # therefore, we handle the above 2 case separately
+    # create filter conditions
+    filter_condition1 = metric_df["Summary"] == "Pass-Pass"
+    filter_condition2 = metric_df["Summary"] == "Pass-Fail"
+    filter_condiiton3 = metric_df["Summary"] == "Fail-Pass"
+    filter_condition4 = metric_df["Summary"] == "Fail-Fail"
+    # we will calculate correlation separately for "PL0 Pass" and "PL0 Fail" samples
+    metric_df_pass = metric_df[filter_condition1 | filter_condition2]
+    gt_df_pass = gt_df[filter_condition1 | filter_condition2]
+    metric_df_fail = metric_df[filter_condiiton3 | filter_condition4]
+    gt_df_fail = gt_df[filter_condiiton3 | filter_condition4]
+
+    # sanity check
+    print(f"Number of PL0 Pass Samples: {len(metric_df_pass)}")
+    print(f"Number of PL0 Fail Samples: {len(metric_df_fail)}")
+
+    # creat DataFrames to store the correlation results
+    # we have Ground Truth (GT) and Relaxed Ground Truth (Relaxed GT)
+    # Relaxed GT means in the docstring, nl description is correct, but some of the examples wrong
+    cor_gt_pass = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
+    cor_relaxed_gt_pass = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
+    cor_gt_fail = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
+    cor_relaxed_gt_fail = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
+    cor_gt_all = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
+    cor_relaxed_gt_all = pd.DataFrame(columns=["Metric", "Pearson's r", "Spearman's rho", "Kendall's tau"])
+
+    # correlation between GT and metrics
+    for case in ["Pass", "Fail", "All"]:
+        # if PL0 pass, we can see NL0 as the Ground Truth for PL1, we can evaluate in both NL and PL space
+        if case == "Pass":
+            gt = gt_df_pass["Ground Truth"].astype(float)
+            relaxed_gt = gt_df_pass["Relaxed GT"].astype(float)
+            # we have 6 NL space metrics
+            bleu_NL = metric_df_pass["BLEU-NL"].astype(float)
+            chrF_NL = metric_df_pass["chrF-NL"].astype(float)
+            rouge_1_NL = metric_df_pass["ROUGE-1-NL"].astype(float)
+            rouge_2_NL = metric_df_pass["ROUGE-2-NL"].astype(float)
+            rouge_L_NL = metric_df_pass["ROUGE-L-NL"].astype(float)
+            bertscore_NL = metric_df_pass["BERTScore-NL"].astype(float)
+            # we have 4 PL space metrics
+            em_PL = metric_df_pass["EM-PL"].astype(float)
+            codebleu = metric_df_pass["CodeBLEU"].astype(float)
+            pfm = metric_df_pass["P/FM"].astype(float)
+            tom = metric_df_pass["TOM"].astype(float)
+        # if PL0 fail, we have no Ground Truth for NL1, we can only evaluate in PL space
+        else:
+            # if case = "All", we will calculate correlation for samples that PL0 fails
+            if case == "Fail":
+                gt = gt_df_fail["Ground Truth"].astype(float)
+                relaxed_gt = gt_df_fail["Relaxed GT"].astype(float)
+                # we have 4 PL space metrics
+                em_PL = metric_df_fail["EM-PL"].astype(float)
+                codebleu = metric_df_fail["CodeBLEU"].astype(float)
+                pfm = metric_df_fail["P/FM"].astype(float)
+                tom = metric_df_fail["TOM"].astype(float)
+            # if case = "All", we will calculate correlation for all samples
+            else:
+                gt = gt_df["Ground Truth"].astype(float)
+                relaxed_gt = gt_df["Relaxed GT"].astype(float)
+                # we have 4 PL space metrics
+                em_PL = metric_df["EM-PL"].astype(float)
+                codebleu = metric_df["CodeBLEU"].astype(float)
+                pfm = metric_df["P/FM"].astype(float)
+                tom = metric_df["TOM"].astype(float)
+            # we don't have NL space metrics
+            bleu_NL = None
+            chrF_NL = None
+            rouge_1_NL = None
+            rouge_2_NL = None
+            rouge_L_NL = None
+            bertscore_NL = None
+
+        # we have Ground Truth (GT) and Relaxed Ground Truth (Relaxed GT)
+        # Relaxed GT means in the docstring, nl description is correct, but some of the examples wrong
+        for gt_type in ["GT", "Relaxed GT"]:
+            # list lout all the metrics we want to compute correlation with
+            if case == "Pass":
+                metrics = {
+                    "BLEU-NL": bleu_NL,
+                    "chrF-NL": chrF_NL,
+                    "ROUGE-1-NL": rouge_1_NL,
+                    "ROUGE-2-NL": rouge_2_NL,
+                    "ROUGE-L-NL": rouge_L_NL,
+                    "BERTScore-NL": bertscore_NL,
+                    "EM-PL": em_PL,
+                    "CodeBLEU": codebleu,
+                    "P/FM": pfm,
+                    "TOM": tom,
+                }
+            # if PL0 fail, we don't have NL space metrics
+            else:
+                metrics = {
+                    "EM-PL": em_PL,
+                    "CodeBLEU": codebleu,
+                    "P/FM": pfm,
+                    "TOM": tom,
+                }
+
+            # for each metric, calculate correlation with GT or Relaxed GT
+            for metric_name, metric_result in metrics.items():
+                print("==========================================")
+                print(f"Correlation between {gt_type} and {metric_name}:")
+                if gt_type == "GT":
+                    pearson_cor, spearman_cor, kendall_tau_cor = calculate_correlation(gt, metric_result)
+                else:
+                    pearson_cor, spearman_cor, kendall_tau_cor = calculate_correlation(relaxed_gt, metric_result)
+
+                print("-----------------------------------------")
+                print(f"Pearson's r: {pearson_cor}")
+                print(f"Spearman's rho: {spearman_cor}")
+                print(f"Kendall's tau: {kendall_tau_cor}")
+                print("==========================================")
+                # add row to the corresponding DataFrame
+                row = {
+                    "Metric": metric_name,
+                    "Pearson's r": pearson_cor[0],
+                    "Spearman's rho": spearman_cor[0],
+                    "Kendall's tau": kendall_tau_cor[0],
+                }
+                if gt_type == "GT":
+                    if case == "Pass":
+                        cor_gt_pass = pd.concat([cor_gt_pass, pd.DataFrame([row])], ignore_index=True)
+                    elif case == "Fail":
+                        cor_gt_fail = pd.concat([cor_gt_fail, pd.DataFrame([row])], ignore_index=True)
+                    else:
+                        cor_gt_all = pd.concat([cor_gt_all, pd.DataFrame([row])], ignore_index=True)
+                else:
+                    if case == "Pass":
+                        cor_relaxed_gt_pass = pd.concat([cor_relaxed_gt_pass, pd.DataFrame([row])], ignore_index=True)
+                    elif case == "Fail":
+                        cor_relaxed_gt_fail = pd.concat([cor_relaxed_gt_fail, pd.DataFrame([row])], ignore_index=True)
+                    else:
+                        cor_relaxed_gt_all = pd.concat([cor_relaxed_gt_all, pd.DataFrame([row])], ignore_index=True)
+
+            print("\n**********************************************************************************\n")
+
+    # write correlation statistics to excel
+    if args.output_path is None:
+        output_path = "Human_Judge_Correlation.xlsx"
+    else:
+        output_path = args.output_path
+    with pd.ExcelWriter(output_path) as writer:
+        gt_df.to_excel(writer, sheet_name="gt", index=False, startrow=1, startcol=1, engine="xlsxwriter")
+        metric_df.to_excel(writer, sheet_name="traj", index=False, startrow=1, startcol=1, engine="xlsxwriter")
+        cor_gt_pass.to_excel(writer, sheet_name="cor_gt_pass", index=False, startrow=1, startcol=1, engine="xlsxwriter")
+        cor_relaxed_gt_pass.to_excel(
+            writer, sheet_name="cor_relaxed_gt_pass", index=False, startrow=1, startcol=1, engine="xlsxwriter"
+        )
+        cor_gt_fail.to_excel(writer, sheet_name="cor_gt_fail", index=False, startrow=1, startcol=1, engine="xlsxwriter")
+        cor_relaxed_gt_fail.to_excel(
+            writer, sheet_name="cor_relaxed_gt_fail", index=False, startrow=1, startcol=1, engine="xlsxwriter"
+        )
+        cor_gt_all.to_excel(writer, sheet_name="cor_gt_all", index=False, startrow=1, startcol=1, engine="xlsxwriter")
+        cor_relaxed_gt_all.to_excel(
+            writer, sheet_name="cor_relaxed_gt_all", index=False, startrow=1, startcol=1, engine="xlsxwriter"
+        )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `identitychain-0.0.1/scripts/reformat_EvalPlus.py` & `identitychain-0.1.0/scripts/reformat_EvalPlus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,208 +1,235 @@
-# Authors: marcusm117
-# License: Apache 2.0
-
-
-# Standard Library Modules
-import argparse
-import json
-import os
-
-# Internal Modules
-from identitychain.utils import g_unzip
-
-
-# extract function signature from a problem descriptions
-# note that this only works for variations of the HumanEval dataset
-def extract_func_signature(prompt):
-    # find all occurrences of three consecutive double quotes
-    res = [i for i in range(len(prompt)) if prompt.startswith('"""', i)]
-
-    # if res is empty, check for both single quotes
-    if not res:
-        res = [i for i in range(len(prompt)) if prompt.startswith("'''", i)]
-
-    # get the end position of the function signature
-    end_position = res[-2] - 4
-
-    return prompt[:end_position]
-
-
-# fix typos, fix wrong/no examples, and remove unnecessary leading newlines
-# rename the field "prompt" into "problem" to avoid confusion with the instrcutrion/few-shot prompt for the model
-def reformat_problem_descriptions(output_path, EvalPlus_tasks, HEE_tasks):
-    with open(output_path, "w", encoding="utf-8") as writer:
-        for i in range(len(HEE_tasks)):
-            EvalPlus_task = json.loads(EvalPlus_tasks[i])
-            HEE_task = json.loads(HEE_tasks[i])
-
-            # for HumanEval/75, 95, 116, 163, we choose the problem descriptions from EvalPlus
-            # otherwise, we choose the problem descriptions from Human-Eval-Enhanced (HEE)
-            # for more information, see the following issue and PR:
-            # https://github.com/evalplus/evalplus/issues/12
-            # https://github.com/openai/human-eval/pull/23
-            if i in {75, 95, 116, 163}:
-                problem = EvalPlus_task["prompt"]
-                problem = problem[1:]  # remove unnecessary leading newlines
-            else:
-                problem = HEE_task["prompt"]
-
-            # rename the field "prompt" into "problem"
-            reformatted_task = {
-                "task_id": EvalPlus_task["task_id"],
-                "problem": problem,
-                "contract": EvalPlus_task["contract"],
-            }
-
-            # write the reformatted task to the output file
-            writer.write(json.dumps(reformatted_task) + "\n")
-            writer.flush()
-
-
-# rename the field "entry_point" into "function_name" for clarity
-# extract function signature from problem descriptions, store in the field "function_signature"
-def reformat_fields(output_path, EvalPlus_tasks):
-    # read previously reformatted tasks
-    with open(output_path, "r", encoding="utf-8") as reader:
-        reformatted_tasks = reader.readlines()
-
-    # write new changes to the reformatted tasks
-    with open(output_path, "w", encoding="utf-8") as writer:
-        for i in range(len(EvalPlus_tasks)):
-            EvalPlus_task = json.loads(EvalPlus_tasks[i])
-            reformatted_task = json.loads(reformatted_tasks[i])
-
-            # rename the field "entry_point" into "function_name"
-            # add the field "function_signature"
-            reformatted_task["function_name"] = EvalPlus_task["entry_point"]
-            reformatted_task["function_signature"] = extract_func_signature(reformatted_task["problem"])
-            reformatted_task["canonical_solution"] = EvalPlus_task["canonical_solution"]
-
-            # write the reformatted task to the output file
-            writer.write(json.dumps(reformatted_task) + "\n")
-            writer.flush()
-
-
-# use the canonical solution provided by EvalPlus
-# to generate outputs for each test case input in EvalPlus-Mini
-# reformat them in into a List of Dicts, for example,
-#    "tests": [
-#        {
-#            "input": "'(()()) ((())) () ((())()())'",
-#            "output": "['(()())', '((()))', '()', '((())()())']",
-#        },
-#        {
-#            "input": "'() (()) ((())) (((())))'",
-#            "output": "['()', '(())', '((()))', '(((())))']",
-#        },
-#        {
-#           "input": "'(()(())((())))'",
-#           "output": "['(()(())((())))']"
-#        },
-#    ]
-def reformat_tests(output_path, EvalPlus_tasks):
-    # read previously reformatted tasks
-    with open(output_path, "r", encoding="utf-8") as reader:
-        reformatted_tasks = reader.readlines()
-
-    # write new changes to the reformatted tasks
-    with open(output_path, "w", encoding="utf-8") as writer:
-        for i in range(len(EvalPlus_tasks)):
-            EvalPlus_task = json.loads(EvalPlus_tasks[i])
-            reformatted_task = json.loads(reformatted_tasks[i])
-
-            # reformat the inputs
-            task_id = EvalPlus_task["task_id"]
-            # remove redundant tests in EvalPlus-Mini/15
-            if task_id == "HumanEval/15":
-                inputs = EvalPlus_task["base_input"] + [[1], [100]]
-            # remove Time Complexity tests in EvalPlus-Mini/83, 100, 130, 139
-            elif task_id in {"HumanEval/83", "HumanEval/100", "HumanEval/130", "HumanEval/139"}:
-                inputs = EvalPlus_task["base_input"] + EvalPlus_task["plus_input"][:-1]
-            # remove an invalid input in EvalPlus-Mini/116
-            elif task_id == "HumanEval/116":
-                EvalPlus_task["base_input"].pop(1)
-                inputs = EvalPlus_task["base_input"] + EvalPlus_task["plus_input"]
-            # otherwise, concatenate the base_inputs and plus_inputs
-            else:
-                inputs = EvalPlus_task["base_input"] + EvalPlus_task["plus_input"]
-
-            # construct the tests List, where each element is a Dict
-            tests = []
-            for input in inputs:
-                # reformat the input as a string
-                input_str = f"{str(input)[1:-1]}"
-                tests.append({"input": input_str, "output": ""})
-
-            # concatenate the problem description, contract, and canonical solution
-            complete_code = (
-                reformatted_task["problem"] + reformatted_task["contract"] + reformatted_task["canonical_solution"]
-            )
-
-            # for debugging, uncomment the following line
-            print(reformatted_task["task_id"])
-            print(complete_code)
-
-            # get corresponding outputs for each test case input
-            for test in tests:
-                # EvalPlus canonical solutions can be trusted, okay to use exec() here
-                exec_globals = {}
-                exec(complete_code, exec_globals)
-                # fetch the function from exec_globals
-                func = exec_globals[f"{reformatted_task['function_name']}"]
-                # get the input from the string
-                input = eval(test["input"])
-                # get corresponding output
-                if type(input) is tuple:
-                    output = func(*input)
-                else:
-                    output = func(input)
-                # store the output to the test Dict
-                if type(output) is str:
-                    # handle escape characters
-                    output = output.replace("\n", "\\n").replace("\r", "\\r").replace("\t", "\\t")
-                    test["output"] = f"'{output}'"
-                else:
-                    test["output"] = str(output)
-
-                # for debugging, uncomment the following line
-                # print(test)
-
-            # add the tests List to the reformatted task
-            reformatted_task["tests"] = tests
-            reformatted_task["atol"] = EvalPlus_task["atol"]
-            writer.write(json.dumps(reformatted_task) + "\n")
-            writer.flush()
-
-
-# EXAMPLE USAGE:
-# python reformat_EvalPlus.py --output_path ../data/EvalPlus-Mini-v0.1.6_reformatted.jsonl
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--output_path", type=str, required=True)
-    args = parser.parse_args()
-
-    # uncompressed the input data
-    g_unzip("../data/HumanEval/HumanEvalPlus-Mini-v0.1.6.jsonl.gz", "../data/HumanEvalPlus-Mini-v0.1.6.jsonl")
-    g_unzip("../data/HumanEval/human-eval-enhanced-202307.jsonl.gz", "../data/human-eval-enhanced-202307.jsonl")
-
-    # read from the HumanEvalPlus-Mini-v0.1.6 (EvalPlus) and human-eval-enhanced-202307 (HEE) datasets
-    # for more information, see the following GitHub Repos:
-    # https://github.com/evalplus/evalplus
-    # https://github.com/marcusm117/human-eval-enhanced
-    with open("../data/HumanEvalPlus-Mini-v0.1.6.jsonl", "r", encoding="utf-8") as reader:
-        EvalPlus_tasks = reader.readlines()
-    with open("../data/human-eval-enhanced-202307.jsonl", "r", encoding="utf-8") as reader:
-        HEE_tasks = reader.readlines()
-
-    # reformat the data
-    reformat_problem_descriptions(args.output_path, EvalPlus_tasks, HEE_tasks)
-    reformat_fields(args.output_path, EvalPlus_tasks)
-    reformat_tests(args.output_path, EvalPlus_tasks)
-
-    # remove the uncompressed input data
-    os.remove("../data/HumanEvalPlus-Mini-v0.1.6.jsonl")
-    os.remove("../data/human-eval-enhanced-202307.jsonl")
-
-
-if __name__ == "__main__":
-    main()
+# Authors: marcusm117
+# License: Apache 2.0
+
+
+# Standard Library Modules
+import argparse
+import json
+import os
+
+# Internal Modules
+from identitychain.utils import g_unzip
+
+
+# extract function signature from a problem descriptions
+# note that this only works for variations of the HumanEval dataset
+def extract_func_signature(prompt):
+    # find all occurrences of three consecutive double quotes
+    res = [i for i in range(len(prompt)) if prompt.startswith('"""', i)]
+
+    # if res is empty, check for both single quotes
+    if not res:
+        res = [i for i in range(len(prompt)) if prompt.startswith("'''", i)]
+
+    # get the end position of the function signature
+    end_position = res[-2] - 4
+
+    return prompt[:end_position]
+
+
+# fix typos, fix wrong/no examples, and remove unnecessary leading newlines
+# rename the field "prompt" into "problem" to avoid confusion with the instrcutrion/few-shot prompt for the model
+def reformat_problem_descriptions(output_path, EvalPlus_tasks, HEE_tasks):
+    with open(output_path, "w", encoding="utf-8") as writer:
+        for i in range(len(HEE_tasks)):
+            EvalPlus_task = json.loads(EvalPlus_tasks[i])
+            HEE_task = json.loads(HEE_tasks[i])
+
+            # for HumanEval/75, 95, 116, 163, we choose the problem descriptions from EvalPlus
+            # otherwise, we choose the problem descriptions from Human-Eval-Enhanced (HEE)
+            # for more information, see the following issue and PR:
+            # https://github.com/evalplus/evalplus/issues/12
+            # https://github.com/openai/human-eval/pull/23
+            # however, for HumanEval/116, one of the example still conflicts the problem description, we keep it
+            # only to stay consistent with the original HumanEval dataset
+            if i in {75, 95, 116, 163}:
+                problem = EvalPlus_task["prompt"]
+                problem = problem[1:]  # remove unnecessary leading newlines
+            else:
+                problem = HEE_task["prompt"]
+
+            # rename the field "prompt" into "problem"
+            reformatted_task = {
+                "task_id": EvalPlus_task["task_id"],
+                "problem": problem,
+                "contract": EvalPlus_task["contract"],
+            }
+
+            # write the reformatted task to the output file
+            writer.write(json.dumps(reformatted_task) + "\n")
+            writer.flush()
+
+
+# rename the field "entry_point" into "function_name" for clarity
+# extract function signature from problem descriptions, store in the field "function_signature"
+def reformat_fields(output_path, EvalPlus_tasks):
+    # read previously reformatted tasks
+    with open(output_path, "r", encoding="utf-8") as reader:
+        reformatted_tasks = reader.readlines()
+
+    # write new changes to the reformatted tasks
+    with open(output_path, "w", encoding="utf-8") as writer:
+        for i in range(len(EvalPlus_tasks)):
+            EvalPlus_task = json.loads(EvalPlus_tasks[i])
+            reformatted_task = json.loads(reformatted_tasks[i])
+
+            # rename the field "entry_point" into "function_name"
+            # add the field "function_signature"
+            reformatted_task["function_name"] = EvalPlus_task["entry_point"]
+            reformatted_task["function_signature"] = extract_func_signature(reformatted_task["problem"])
+            reformatted_task["canonical_solution"] = EvalPlus_task["canonical_solution"]
+
+            # correct invalid contract for HumanEvalPlus-Mini/99, for HumanEvalPlus-Mini-v0.1.9 only
+            if (
+                reformatted_task["task_id"] == "HumanEval/99"
+                and output_path == "../data/EvalPlus-Mini-v0.1.9_reformatted.jsonl"
+            ):
+                reformatted_task["contract"] = (
+                    "\n    try: # $_CONTRACT_$\n        assert isinstance(value, str) "
+                    "# $_CONTRACT_$\n        value = float(value) # $_CONTRACT_$\n    except: # $_CONTRACT_$\n        "
+                    "raise Exception(\"invalid inputs\") # $_CONTRACT_$\n    import math # $_CONTRACT_$\n    "
+                    "assert not (math.isinf(value) or math.isnan(value)), \"invalid inputs\" # $_CONTRACT_$\n"
+                )
+
+            # write the reformatted task to the output file
+            writer.write(json.dumps(reformatted_task) + "\n")
+            writer.flush()
+
+
+# use the canonical solution provided by EvalPlus
+# to generate outputs for each test case input in EvalPlus-Mini
+# reformat them in into a List of Dicts, for example,
+#    "tests": [
+#        {
+#            "input": "'(()()) ((())) () ((())()())'",
+#            "output": "['(()())', '((()))', '()', '((())()())']",
+#        },
+#        {
+#            "input": "'() (()) ((())) (((())))'",
+#            "output": "['()', '(())', '((()))', '(((())))']",
+#        },
+#        {
+#           "input": "'(()(())((())))'",
+#           "output": "['(()(())((())))']"
+#        },
+#    ]
+def reformat_tests(output_path, EvalPlus_tasks):
+    # read previously reformatted tasks
+    with open(output_path, "r", encoding="utf-8") as reader:
+        reformatted_tasks = reader.readlines()
+
+    # write new changes to the reformatted tasks
+    with open(output_path, "w", encoding="utf-8") as writer:
+        for i in range(len(EvalPlus_tasks)):
+            EvalPlus_task = json.loads(EvalPlus_tasks[i])
+            reformatted_task = json.loads(reformatted_tasks[i])
+
+            # reformat the inputs
+            task_id = EvalPlus_task["task_id"]
+            # remove redundant tests in HumanEvalPlus-Mini/15
+            if task_id == "HumanEval/15":
+                inputs = EvalPlus_task["base_input"] + [[1], [100]]
+            # remove Time Complexity tests in HumanEvalPlus-Mini/83, 100, 130, 139
+            elif task_id in {"HumanEval/83", "HumanEval/100", "HumanEval/130", "HumanEval/139"}:
+                inputs = EvalPlus_task["base_input"] + EvalPlus_task["plus_input"][:-1]
+            # remove an invalid input in HumanEvalPlus-Mini/116
+            elif task_id == "HumanEval/116":
+                EvalPlus_task["base_input"].pop(1)
+                inputs = EvalPlus_task["base_input"] + EvalPlus_task["plus_input"]
+            # remove an invalid input in HumanEvalPlus-Mini/1, for HumanEvalPlus-Mini-v0.1.9 only
+            elif task_id == "HumanEval/1" and output_path == "../data/EvalPlus-Mini-v0.1.9_reformatted.jsonl":
+                EvalPlus_task["plus_input"].pop(1)
+                EvalPlus_task["plus_input"].pop(-2)
+                inputs = EvalPlus_task["base_input"] + EvalPlus_task["plus_input"]
+            # remove an invalid input in HumanEvalPlus-Mini/28, for HumanEvalPlus-Mini-v0.1.9 only
+            elif task_id == "HumanEval/28" and output_path == "../data/EvalPlus-Mini-v0.1.9_reformatted.jsonl":
+                EvalPlus_task["plus_input"].pop(1)
+                inputs = EvalPlus_task["base_input"] + EvalPlus_task["plus_input"]
+            # otherwise, concatenate the base_inputs and plus_inputs
+            else:
+                inputs = EvalPlus_task["base_input"] + EvalPlus_task["plus_input"]
+
+            # construct the tests List, where each element is a Dict
+            tests = []
+            for input in inputs:
+                # reformat the input as a string
+                input_str = f"{str(input)[1:-1]}"
+                tests.append({"input": input_str, "output": ""})
+
+            # concatenate the problem description, contract, and canonical solution
+            complete_code = (
+                reformatted_task["problem"] + reformatted_task["contract"] + reformatted_task["canonical_solution"]
+            )
+
+            # for debugging, uncomment the following line
+            print(reformatted_task["task_id"])
+            print(complete_code)
+
+            # get corresponding outputs for each test case input
+            for test in tests:
+                # EvalPlus canonical solutions can be trusted, okay to use exec() here
+                exec_globals = {}
+                exec(complete_code, exec_globals)
+                # fetch the function from exec_globals
+                func = exec_globals[f"{reformatted_task['function_name']}"]
+                # get the input from the string
+                input = eval(test["input"])
+                # get corresponding output
+                if type(input) is tuple:
+                    output = func(*input)
+                else:
+                    print(input)
+                    output = func(input)
+                # store the output to the test Dict
+                if type(output) is str:
+                    # handle escape characters
+                    output = output.replace("\n", "\\n").replace("\r", "\\r").replace("\t", "\\t")
+                    test["output"] = f"'{output}'"
+                else:
+                    test["output"] = str(output)
+
+                # for debugging, uncomment the following line
+                # print(test)
+
+            # add the tests List to the reformatted task
+            reformatted_task["tests"] = tests
+            reformatted_task["atol"] = EvalPlus_task["atol"]
+            writer.write(json.dumps(reformatted_task) + "\n")
+            writer.flush()
+
+
+# EXAMPLE USAGE:
+# python reformat_EvalPlus.py --evalplus_path ../data/HumanEval/HumanEvalPlus-Mini-v0.1.10.jsonl.gz
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--evalplus_path", type=str, required=True)
+    args = parser.parse_args()
+
+    # uncompressed the input data
+    uncompressed_file_name = args.evalplus_path[18:-3]
+    uncompressed_path = f"../data/{uncompressed_file_name}"
+    g_unzip(args.evalplus_path, uncompressed_path)
+    g_unzip("../data/HumanEval/human-eval-enhanced-202307.jsonl.gz", "../data/human-eval-enhanced-202307.jsonl")
+
+    # read from the HumanEvalPlus-Mini-v0.1.6 (EvalPlus) and human-eval-enhanced-202307 (HEE) datasets
+    # for more information, see the following GitHub Repos:
+    # https://github.com/evalplus/evalplus
+    # https://github.com/marcusm117/human-eval-enhanced
+    with open(uncompressed_path, "r", encoding="utf-8") as reader:
+        EvalPlus_tasks = reader.readlines()
+    with open("../data/human-eval-enhanced-202307.jsonl", "r", encoding="utf-8") as reader:
+        HEE_tasks = reader.readlines()
+
+    # reformat the data
+    output_path = "../data/" + uncompressed_file_name[5:-6] + "_reformatted.jsonl"
+    reformat_problem_descriptions(output_path, EvalPlus_tasks, HEE_tasks)
+    reformat_fields(output_path, EvalPlus_tasks)
+    reformat_tests(output_path, EvalPlus_tasks)
+
+    # remove the uncompressed input data
+    os.remove(uncompressed_path)
+    os.remove("../data/human-eval-enhanced-202307.jsonl")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `identitychain-0.0.1/scripts/reformat_MBPP-S.py` & `identitychain-0.1.0/scripts/reformat_MBPP-S.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-# Authors: marcusm117
-# License: Apache 2.0
-
-
-# Standard Library Modules
-import argparse
-import json
-import os
-import re
-
-# Internal Modules
-from identitychain.utils import g_unzip
-
-
-# extract function signature from a canonical solution
-# note that this only works for variations of the MBPP dataset
-def extract_func_signature(canonical_sol):
-    # find all occurrences of "def "
-    res = [i for i in range(len(canonical_sol)) if canonical_sol.startswith("def ", i)]
-    # pick the last one if it follows a newline, otherwise pick the first one
-    if canonical_sol[res[-1] - 1] == "\n":
-        start_position = res[-1]
-    else:
-        start_position = res[0]
-
-    # find the end position of the function signature
-    canonical_sol = canonical_sol[start_position:]
-    end_position_candidate1 = canonical_sol.find("):")
-    end_position_candidate2 = canonical_sol.find(") :")
-
-    # choose candidate2 if candidate1 is not found
-    if end_position_candidate1 == -1:
-        end_position = end_position_candidate2 + 3
-    # choose candidate1 if candidate2 is not found
-    elif end_position_candidate2 == -1:
-        end_position = end_position_candidate1 + 2
-    else:
-        # choose the smaller one if both are found
-        if end_position_candidate1 < end_position_candidate2:
-            end_position = end_position_candidate1 + 2
-        else:
-            end_position = end_position_candidate2 + 3
-
-    return canonical_sol[:end_position]
-
-
-# extract function name from a function signature
-# note that this only works for variations of the MBPP dataset
-def extract_func_name(func_signature):
-    start_position = func_signature.find("def ") + 4
-    end_position = func_signature.find("(")
-    return func_signature[start_position:end_position].strip()
-
-
-# rename the field "prompt" into "problem" to avoid confusion with the instrcutrion/few-shot prompt for the model
-# reformat the field "problem" into HumanEval style: function signature + problem description in the docstring
-# extract the function signature from the field "code", store in the field "function_signature"
-# extract function name from function signature, store in the field "function_name"
-# remove the function signature from the field "code", rename it to "canonical_solution"
-def reformat_fields(output_path, MBPP_S_tasks):
-    with open(output_path, "w", encoding="utf-8") as writer:
-        for MBBP_S_task in MBPP_S_tasks:
-            MBBP_S_task = json.loads(MBBP_S_task)
-
-            # extract function signature from the field "code"
-            func_signature = extract_func_signature(MBBP_S_task["code"])
-
-            # rename the field "prompt" into "problem", and reformat it
-            reformatted_task = {
-                "task_id": MBBP_S_task["task_id"],
-                "problem": func_signature + '\n    \"\"\" ' + MBBP_S_task["prompt"] + '\n    \"\"\"\n',
-                "contract": "",
-            }
-
-            # add the fields "function_name" and "function_signature"
-            reformatted_task["function_name"] = extract_func_name(func_signature)
-            reformatted_task["function_signature"] = func_signature
-
-            # write the reformatted task to the output file
-            writer.write(json.dumps(reformatted_task) + "\n")
-            writer.flush()
-
-
-# rename the field "code" into "canonical_solution" for clarity
-# reformat "canonical_solution" so that all indentation is exactly 4 spaces
-def reformat_canonical_solution(output_path, MBPP_S_tasks):
-    # read previously reformatted tasks
-    with open(output_path, "r", encoding="utf-8") as reader:
-        reformatted_tasks = reader.readlines()
-
-    # write new changes to the reformatted tasks
-    with open(output_path, "w", encoding="utf-8") as writer:
-        for i in range(len(MBPP_S_tasks)):
-            MBBP_S_task = json.loads(MBPP_S_tasks[i])
-            reformatted_task = json.loads(reformatted_tasks[i])
-            task_id = reformatted_task["task_id"]
-
-            # reformat the canonical solution
-            func_signature = reformatted_task["function_signature"]
-            canonical_sol = MBBP_S_task["code"]
-            # remove the import statements, add back inside the function body later
-            import_statements = []
-            position = canonical_sol.find(func_signature)
-            if position != 0:
-                import_str = canonical_sol[:position]
-                canonical_sol = canonical_sol.replace(import_str, "")
-                assert canonical_sol[: len(func_signature)] == func_signature  # for debugging
-                import_statements = import_str.splitlines()
-                import_statements = [statement.rstrip() for statement in import_statements]
-            # remove the function signature
-            canonical_sol = canonical_sol.replace(func_signature, "")
-            # remove unnecessary leading spaces
-            canonical_sol = canonical_sol.lstrip(" ")
-            # remove all comments
-            canonical_sol = re.sub(r"#.*\n", "", canonical_sol)
-            # replace tabs with 4 spaces
-            canonical_sol = canonical_sol.replace("\t", "    ")
-            # replace 3 or less spaces with 4 spaces
-            pattern = r"^\n {1,3}"
-            match = re.match(pattern, canonical_sol)
-            if match:
-                assert match.start() == 0  # for debugging
-                canonical_sol = canonical_sol.replace(canonical_sol[1 : match.end()], "    ")
-            # replace 5 or more spaces with 4 spaces
-            pattern = r"^\n {5,}"
-            match = re.match(pattern, canonical_sol)
-            if match:
-                assert match.start() == 0  # for debugging
-                canonical_sol = canonical_sol.replace(canonical_sol[1 : match.end()], "    ")
-            # add back the import statements, if any
-            if import_statements:
-                canonical_sol = "    " + "\n    ".join(import_statements) + "\n" + canonical_sol
-            # remove unnecessary ";", spaces, and newlines at the end, if any
-            while canonical_sol[-1] in [";", " ", "\n"]:
-                canonical_sol = canonical_sol[:-1]
-            # add one trailing newline back
-            canonical_sol += "\n"
-
-            # hanlde special cases
-            if task_id == 223:
-                reformatted_task["function_name"] = "is_majority"
-                reformatted_task["function_signature"] = "def is_majority(arr, n, x):\n"
-                reformatted_task["problem"] = reformatted_task["function_signature"] + reformatted_task["problem"][38:]
-                canonical_sol = """    def binary_search(arr, low, high, x):
-        if high >= low:
-            mid = (low + high)//2
-            if (mid == 0 or x > arr[mid-1]) and (arr[mid] == x):
-                return mid
-            elif x > arr[mid]:
-                return binary_search(arr, (mid + 1), high, x)
-            else:
-                return binary_search(arr, low, (mid -1), x)
-        return -1
-
-    i = binary_search(arr, 0, n-1, x)
-    if i == -1:
-            return False
-    if ((i + n//2) <= (n -1)) and arr[i + n//2] == x:
-            return True
-    else:
-            return False\n"""
-            if task_id == 230:
-                canonical_sol = "    str2 = str1.replace(' ', char)\n    return str2"
-            if task_id == 640:
-                canonical_sol = (
-                    "    import re\n\n    for item in items:\n        return (re.sub(r\" ?\\([^)]+\\)\", \"\", item))\n"
-                )
-
-            # rename the field "code" into "canonical_solution"
-            reformatted_task["canonical_solution"] = canonical_sol
-
-            # add trailnig newline to function signature
-            reformatted_task["function_signature"] += "\n"
-
-            # write the reformatted task to the output file
-            writer.write(json.dumps(reformatted_task) + "\n")
-            writer.flush()
-
-
-# reformat "tests" by reporting the output of each test case when assertion fails
-# add the field "atol"
-def reformat_tests(output_path, MBPP_S_tasks):
-    # read previously reformatted tasks
-    with open(output_path, "r", encoding="utf-8") as reader:
-        reformatted_tasks = reader.readlines()
-
-    # write new changes to the reformatted tasks
-    with open(output_path, "w", encoding="utf-8") as writer:
-        for i in range(len(MBPP_S_tasks)):
-            MBBP_S_task = json.loads(MBPP_S_tasks[i])
-            reformatted_task = json.loads(reformatted_tasks[i])
-            task_id = reformatted_task["task_id"]
-
-            # reformat tests
-            tests = MBBP_S_task["test_list"]
-            for j in range(len(tests)):
-                # add import statements if necessary
-                import_stmt = ""
-                if "sys." in tests[j]:
-                    import_stmt += "import sys\n"
-                if "math." in tests[j]:
-                    import_stmt += "import math\n"
-
-                # capture the function call stmt, which will be evlauted as the output
-                func_name = reformatted_task["function_name"]
-                assert tests[j].count(func_name) == 1  # for debugging
-                start_position = tests[j].find(f"{func_name}")
-                end_position = tests[j].find("==")
-                if end_position == -1:
-                    end_position = tests[j].find(")") + 1
-                func_call_stmt = tests[j][start_position:end_position].strip()
-                # remove necessary spaces
-                while func_call_stmt[len(func_name)] == " ":
-                    func_call_stmt = func_call_stmt[: len(func_name)] + func_call_stmt[len(func_name) + 1 :]
-                while func_call_stmt[len(func_name) + 1] == " ":
-                    func_call_stmt = func_call_stmt[: len(func_name) + 1] + func_call_stmt[len(func_name) + 2 :]
-
-                # hanlde special cases
-                if task_id in {2, 7, 111, 140, 232, 769}:
-                    func_call_stmt = func_call_stmt[:-1]
-                if task_id == 98:
-                    func_call_stmt += ")"
-
-                # capture output and report it when assertion fails
-                capture_output = f"test_out = {func_call_stmt}\n"
-                assertion_stmt = tests[j].replace(func_call_stmt, "test_out") + r", f'outputs {test_out}'"
-
-                # reformat test
-                tests[j] = import_stmt + capture_output + assertion_stmt
-
-            # add the fields "tests" and "atol"
-            reformatted_task["tests"] = tests
-            reformatted_task["atol"] = ""
-            writer.write(json.dumps(reformatted_task) + "\n")
-            writer.flush()
-
-
-# EXAMPLE USAGE:
-# python reformat_MBPP-S.py --output_path ../data/MBPP-S_test_reformatted.jsonl
-# python reformat_MBPP-S.py --input_path ../data/MBPP-S/MBPP-S.jsonl.gz --output_path ../data/MBPP-S_reformatted.jsonl
-# note that this script only works for the MBPP-S (sanitized) dataset, NOT the full MBPP dataset
-# for more information, see the following HuggingFace Dataset:
-# https://huggingface.co/datasets/mbpp/viewer
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--input_path", type=str, default="../data/MBPP-S/MBPP-S_test.jsonl.gz")
-    parser.add_argument("--output_path", type=str, required=True)
-    args = parser.parse_args()
-
-    # uncompressed the data
-    # note that, for model  evluation, we only need the test split of the MBPP-S dataset
-    # however, this script works for the entire MBPP-S dataset as well
-    # if you want to reformat the entrie dataset or other splits, specify the input_path and output_path accordingly
-    uncompressed_path = args.input_path[:-3].replace("MBPP-S/", "")
-    g_unzip(args.input_path, uncompressed_path)
-
-    # read from the test split of the MBPP-S (sanitized) dataset
-    # for more information, see the following GitHub Repo:
-    # https://github.com/google-research/google-research/tree/master/mbpp
-    with open(uncompressed_path, "r", encoding="utf-8") as reader:
-        MBPP_S_tasks = reader.readlines()
-
-    # reformat the data
-    reformat_fields(args.output_path, MBPP_S_tasks)
-    reformat_canonical_solution(args.output_path, MBPP_S_tasks)
-    reformat_tests(args.output_path, MBPP_S_tasks)
-
-    # remove the uncompressed input data
-    os.remove(uncompressed_path)
-
-
-if __name__ == "__main__":
-    main()
+# Authors: marcusm117
+# License: Apache 2.0
+
+
+# Standard Library Modules
+import argparse
+import json
+import os
+import re
+
+# Internal Modules
+from identitychain.utils import g_unzip
+
+
+# extract function signature from a canonical solution
+# note that this only works for variations of the MBPP dataset
+def extract_func_signature(canonical_sol):
+    # find all occurrences of "def "
+    res = [i for i in range(len(canonical_sol)) if canonical_sol.startswith("def ", i)]
+    # pick the last one if it follows a newline, otherwise pick the first one
+    if canonical_sol[res[-1] - 1] == "\n":
+        start_position = res[-1]
+    else:
+        start_position = res[0]
+
+    # find the end position of the function signature
+    canonical_sol = canonical_sol[start_position:]
+    end_position_candidate1 = canonical_sol.find("):")
+    end_position_candidate2 = canonical_sol.find(") :")
+
+    # choose candidate2 if candidate1 is not found
+    if end_position_candidate1 == -1:
+        end_position = end_position_candidate2 + 3
+    # choose candidate1 if candidate2 is not found
+    elif end_position_candidate2 == -1:
+        end_position = end_position_candidate1 + 2
+    else:
+        # choose the smaller one if both are found
+        if end_position_candidate1 < end_position_candidate2:
+            end_position = end_position_candidate1 + 2
+        else:
+            end_position = end_position_candidate2 + 3
+
+    return canonical_sol[:end_position]
+
+
+# extract function name from a function signature
+# note that this only works for variations of the MBPP dataset
+def extract_func_name(func_signature):
+    start_position = func_signature.find("def ") + 4
+    end_position = func_signature.find("(")
+    return func_signature[start_position:end_position].strip()
+
+
+# rename the field "prompt" into "problem" to avoid confusion with the instrcutrion/few-shot prompt for the model
+# reformat the field "problem" into HumanEval style: function signature + problem description in the docstring
+# extract the function signature from the field "code", store in the field "function_signature"
+# extract function name from function signature, store in the field "function_name"
+# remove the function signature from the field "code", rename it to "canonical_solution"
+def reformat_fields(output_path, MBPP_S_tasks):
+    with open(output_path, "w", encoding="utf-8") as writer:
+        for MBBP_S_task in MBPP_S_tasks:
+            MBBP_S_task = json.loads(MBBP_S_task)
+
+            # extract function signature from the field "code"
+            func_signature = extract_func_signature(MBBP_S_task["code"])
+
+            # rename the field "prompt" into "problem", and reformat it
+            reformatted_task = {
+                "task_id": MBBP_S_task["task_id"],
+                "problem": func_signature + '\n    \"\"\" ' + MBBP_S_task["prompt"] + '\n    \"\"\"\n',
+                "contract": "",
+            }
+
+            # add the fields "function_name" and "function_signature"
+            reformatted_task["function_name"] = extract_func_name(func_signature)
+            reformatted_task["function_signature"] = func_signature
+
+            # write the reformatted task to the output file
+            writer.write(json.dumps(reformatted_task) + "\n")
+            writer.flush()
+
+
+# rename the field "code" into "canonical_solution" for clarity
+# reformat "canonical_solution" so that all indentation is exactly 4 spaces
+def reformat_canonical_solution(output_path, MBPP_S_tasks):
+    # read previously reformatted tasks
+    with open(output_path, "r", encoding="utf-8") as reader:
+        reformatted_tasks = reader.readlines()
+
+    # write new changes to the reformatted tasks
+    with open(output_path, "w", encoding="utf-8") as writer:
+        for i in range(len(MBPP_S_tasks)):
+            MBBP_S_task = json.loads(MBPP_S_tasks[i])
+            reformatted_task = json.loads(reformatted_tasks[i])
+            task_id = reformatted_task["task_id"]
+
+            # reformat the canonical solution
+            func_signature = reformatted_task["function_signature"]
+            canonical_sol = MBBP_S_task["code"]
+            # remove the import statements, add back inside the function body later
+            import_statements = []
+            position = canonical_sol.find(func_signature)
+            if position != 0:
+                import_str = canonical_sol[:position]
+                canonical_sol = canonical_sol.replace(import_str, "")
+                assert canonical_sol[: len(func_signature)] == func_signature  # for debugging
+                import_statements = import_str.splitlines()
+                import_statements = [statement.rstrip() for statement in import_statements]
+            # remove the function signature
+            canonical_sol = canonical_sol.replace(func_signature, "")
+            # remove unnecessary leading spaces
+            canonical_sol = canonical_sol.lstrip(" ")
+            # remove all comments
+            canonical_sol = re.sub(r"#.*\n", "", canonical_sol)
+            # replace tabs with 4 spaces
+            canonical_sol = canonical_sol.replace("\t", "    ")
+            # replace 3 or less spaces with 4 spaces
+            pattern = r"^\n {1,3}"
+            match = re.match(pattern, canonical_sol)
+            if match:
+                assert match.start() == 0  # for debugging
+                canonical_sol = canonical_sol.replace(canonical_sol[1 : match.end()], "    ")
+            # replace 5 or more spaces with 4 spaces
+            pattern = r"^\n {5,}"
+            match = re.match(pattern, canonical_sol)
+            if match:
+                assert match.start() == 0  # for debugging
+                canonical_sol = canonical_sol.replace(canonical_sol[1 : match.end()], "    ")
+            # add back the import statements, if any
+            if import_statements:
+                canonical_sol = "    " + "\n    ".join(import_statements) + "\n" + canonical_sol
+            # remove unnecessary ";", spaces, and newlines at the end, if any
+            while canonical_sol[-1] in [";", " ", "\n"]:
+                canonical_sol = canonical_sol[:-1]
+            # add one trailing newline back
+            canonical_sol += "\n"
+
+            # hanlde special cases
+            if task_id == 223:
+                reformatted_task["function_name"] = "is_majority"
+                reformatted_task["function_signature"] = "def is_majority(arr, n, x):\n"
+                reformatted_task["problem"] = reformatted_task["function_signature"] + reformatted_task["problem"][38:]
+                canonical_sol = """    def binary_search(arr, low, high, x):
+        if high >= low:
+            mid = (low + high)//2
+            if (mid == 0 or x > arr[mid-1]) and (arr[mid] == x):
+                return mid
+            elif x > arr[mid]:
+                return binary_search(arr, (mid + 1), high, x)
+            else:
+                return binary_search(arr, low, (mid -1), x)
+        return -1
+
+    i = binary_search(arr, 0, n-1, x)
+    if i == -1:
+            return False
+    if ((i + n//2) <= (n -1)) and arr[i + n//2] == x:
+            return True
+    else:
+            return False\n"""
+            if task_id == 230:
+                canonical_sol = "    str2 = str1.replace(' ', char)\n    return str2"
+            if task_id == 640:
+                canonical_sol = (
+                    "    import re\n\n    for item in items:\n        return (re.sub(r\" ?\\([^)]+\\)\", \"\", item))\n"
+                )
+
+            # rename the field "code" into "canonical_solution"
+            reformatted_task["canonical_solution"] = canonical_sol
+
+            # add trailnig newline to function signature
+            reformatted_task["function_signature"] += "\n"
+
+            # write the reformatted task to the output file
+            writer.write(json.dumps(reformatted_task) + "\n")
+            writer.flush()
+
+
+# reformat "tests" by reporting the output of each test case when assertion fails
+# add the field "atol"
+def reformat_tests(output_path, MBPP_S_tasks):
+    # read previously reformatted tasks
+    with open(output_path, "r", encoding="utf-8") as reader:
+        reformatted_tasks = reader.readlines()
+
+    # write new changes to the reformatted tasks
+    with open(output_path, "w", encoding="utf-8") as writer:
+        for i in range(len(MBPP_S_tasks)):
+            MBBP_S_task = json.loads(MBPP_S_tasks[i])
+            reformatted_task = json.loads(reformatted_tasks[i])
+            task_id = reformatted_task["task_id"]
+
+            # reformat tests
+            tests = MBBP_S_task["test_list"]
+            for j in range(len(tests)):
+                # add import statements if necessary
+                import_stmt = ""
+                if "sys." in tests[j]:
+                    import_stmt += "import sys\n"
+                if "math." in tests[j]:
+                    import_stmt += "import math\n"
+
+                # capture the function call stmt, which will be evlauted as the output
+                func_name = reformatted_task["function_name"]
+                assert tests[j].count(func_name) == 1  # for debugging
+                start_position = tests[j].find(f"{func_name}")
+                end_position = tests[j].find("==")
+                if end_position == -1:
+                    end_position = tests[j].find(")") + 1
+                func_call_stmt = tests[j][start_position:end_position].strip()
+                # remove necessary spaces
+                while func_call_stmt[len(func_name)] == " ":
+                    func_call_stmt = func_call_stmt[: len(func_name)] + func_call_stmt[len(func_name) + 1 :]
+                while func_call_stmt[len(func_name) + 1] == " ":
+                    func_call_stmt = func_call_stmt[: len(func_name) + 1] + func_call_stmt[len(func_name) + 2 :]
+
+                # hanlde special cases
+                if task_id in {2, 7, 111, 140, 232, 769}:
+                    func_call_stmt = func_call_stmt[:-1]
+                if task_id == 98:
+                    func_call_stmt += ")"
+
+                # capture output and report it when assertion fails
+                capture_output = f"test_out = {func_call_stmt}\n"
+                assertion_stmt = tests[j].replace(func_call_stmt, "test_out") + r", f'outputs {test_out}'"
+
+                # reformat test
+                tests[j] = import_stmt + capture_output + assertion_stmt
+
+            # add the fields "tests" and "atol"
+            reformatted_task["tests"] = tests
+            reformatted_task["atol"] = ""
+            writer.write(json.dumps(reformatted_task) + "\n")
+            writer.flush()
+
+
+# EXAMPLE USAGE:
+# python reformat_MBPP-S.py --output_path ../data/MBPP-S_test_reformatted.jsonl
+# python reformat_MBPP-S.py --input_path ../data/MBPP-S/MBPP-S.jsonl.gz --output_path ../data/MBPP-S_reformatted.jsonl
+# note that this script only works for the MBPP-S (sanitized) dataset, NOT the full MBPP dataset
+# for more information, see the following HuggingFace Dataset:
+# https://huggingface.co/datasets/mbpp/viewer
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--input_path", type=str, default="../data/MBPP-S/MBPP-S_test.jsonl.gz")
+    parser.add_argument("--output_path", type=str, required=True)
+    args = parser.parse_args()
+
+    # uncompressed the data
+    # note that, for model  evluation, we only need the test split of the MBPP-S dataset
+    # however, this script works for the entire MBPP-S dataset as well
+    # if you want to reformat the entrie dataset or other splits, specify the input_path and output_path accordingly
+    uncompressed_path = args.input_path[:-3].replace("MBPP-S/", "")
+    g_unzip(args.input_path, uncompressed_path)
+
+    # read from the test split of the MBPP-S (sanitized) dataset
+    # for more information, see the following GitHub Repo:
+    # https://github.com/google-research/google-research/tree/master/mbpp
+    with open(uncompressed_path, "r", encoding="utf-8") as reader:
+        MBPP_S_tasks = reader.readlines()
+
+    # reformat the data
+    reformat_fields(args.output_path, MBPP_S_tasks)
+    reformat_canonical_solution(args.output_path, MBPP_S_tasks)
+    reformat_tests(args.output_path, MBPP_S_tasks)
+
+    # remove the uncompressed input data
+    os.remove(uncompressed_path)
+
+
+if __name__ == "__main__":
+    main()
```

