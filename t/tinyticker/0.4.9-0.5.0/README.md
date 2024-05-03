# Comparing `tmp/tinyticker-0.4.9.tar.gz` & `tmp/tinyticker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.4.9.tar", max compression
+gzip compressed data, was "tinyticker-0.5.0.tar", max compression
```

## Comparing `tinyticker-0.4.9.tar` & `tinyticker-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-03-27 23:36:51.638880 tinyticker-0.4.9/LICENSE
--rw-r--r--   0        0        0     3863 2024-03-27 23:36:51.638880 tinyticker-0.4.9/README.md
--rw-r--r--   0        0        0      869 2024-03-27 23:36:51.638880 tinyticker-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      207 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/__init__.py
--rw-r--r--   0        0        0     5101 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/__main__.py
--rw-r--r--   0        0        0     1731 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/config.py
--rw-r--r--   0        0        0     9202 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/paths.py
--rw-r--r--   0        0        0    15408 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/ticker.py
--rw-r--r--   0        0        0     3155 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/utils.py
--rw-r--r--   0        0        0      318 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1060 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     8353 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    11878 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14564 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10440 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     5824 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6616 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5679 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     3148 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epdconfig.py
--rw-r--r--   0        0        0     1285 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2547 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6826 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/app.py
--rw-r--r--   0        0        0     2566 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    10616 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0      787 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     1275 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 tinyticker-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-03 22:53:19.227821 tinyticker-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3863 2024-05-03 22:53:19.227821 tinyticker-0.5.0/README.md
+-rw-r--r--   0        0        0      899 2024-05-03 22:53:19.227821 tinyticker-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/__init__.py
+-rw-r--r--   0        0        0     5821 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/__main__.py
+-rw-r--r--   0        0        0     1731 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/config.py
+-rw-r--r--   0        0        0     9301 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/paths.py
+-rw-r--r--   0        0        0    15408 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/ticker.py
+-rw-r--r--   0        0        0     3123 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/utils.py
+-rw-r--r--   0        0        0      318 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1259 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     8376 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    11895 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14581 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10457 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     5835 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6627 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5690 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0     3148 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epdconfig.py
+-rw-r--r--   0        0        0     1283 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2547 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6931 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/web/app.py
+-rw-r--r--   0        0        0     2909 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    15092 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0      787 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     1369 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 tinyticker-0.5.0/PKG-INFO
```

### Comparing `tinyticker-0.4.9/LICENSE` & `tinyticker-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/README.md` & `tinyticker-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/pyproject.toml` & `tinyticker-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.4.9"
+version = "0.5.0"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9"
 "RPi.GPIO" = "^0.7.0"
 spidev = "^3.5"
 Pillow = "^10.0.1"
 cryptocompare = "^0.7.5"
 pandas = "^1.3.5"
 matplotlib = "^3.5.1"
 mplfinance = "^0.12.7-alpha.17"
 Flask = "^2.0.2"
 yfinance = "^0.2.0"
 qrcode = "^7.3.1"
 packaging = "^23.0"
+numpy = "^1.26"
+watchdog = "^4.0.0"
 
 [tool.poetry.scripts]
 tinyticker = 'tinyticker.__main__:main'
 tinyticker-web = 'tinyticker.web.__main__:main'
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
```

### Comparing `tinyticker-0.4.9/tinyticker/__main__.py` & `tinyticker-0.5.0/tinyticker/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import os
 import signal
 import sys
 from pathlib import Path
 from time import sleep
 from typing import List
 
+from watchdog.events import FileModifiedEvent, FileSystemEventHandler
+from watchdog.observers import Observer
+
 from . import __version__, logger
 from .config import TinytickerConfig
 from .display import Display
 from .paths import CONFIG_FILE, PID_FILE
 from .ticker import Sequence
 from .utils import RawTextArgumentDefaultsHelpFormatter, set_verbosity
 
@@ -143,25 +146,42 @@
         os.execv(sys.argv[0], sys.argv)
 
     signal.signal(signal.SIGUSR1, restart)
 
     def refresh(*_) -> None:
         """Kill the ticker process, it gets restarted in the main thread."""
         logger.info("Refreshing ticker process.")
