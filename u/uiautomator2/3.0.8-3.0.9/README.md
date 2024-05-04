# Comparing `tmp/uiautomator2-3.0.8.tar.gz` & `tmp/uiautomator2-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiautomator2-3.0.8.tar", max compression
+gzip compressed data, was "uiautomator2-3.0.9.tar", max compression
```

## Comparing `uiautomator2-3.0.8.tar` & `uiautomator2-3.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1064 2024-04-09 14:35:00.879628 uiautomator2-3.0.8/LICENSE
--rw-r--r--   0        0        0    53306 2024-04-09 14:35:00.883628 uiautomator2-3.0.8/README.md
--rw-r--r--   0        0        0     1036 2024-04-09 14:35:16.503848 uiautomator2-3.0.8/pyproject.toml
--rw-r--r--   0        0        0    68753 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/__init__.py
--rw-r--r--   0        0        0     8063 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/__main__.py
--rw-r--r--   0        0        0      289 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/_proto.py
--rw-r--r--   0        0        0    21287 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/_selector.py
--rw-r--r--   0        0        0      646 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/abcd.py
--rw-r--r--   0        0        0       27 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/assets/.gitignore
--rw-r--r--   0        0        0  1061950 2024-04-09 14:35:15.599835 uiautomator2-3.0.8/uiautomator2/assets/app-uiautomator-test.apk
--rw-r--r--   0        0        0  2191186 2024-04-09 14:35:14.835825 uiautomator2-3.0.8/uiautomator2/assets/app-uiautomator.apk
--rwxr-xr-x   0        0        0 10092696 2024-04-07 08:30:35.000000 uiautomator2-3.0.8/uiautomator2/assets/atx-agent
--rwxr-xr-x   0        0        0      886 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/assets/sync.sh
--rw-r--r--   0        0        0       80 2024-04-09 14:35:15.623836 uiautomator2-3.0.8/uiautomator2/assets/version.txt
--rw-r--r--   0        0        0     2602 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext/__init__.py
--rw-r--r--   0        0        0      405 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/README.md
--rw-r--r--   0        0        0     5574 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/__init__.py
--rw-r--r--   0        0        0     4802 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/index.html
--rw-r--r--   0        0        0    61137 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/pig.jpg
--rw-r--r--   0        0        0     1100 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
--rw-r--r--   0        0        0       29 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/start.bat
--rw-r--r--   0        0        0     2645 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/info/__init__.py
--rw-r--r--   0        0        0    28515 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/info/conf.py
--rw-r--r--   0        0        0     2852 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/perf/README.md
--rw-r--r--   0        0        0    12384 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/perf/__init__.py
--rw-r--r--   0        0        0    41467 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/perf/net.png
--rw-r--r--   0        0        0    26928 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/perf/summary.png
--rw-r--r--   0        0        0     4180 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/aircv/README.md
--rw-r--r--   0        0        0    18456 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/aircv/__init__.py
--rw-r--r--   0        0        0      947 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/README.md
--rw-r--r--   0        0        0     2495 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/__init__.py
--rw-r--r--   0        0        0     3308 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/baiduOCR.py
--rw-r--r--   0        0        0    10476 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/image.py
--rw-r--r--   0        0        0    15094 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/init.py
--rw-r--r--   0        0        0     1801 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/messagebox.py
--rw-r--r--   0        0        0     3776 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/screenrecord.py
--rw-r--r--   0        0        0     3342 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/settings.py
--rw-r--r--   0        0        0     1762 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/swipe.py
--rw-r--r--   0        0        0     5856 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/utils.py
--rw-r--r--   0        0        0     4908 2024-04-09 14:35:16.503848 uiautomator2-3.0.8/uiautomator2/version.py
--rw-r--r--   0        0        0     9456 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/watcher.py
--rw-r--r--   0        0        0     6710 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/webview.py
--rw-r--r--   0        0        0    14389 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/widget.py
--rw-r--r--   0        0        0    24156 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/xpath.py
--rw-r--r--   0        0        0    54216 1970-01-01 00:00:00.000000 uiautomator2-3.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-28 06:18:06.441822 uiautomator2-3.0.9/LICENSE
+-rw-r--r--   0        0        0    50066 2024-04-28 06:18:06.441822 uiautomator2-3.0.9/README.md
+-rw-r--r--   0        0        0      958 2024-04-28 06:18:27.537683 uiautomator2-3.0.9/pyproject.toml
+-rw-r--r--   0        0        0    34588 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/__init__.py
+-rw-r--r--   0        0        0     7180 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/__main__.py
+-rw-r--r--   0        0        0     4180 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_archived/aircv/README.md
+-rw-r--r--   0        0        0    18456 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_archived/aircv/__init__.py
+-rw-r--r--   0        0        0    15094 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_archived/init.py
+-rw-r--r--   0        0        0     1801 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_archived/messagebox.py
+-rw-r--r--   0        0        0      947 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_archived/ocr/README.md
+-rw-r--r--   0        0        0     2495 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_archived/ocr/__init__.py
+-rw-r--r--   0        0        0     3308 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_archived/ocr/baiduOCR.py
+-rw-r--r--   0        0        0     6707 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_archived/webview.py
+-rw-r--r--   0        0        0    14467 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_archived/widget.py
+-rw-r--r--   0        0        0      289 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_proto.py
+-rw-r--r--   0        0        0    21323 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/_selector.py
+-rw-r--r--   0        0        0     1381 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/abstract.py
+-rw-r--r--   0        0        0       27 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/assets/.gitignore
+-rw-r--r--   0        0        0  1061950 2024-04-28 06:18:26.425690 uiautomator2-3.0.9/uiautomator2/assets/app-uiautomator-test.apk
+-rw-r--r--   0        0        0  2191186 2024-04-28 06:18:26.065692 uiautomator2-3.0.9/uiautomator2/assets/app-uiautomator.apk
+-rwxr-xr-x   0        0        0      845 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/assets/sync.sh
+-rw-r--r--   0        0        0       19 2024-04-28 06:18:26.449690 uiautomator2-3.0.9/uiautomator2/assets/version.txt
+-rw-r--r--   0        0        0    11734 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/core.py
+-rw-r--r--   0        0        0     1019 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/htmlreport/README.md
+-rw-r--r--   0        0        0     5574 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/htmlreport/__init__.py
+-rw-r--r--   0        0        0     4802 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/htmlreport/assets/index.html
+-rw-r--r--   0        0        0    61137 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/htmlreport/assets/pig.jpg
+-rw-r--r--   0        0        0     1100 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
+-rw-r--r--   0        0        0       29 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/htmlreport/assets/start.bat
+-rw-r--r--   0        0        0     2645 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/info/__init__.py
+-rw-r--r--   0        0        0    28515 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/info/conf.py
+-rw-r--r--   0        0        0     2852 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/perf/README.md
+-rw-r--r--   0        0        0    12384 2024-04-28 06:18:06.445822 uiautomator2-3.0.9/uiautomator2/ext/perf/__init__.py
+-rw-r--r--   0        0        0    41467 2024-04-28 06:18:06.449822 uiautomator2-3.0.9/uiautomator2/ext/perf/net.png
+-rw-r--r--   0        0        0    26928 2024-04-28 06:18:06.449822 uiautomator2-3.0.9/uiautomator2/ext/perf/summary.png
+-rw-r--r--   0        0        0    10476 2024-04-28 06:18:06.449822 uiautomator2-3.0.9/uiautomator2/image.py
+-rw-r--r--   0        0        0     3776 2024-04-28 06:18:06.449822 uiautomator2-3.0.9/uiautomator2/screenrecord.py
+-rw-r--r--   0        0        0     3342 2024-04-28 06:18:06.449822 uiautomator2-3.0.9/uiautomator2/settings.py
+-rw-r--r--   0        0        0     1762 2024-04-28 06:18:06.449822 uiautomator2-3.0.9/uiautomator2/swipe.py
+-rw-r--r--   0        0        0     5375 2024-04-28 06:18:06.449822 uiautomator2-3.0.9/uiautomator2/utils.py
+-rw-r--r--   0        0        0     4912 2024-04-28 06:18:27.537683 uiautomator2-3.0.9/uiautomator2/version.py
+-rw-r--r--   0        0        0     9456 2024-04-28 06:18:06.449822 uiautomator2-3.0.9/uiautomator2/watcher.py
+-rw-r--r--   0        0        0    24516 2024-04-28 06:18:06.449822 uiautomator2-3.0.9/uiautomator2/xpath.py
+-rw-r--r--   0        0        0    50875 1970-01-01 00:00:00.000000 uiautomator2-3.0.9/PKG-INFO
```

### Comparing `uiautomator2-3.0.8/LICENSE` & `uiautomator2-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/README.md` & `uiautomator2-3.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,35 +5,37 @@
 
 QQ交流群: **815453846**
 
 > 有段时间没有维护这个项目了（可能有两年了），但是最近工作需要又重新研究一下Android原生自动化，当然又调研了Appium，对比下来一看，发现uiautomator2这个项目的运行速度是真的好快，从检测元素到点击，都是毫秒级的，代码也比较好理解。真是没想到以前竟然写出了这么神奇的项目，这么好的项目怎么能让它落灰呢，得好好整一整，一些垃圾代码清理清理。所以项目版本从2.x.x升级到了3.x.x
 
 还在用2.x.x版本的用户，可以先看一下[2to3](docs/2to3.md) 再决定是否要升级3.x.x （我个人还是非常建议升级的）
 