-        tick_process.kill()
-        tick_process.join()
-        tick_process.close()
+        if not tick_process._closed and tick_process.is_alive():  # type: ignore
+            tick_process.kill()
+            tick_process.join()
+            tick_process.close()
+
+    class ConfigModifiedHandler(FileSystemEventHandler):
+        def on_modified(self, event):
+            logger.info(f"{event.src_path} was changed, refreshing ticker thread.")
+            refresh()
+
+    observer = Observer()
+    config_modified_handler = ConfigModifiedHandler()
+    observer.schedule(
+        config_modified_handler, config_file, event_filter=[FileModifiedEvent]
+    )
+    observer.start()
 
     signal.signal(signal.SIGUSR2, refresh)
 
     def cleanup():
         """Remove the PID file on exit."""
         logger.info("Exiting.")
         if PID_FILE.is_file():
             PID_FILE.unlink()
+        observer.stop()
+        observer.join()
+        tick_process.kill()
+        tick_process.join()
 
     atexit.register(cleanup)
 
     # start ticking
     tick_process = start_ticker_process(config_file)
     while True:
         if tick_process._closed or not tick_process.is_alive():  # type: ignore
```

### Comparing `tinyticker-0.4.9/tinyticker/config.py` & `tinyticker-0.5.0/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/display.py` & `tinyticker-0.5.0/tinyticker/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 from typing import Optional, Tuple
 
-import matplotlib
+import matplotlib as mpl
+from matplotlib.figure import Figure
+from matplotlib.axes import Axes
 import matplotlib.pyplot as plt
 import mplfinance as mpf
 import numpy as np
 import pandas as pd
 from PIL import Image
 
 from .config import TinytickerConfig
@@ -16,14 +18,15 @@
     up="white",
     down="black",
     edge="black",
     wick="black",
     ohlc="black",
     volume="black",
 )
+MARKETCOLORS["vcedge"] = {"up": "black", "down": "black"}
 STYLE = mpf.make_mpf_style(marketcolors=MARKETCOLORS, mavcolors=["k"])
 STYLE_HIGHLIGHT = mpf.make_mpf_style(marketcolors=MARKETCOLORS, mavcolors=["r"])
 TEXT_BBOX = {
     "boxstyle": "square,pad=0",
     "facecolor": "white",
     "edgecolor": "white",
 }
@@ -59,34 +62,31 @@
     def init_epd(self):
         """Initialize the ePaper display module."""
         self._log.info("Init ePaper display.")
         self.epd.init()
         self.epd.Clear()
 
     @staticmethod
-    def fig_to_image(fig: plt.Figure) -> Image.Image:
+    def fig_to_image(fig: Figure) -> Image.Image:
         """Convert a `plt.Figure` to `PIL.Image.Image`.
 
         Args:
             fig: The `plt.Figure` to convert.
 
         Returns:
             The `PIL.Image.Image` representation of the provided `plt.Figure`.
         """
-        matplotlib.use("Agg")
+        mpl.use("Agg")
         fig.canvas.draw()
-        return Image.frombytes(
-            "RGB",
-            fig.canvas.get_width_height(),
-            fig.canvas.tostring_rgb(),
-        )
+        return Image.fromarray(
+            np.asarray(fig.canvas.buffer_rgba()),  # type: ignore
+            mode="RGBA",
+        ).convert("RGB")
 
-    def _create_fig_ax(
-        self, n_axes: int = 1, **kwargs
-    ) -> Tuple[plt.Figure, np.ndarray]:
+    def _create_fig_ax(self, n_axes: int = 1, **kwargs) -> Tuple[Figure, np.ndarray]:
         """Create the `plt.Figure` and `plt.Axes` used to plot the chart.
 
         Args:
             n_axes: the number of subplot axes to create.
             **kwargs: passed to `plt.subplots`.
 
         Returns:
@@ -104,25 +104,23 @@
             **kwargs,
         )
         if not isinstance(axes, np.ndarray):
             axes = np.array([axes])
         fig.subplots_adjust(top=1, bottom=0, right=1, left=0, hspace=0, wspace=0)
         for ax in axes:
             self._strip_ax(ax)
-        return fig, axes
+        return fig, axes  # type: ignore
 
-    def _strip_ax(self, ax: plt.Axes) -> None:
+    def _strip_ax(self, ax: Axes) -> None:
         """Strip all visuals from `plt.Axes` object."""
         ax.axis(False)
         ax.margins(0, 0)
         ax.grid(False)
 
-    def text(
-        self, text: str, show: bool = False, **kwargs
-    ) -> Tuple[plt.Figure, plt.Axes]:
+    def text(self, text: str, show: bool = False, **kwargs) -> Tuple[Figure, Axes]:
         """Create a `plt.Figure` and `plt.Axes` with centered text.
 
         Args:
             text: Text on the plot.
             show: Display the figure on the display.
             **kwargs: Passed to `ax.text`.
 
@@ -132,15 +130,15 @@
         fig, ax = self._create_fig_ax(n_axes=1)
         ax = ax[0]
         ax.text(0, 0, text, ha="center", va="center", wrap=True, **kwargs)
         if show:
             self.show_fig(fig)
         return fig, ax
 
-    def show_fig(self, fig: plt.Figure) -> None:
+    def show_fig(self, fig: Figure) -> None:
         """Show a `plt.Figure` on the display."""
         image = self.fig_to_image(fig)
         self.show_image(image)
 
     def _show_image(
         self, image: Image.Image, highlight: Optional[Image.Image] = None
     ) -> None:
@@ -167,22 +165,22 @@
             colored_pixels = ~(image_ar == image_ar[:, :, 0][:, :, None]).all(axis=-1)
             highlight_image = np.ones(image_ar.shape[:-1], dtype=image_ar.dtype) * 255
             self._log.debug("Number of coloured pixels: %s", colored_pixels.sum())
             highlight_image[colored_pixels] = 0
             # I think there is a bug with PIL, need to convert from "L"
             # https://stackoverflow.com/questions/32159076/python-pil-bitmap-png-from-array-with-mode-1
             highlight_image = Image.fromarray(highlight_image, mode="L").convert(
-                "1", dither=Image.NONE
+                "1", dither=Image.Dither.NONE
             )
             if self.flip:
                 highlight_image = highlight_image.rotate(180)
             self._log.debug("Highlight image size: %s", highlight_image.size)
 
         if image.mode != "1":
-            image = image.convert("1", dither=Image.NONE)
+            image = image.convert("1", dither=Image.Dither.NONE)
         if self.flip:
             image = image.rotate(180)
         self._log.debug("Image size: %s", image.size)
         self._log.info("Wake up.")
         # I think this wakes it from sleep
         self.epd.init()
         self._show_image(image, highlight_image)
@@ -196,15 +194,15 @@
         delta: Optional[float] = None,
         top_string: Optional[str] = None,
         sub_string: Optional[str] = None,
         show: bool = False,
         type: str = "candle",
         volume: bool = False,
         **kwargs,
-    ) -> Tuple[plt.Figure, plt.Axes]:
+    ) -> Tuple[Figure, Axes]:
         """Plot symbol historical data chart.
 
         Args:
             historical: API response, `pd.DataFrame` containing the historical
                 price of the symbol.
             current_price: API response, the current price of the symbol.
             delta: relative percentage change.
@@ -223,15 +221,15 @@
             fig, axes = self._create_fig_ax(
                 n_axes=2, gridspec_kw={"height_ratios": [3, 1]}
             )
             volume_ax = axes[1]
         else:
             fig, axes = self._create_fig_ax(n_axes=1)
             volume_ax = False
-        ax: plt.Axes = axes[0]
+        ax: Axes = axes[0]
         # remove Nones, it doesn't play well with mplfinance
         kwargs = {key: value for key, value in kwargs.items() if value is not None}
         mpf.plot(
             historical,
             type=type,
             ax=ax,
             update_width_config={"line_width": 1},
```

### Comparing `tinyticker-0.4.9/tinyticker/ticker.py` & `tinyticker-0.5.0/tinyticker/ticker.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/utils.py` & `tinyticker-0.5.0/tinyticker/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,26 +76,25 @@
     this_version = Version(current_version)
     return pypy_version > this_version
 
 
 def now() -> pd.Timestamp:
     """Return the current timestamp."""
     return pd.to_datetime("now", utc=True)
-    # return datetime.now(timezone.utc)
 
 
 def set_verbosity(logger: logging.Logger, verbosity: int) -> logging.Logger:
     """Set the logger's verbosity.
 
     Args:
         logger: `logging.Logger`.
         verbosity: verbosity level, 1, or 2.
 
     Return:
-        The `logger` object with configured verbosity.
+        The `logging.Logger` object with configured verbosity.
     """
     verbose_map = {1: logging.INFO, 2: logging.DEBUG}
     level = verbose_map[verbosity]
     # from https://docs.python.org/3/howto/logging.html#configuring-logging
     logger.setLevel(level)
     # create console handler and set level to debug
     handler = logging.StreamHandler()
```

### Comparing `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 
 import logging
 
-from ._base import EPDBase
+from ._base import EPDMonochrome
 from .epdconfig import CONFIG
 
 # Display resolution
 EPD_WIDTH = 122
 EPD_HEIGHT = 250
 
 logger = logging.getLogger(__name__)
 
 
-class EPD(EPDBase):
+class EPD(EPDMonochrome):
     def __init__(self):
         self.reset_pin = CONFIG.RST_PIN
         self.dc_pin = CONFIG.DC_PIN
         self.busy_pin = CONFIG.BUSY_PIN
         self.cs_pin = CONFIG.CS_PIN
         self.width = EPD_WIDTH
         self.height = EPD_HEIGHT
@@ -234,15 +234,15 @@
             for y in range(imheight):
                 for x in range(imwidth):
                     newx = y
                     newy = self.height - x - 1
                     if image_monocolor.getpixel((x, y)) == 0:
                         # newy = imwidth - newy - 1
                         buf[int(newx / 8) + newy * linewidth] &= ~(0x80 >> (y % 8))
-        return buf
+        return bytearray(buf)
 
     def display(self, image):
         if self.width % 8 == 0:
             linewidth = int(self.width / 8)
         else:
             linewidth = int(self.width / 8) + 1
```

### Comparing `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 
 import logging
 
-from ._base import EPDPartial
+from ._base import EPDMonochrome
 from .epdconfig import CONFIG
 
 # Display resolution
 EPD_WIDTH = 122
 EPD_HEIGHT = 250
 
 logger = logging.getLogger(__name__)
 
 
-class EPD(EPDPartial):
+class EPD(EPDMonochrome):
     def __init__(self):
         self.reset_pin = CONFIG.RST_PIN
         self.dc_pin = CONFIG.DC_PIN
         self.busy_pin = CONFIG.BUSY_PIN
         self.cs_pin = CONFIG.CS_PIN
         self.width = EPD_WIDTH
         self.height = EPD_HEIGHT
@@ -366,15 +366,15 @@
             for y in range(imheight):
                 for x in range(imwidth):
                     newx = y
                     newy = self.height - x - 1
                     if image_monocolor.getpixel((x, y)) == 0:
                         newy = imwidth - newy - 1
                         buf[int(newx / 8) + newy * linewidth] &= ~(0x80 >> (y % 8))
-        return buf
+        return bytearray(buf)
 
     def display(self, image):
         self.send_command(0x24)
         self.send_data2(image)
         self.TurnOnDisplay()
 
     def displayPartial(self, image):
```

### Comparing `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 
 import logging
 
-from ._base import EPDPartial
+from ._base import EPDMonochrome
 from .epdconfig import CONFIG
 
 # Display resolution
 EPD_WIDTH = 122
 EPD_HEIGHT = 250
 
 logger = logging.getLogger(__name__)
 
 
-class EPD(EPDPartial):
+class EPD(EPDMonochrome):
     def __init__(self):
         self.reset_pin = CONFIG.RST_PIN
         self.dc_pin = CONFIG.DC_PIN
         self.busy_pin = CONFIG.BUSY_PIN
         self.cs_pin = CONFIG.CS_PIN
         self.width = EPD_WIDTH
         self.height = EPD_HEIGHT
@@ -577,15 +577,15 @@
             logger.warning(
                 "Wrong image dimensions: must be "
                 + str(self.width)
                 + "x"
                 + str(self.height)
             )
             # return a blank buffer
-            return [0x00] * (int(self.width / 8) * self.height)
+            return bytearray([0x00] * (int(self.width / 8) * self.height))
 
         buf = bytearray(img.tobytes("raw"))
         return buf
 
     """
     function : Sends the image buffer in RAM to e-Paper and displays
     parameter:
```

### Comparing `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 
 import logging
 
-from ._base import EPDPartial
+from ._base import EPDMonochrome
 from .epdconfig import CONFIG
 
 # Display resolution
 EPD_WIDTH = 122
 EPD_HEIGHT = 250
 
 logger = logging.getLogger(__name__)
 
 