+2到3毕竟是大版本升级，很多的函数删掉了。首先删掉的就是atx-agent，其次还有一堆atx-agent相关的函数。废弃的功能比如init.
+
 各种依赖库的版本号
 
 - [![PyPI](https://img.shields.io/pypi/v/uiautomator2.svg?label=uiautomator2)](https://pypi.python.org/pypi/uiautomator2)
 - [![PyPI](https://img.shields.io/pypi/v/adbutils.svg?label=adbutils)](https://github.com/openatx/adbutils)
-- [![GitHub tag (latest SemVer)](https://img.shields.io/github/tag/openatx/atx-agent.svg?label=atx-agent)](https://github.com/openatx/atx-agent)
 - [![GitHub tag (latest SemVer)](https://img.shields.io/github/tag/openatx/android-uiautomator-server.svg?label=android-uiautomator-server)](https://github.com/openatx/android-uiautomator-server)
+- ~~[![GitHub tag (latest SemVer)](https://img.shields.io/github/tag/openatx/atx-agent.svg?label=atx-agent)](https://github.com/openatx/atx-agent)~~
 
 [UiAutomator](https://developer.android.com/training/testing/ui-automator.html)是Google提供的用来做安卓自动化测试的一个Java库，基于Accessibility服务。功能很强，可以对第三方App进行测试，获取屏幕上任意一个APP的任意一个控件属性，并对其进行任意操作，但有两个缺点：1. 测试脚本只能使用Java语言 2. 测试脚本要打包成jar或者apk包上传到设备上才能运行。
 
 我们希望测试逻辑能够用Python编写，能够在电脑上运行的时候就控制手机。这里要非常感谢 Xiaocong He ([@xiaocong][])，他将这个想法实现了出来（见[xiaocong/uiautomator](https://github.com/xiaocong/uiautomator)），原理是在手机上运行了一个http rpc服务，将uiautomator中的功能开放出来，然后再将这些http接口封装成Python库。
-因为`xiaocong/uiautomator`这个库，已经很久不见更新。所以我们直接fork了一个版本，为了方便做区分我们就在后面加了个2 [openatx/uiautomator2](https://github.com/openatx/uiautomator2)
+因为`xiaocong/uiautomator`这个库，已经很久不见更新。所以我们直接fork了一个版本，为了方便做区分我们就在后面加了个2 [openatx/uiautomator2](https://github.com/openatx/uiautomator2),对应的Android包源码我也fork了一份，[openatx/android-uiautomator-server](https://github.com/openatx/android-uiautomator-server)
 
 除了对原有的库的bug进行了修复，还增加了很多新的Feature。主要有以下部分：
 
-* 设备和开发机可以脱离数据线，通过WiFi互联（基于[atx-agent](https://github.com/openatx/atx-agent)）
+* ~~设备和开发机可以脱离数据线，通过WiFi互联（基于[atx-agent](https://github.com/openatx/atx-agent)~~
 * ~~集成了[openstf/minicap](https://github.com/openstf/minicap)达到实时屏幕投频，以及实时截图~~
 * ~~集成了[openstf/minitouch](https://github.com/openstf/minitouch)达到精确实时控制设备~~
 * 修复了[xiaocong/uiautomator](https://github.com/xiaocong/uiautomator)经常性退出的问题
 * 代码进行了重构和精简，方便维护
 * 实现了一个设备管理平台(也支持iOS) [atxserver2](https://github.com/openatx/atxserver2) （注：目前不怎么维护了）
-* 扩充了toast获取和展示的功能
+* 扩充了toast获取和展示的功能（需要手动开启ATX的悬浮窗权限） 貌似有bug用不了
 
 >这里要先说明下，因为经常有很多人问 openatx/uiautomator2 并不支持iOS测试，需要iOS自动化测试，可以转到这个库 [openatx/facebook-wda](https://github.com/openatx/facebook-wda)。
 
 > PS: 这个库 ~~<https://github.com/NeteaseGame/ATX>~~ 目前已经不维护了，请尽快更换。
 
 这里有一份快速参考，适合已经入门的人 [QUICK REFERENCE GUIDE](QUICK_REFERENCE.md)，欢迎多提意见。
 
@@ -58,15 +60,15 @@
 这时看到类似下面的输出，就可以正式开始用我们这个库了。因为这个库功能太多，后面还有很多的内容，需要慢慢去看 ....
 
 ```
 {'currentPackageName': 'net.oneplus.launcher', 'displayHeight': 1920, 'displayRotation': 0, 'displaySizeDpX': 411, 'displaySizeDpY': 731, 'displayWidth': 1080, 'productName': 'OnePlus5', '
 screenOn': True, 'sdkInt': 27, 'naturalOrientation': True}
 ```
 
-一般情况下都会成功，不过也可能会有意外。可以加QQ群反馈问题，群里有很多大佬可以帮你解决问题。
+一般情况下都会成功，不过也可能会有意外。可以加QQ群反馈问题(群号在最上面），群里有很多大佬可以帮你解决问题。
 
 ## Sponsors
 Thank you to all our sponsors! ✨🍰✨
 
 ### 金牌赞助商（Gold Sponsor）
 [![霍格沃兹测试开发学社](https://testing-studio.com/img/icon.png)](https://qrcode.testing-studio.com/f?from=ATX&url=https://testing-studio.com/)
 
@@ -76,17 +78,17 @@
 优秀文章推荐 (欢迎QQ群里at我反馈）
 
 - [py-uiautomator2通过悬浮窗让服务长时间可用](https://zhuanlan.zhihu.com/p/688009468) 这个**强烈推荐**看一下
 - [termux里如何部署uiautomator2简介](https://www.cnblogs.com/ze-yan/p/12242383.html) by `成都-测试只会一点点`
 
 ## 相关项目
 - 基于adb协议与Android进行交互的库 [adbutils](https://github.com/openatx/adbutils)
-- 设备管理平台，设备多了就会用到 [atxserver2](https://github.com/openatx/atxserver2) （寻找项目维护人员）
-- [atx-agent](https://github.com/openatx/atx-agent) 运行在设备上的驻守程序，go开发，用于保活设备上相关的服务
 - [uiauto.dev](https://uiauto.dev) 用于查看UI层级结构，类似于uiautomatorviewer(用于替代之前写的weditor），用于查看UI层级结构 
+- 设备管理平台，设备多了就会用到 [atxserver2](https://github.com/openatx/atxserver2) （寻找项目维护人员）
+- ~~[atx-agent](https://github.com/openatx/atx-agent) 运行在设备上的驻守程序，go开发，用于保活设备上相关的服务~~
 - ~~[weditor](https://github.com/openatx/weditor) 类似于uiautomatorviewer，专门为本项目开发的辅助编辑器(这个暂不维护了~~
 
 **[Installation](#installation)**
 
 **[Connect to a device](#connect-to-a-device)**
 
 **[Command line](#command-line)**
@@ -114,31 +116,16 @@
   - **[Selector](#selector)**
   - **[Watcher](#watcher)**
   - **[Global settings](#global-settings)**
   - **[Input method](#input-method)**
   - **[Toast](#toast)**
   - **[XPath](#xpath)**
   - **[Screenrecord](#screenrecord)**
-  - **[Image match](#image-match)**
-
-**常见问题**
-  - **[停止UiAutomator守护服务，释放AccessibilityService](#stop-uiautomator)**
-  - **[502错误](https://github.com/openatx/uiautomator2/wiki/Common-issues)**
-  - **[Connection Error, 深度睡眠, 点击偏差 等](https://github.com/openatx/uiautomator2/wiki/Common-issues)**
-  
-
-**[实验性功能](https://github.com/openatx/uiautomator2/wiki/Common-issues#%E5%AE%9E%E9%AA%8C%E6%80%A7%E5%8A%9F%E8%83%BD)**
-  - **远程投屏**
-  - **htmlreport**
-  - **诊断uiautomator2方法**
-  - **Plugin**
-  - **Hooks**
-  - **失败时弹出提示框**
+  - **[Image match](#image-match) Removed**
 
-**[项目历史](#项目历史)**
 
 **[Contributors](#contributors)**
 
 **[LICENSE](#license)**
 
 
 # Installation
@@ -161,59 +148,37 @@
     浏览器打开 https://uiauto.dev 查看当前设备的界面结构。
 
     **appinspector介绍**
 
     [uiauto.dev](https://github.com/codeskyblue/uiauto.dev) 是一个独立与uiautomator2之外的一个项目，用于查看图层结构的。属于旧版项目[weditor的重构版本](https://github.com/openatx/weditor)，后续也许会收费（价格肯定物超所值），来支持当前这个项目继续维护下去。感兴趣的可以加群讨论(也包含提需求) QQ群 536481989
 
 # Connect to a device
-There are two ways to connect to the device. 
-
-1. **Through WiFi**
-
-Suppose device IP is `10.0.0.1` and your PC is in the same network.
-
-```python
-import uiautomator2 as u2
-
-d = u2.connect('10.0.0.1') # alias for u2.connect_wifi('10.0.0.1')
-print(d.info)
-```
-
-2. **Through USB**
-
-Suppose the device serial is `123456f` (seen from `adb devices`)
+use serialno to connect device eg. `123456f` (seen from `adb devices`)
 
 ```python
 import uiautomator2 as u2
 
 d = u2.connect('123456f') # alias for u2.connect_usb('123456f')
 print(d.info)
 ```
 
-3. **Through ADB WiFi**
+Serial can be passed through env-var `ANDROID_SERIAL`
 
-```python
-import uiautomator2 as u2
 
-d = u2.connect_adb_wifi("10.0.0.1:5555")
-
-# Equals to 
-# + Shell: adb connect 10.0.0.1:5555
-# + Python: u2.connect_usb("10.0.0.1:5555")
+```python
+# export ANDROID_SERIAL=123456f
+d = u2.connect()
 ```
 
-Calling `u2.connect()` with no argument, `uiautomator2` will obtain device IP from the environment variable `ANDROID_DEVICE_IP` or `ANDROID_SERIAL`.
-If this environment variable is empty, uiautomator will fall back to `connect_usb` and you need to make sure that there is only one device connected to the computer.
-
 # Command line
 其中的`$device_ip`代表设备的ip地址
 
 如需指定设备需要传入`--serial` 如 `python3 -m uiautomator2 --serial bff1234 <SubCommand>`, SubCommand为子命令（screenshot, current 等）
 
-> 1.0.3 Added: `python3 -m uiautomator2`可以简写为`uiautomator2`
+> 1.0.3 Added: `python3 -m uiautomator2` equals to `uiautomator2`
 
 - screenshot: 截图
 
     ```bash
     $ uiautomator2 screenshot screenshot.jpg
     ```
 
@@ -224,57 +189,47 @@
     {
         "package": "com.android.browser",
         "activity": "com.uc.browser.InnerUCMobile",
         "pid": 28478
     }
     ```
     
-- uninstall： 卸载
+- uninstall： Uninstall app
 
     ```bash
     $ uiautomator2 uninstall <package-name> # 卸载一个包
     $ uiautomator2 uninstall <package-name-1> <package-name-2> # 卸载多个包
     $ uiautomator2 uninstall --all # 全部卸载
     ```
 
-- stop: 停止应用
+- stop: Stop app
 
     ```bash
     $ uiautomator2 stop com.example.app # 停止一个app
     $ uiautomator2 stop --all # 停止所有的app
     ```
-    
-- install: 安装apk，apk通过URL给出 (暂时不能用)
-- healthcheck: 健康检查 (暂不能用)
 
-- doctor: 检查uiautomator2无法使用的原因
+- doctor:
 
     ```bash
     $ uiautomator2 doctor
-    I 210519 16:48:45 init:156] uiautomator2 version: 2.14.2.dev1
-    [D 210519 16:48:45 __main__:105] sdk:29 abi:arm64-v8a
-    CHECK atx-agent
-            GOOD: atx-agent version 0.10.0
-    CHECK uiautomator-apks
-            GOOD: com.github.uiautomator 2.3.3
-    CHECK jsonrpc
-            GOOD: d.info success
-    ==> GOOD <==
+    [I 2024-04-25 19:53:36,288 __main__:101 pid:15596] uiautomator2 is OK
     ```
     
 # API Documents
 
-### New command timeout
-How long (in seconds) will wait for a new command from the client before assuming the client quit and ending the uiautomator service （Default 3 minutes）
+### New command timeout （Removed)
+When python quit, the UiAutomation service also quit.
+<!-- How long (in seconds) will wait for a new command from the client before assuming the client quit and ending the uiautomator service （Default 3 minutes）
 
 配置accessibility服务的最大空闲时间，超时将自动释放。默认3分钟。
 
 ```python
 d.set_new_command_timeout(300) # change to 5 minutes, unit seconds
-```
+``` -->
 
 ### Debug HTTP requests
 打印出代码背后的HTTP请求信息
 
 ```python
 >>> d.debug = True
 >>> d.info
@@ -394,30 +349,26 @@
     ```python
     d.pull("/sdcard/tmp.txt", "tmp.txt")
 
     # FileNotFoundError will raise if the file is not found on the device
     d.pull("/sdcard/some-file-not-exists.txt", "tmp.txt")
     ```
 
-### 检查并维持设备端守护进程处于运行状态
-```python
-d.healthcheck()
-```
 
-### ~~Auto click permission dialogs~~
+### ~~Auto click permission dialogs~~ (Removed)
 **注意注意** `disable_popups`函数，检测发现很不稳定，暂时不要使用，等候通知。
-
+<!-- 
 Import in version 0.1.1
 
 ```python
 d.disable_popups() # automatic skip popups
 d.disable_popups(False) # disable automatic skip popups
 ```
 
-![popup](docs/img/popup.png)
+![popup](docs/img/popup.png) -->
 
 ### Open Scheme
 
 ```python
 d.open_url("appname://appnamehost")
 ```
 
@@ -452,16 +403,16 @@
     output, exit_code = d.shell(["ls", "-l"])
     # output: "/....", exit_code: 0
     ```
 
    This returns a string for stdout merged with stderr.
    If the command is a blocking command, `shell` will also block until the command is completed or the timeout kicks in. No partial output will be received during the execution of the command. This API is not suitable for long-running commands. The shell command given runs in a similar environment of `adb shell`, which has a Linux permission level of `adb` or `shell` (higher than an app permission).
 
-* Run a long-running shell command
-
+* Run a long-running shell command (Removed)
+<!-- 
     add stream=True will return `requests.models.Response` object. More info see [requests stream](http://docs.python-requests.org/zh_CN/latest/user/quickstart.html#id5)
 
     ```python
     r = d.shell("logcat", stream=True)
     # r: requests.models.Response
     deadline = time.time() + 10 # run maxium 10s
     try:
@@ -469,17 +420,17 @@
             if time.time() > deadline:
                 break
             print("Read:", line.decode('utf-8'))
     finally:
         r.close() # this method must be called
     ```
 
-    Command will be terminated when `r.close()` called.
+    Command will be terminated when `r.close()` called. -->
     
-### Session
+### Session (Removed)
 Session represent an app lifecycle. Can be used to start app, detect app crash.
 
 * Launch and close app
 
     ```python
     sess = d.session("com.netease.cloudmusic") # start 网易云音乐
     sess.close() # 停止网易云音乐
@@ -494,17 +445,14 @@
     ```
 
 * Attach to the running app
 
     ```python
     # launch app if not running, skip launch if already running
     sess = d.session("com.netease.cloudmusic", attach=True)
-
-    # raise SessionBrokenError if not running
-    sess = d.session("com.netease.cloudmusic", attach=True, strict=True)
     ```
 
 * Detect app crash
 
     ```python
     # When app is still running
     sess(text="Music").click() # operation goes normal
@@ -528,25 +476,24 @@
 ```python
 d.info
 ```
 
 Below is a possible output:
 
 ```
-{ 
-    u'displayRotation': 0,
-    u'displaySizeDpY': 640,
-    u'displaySizeDpX': 360,
-    u'currentPackageName': u'com.android.launcher',
-    u'productName': u'takju',
-    u'displayWidth': 720,
-    u'sdkInt': 18,
-    u'displayHeight': 1184,
-    u'naturalOrientation': True
-}
+{'currentPackageName': 'com.android.systemui',
+ 'displayHeight': 1560,
+ 'displayRotation': 0,
+ 'displaySizeDpX': 360,
+ 'displaySizeDpY': 780,
+ 'displayWidth': 720,
+ 'naturalOrientation': True,
+ 'productName': 'ELE-AL00',
+ 'screenOn': True,
+ 'sdkInt': 29}
 ```
 
 Get window size
 
 ```python
 print(d.window_size())
 # device upright output example: (1080, 1920)
@@ -576,18 +523,21 @@
 # output example: 74aAEDR428Z9
 ```
 
 Get WLAN ip
 
 ```python
 print(d.wlan_ip)
-# output example: 10.0.0.1
+# output example: 10.0.0.1 or None
 ```
 
-Get detailed device info
+
+~~Get detailed device info~~ `d.device_info`
+
+device_info was Removed since 3.x
 
 ```python
 print(d.device_info)
 ```
 
 Below is a possible output:
 
@@ -677,16 +627,16 @@
 You can find all key code definitions at [Android KeyEvnet](https://developer.android.com/reference/android/view/KeyEvent.html)
 
 * Unlock screen
 
     ```python
     d.unlock()
     # This is equivalent to
-    # 1. launch activity: com.github.uiautomator.ACTION_IDENTIFY
-    # 2. press the "home" key
+    # 1. press("power")
+    # 2. swipe from left-bottom to right-top
     ```
 
 ### Gesture interaction with the device
 * Click on the screen
 
     ```python
     d.click(x, y)
@@ -753,15 +703,15 @@
 
     这个接口属于比较底层的原始接口，感觉并不完善，不过凑合能用。注：这个地方并不支持百分比
 
     ```python
     d.touch.down(10, 10) # 模拟按下
     time.sleep(.01) # down 和 move 之间的延迟，自己控制
     d.touch.move(15, 15) # 模拟移动
-    d.touch.up() # 模拟抬起
+    d.touch.up(10, 10) # 模拟抬起
     ```
 
 Note: click, swipe, drag operations support percentage position values. Example:
 
 `d.long_click(0.5, 0.5)` means long click center of screen
 
 ### Screen-related
@@ -815,15 +765,15 @@
     imagebin = d.screenshot(format='raw')
     open("some.jpg", "wb").write(imagebin)
     ```
 
 * Dump UI hierarchy
 
     ```python
-    # get the UI hierarchy dump content (unicoded).
+    # get the UI hierarchy dump content
     xml = d.dump_hierarchy()
     ```
 
 * Open notification or quick settings
 
     ```python
     d.open_notification()
@@ -1267,37 +1217,31 @@
 ```
 
 另外文档还是有很多没有写，推荐直接去看源码[watcher.py](uiautomator2/watcher.py)
 
 ### Global settings
 
 ```python
-d.HTTP_TIMEOUT = 60 # 默认值60s, http默认请求超时时间
-
-# 当设备掉线时，等待设备在线时长，仅当TMQ=true时有效，支持通过环境变量 WAIT_FOR_DEVICE_TIMEOUT 设置
-d.WAIT_FOR_DEVICE_TIMEOUT = 70 
+u2.HTTP_TIMEOUT = 60 # 默认值60s, http默认请求超时时间
 ```
 
 其他的配置，目前已大部分集中到 `d.settings` 中，根据后期的需求配置可能会有增减。
 
 ```python
 print(d.settings)
 {'operation_delay': (0, 0),
  'operation_delay_methods': ['click', 'swipe'],
- 'wait_timeout': 20.0,
- 'xpath_debug': False}
+ 'wait_timeout': 20.0}
 
 # 配置点击前延时0.5s，点击后延时1s
 d.settings['operation_delay'] = (.5, 1)
 
 # 修改延迟生效的方法
 # 其中 double_click, long_click 都对应click
 d.settings['operation_delay_methods'] = ['click', 'swipe', 'drag', 'press']
-
-d.settings['xpath_debug'] = True # 开启xpath插件的调试日志
 d.settings['wait_timeout'] = 20.0 # 默认控件等待时间（原生操作，xpath插件的等待时间）
 ```
 
 对于随着版本升级，设置过期的配置时，会提示Deprecated，但是不会抛异常。
 
 ```bash
 >>> d.settings['click_before_delay'] = 1  
@@ -1354,15 +1298,15 @@
 _什么时候该使用这个函数呢？_
 
 有些时候在EditText中输入完内容之后，调用`press("search")` or `press("enter")`发现并没有什么反应。
 这个时候就需要`send_action`函数了，这里用到了只有输入法才能用的[IME_ACTION_CODE](https://developer.android.com/reference/android/view/inputmethod/EditorInfo)。
 `send_action`先broadcast命令发送给输入法操作`IME_ACTION_CODE`，由输入法完成后续跟EditText的通信。（原理我不太清楚，有了解的，提issue告诉我)
 
 ### Toast (2.2版本之后有添加回来)
-Show Toast
+Show Toast (好像有点bug)
 
 ```python
 d.toast.show("Hello world")
 d.toast.show("Hello world", 1.0) # show for 1.0s, default 1.0s
 ```
 
 Get Toast
@@ -1449,66 +1393,36 @@
 # or do something else
 
 d.screenrecord.stop() # 停止录制后，output.mp4文件才能打开
 ```
 
 录制的时候也可以指定fps（当前是20），这个值是率低于minicap输出图片的速度，感觉已经很好了，不建议你修改。
 
-### Image match (3.x开始移除该功能)
-3.x开始废弃
-
-图像匹配，在使用这个功能之前你需要先把依赖安装上
-
-```bash
-pip3 install -U "uiautomator2[image]" -i https://pypi.doubanio.com/simple
-```
+# Enable uiautomator2 logger
 
-目前开放两个接口
- 
+```python
+from uiautomator2 import enable_pretty_logging
+enable_pretty_logging()
 ```
-imdata = "target.png" # 也可以是URL, PIL.Image或OpenCV打开的图像
 
-d.image.match(imdata) 
-# 匹配待查找的图片，立刻返回一个结果
-# 返回一个dict, eg: {"similarity": 0.9, "point": [200, 300]}
+Or
 
-d.image.click(imdata, timeout=20.0)
-# 在20s的时间内调用match轮询查找图片，当similarity>0.9时，执行点击操作
 ```
-
-该功能还在完善中，图片需要手机的原图裁剪后的图才可以。
-
-# 常见问题
-很多没写在这个地方的，都放到了这里 [Common Issues](https://github.com/openatx/uiautomator2/wiki/Common-issues)
+logger = logging.getLogger("uiautomator2")
+# setup logger
+```
 
 ## Stop UiAutomator
-停止UiAutomator守护服务
-
-https://github.com/openatx/uiautomator2/wiki/Common-issues
-
-因为有`atx-agent`的存在，Uiautomator会被一直守护着，如果退出了就会被重新启动起来。但是Uiautomator又是霸道的，一旦它在运行，手机上的辅助功能、电脑上的uiautomatorviewer 就都不能用了，除非关掉该框架本身的uiautomator。下面就说下两种关闭方法
-
-方法1：
-
-直接打开uiautomator app（init成功后，就会安装上的），点击`关闭UIAutomator`
-
-方法2:
+Python程序退出了，UiAutomation就退出了。
+不过也可以通过接口的方法停止服务
 
 ```python
-d.uiautomator.stop()
-
-# d.uiautomator.start() # 启动
-# d.uiautomator.running() # 是否在运行
+d.stop_uiautomator()
 ```
 
-[ATX与Maxim共存AccessibilityService的方法](https://testerhome.com/topics/17179)
-
-# 项目历史
-* 项目重构自 <https://github.com/xiaocong/uiautomator>
-
 ## Google UiAutomator 2.0和1.x的区别
 https://www.cnblogs.com/insist8089/p/6898181.html
 
 - 新增接口：UiObject2、Until、By、BySelector
 - 引入方式：2.0中，com.android.uiautomator.core.* 引入方式被废弃。改为android.support.test.uiautomator
 - 构建系统：Maven 和/或 Ant（1.x）；Gradle（2.0）
 - 产生的测试包的形式：从zip /jar（1.x） 到 apk（2.0）
@@ -1516,31 +1430,18 @@
   adb shell uiautomator runtest UiTest.jar -c package.name.ClassName（1.x）
   adb shell am instrument -e class com.example.app.MyTest 
   com.example.app.test/android.support.test.runner.AndroidJUnitRunner（2.0）
 - 能否使用Android服务及接口？ 1.x~不能；2.0~能。
 - og输出？ 使用System.out.print输出流回显至执行端（1.x）； 输出至Logcat（2.0）
 - 执行？测试用例无需继承于任何父类，方法名不限，使用注解 Annotation进行（2.0）;  需要继承UiAutomatorTestCase，测试方法需要以test开头(1.x) 
 
-## [CHANGELOG (generated by pbr)](CHANGELOG)
-重大更新
-
-- 3.x
-
-    最低Python从3.5改为3.8
-    使用poetry代替pbr管理包依赖
-    移除图片匹配和视频录制功能
-
-- 1.0.0
-
-    移除 `d.watchers.watched` (会拖慢自动化的执行速度并且还会降低稳定性)
-
 
 ## 依赖项目
-- uiautomator守护程序 <https://github.com/openatx/atx-agent>
 - uiautomator jsonrpc server<https://github.com/openatx/android-uiautomator-server/>
+- ~~uiautomator守护程序 <https://github.com/openatx/atx-agent>~~
 
 # Contributors
 - codeskyblue ([@codeskyblue][])
 - Xiaocong He ([@xiaocong][])
 - Yuanyuan Zou ([@yuanyuan][])
 - Qian Jin ([@QianJin2013][])
 - Xu Jingjie ([@xiscoxu][])
@@ -1553,16 +1454,18 @@
 [@QianJin2013]: https://github.com/QianJin2013
 [@xiscoxu]: https://github.com/xiscoxu
 [@mingyuan-xia]: https://github.com/mingyuan-xia
 [@artikz]: https://github.com/artikz
 
 Other [contributors](../../graphs/contributors)
 
-## 其他优秀的项目 （好久没更新了，去谷歌吧）
-- [google/mobly](https://github.com/google/mobly) 谷歌内部的测试框架，虽然我不太懂，但是感觉很好用
-- https://www.appetizer.io/ 包含一个很好用的IDE，快速编写脚本，也可以插桩采集性能。
+## 其他优秀的项目
 - https://github.com/atinfo/awesome-test-automation 所有优秀测试框架的集合，包罗万象
+- [google/mobly](https://github.com/google/mobly) 谷歌内部的测试框架，虽然我不太懂，但是感觉很好用
+- https://github.com/zhangzhao4444/Maxim 基于Uiautomator的monkey
 - http://www.sikulix.com/ 基于图像识别的自动化测试框架，非常的老牌
 - http://airtest.netease.com/ 本项目的前身，后来被网易广州团队接手并继续优化。实现有一个不错的IDE
 
+排名有先后，欢迎补充
+
 # LICENSE
 [MIT](LICENSE)
```

### Comparing `uiautomator2-3.0.8/pyproject.toml` & `uiautomator2-3.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 [tool.poetry]
 name = "uiautomator2"
-version = "3.0.8"
-description = "automator for anroid device"
+version = "3.0.9"
+description = "uiautomator for android device"
 homepage = "https://github.com/openatx/uiautomator2"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["*/assets/*"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "*"
 lxml = "*"
 adbutils = "^2.2.3,!=2.3.0"
 retry = ">=0,<1"
-packaging = ">=20.3"
-pillow = "*"
-
-# TODO: remove later
 Deprecated = "*"
-filelock = ">=3,<4"
-progress = "^1.6"
+Pillow = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 isort = "^5.13.2"
 pytest-cov = "^4.1.0"
 ipython = "*"
```

### Comparing `uiautomator2-3.0.8/uiautomator2/__main__.py` & `uiautomator2-3.0.9/uiautomator2/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,247 +2,217 @@
 #
 
 from __future__ import absolute_import, print_function
 
 import argparse
 import json
 import logging
+import sys
 
 import adbutils
 
 import uiautomator2 as u2
-
-from uiautomator2.init import Initer
 from uiautomator2.version import __version__
 from uiautomator2 import enable_pretty_logging
 
 
 logger = logging.getLogger(__name__)
 
+
 def cmd_init(args):
     serial = args.serial or args.serial_optional
     if serial:
-        device = adbutils.adb.device(serial)
-        init = Initer(device)
-        init.install()
+        d = u2.connect(serial)
+        logger.debug("install apk to %s", d.serial)
+        d._setup_apks()
     else:
-        for device in adbutils.adb.iter_device():
-            init = Initer(device, loglevel=logging.DEBUG)
-            if args.addr:
-                init.set_atx_agent_addr(args.addr)
-            init.install()
+        for dev in adbutils.adb.iter_device():
+            d = u2.connect(dev)
+            logger.debug("install apk to %s", d.serial)
+            d._setup_apks()
 
 
 def cmd_purge(args):
-    """ remove minicap, minitouch, uiautomator ... """
-    device = adbutils.adb.device(args.serial)
-    init = Initer(device, loglevel=logging.DEBUG)
-    init.uninstall()
+    """remove minicap, minitouch, uiautomator ..."""
+    dev = adbutils.adb.device(args.serial)
+    dev.uninstall("com.github.uiautomator")
+    dev.uninstall("com.github.uiautomator.test")
+    dev.shell(["/data/local/tmp/atx-agent", "server", "--stop"])
+    dev.shell(["rm", "/data/local/tmp/atx-agent"])
+    logger.info("atx-agent stopped and removed")
+    dev.shell(["rm", "/data/local/tmp/minicap"])
+    dev.shell(["rm", "/data/local/tmp/minicap.so"])
+    dev.shell(["rm", "/data/local/tmp/minitouch"])
+    logger.info("minicap, minitouch removed")
+    dev.shell(["pm", "uninstall", "com.github.uiautomator"])
+    dev.shell(["pm", "uninstall", "com.github.uiautomator.test"])
+    logger.info("com.github.uiautomator uninstalled, all done !!!")
 
 
 def cmd_screenshot(args):
     d = u2.connect(args.serial)
     d.screenshot().save(args.filename)
     print("Save screenshot to %s" % args.filename)
 
 
-def cmd_identify(args):
-    d = u2.connect(args.serial)
-    d.press("home")
-    d.open_identify(args.theme)
-
-
 def cmd_install(args):
     u = u2.connect(args.serial)
     pkg_name = u.app_install(args.url)
     print("Installed", pkg_name)
 
 
 def cmd_uninstall(args):
     d = u2.connect(args.serial)
     if args.all:
         d.app_uninstall_all(verbose=True)
     else:
         for package_name in args.package_name:
-            print("Uninstall \"%s\" " % package_name, end="", flush=True)
+            print('Uninstall "%s" ' % package_name, end="", flush=True)
             ok = d.app_uninstall(package_name)
             print("OK" if ok else "FAIL")
 
 
-def cmd_healthcheck(args):
-    d = u2.connect(args.serial)
-    d.healthcheck()
-
-
 def cmd_start(args):
     d = u2.connect(args.serial)
     d.app_start(args.package_name)
 
 
 def cmd_stop(args):
     d = u2.connect(args.serial)
     if args.all:
         d.app_stop_all()
         return
 
     for package_name in args.package_name:
-        print("am force-stop \"%s\" " % package_name)
+        print('am force-stop "%s" ' % package_name)
         d.app_stop(package_name)
 
 
 def cmd_current(args):
     d = u2.connect(args.serial)
-    print(json.dumps(d.app_current(), indent=4))
+    print(json.dumps(d.app_current(), indent=4), flush=True)
 
 
 def cmd_doctor(args):
-    d = adbutils.adb.device(args.serial)
-    from .init import Initer
-    init = Initer(d)
-    logger.debug("sdk:%s abi:%s", init.sdk, init.abi)
-
-    ok = True
-    print("CHECK atx-agent")
-    if init.is_atx_agent_outdated():
-        print("\tFAIL")
-        ok = False
-        # logger.warning("atx-agent is invalid")
-    else:
-        version = init.check_atx_agent_version()
-        print("\tGOOD: atx-agent version", version)
+    """check if environment is fine"""
+    d = u2.connect(args.serial)
+    logger.debug("device serial: %s", d.serial)
+    try:
+        d.info
+        logger.info("uiautomator2 is OK")
+    except Exception as e:
+        logger.error("error: %s", e)
+        sys.exit(1)
 
-    print("CHECK uiautomator-apks")
-    if init.is_apk_outdated():
-        print("\tFAIL")
-        logger.warning("apk is invalid")
-        ok = False
-    else:
-        apk_debug = init._device.package_info("com.github.uiautomator")
-        version = apk_debug['version_name']
-        print("\tGOOD: com.github.uiautomator", version)
-    
-    if ok:
-        print("CHECK jsonrpc")
-        d = u2.connect(args.serial)
-        # print(d.info)
-        if d.alive:
-            print("\tGOOD: d.info success")
-        else:
-            ok = False
-    
-    print("==> %s <==" % ("GOOD" if ok else "FAIL"))
-    
 
 def cmd_version(args):
+    """print uiautomator2 lib version"""
     print("uiautomator2 version: %s" % __version__)
 
 
 def cmd_console(args):
     import code
     import platform
-    enable_pretty_logging()
 
     d = u2.connect(args.serial)
     model = d.shell("getprop ro.product.model").output.strip()
     serial = d.serial
     try:
         import IPython
         from traitlets.config import get_config
+
         c = get_config()
         c.InteractiveShellEmbed.colors = "neutral"
         IPython.embed(config=c, header="IPython -- d.info is ready")
     except ImportError:
         _vars = globals().copy()
         _vars.update(locals())
         shell = code.InteractiveConsole(_vars)
-        shell.interact(banner="Python: %s\nDevice: %s(%s)" %
-                       (platform.python_version(), model, serial))
+        shell.interact(
+            banner="Python: %s\nDevice: %s(%s)"
+            % (platform.python_version(), model, serial)
+        )
 
 
 _commands = [
-    dict(action=cmd_version,
-         command="version",
-         help="show version"),
-    dict(action=cmd_init,
-         command="init",
-         help="install enssential resources to device",
-         flags=[
-             dict(args=['--addr'], default='127.0.0.1:7912', help='atx-agent listen address'),
-             dict(args=['--serial', '-s'], type=str, help='serial number'),
-             dict(args=['serial_optional'],
-                  nargs='?',
-                  help='serial number, same as --serial'),
-         ]),
-    dict(action=cmd_screenshot,
-         command="screenshot",
-         help="take device screenshot",
-         flags=[
-             dict(args=['filename'],
-                  nargs='?',
-                  default="screenshot.jpg",
-                  type=str,
-                  help="output filename, jpg or png")
-         ]),
-    dict(action=cmd_identify,
-         command="identify",
-         help="quickly find your device by change device screen color",
-         flags=[
-             dict(args=['--theme'],
-                  type=str,
-                  default='red',
-                  help="black or red")
-         ]),
-    dict(action=cmd_install,
-         command="install",
-         help="install packages",
-         flags=[
-             dict(args=["url"], help="package url"),
-         ]),
-    dict(action=cmd_uninstall,
-         command="uninstall",
-         help="uninstall packages",
-         flags=[
-             dict(args=["--all"],
-                  action="store_true",
-                  help="uninstall all packages"),
-             dict(args=["package_name"], nargs="*", help="package name")
-         ]),
-    dict(action=cmd_healthcheck,
-         command="healthcheck",
-         help="recover uiautomator service"),
-    dict(action=cmd_healthcheck, command="check",
-         help="alias of healthcheck"),  # yapf: disable
-    dict(action=cmd_start,
-         command="start",
-         help="start application",
-         flags=[
-             dict(args=["package_name"],
-                  type=str,
-                  nargs=None,
-                  help="package name")
-         ]),
-    dict(action=cmd_stop,
-         command="stop",
-         help="stop application",
-         flags=[
-             dict(args=["--all"], action="store_true", help="stop all"),
-             dict(args=["package_name"], nargs="*", help="package name")
-         ]),
-    dict(action=cmd_current,
-         command="current",
-         help="show current application"),
-    dict(action=cmd_doctor,
-         command='doctor',
-         help='detect connect problem'),
-    dict(action=cmd_console,
-         command="console",
-         help="launch interactive python console"),
-    dict(action=cmd_purge,
+    dict(action=cmd_version, command="version", help="show version"),
+    dict(
+        action=cmd_init,
+        command="init",
+        help="install enssential resources to device",
+        flags=[
+            dict(
+                args=["--addr"],
+                default="127.0.0.1:7912",
+                help="atx-agent listen address",
+            ),
+            dict(args=["--serial", "-s"], type=str, help="serial number"),
+            dict(
+                args=["serial_optional"],
+                nargs="?",
+                help="serial number, same as --serial",
+            ),
+        ],
+    ),
+    dict(
+        action=cmd_screenshot,
+        command="screenshot",
+        help="take device screenshot",
+        flags=[
+            dict(
+                args=["filename"],
+                nargs="?",
+                default="screenshot.jpg",
+                type=str,
+                help="output filename, jpg or png",
+            )
+        ],
+    ),
+    dict(
+        action=cmd_install,
+        command="install",
+        help="install packages",
+        flags=[
+            dict(args=["url"], help="package url"),
+        ],
+    ),
+    dict(
+        action=cmd_uninstall,
+        command="uninstall",
+        help="uninstall packages",
+        flags=[
+            dict(args=["--all"], action="store_true", help="uninstall all packages"),
+            dict(args=["package_name"], nargs="*", help="package name"),
+        ],
+    ),
+    dict(
+        action=cmd_start,
+        command="start",
+        help="start application",
+        flags=[dict(args=["package_name"], type=str, nargs=None, help="package name")],
+    ),
+    dict(
+        action=cmd_stop,
+        command="stop",
+        help="stop application",
+        flags=[
+            dict(args=["--all"], action="store_true", help="stop all"),
+            dict(args=["package_name"], nargs="*", help="package name"),
+        ],
+    ),
+    dict(action=cmd_current, command="current", help="show current application"),
+    dict(action=cmd_doctor, command="doctor", help="detect connect problem"),
+    dict(
+        action=cmd_console, command="console", help="launch interactive python console"
+    ),
+    dict(
+        action=cmd_purge,
         command="purge",
-        help="remove minitouch, minicap, atx app etc, from device"),
+        help="remove minitouch, minicap, atx app etc, from device",
+    ),
 ]
 
 
 def main():
     # yapf: disable
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
@@ -265,20 +235,22 @@
                 args = ['-'*min(2, len(n)) + n for n in f['name']]
             kwargs = f.copy()
             kwargs.pop('name', None)
             kwargs.pop('args', None)
             sp.add_argument(*args, **kwargs)
 
     args = parser.parse_args()
+    enable_pretty_logging()
+
     if args.debug:
         logger.debug("args: %s", args)
 
     if args.subparser:
         actions[args.subparser](args)
         return
 
     parser.print_help()
     # yapf: enable
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `uiautomator2-3.0.8/uiautomator2/_selector.py` & `uiautomator2-3.0.9/uiautomator2/_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import time
 import warnings
 
 import requests
 from PIL import Image
 from retry import retry
 
-from ._proto import SCROLL_STEPS
-from .exceptions import UiObjectNotFoundError
-from .utils import Exists, intersect
+from uiautomator2._proto import SCROLL_STEPS
+from uiautomator2.exceptions import UiObjectNotFoundError
+from uiautomator2.utils import Exists, intersect
 
 
 class Selector(dict):
     """The class is to build parameters for UiSelector passed to Android device.
     """
     __fields = {
         "text": (0x01, None),  # MASK_TEXT,
```

### Comparing `uiautomator2-3.0.8/uiautomator2/assets/app-uiautomator-test.apk` & `uiautomator2-3.0.9/uiautomator2/assets/app-uiautomator-test.apk`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/assets/app-uiautomator.apk` & `uiautomator2-3.0.9/uiautomator2/assets/app-uiautomator.apk`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/assets/sync.sh` & `uiautomator2-3.0.9/uiautomator2/assets/sync.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 #!/bin/bash
 #
 
 set -e
 
 APK_VERSION="2.3.3"
-AGENT_VERSION="0.10.1"
-
-echo "Created at $(date +"%Y-%m-%d %H:%M:%S %Z")" > version.txt
+# AGENT_VERSION="0.10.1"
 
 cd "$(dirname $0)"
 
-function download_atx_agent() {
-	VERSION=$1
-	NAME="tmp-atx-agent.tar.gz"
-	URL="https://github.com/openatx/atx-agent/releases/download/$VERSION/atx-agent_${VERSION}_linux_armv6.tar.gz"
-	echo "$URL"
-	curl -L "$URL" --output "$NAME"
-	tar -xzvf "$NAME" atx-agent
-	rm -f "$NAME"
-}
+# function download_atx_agent() {
+# 	VERSION=$1
+# 	NAME="tmp-atx-agent.tar.gz"
+# 	URL="https://github.com/openatx/atx-agent/releases/download/$VERSION/atx-agent_${VERSION}_linux_armv6.tar.gz"
+# 	echo "$URL"
+# 	curl -L "$URL" --output "$NAME"
+# 	tar -xzvf "$NAME" atx-agent
+# 	rm -f "$NAME"
+# }
 
 function download_apk(){
 	VERSION=$1
 	NAME=$2
 	URL="https://github.com/openatx/android-uiautomator-server/releases/download/$VERSION/$NAME"
 	echo "$URL"
 	curl -L "$URL" --output "$NAME"
 	unzip -tq "$NAME"
 }
 
-download_atx_agent "$AGENT_VERSION"
-echo "atx_agent_version: $AGENT_VERSION" >> version.txt
+# download_atx_agent "$AGENT_VERSION"
+# echo "atx_agent_version: $AGENT_VERSION" >> version.txt
 
 download_apk "$APK_VERSION" "app-uiautomator.apk"
 download_apk "$APK_VERSION" "app-uiautomator-test.apk"
 
 echo "apk_version: $APK_VERSION" >> version.txt
```

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/htmlreport/__init__.py` & `uiautomator2-3.0.9/uiautomator2/ext/htmlreport/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/index.html` & `uiautomator2-3.0.9/uiautomator2/ext/htmlreport/assets/index.html`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/pig.jpg` & `uiautomator2-3.0.9/uiautomator2/ext/htmlreport/assets/pig.jpg`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/simplehttpserver.py` & `uiautomator2-3.0.9/uiautomator2/ext/htmlreport/assets/simplehttpserver.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/info/__init__.py` & `uiautomator2-3.0.9/uiautomator2/ext/info/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/info/conf.py` & `uiautomator2-3.0.9/uiautomator2/ext/info/conf.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/perf/README.md` & `uiautomator2-3.0.9/uiautomator2/ext/perf/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/perf/__init__.py` & `uiautomator2-3.0.9/uiautomator2/ext/perf/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/perf/net.png` & `uiautomator2-3.0.9/uiautomator2/ext/perf/net.png`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext/perf/summary.png` & `uiautomator2-3.0.9/uiautomator2/ext/perf/summary.png`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext-archived/aircv/README.md` & `uiautomator2-3.0.9/uiautomator2/_archived/aircv/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext-archived/aircv/__init__.py` & `uiautomator2-3.0.9/uiautomator2/_archived/aircv/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/README.md` & `uiautomator2-3.0.9/uiautomator2/_archived/ocr/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/__init__.py` & `uiautomator2-3.0.9/uiautomator2/_archived/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/baiduOCR.py` & `uiautomator2-3.0.9/uiautomator2/_archived/ocr/baiduOCR.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/image.py` & `uiautomator2-3.0.9/uiautomator2/image.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/init.py` & `uiautomator2-3.0.9/uiautomator2/_archived/init.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/messagebox.py` & `uiautomator2-3.0.9/uiautomator2/_archived/messagebox.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/screenrecord.py` & `uiautomator2-3.0.9/uiautomator2/screenrecord.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/settings.py` & `uiautomator2-3.0.9/uiautomator2/settings.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/swipe.py` & `uiautomator2-3.0.9/uiautomator2/swipe.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/utils.py` & `uiautomator2-3.0.9/uiautomator2/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # coding: utf-8
 #
 
 import functools
 import inspect
-import os
 import shlex
 import threading
 import typing
 from typing import Union
 
-import filelock
-
-from ._proto import Direction
-from .exceptions import SessionBrokenError, UiObjectNotFoundError
+from uiautomator2._proto import Direction
+from uiautomator2.exceptions import SessionBrokenError, UiObjectNotFoundError
 
 
 def check_alive(fn):
     @functools.wraps(fn)
     def inner(self, *args, **kwargs):
         if not self.running():
             raise SessionBrokenError(self._pkg_name)
@@ -101,15 +98,17 @@
             return self.uiobject.wait(timeout=timeout)
         return bool(self)
 
     def __repr__(self):
         return str(bool(self))
 
 
-def list2cmdline(args: Union[list, tuple]):
+def list2cmdline(args: Union[str, list, tuple]) -> str:
+    if isinstance(args, str):
+        return args
     return ' '.join(list(map(shlex.quote, args)))
 
 
 def inject_call(fn, *args, **kwargs):
     """
     Call function without known all the arguments
 
@@ -206,28 +205,10 @@
 
         with self._lock:
             return fn(self, *args, **kwargs)
     
     return inner
 
 
-def process_safe_wrapper(fn: typing.Callable[..., typing.Any]) -> typing.Callable[..., typing.Any]:
-    """
-    threadsafe for process calls
-    """
-    lockfile_path = os.path.expanduser("~/.uiautomator2/" + fn.__name__ + ".lock")
-    flock = filelock.FileLock(lockfile_path, timeout=120) # default timeout
-
-    @functools.wraps(fn)
-    def inner(self, *args, **kwargs):
-        if not hasattr(self, "_plock"):
-            self._plock = flock
-
-        with self._plock:
-            return fn(self, *args, **kwargs)
-    
-    return inner
-
-
 if __name__ == "__main__":
     for n in (1, 10000, 10000000, 10000000000):
         print(n, natualsize(n))
```

### Comparing `uiautomator2-3.0.8/uiautomator2/version.py` & `uiautomator2-3.0.9/uiautomator2/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 #
 
 # version managed by poetry
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 
 # See ChangeLog for details
 
-__apk_version__ = '2.3.3'
+# __apk_version__ = '2.3.3'
 # 2.3.3 make float windows smaller
 # 2.3.2 merge pull requests # require atx-agent>=0.10.0
 # 2.3.1 support minicapagent, rotationagent, minitouchagent
 # 2.2.1 fix click bottom(infinitly display) not working bug
 # 2.2.0 add MinitouchAgent instead of /data/local/tmp/minitouch
 # 2.1.1 add show floatWindow support(pm grant, still have no idea), add TC_TREND analysis
 # 2.0.5 add ToastActivity to show toast or just launch and quit
@@ -32,15 +32,15 @@
 # 1.0.12 add toast support
 # 1.0.11 add auto install support
 # 1.0.10 fix service not started bug
 # 1.0.9 fix apk version code and version name
 # ERR: 1.0.8 bad version number. show ip on notification
 # ERR: 1.0.7 bad version number. new input method, some bug fix
 
-__jar_version__ = 'v0.1.6'  # no useless for now.
+# __jar_version__ = 'v0.1.6'  # no useless for now.
 # v0.1.6 first release version
 
 __atx_agent_version__ = '0.10.1' # sync.sh verison should also be updated
 # 0.10.1 update androidbinary version, https://github.com/openatx/atx-agent/issues/115
 # 0.10.0 remove tunnel code, use androidx.test.runner
 # 0.9.6 fix security reason for remote control device
 # 0.9.5 log support rotate, prevent log too large
```

### Comparing `uiautomator2-3.0.8/uiautomator2/watcher.py` & `uiautomator2-3.0.9/uiautomator2/watcher.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.8/uiautomator2/webview.py` & `uiautomator2-3.0.9/uiautomator2/_archived/webview.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
 
 def runtest():
     import uiautomator2 as u2
 
     d = u2.connect_usb()
     pprint(d.request_agent("/webviews").json())
-    port = d._adb_device.forward_port("localabstract:chrome_devtools_remote")
+    port = d.adb_device.forward_port("localabstract:chrome_devtools_remote")
     wd = WebviewDriver(f"http://localhost:{port}")
     tabs = wd.get_active_tab_list()
     pprint(tabs)
 
 
 def main():
     import argparse
@@ -202,17 +202,17 @@
     parser.add_argument("-t", "--test", action="store_true", help="run test_self_driver")
     args = parser.parse_args()
 
     # WebviewDriver()
     import uiautomator2 as u2
 
     d = u2.connect_usb()
-    assert d._adb_device, "must connect with usb"
+    assert d.adb_device, "must connect with usb"
     for socket_path in d.request_agent("/webviews").json():
-        port = d._adb_device.forward_port("localabstract:"+socket_path)
+        port = d.adb_device.forward_port("localabstract:"+socket_path)
         data = requests.get(f"http://localhost:{port}/json/version").json()
         import pprint
         pprint.pprint(data)
     
 
 if __name__ == "__main__":
     main()
```

### Comparing `uiautomator2-3.0.8/uiautomator2/widget.py` & `uiautomator2-3.0.9/uiautomator2/_archived/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # coding: utf-8
 #
+#  DEPRECATED
+#
+#  This file is deprecated and will be removed in the future.
 import logging
 import re
 import time
 from collections import defaultdict, namedtuple
 from functools import partial
 from pprint import pprint
 from typing import Union
```

### Comparing `uiautomator2-3.0.8/uiautomator2/xpath.py` & `uiautomator2-3.0.9/uiautomator2/xpath.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from deprecated import deprecated
 from PIL import Image
 from lxml import etree
 
 from uiautomator2._proto import Direction
-from uiautomator2.abcd import AbstractDevice
+from uiautomator2.abstract import AbstractXPathBasedDevice
 from uiautomator2.exceptions import XPathElementNotFoundError
 from uiautomator2.utils import inject_call, swipe_in_bounds
 
 
 logger = logging.getLogger(__name__)
 
 def safe_xmlstr(s: str) -> str:
@@ -105,15 +105,15 @@
     pass
 
 
 class XPathError(Exception):
     """basic error for xpath plugin"""
 
 class XPath(object):
-    def __init__(self, d: AbstractDevice):
+    def __init__(self, d: AbstractXPathBasedDevice):
         """
         Args:
             d (uiautomator2 instance)
         """
         self._d = d
         assert hasattr(d, "wait_timeout")
         # TODO: remove wait_timeout
@@ -769,19 +769,25 @@
 
     @property
     def info(self) -> Dict[str, Any]:
         ret = {}
         for k, v in dict(self.attrib).items():
             if k in ("bounds", "class", "package", "content-desc"):
                 continue
-            ret[convert_to_camel_case(k)] = v
+            if k in ("checkable", "checked", "clickable", "enabled", "focusable", "focused", "scrollable",
+                     "long-clickable", "password", "selected", "visible-to-user"):
+                ret[convert_to_camel_case(k)] = v == "true"
+            elif k == "index":
+                ret[k] = int(v)
+            else:
+                ret[convert_to_camel_case(k)] = v
 
         ret["childCount"] = len(self.elem.getchildren())
         ret["className"] = self.elem.tag
         lx, ly, rx, ry = self.bounds
         ret["bounds"] = {"left": lx, "top": ly, "right": rx, "bottom": ry}
 
         # 名字命名的有点奇怪，为了兼容性暂时保留
         ret["packageName"] = self.attrib.get("package")
         ret["contentDescription"] = self.attrib.get("content-desc")
         ret["resourceName"] = self.attrib.get("resource-id")
-        return ret
+        return ret
```

### Comparing `uiautomator2-3.0.8/PKG-INFO` & `uiautomator2-3.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: uiautomator2
-Version: 3.0.8
-Summary: automator for anroid device
+Version: 3.0.9
+Summary: uiautomator for android device
 Home-page: https://github.com/openatx/uiautomator2
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Deprecated
+Requires-Dist: Pillow
 Requires-Dist: adbutils (>=2.2.3,<3.0.0,!=2.3.0)
-Requires-Dist: filelock (>=3,<4)
 Requires-Dist: lxml
-Requires-Dist: packaging (>=20.3)
-Requires-Dist: pillow
-Requires-Dist: progress (>=1.6,<2.0)
 Requires-Dist: requests
 Requires-Dist: retry (>=0,<1)
 Description-Content-Type: text/markdown
 
 # uiautomator2
 [![PyPI](https://img.shields.io/pypi/v/uiautomator2.svg)](https://pypi.python.org/pypi/uiautomator2)
 ![PyPI](https://img.shields.io/pypi/pyversions/uiautomator2.svg)
@@ -32,35 +29,37 @@
 
 QQ交流群: **815453846**
 
 > 有段时间没有维护这个项目了（可能有两年了），但是最近工作需要又重新研究一下Android原生自动化，当然又调研了Appium，对比下来一看，发现uiautomator2这个项目的运行速度是真的好快，从检测元素到点击，都是毫秒级的，代码也比较好理解。真是没想到以前竟然写出了这么神奇的项目，这么好的项目怎么能让它落灰呢，得好好整一整，一些垃圾代码清理清理。所以项目版本从2.x.x升级到了3.x.x
 
 还在用2.x.x版本的用户，可以先看一下[2to3](docs/2to3.md) 再决定是否要升级3.x.x （我个人还是非常建议升级的）
 
+2到3毕竟是大版本升级，很多的函数删掉了。首先删掉的就是atx-agent，其次还有一堆atx-agent相关的函数。废弃的功能比如init.
+
 各种依赖库的版本号
 
 - [![PyPI](https://img.shields.io/pypi/v/uiautomator2.svg?label=uiautomator2)](https://pypi.python.org/pypi/uiautomator2)
 - [![PyPI](https://img.shields.io/pypi/v/adbutils.svg?label=adbutils)](https://github.com/openatx/adbutils)
-- [![GitHub tag (latest SemVer)](https://img.shields.io/github/tag/openatx/atx-agent.svg?label=atx-agent)](https://github.com/openatx/atx-agent)
 - [![GitHub tag (latest SemVer)](https://img.shields.io/github/tag/openatx/android-uiautomator-server.svg?label=android-uiautomator-server)](https://github.com/openatx/android-uiautomator-server)
+- ~~[![GitHub tag (latest SemVer)](https://img.shields.io/github/tag/openatx/atx-agent.svg?label=atx-agent)](https://github.com/openatx/atx-agent)~~
 
 [UiAutomator](https://developer.android.com/training/testing/ui-automator.html)是Google提供的用来做安卓自动化测试的一个Java库，基于Accessibility服务。功能很强，可以对第三方App进行测试，获取屏幕上任意一个APP的任意一个控件属性，并对其进行任意操作，但有两个缺点：1. 测试脚本只能使用Java语言 2. 测试脚本要打包成jar或者apk包上传到设备上才能运行。
 
 我们希望测试逻辑能够用Python编写，能够在电脑上运行的时候就控制手机。这里要非常感谢 Xiaocong He ([@xiaocong][])，他将这个想法实现了出来（见[xiaocong/uiautomator](https://github.com/xiaocong/uiautomator)），原理是在手机上运行了一个http rpc服务，将uiautomator中的功能开放出来，然后再将这些http接口封装成Python库。
-因为`xiaocong/uiautomator`这个库，已经很久不见更新。所以我们直接fork了一个版本，为了方便做区分我们就在后面加了个2 [openatx/uiautomator2](https://github.com/openatx/uiautomator2)
+因为`xiaocong/uiautomator`这个库，已经很久不见更新。所以我们直接fork了一个版本，为了方便做区分我们就在后面加了个2 [openatx/uiautomator2](https://github.com/openatx/uiautomator2),对应的Android包源码我也fork了一份，[openatx/android-uiautomator-server](https://github.com/openatx/android-uiautomator-server)
 
 除了对原有的库的bug进行了修复，还增加了很多新的Feature。主要有以下部分：
 
-* 设备和开发机可以脱离数据线，通过WiFi互联（基于[atx-agent](https://github.com/openatx/atx-agent)）
+* ~~设备和开发机可以脱离数据线，通过WiFi互联（基于[atx-agent](https://github.com/openatx/atx-agent)~~
 * ~~集成了[openstf/minicap](https://github.com/openstf/minicap)达到实时屏幕投频，以及实时截图~~
 * ~~集成了[openstf/minitouch](https://github.com/openstf/minitouch)达到精确实时控制设备~~
 * 修复了[xiaocong/uiautomator](https://github.com/xiaocong/uiautomator)经常性退出的问题
 * 代码进行了重构和精简，方便维护
 * 实现了一个设备管理平台(也支持iOS) [atxserver2](https://github.com/openatx/atxserver2) （注：目前不怎么维护了）
-* 扩充了toast获取和展示的功能
+* 扩充了toast获取和展示的功能（需要手动开启ATX的悬浮窗权限） 貌似有bug用不了
 
 >这里要先说明下，因为经常有很多人问 openatx/uiautomator2 并不支持iOS测试，需要iOS自动化测试，可以转到这个库 [openatx/facebook-wda](https://github.com/openatx/facebook-wda)。
 
 > PS: 这个库 ~~<https://github.com/NeteaseGame/ATX>~~ 目前已经不维护了，请尽快更换。
 
 这里有一份快速参考，适合已经入门的人 [QUICK REFERENCE GUIDE](QUICK_REFERENCE.md)，欢迎多提意见。
 
@@ -85,15 +84,15 @@
 这时看到类似下面的输出，就可以正式开始用我们这个库了。因为这个库功能太多，后面还有很多的内容，需要慢慢去看 ....
 
 ```
 {'currentPackageName': 'net.oneplus.launcher', 'displayHeight': 1920, 'displayRotation': 0, 'displaySizeDpX': 411, 'displaySizeDpY': 731, 'displayWidth': 1080, 'productName': 'OnePlus5', '
 screenOn': True, 'sdkInt': 27, 'naturalOrientation': True}
 ```
 
-一般情况下都会成功，不过也可能会有意外。可以加QQ群反馈问题，群里有很多大佬可以帮你解决问题。
+一般情况下都会成功，不过也可能会有意外。可以加QQ群反馈问题(群号在最上面），群里有很多大佬可以帮你解决问题。
 
 ## Sponsors
 Thank you to all our sponsors! ✨🍰✨
 
 ### 金牌赞助商（Gold Sponsor）
 [![霍格沃兹测试开发学社](https://testing-studio.com/img/icon.png)](https://qrcode.testing-studio.com/f?from=ATX&url=https://testing-studio.com/)
 
@@ -103,17 +102,17 @@
 优秀文章推荐 (欢迎QQ群里at我反馈）
 
 - [py-uiautomator2通过悬浮窗让服务长时间可用](https://zhuanlan.zhihu.com/p/688009468) 这个**强烈推荐**看一下
 - [termux里如何部署uiautomator2简介](https://www.cnblogs.com/ze-yan/p/12242383.html) by `成都-测试只会一点点`
 
 ## 相关项目
 - 基于adb协议与Android进行交互的库 [adbutils](https://github.com/openatx/adbutils)
-- 设备管理平台，设备多了就会用到 [atxserver2](https://github.com/openatx/atxserver2) （寻找项目维护人员）
-- [atx-agent](https://github.com/openatx/atx-agent) 运行在设备上的驻守程序，go开发，用于保活设备上相关的服务
 - [uiauto.dev](https://uiauto.dev) 用于查看UI层级结构，类似于uiautomatorviewer(用于替代之前写的weditor），用于查看UI层级结构 
+- 设备管理平台，设备多了就会用到 [atxserver2](https://github.com/openatx/atxserver2) （寻找项目维护人员）
+- ~~[atx-agent](https://github.com/openatx/atx-agent) 运行在设备上的驻守程序，go开发，用于保活设备上相关的服务~~
 - ~~[weditor](https://github.com/openatx/weditor) 类似于uiautomatorviewer，专门为本项目开发的辅助编辑器(这个暂不维护了~~
 
 **[Installation](#installation)**
 
 **[Connect to a device](#connect-to-a-device)**
 
 **[Command line](#command-line)**
@@ -141,31 +140,16 @@
   - **[Selector](#selector)**
   - **[Watcher](#watcher)**
   - **[Global settings](#global-settings)**
   - **[Input method](#input-method)**
   - **[Toast](#toast)**
   - **[XPath](#xpath)**
   - **[Screenrecord](#screenrecord)**
-  - **[Image match](#image-match)**
-
-**常见问题**
-  - **[停止UiAutomator守护服务，释放AccessibilityService](#stop-uiautomator)**
-  - **[502错误](https://github.com/openatx/uiautomator2/wiki/Common-issues)**
-  - **[Connection Error, 深度睡眠, 点击偏差 等](https://github.com/openatx/uiautomator2/wiki/Common-issues)**
-  
-
-**[实验性功能](https://github.com/openatx/uiautomator2/wiki/Common-issues#%E5%AE%9E%E9%AA%8C%E6%80%A7%E5%8A%9F%E8%83%BD)**
-  - **远程投屏**
-  - **htmlreport**
-  - **诊断uiautomator2方法**
-  - **Plugin**
-  - **Hooks**
-  - **失败时弹出提示框**
+  - **[Image match](#image-match) Removed**
 
-**[项目历史](#项目历史)**
 
 **[Contributors](#contributors)**
 
 **[LICENSE](#license)**
 
 
 # Installation
@@ -188,59 +172,37 @@
     浏览器打开 https://uiauto.dev 查看当前设备的界面结构。
 
     **appinspector介绍**
 
     [uiauto.dev](https://github.com/codeskyblue/uiauto.dev) 是一个独立与uiautomator2之外的一个项目，用于查看图层结构的。属于旧版项目[weditor的重构版本](https://github.com/openatx/weditor)，后续也许会收费（价格肯定物超所值），来支持当前这个项目继续维护下去。感兴趣的可以加群讨论(也包含提需求) QQ群 536481989
 
 # Connect to a device
-There are two ways to connect to the device. 
-
-1. **Through WiFi**
-
-Suppose device IP is `10.0.0.1` and your PC is in the same network.
-
-```python
-import uiautomator2 as u2
-
-d = u2.connect('10.0.0.1') # alias for u2.connect_wifi('10.0.0.1')
-print(d.info)
-```
-
-2. **Through USB**
-
-Suppose the device serial is `123456f` (seen from `adb devices`)
+use serialno to connect device eg. `123456f` (seen from `adb devices`)
 
 ```python
 import uiautomator2 as u2
 
 d = u2.connect('123456f') # alias for u2.connect_usb('123456f')
 print(d.info)
 ```
 
-3. **Through ADB WiFi**
+Serial can be passed through env-var `ANDROID_SERIAL`
 
-```python
-import uiautomator2 as u2
 
-d = u2.connect_adb_wifi("10.0.0.1:5555")
-
-# Equals to 
-# + Shell: adb connect 10.0.0.1:5555
-# + Python: u2.connect_usb("10.0.0.1:5555")
+```python
+# export ANDROID_SERIAL=123456f
+d = u2.connect()
 ```
 
-Calling `u2.connect()` with no argument, `uiautomator2` will obtain device IP from the environment variable `ANDROID_DEVICE_IP` or `ANDROID_SERIAL`.
-If this environment variable is empty, uiautomator will fall back to `connect_usb` and you need to make sure that there is only one device connected to the computer.
-
 # Command line
 其中的`$device_ip`代表设备的ip地址
 
 如需指定设备需要传入`--serial` 如 `python3 -m uiautomator2 --serial bff1234 <SubCommand>`, SubCommand为子命令（screenshot, current 等）
 
-> 1.0.3 Added: `python3 -m uiautomator2`可以简写为`uiautomator2`
+> 1.0.3 Added: `python3 -m uiautomator2` equals to `uiautomator2`
 
 - screenshot: 截图
 
     ```bash
     $ uiautomator2 screenshot screenshot.jpg
     ```
 
@@ -251,57 +213,47 @@
     {
         "package": "com.android.browser",
         "activity": "com.uc.browser.InnerUCMobile",
         "pid": 28478
     }
     ```
     
-- uninstall： 卸载
+- uninstall： Uninstall app
 
     ```bash
     $ uiautomator2 uninstall <package-name> # 卸载一个包
     $ uiautomator2 uninstall <package-name-1> <package-name-2> # 卸载多个包
     $ uiautomator2 uninstall --all # 全部卸载
     ```
 
-- stop: 停止应用
+- stop: Stop app
 
     ```bash
     $ uiautomator2 stop com.example.app # 停止一个app
     $ uiautomator2 stop --all # 停止所有的app
     ```
-    
-- install: 安装apk，apk通过URL给出 (暂时不能用)
-- healthcheck: 健康检查 (暂不能用)
 
-- doctor: 检查uiautomator2无法使用的原因
+- doctor:
 
     ```bash
     $ uiautomator2 doctor
-    I 210519 16:48:45 init:156] uiautomator2 version: 2.14.2.dev1
-    [D 210519 16:48:45 __main__:105] sdk:29 abi:arm64-v8a
-    CHECK atx-agent
-            GOOD: atx-agent version 0.10.0
-    CHECK uiautomator-apks
-            GOOD: com.github.uiautomator 2.3.3
-    CHECK jsonrpc
-            GOOD: d.info success
-    ==> GOOD <==
+    [I 2024-04-25 19:53:36,288 __main__:101 pid:15596] uiautomator2 is OK
     ```
     
 # API Documents
 
-### New command timeout
-How long (in seconds) will wait for a new command from the client before assuming the client quit and ending the uiautomator service （Default 3 minutes）
+### New command timeout （Removed)
+When python quit, the UiAutomation service also quit.
+<!-- How long (in seconds) will wait for a new command from the client before assuming the client quit and ending the uiautomator service （Default 3 minutes）
 
 配置accessibility服务的最大空闲时间，超时将自动释放。默认3分钟。
 
 ```python
 d.set_new_command_timeout(300) # change to 5 minutes, unit seconds
-```
+``` -->
 
 ### Debug HTTP requests
 打印出代码背后的HTTP请求信息
 
 ```python
 >>> d.debug = True
 >>> d.info
@@ -421,30 +373,26 @@
     ```python
     d.pull("/sdcard/tmp.txt", "tmp.txt")
 
     # FileNotFoundError will raise if the file is not found on the device
     d.pull("/sdcard/some-file-not-exists.txt", "tmp.txt")
     ```
 
-### 检查并维持设备端守护进程处于运行状态
-```python
-d.healthcheck()
-```
 
-### ~~Auto click permission dialogs~~
+### ~~Auto click permission dialogs~~ (Removed)
 **注意注意** `disable_popups`函数，检测发现很不稳定，暂时不要使用，等候通知。
-
+<!-- 
 Import in version 0.1.1
 
 ```python
 d.disable_popups() # automatic skip popups
 d.disable_popups(False) # disable automatic skip popups
 ```
 
-![popup](docs/img/popup.png)
+![popup](docs/img/popup.png) -->
 
 ### Open Scheme
 
 ```python
 d.open_url("appname://appnamehost")
 ```
 
@@ -479,16 +427,16 @@
     output, exit_code = d.shell(["ls", "-l"])
     # output: "/....", exit_code: 0
     ```
 
    This returns a string for stdout merged with stderr.
    If the command is a blocking command, `shell` will also block until the command is completed or the timeout kicks in. No partial output will be received during the execution of the command. This API is not suitable for long-running commands. The shell command given runs in a similar environment of `adb shell`, which has a Linux permission level of `adb` or `shell` (higher than an app permission).
 
-* Run a long-running shell command
-
+* Run a long-running shell command (Removed)
+<!-- 
     add stream=True will return `requests.models.Response` object. More info see [requests stream](http://docs.python-requests.org/zh_CN/latest/user/quickstart.html#id5)
 
     ```python
     r = d.shell("logcat", stream=True)
     # r: requests.models.Response
     deadline = time.time() + 10 # run maxium 10s
     try:
@@ -496,17 +444,17 @@
             if time.time() > deadline:
                 break
             print("Read:", line.decode('utf-8'))
     finally:
         r.close() # this method must be called
     ```
 
-    Command will be terminated when `r.close()` called.
+    Command will be terminated when `r.close()` called. -->
     
-### Session
+### Session (Removed)
 Session represent an app lifecycle. Can be used to start app, detect app crash.
 
 * Launch and close app
 
     ```python
     sess = d.session("com.netease.cloudmusic") # start 网易云音乐
     sess.close() # 停止网易云音乐
@@ -521,17 +469,14 @@
     ```
 
 * Attach to the running app
 
     ```python
     # launch app if not running, skip launch if already running
     sess = d.session("com.netease.cloudmusic", attach=True)
-
-    # raise SessionBrokenError if not running
-    sess = d.session("com.netease.cloudmusic", attach=True, strict=True)
     ```
 
 * Detect app crash
 
     ```python
     # When app is still running
     sess(text="Music").click() # operation goes normal
@@ -555,25 +500,24 @@
 ```python
 d.info
 ```
 
 Below is a possible output:
 
 ```
-{ 
-    u'displayRotation': 0,
-    u'displaySizeDpY': 640,
-    u'displaySizeDpX': 360,
-    u'currentPackageName': u'com.android.launcher',
-    u'productName': u'takju',
-    u'displayWidth': 720,
-    u'sdkInt': 18,
-    u'displayHeight': 1184,
-    u'naturalOrientation': True
-}
+{'currentPackageName': 'com.android.systemui',
+ 'displayHeight': 1560,
+ 'displayRotation': 0,
+ 'displaySizeDpX': 360,
+ 'displaySizeDpY': 780,
+ 'displayWidth': 720,
+ 'naturalOrientation': True,
+ 'productName': 'ELE-AL00',
+ 'screenOn': True,
+ 'sdkInt': 29}
 ```
 
 Get window size
 
 ```python
 print(d.window_size())
 # device upright output example: (1080, 1920)
@@ -603,18 +547,21 @@
 # output example: 74aAEDR428Z9
 ```
 
 Get WLAN ip
 
 ```python
 print(d.wlan_ip)
-# output example: 10.0.0.1
+# output example: 10.0.0.1 or None
 ```
 
-Get detailed device info
+
+~~Get detailed device info~~ `d.device_info`
+
+device_info was Removed since 3.x
 
 ```python
 print(d.device_info)
 ```
 
 Below is a possible output:
 
@@ -704,16 +651,16 @@
 You can find all key code definitions at [Android KeyEvnet](https://developer.android.com/reference/android/view/KeyEvent.html)
 
 * Unlock screen
 
     ```python
     d.unlock()
     # This is equivalent to
-    # 1. launch activity: com.github.uiautomator.ACTION_IDENTIFY
-    # 2. press the "home" key
+    # 1. press("power")
+    # 2. swipe from left-bottom to right-top
     ```
 
 ### Gesture interaction with the device
 * Click on the screen
 
     ```python
     d.click(x, y)
@@ -780,15 +727,15 @@
 
     这个接口属于比较底层的原始接口，感觉并不完善，不过凑合能用。注：这个地方并不支持百分比
 
     ```python
     d.touch.down(10, 10) # 模拟按下
     time.sleep(.01) # down 和 move 之间的延迟，自己控制
     d.touch.move(15, 15) # 模拟移动
-    d.touch.up() # 模拟抬起
+    d.touch.up(10, 10) # 模拟抬起
     ```
 
 Note: click, swipe, drag operations support percentage position values. Example:
 
 `d.long_click(0.5, 0.5)` means long click center of screen
 
 ### Screen-related
@@ -842,15 +789,15 @@
     imagebin = d.screenshot(format='raw')
     open("some.jpg", "wb").write(imagebin)
     ```
 
 * Dump UI hierarchy
 
     ```python
-    # get the UI hierarchy dump content (unicoded).
+    # get the UI hierarchy dump content
     xml = d.dump_hierarchy()
     ```
 
 * Open notification or quick settings
 
     ```python
     d.open_notification()
@@ -1294,37 +1241,31 @@
 ```
 
 另外文档还是有很多没有写，推荐直接去看源码[watcher.py](uiautomator2/watcher.py)
 
 ### Global settings
 
 ```python
-d.HTTP_TIMEOUT = 60 # 默认值60s, http默认请求超时时间
-
-# 当设备掉线时，等待设备在线时长，仅当TMQ=true时有效，支持通过环境变量 WAIT_FOR_DEVICE_TIMEOUT 设置
-d.WAIT_FOR_DEVICE_TIMEOUT = 70 
+u2.HTTP_TIMEOUT = 60 # 默认值60s, http默认请求超时时间
 ```
 
 其他的配置，目前已大部分集中到 `d.settings` 中，根据后期的需求配置可能会有增减。
 
 ```python
 print(d.settings)
 {'operation_delay': (0, 0),
  'operation_delay_methods': ['click', 'swipe'],
- 'wait_timeout': 20.0,
- 'xpath_debug': False}
+ 'wait_timeout': 20.0}
 
 # 配置点击前延时0.5s，点击后延时1s
 d.settings['operation_delay'] = (.5, 1)
 
 # 修改延迟生效的方法
 # 其中 double_click, long_click 都对应click
 d.settings['operation_delay_methods'] = ['click', 'swipe', 'drag', 'press']
-
-d.settings['xpath_debug'] = True # 开启xpath插件的调试日志
 d.settings['wait_timeout'] = 20.0 # 默认控件等待时间（原生操作，xpath插件的等待时间）
 ```
 
 对于随着版本升级，设置过期的配置时，会提示Deprecated，但是不会抛异常。
 
 ```bash
 >>> d.settings['click_before_delay'] = 1  
@@ -1381,15 +1322,15 @@
 _什么时候该使用这个函数呢？_
 
 有些时候在EditText中输入完内容之后，调用`press("search")` or `press("enter")`发现并没有什么反应。
 这个时候就需要`send_action`函数了，这里用到了只有输入法才能用的[IME_ACTION_CODE](https://developer.android.com/reference/android/view/inputmethod/EditorInfo)。
 `send_action`先broadcast命令发送给输入法操作`IME_ACTION_CODE`，由输入法完成后续跟EditText的通信。（原理我不太清楚，有了解的，提issue告诉我)
 
 ### Toast (2.2版本之后有添加回来)
-Show Toast
+Show Toast (好像有点bug)
 
 ```python
 d.toast.show("Hello world")
 d.toast.show("Hello world", 1.0) # show for 1.0s, default 1.0s
 ```
 
 Get Toast
@@ -1476,66 +1417,36 @@
 # or do something else
 
 d.screenrecord.stop() # 停止录制后，output.mp4文件才能打开
 ```
 
 录制的时候也可以指定fps（当前是20），这个值是率低于minicap输出图片的速度，感觉已经很好了，不建议你修改。
 
-### Image match (3.x开始移除该功能)
-3.x开始废弃
-
-图像匹配，在使用这个功能之前你需要先把依赖安装上
-
-```bash
-pip3 install -U "uiautomator2[image]" -i https://pypi.doubanio.com/simple
-```
+# Enable uiautomator2 logger
 
-目前开放两个接口
- 
+```python
+from uiautomator2 import enable_pretty_logging
+enable_pretty_logging()
 ```
-imdata = "target.png" # 也可以是URL, PIL.Image或OpenCV打开的图像
 
-d.image.match(imdata) 
-# 匹配待查找的图片，立刻返回一个结果
-# 返回一个dict, eg: {"similarity": 0.9, "point": [200, 300]}
+Or
 
-d.image.click(imdata, timeout=20.0)
-# 在20s的时间内调用match轮询查找图片，当similarity>0.9时，执行点击操作
 ```
-
-该功能还在完善中，图片需要手机的原图裁剪后的图才可以。
-
-# 常见问题
-很多没写在这个地方的，都放到了这里 [Common Issues](https://github.com/openatx/uiautomator2/wiki/Common-issues)
+logger = logging.getLogger("uiautomator2")
+# setup logger
+```
 
 ## Stop UiAutomator
-停止UiAutomator守护服务
-
-https://github.com/openatx/uiautomator2/wiki/Common-issues
-
-因为有`atx-agent`的存在，Uiautomator会被一直守护着，如果退出了就会被重新启动起来。但是Uiautomator又是霸道的，一旦它在运行，手机上的辅助功能、电脑上的uiautomatorviewer 就都不能用了，除非关掉该框架本身的uiautomator。下面就说下两种关闭方法
-
-方法1：
-
-直接打开uiautomator app（init成功后，就会安装上的），点击`关闭UIAutomator`
-
-方法2:
+Python程序退出了，UiAutomation就退出了。
+不过也可以通过接口的方法停止服务
 
 ```python
-d.uiautomator.stop()
-
-# d.uiautomator.start() # 启动
-# d.uiautomator.running() # 是否在运行
+d.stop_uiautomator()
 ```
 
-[ATX与Maxim共存AccessibilityService的方法](https://testerhome.com/topics/17179)
-
-# 项目历史
-* 项目重构自 <https://github.com/xiaocong/uiautomator>
-
 ## Google UiAutomator 2.0和1.x的区别
 https://www.cnblogs.com/insist8089/p/6898181.html
 
 - 新增接口：UiObject2、Until、By、BySelector
 - 引入方式：2.0中，com.android.uiautomator.core.* 引入方式被废弃。改为android.support.test.uiautomator
 - 构建系统：Maven 和/或 Ant（1.x）；Gradle（2.0）
 - 产生的测试包的形式：从zip /jar（1.x） 到 apk（2.0）
@@ -1543,31 +1454,18 @@
   adb shell uiautomator runtest UiTest.jar -c package.name.ClassName（1.x）
   adb shell am instrument -e class com.example.app.MyTest 
   com.example.app.test/android.support.test.runner.AndroidJUnitRunner（2.0）
 - 能否使用Android服务及接口？ 1.x~不能；2.0~能。
 - og输出？ 使用System.out.print输出流回显至执行端（1.x）； 输出至Logcat（2.0）
 - 执行？测试用例无需继承于任何父类，方法名不限，使用注解 Annotation进行（2.0）;  需要继承UiAutomatorTestCase，测试方法需要以test开头(1.x) 
 
-## [CHANGELOG (generated by pbr)](CHANGELOG)
-重大更新
-
-- 3.x
-
-    最低Python从3.5改为3.8
-    使用poetry代替pbr管理包依赖
-    移除图片匹配和视频录制功能
-
-- 1.0.0
-
-    移除 `d.watchers.watched` (会拖慢自动化的执行速度并且还会降低稳定性)
-
 
 ## 依赖项目
-- uiautomator守护程序 <https://github.com/openatx/atx-agent>
 - uiautomator jsonrpc server<https://github.com/openatx/android-uiautomator-server/>
+- ~~uiautomator守护程序 <https://github.com/openatx/atx-agent>~~
 
 # Contributors
 - codeskyblue ([@codeskyblue][])
 - Xiaocong He ([@xiaocong][])
 - Yuanyuan Zou ([@yuanyuan][])
 - Qian Jin ([@QianJin2013][])
 - Xu Jingjie ([@xiscoxu][])
@@ -1580,17 +1478,19 @@
 [@QianJin2013]: https://github.com/QianJin2013
 [@xiscoxu]: https://github.com/xiscoxu
 [@mingyuan-xia]: https://github.com/mingyuan-xia
 [@artikz]: https://github.com/artikz
 
 Other [contributors](../../graphs/contributors)
 
-## 其他优秀的项目 （好久没更新了，去谷歌吧）
-- [google/mobly](https://github.com/google/mobly) 谷歌内部的测试框架，虽然我不太懂，但是感觉很好用
-- https://www.appetizer.io/ 包含一个很好用的IDE，快速编写脚本，也可以插桩采集性能。
+## 其他优秀的项目
 - https://github.com/atinfo/awesome-test-automation 所有优秀测试框架的集合，包罗万象
+- [google/mobly](https://github.com/google/mobly) 谷歌内部的测试框架，虽然我不太懂，但是感觉很好用
+- https://github.com/zhangzhao4444/Maxim 基于Uiautomator的monkey
 - http://www.sikulix.com/ 基于图像识别的自动化测试框架，非常的老牌
 - http://airtest.netease.com/ 本项目的前身，后来被网易广州团队接手并继续优化。实现有一个不错的IDE
 
+排名有先后，欢迎补充
+
 # LICENSE
 [MIT](LICENSE)
```