-class EPD(EPDPartial):
+class EPD(EPDMonochrome):
     def __init__(self):
         self.reset_pin = CONFIG.RST_PIN
         self.dc_pin = CONFIG.DC_PIN
         self.busy_pin = CONFIG.BUSY_PIN
         self.cs_pin = CONFIG.CS_PIN
         self.width = EPD_WIDTH
         self.height = EPD_HEIGHT
@@ -271,15 +271,15 @@
             logger.warning(
                 "Wrong image dimensions: must be "
                 + str(self.width)
                 + "x"
                 + str(self.height)
             )
             # return a blank buffer
-            return [0x00] * (int(self.width / 8) * self.height)
+            return bytearray([0x00] * (int(self.width / 8) * self.height))
 
         buf = bytearray(img.tobytes("raw"))
         return buf
 
     """
     function : Sends the image buffer in RAM to e-Paper and displays
     parameter:
```

### Comparing `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             logger.debug("Horizontal")
             for y in range(imheight):
                 for x in range(imwidth):
                     newx = y
                     newy = self.height - x - 1
                     if image_monocolor.getpixel((x, y)) == 0:
                         buf[int((newx + newy * self.width) / 8)] &= ~(0x80 >> (y % 8))
-        return buf
+        return bytearray(buf)
 
     def display(self, imageblack, highlights=None):
         self.send_command(0x10)
         for i in range(0, int(self.width * self.height / 8)):
             self.send_data(imageblack[i])
 
         if highlights is not None:
```

### Comparing `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             logger.warning(
                 "Wrong image dimensions: must be "
                 + str(self.width)
                 + "x"
                 + str(self.height)
             )
             # return a blank buffer
-            return [0x00] * (int(self.width / 8) * self.height)
+            return bytearray([0x00] * (int(self.width / 8) * self.height))
 
         buf = bytearray(img.tobytes("raw"))
         return buf
 
     # display image
     def display(self, imageblack, highlights=None):
         self.send_command(0x24)
```

### Comparing `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             logger.debug("Horizontal")
             for y in range(imheight):
                 for x in range(imwidth):
                     newx = y
                     newy = self.height - x - 1
                     if image_monocolor.getpixel((x, y)) == 0:
                         buf[int((newx + newy * self.width) / 8)] &= ~(0x80 >> (y % 8))
-        return buf
+        return bytearray(buf)
 
     def display(self, imageblack, highlights=None):
         self.send_command(0x10)
         for i in range(0, int(self.width * self.height / 8)):
             self.send_data(imageblack[i])
         # self.send_command(0x92)
```

### Comparing `tinyticker-0.4.9/tinyticker/waveshare_lib/epdconfig.py` & `tinyticker-0.5.0/tinyticker/waveshare_lib/epdconfig.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/waveshare_lib/models.py` & `tinyticker-0.5.0/tinyticker/waveshare_lib/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from dataclasses import dataclass
 from typing import Type, Union
 
-from . import (epd2in13, epd2in13_V2, epd2in13_V3, epd2in13_V4, epd2in13b_V3,
-               epd2in13b_V4, epd2in13bc)
-from ._base import EPDBase, EPDHighlight, EPDPartial
+from . import (
+    epd2in13,
+    epd2in13_V2,
+    epd2in13_V3,
+    epd2in13_V4,
+    epd2in13b_V3,
+    epd2in13b_V4,
+    epd2in13bc,
+)
+from ._base import EPDMonochrome, EPDHighlight
 
 
 @dataclass
 class EPDModel:
     name: str
-    class_: Union[Type[EPDBase], Type[EPDHighlight], Type[EPDPartial]]
+    class_: Union[Type[EPDMonochrome], Type[EPDHighlight]]
     desc: str
 
 
 MODELS = [
     EPDModel(
         name="EPD",
         class_=epd2in13.EPD,
```

### Comparing `tinyticker-0.4.9/tinyticker/web/__main__.py` & `tinyticker-0.5.0/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/web/app.py` & `tinyticker-0.5.0/tinyticker/web/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from .. import __version__
 from ..config import PLOT_TYPES, SequenceConfig, TickerConfig, TinytickerConfig
 from ..paths import CONFIG_FILE, LOG_DIR
 from ..ticker import INTERVAL_LOOKBACKS, INTERVAL_TIMEDELTAS, SYMBOL_TYPES
 from ..utils import check_for_update
 from ..waveshare_lib.models import MODELS
-from .command import COMMANDS, reboot, refresh
+from .command import COMMANDS, reboot
 
 LOGGER = logging.getLogger(__name__)
 TEMPLATE_PATH = str(Path(__file__).parent / "templates")
 INTERVAL_WAIT_TIMES = {k: v.value * 1e-9 for k, v in INTERVAL_TIMEDELTAS.items()}
 
 
 def no_empty_str(data: str) -> Optional[str]:
@@ -107,15 +107,15 @@
         tickers["lookback"] = request.args.getlist("lookback", type=no_empty_int)
         tickers["wait_time"] = request.args.getlist("wait_time", type=no_empty_int)
         tickers["mav"] = request.args.getlist("mav", type=no_empty_int)
         tickers["volume"] = request.args.getlist("volume", type=str_to_bool)
 
         sequence = SequenceConfig(
             skip_outdated=request.args.get("skip_outdated", False, type=bool),
-            # Note: currently not toggleable from the web app
+            # NOTE: currently not toggleable from the web app
             skip_empty=request.args.get("skip_empty", True, type=bool),
         )
 
         # invert the ticker dict of list to list of dict and create ticker list
         tickers = [
             TickerConfig(**dict(zip(tickers, t))) for t in zip(*tickers.values())
         ]
@@ -123,16 +123,17 @@
             api_key=request.args.get("api_key", type=no_empty_str),
             flip=request.args.get("flip", default=False, type=bool),
             epd_model=request.args.get("epd_model", "EPD_v3"),
             tickers=tickers,
             sequence=sequence,
         )
         LOGGER.debug(tt_config)
+        # writing the config to file, the main ticker process is monitoring this file
+        # and will refresh the ticker process
         tt_config.to_file(config_file)
-        refresh()
         return redirect("/", code=302)
 
     @app.route("/command")
     def command():
         LOGGER.debug("/command url args: %s", request.args)
         command = request.args.get("command")
         if command:
```

### Comparing `tinyticker-0.4.9/tinyticker/web/command.py` & `tinyticker-0.5.0/tinyticker/web/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,21 @@
     try_command("sudo comitup-cli d")
     reboot()
 
 
 @register
 def update() -> None:
     """Update tinyticker with pip."""
-    pipmain(["install", "--upgrade", "tinyticker"])
+    args = ["install", "--upgrade", "tinyticker"]
+    # rpi requires an added flag to update system packages
+    # https://www.raspberrypi.com/documentation/computers/os.html#about-python-virtual-environments
+    error = pipmain(args + ["--break-system-packages"])
+    if error:
+        # if for some reason we are not running on an rpi, try again without the flag
+        error = pipmain(args)
 
 
 @register
 def default() -> None:
     """Write the default config."""
     LOGGER.info("Setting config to default.")
     TinytickerConfig().to_file(CONFIG_FILE)
```

### Comparing `tinyticker-0.4.9/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.5.0/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.5.0/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.5.0/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.5.0/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/web/templates/js/index.js` & `tinyticker-0.5.0/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.5.0/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.5.0/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.9/tinyticker/web/templates/logfiles.html` & `tinyticker-0.5.0/tinyticker/web/templates/logfiles.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,30 @@
-<!DOCTYPE html>
+<!doctype html>
 <html lang="en" class="uk-height-1-1">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <title>TinyTicker - Log Files</title>
-    <link rel="apple-touch-icon" sizes="180x180" href="img/apple-touch-icon.png">
-    <link rel="icon" type="image/png" sizes="32x32" href="img/favicon-32x32.png">
-    <link rel="icon" type="image/png" sizes="16x16" href="img/favicon-16x16.png">
+    <link
+      rel="apple-touch-icon"
+      sizes="180x180"
+      href="img/apple-touch-icon.png"
+    />
+    <link
+      rel="icon"
+      type="image/png"
+      sizes="32x32"
+      href="img/favicon-32x32.png"
+    />
+    <link
+      rel="icon"
+      type="image/png"
+      sizes="16x16"
+      href="img/favicon-16x16.png"
+    />
     <!-- CSS FILES -->
     <link rel="stylesheet" type="text/css" href="css/uikit.min.css" />
     <!-- JS FILES -->
     <script src="js/uikit.min.js"></script>
     <script src="js/uikit-icons.min.js"></script>
   </head>
   <body class="uk-background-muted uk-height-1-1 uk-padding-small">
@@ -18,16 +32,16 @@
       <div class="uk-width-large">
         <div class="uk-width-1-1 uk-text-center">
           <p class="uk-text-large">🚀 TinyTicker Log Files 🚀</p>
         </div>
         <p class="uk-text-large">Log files:</p>
         <ul class="uk-list uk-list-square">
           {% for log_file in log_files %}
-          <li>
-            <a href="/get-log/{{log_file}}">{{log_file}}</a>
-          </li>
+            <li>
+              <a href="/get-log/{{ log_file }}">{{ log_file }}</a>
+            </li>
           {% endfor %}
         </ul>
       </div>
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 🚀 TinyTicker Log Files 🚀
 Log files:
     * {% for log_file in log_files %}
-    * _{_{_l_o_g___f_i_l_e_}_}
+    * _{_{_ _l_o_g___f_i_l_e_ _}_}
     * {% endfor %}
```

### Comparing `tinyticker-0.4.9/PKG-INFO` & `tinyticker-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.4.9
+Version: 0.5.0
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Flask (>=2.0.2,<3.0.0)
 Requires-Dist: Pillow (>=10.0.1,<11.0.0)
 Requires-Dist: RPi.GPIO (>=0.7.0,<0.8.0)
 Requires-Dist: cryptocompare (>=0.7.5,<0.8.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: mplfinance (>=0.12.7-alpha.17,<0.13.0)
+Requires-Dist: numpy (>=1.26,<2.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: qrcode (>=7.3.1,<8.0.0)
 Requires-Dist: spidev (>=3.5,<4.0)
+Requires-Dist: watchdog (>=4.0.0,<5.0.0)
 Requires-Dist: yfinance (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/loiccoyle/tinyticker
 Description-Content-Type: text/markdown
 
 <h1 align="center">🚀 tinyticker 🚀</h1>
 <div align="center">
   <img  src="https://i.imgur.com/J4k3PCM.png" height=400>
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.4.9 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.5.0 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
-Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.8,<3.12
+Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Flask (>=2.0.2,<3.0.0) Requires-Dist: Pillow (>=10.0.1,<11.0.0)
 Requires-Dist: RPi.GPIO (>=0.7.0,<0.8.0) Requires-Dist: cryptocompare
 (>=0.7.5,<0.8.0) Requires-Dist: matplotlib (>=3.5.1,<4.0.0) Requires-Dist:
-mplfinance (>=0.12.7-alpha.17,<0.13.0) Requires-Dist: packaging (>=23.0,<24.0)
-Requires-Dist: pandas (>=1.3.5,<2.0.0) Requires-Dist: qrcode (>=7.3.1,<8.0.0)
-Requires-Dist: spidev (>=3.5,<4.0) Requires-Dist: yfinance (>=0.2.0,<0.3.0)
-Project-URL: Repository, https://github.com/loiccoyle/tinyticker Description-
-Content-Type: text/markdown
+mplfinance (>=0.12.7-alpha.17,<0.13.0) Requires-Dist: numpy (>=1.26,<2.0)
+Requires-Dist: packaging (>=23.0,<24.0) Requires-Dist: pandas (>=1.3.5,<2.0.0)
+Requires-Dist: qrcode (>=7.3.1,<8.0.0) Requires-Dist: spidev (>=3.5,<4.0)
+Requires-Dist: watchdog (>=4.0.0,<5.0.0) Requires-Dist: yfinance
+(>=0.2.0,<0.3.0) Project-URL: Repository, https://github.com/loiccoyle/
+tinyticker Description-Content-Type: text/markdown
                       ************ ?ð??? ttiinnyyttiicckkeerr ?ð??? ************
       [https://i.imgur.com/J4k3PCM.png][https://i.imgur.com/QWP7bpH.png]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_i_n_y_t_i_c_k_e_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
     _l_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_o_i_c_c_o_y_l_e_/_t_i_n_y_t_i_c_k_e_r_/_a_c_t_i_o_n_s_/
                           _w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]
 ===============================================================================
 `tinyticker` uses a Raspberry Pi zero W and a small ePaper display to
```

