# Comparing `tmp/TH_camera_calibration-0.4.6.tar.gz` & `tmp/TH_camera_calibration-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TH_camera_calibration-0.4.6.tar", last modified: Thu May  2 17:14:57 2024, max compression
+gzip compressed data, was "TH_camera_calibration-0.4.7.tar", last modified: Sat May  4 11:25:01 2024, max compression
```

## Comparing `TH_camera_calibration-0.4.6.tar` & `TH_camera_calibration-0.4.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 17:14:57.313776 TH_camera_calibration-0.4.6/
--rw-rw-rw-   0        0        0     2729 2024-05-02 17:14:57.312778 TH_camera_calibration-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     5238 2024-04-21 07:06:15.000000 TH_camera_calibration-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 17:14:57.300783 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/
--rw-rw-rw-   0        0        0     2729 2024-05-02 17:14:56.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-02 17:14:57.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 17:14:56.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-05-02 17:14:56.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-02 17:14:56.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 17:14:57.307779 TH_camera_calibration-0.4.6/camera_calibration/
--rw-rw-rw-   0        0        0       51 2024-04-21 06:12:27.000000 TH_camera_calibration-0.4.6/camera_calibration/__init__.py
--rw-rw-rw-   0        0        0    14163 2024-05-02 16:25:32.000000 TH_camera_calibration-0.4.6/camera_calibration/camera_calibration.py
--rw-rw-rw-   0        0        0       42 2024-05-02 17:14:57.314776 TH_camera_calibration-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      481 2024-05-02 16:28:44.000000 TH_camera_calibration-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:25:01.006950 TH_camera_calibration-0.4.7/
+-rw-rw-rw-   0        0        0     4604 2024-05-04 11:25:01.004951 TH_camera_calibration-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2994 2024-05-04 11:20:57.000000 TH_camera_calibration-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 11:25:00.990954 TH_camera_calibration-0.4.7/TH_camera_calibration.egg-info/
+-rw-rw-rw-   0        0        0     4604 2024-05-04 11:25:00.000000 TH_camera_calibration-0.4.7/TH_camera_calibration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-04 11:25:00.000000 TH_camera_calibration-0.4.7/TH_camera_calibration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 11:25:00.000000 TH_camera_calibration-0.4.7/TH_camera_calibration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-04 11:25:00.000000 TH_camera_calibration-0.4.7/TH_camera_calibration.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-04 11:25:00.000000 TH_camera_calibration-0.4.7/TH_camera_calibration.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 11:25:01.000973 TH_camera_calibration-0.4.7/camera_calibration/
+-rw-rw-rw-   0        0        0       51 2024-04-21 06:12:27.000000 TH_camera_calibration-0.4.7/camera_calibration/__init__.py
+-rw-rw-rw-   0        0        0    14593 2024-05-04 11:17:37.000000 TH_camera_calibration-0.4.7/camera_calibration/camera_calibration.py
+-rw-rw-rw-   0        0        0       42 2024-05-04 11:25:01.006950 TH_camera_calibration-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      484 2024-05-04 11:24:57.000000 TH_camera_calibration-0.4.7/setup.py
```

### Comparing `TH_camera_calibration-0.4.6/PKG-INFO` & `TH_camera_calibration-0.4.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-Metadata-Version: 2.1
-Name: TH_camera_calibration
-Version: 0.4.6
-Description-Content-Type: text/markdown
-
-# Calibration_camera
+﻿# Camera Calibration
 
 Created on Sunday, April 21, 2024  
 Author: Tung Nguyen - Handsome  
 Reference: Camera Calibration by OpenCV ([OpenCV Tutorial](https://docs.opencv.org/4.x/dc/dbb/tutorial_py_calibration.html))
 
+![Banner Tung Handsome Camera Calibration](https://github.com/nguyenquangtung/Camera_Calibration/assets/59195029/023dd5de-9801-44c7-a990-176921246aa8)
+
 ## Overview
 
-This Python script provides a class, `CameraCalibration`, to perform camera calibration based on a set of image points and their corresponding object points.
+This Python script provides a class, `CameraCalibration`, to perform camera calibration based on a set of image points and their corresponding object points / undistort image or frame from camera
 
 ## Description
 
 This script includes functionalities to:
 
 - Calculate camera calibration data based on a set of images.
 - Save and load the camera calibration data.
 - Undistort images or points using the calibration data.
 
 ## Usage
 
-Using this command for install package (or clone this repository):
+Using this command to install the packages (or clone this repository):
 
 ```
 pip install TH-camera-calibration
 ```
 
 ### Requirements
 
@@ -59,23 +56,27 @@
 
    ```python
    camera_calibrator.calculate_calibration_data(
        run=True,
        chessboardSize=(9, 6),
        size_of_chessboard_squares_mm=25,
        framesize=(1280, 720),
-       calibrationDir=None,
-       savepath=None,
+       calibrationDir=None, #path of calibration dir
+       savepath="",
        saveformat="pkl",
        show_process_img=True,
        show_calibration_data=True,
    )
    ```
 
-4. Undistort an image.
+4. Read calibration data. (run when have calib data already and do not want to calculate calib data from scratch)
+   ```python
+   calibrator.read_calibration_data(r"calibration.pkl", "pkl", True)
+   ```
+5. Undistort an image. (If not calculate calib data from scratch, require to read calib data first)
 
    ```python
    undistorted_image = camera_calibrator.undistortion_img(
        img,
        method="default",
        img_size=(1280, 720),
        verbose=False
@@ -89,21 +90,15 @@
        img,
        method="Remapping",
        img_size=(1280, 720),
        verbose=False
    )
    ```
 
-5. Undistort a set of image points.
-
-   ```python
-   undistorted_points = camera_calibrator.undistortion_points(points, verbose=False)
-   ```
-
 ## Results
 
-## Additional Information
+## 💚🖤 Join me on Social Media 🖤💚
 
-- My email: quangtung.work73@gmail.com
+- My Gmail: quangtung.work73@gmail.com
 - My Github: [Tung Nguyen - Handsome - Github](https://github.com/nguyenquangtung)
 - My Youtube channel: [Tung Nguyen - Handsome - Youtube](https://www.youtube.com/@tungquangnguyen731)
-- My linkedin: [Tung Nguyen - Handsome - Linkedin](https://www.linkedin.com/in/tungnguyen73/)
+- My Linkedin: [Tung Nguyen - Handsome - Linkedin](https://www.linkedin.com/in/tungnguyen73/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TH_camera_calibration-0.4.6/camera_calibration/camera_calibration.py` & `TH_camera_calibration-0.4.7/camera_calibration/camera_calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 import numpy as np
 import cv2 as cv
 import glob
 import pickle
 import os
+import time
 
 
 class CameraCalibration:
     """
     A class to perform camera calibration based on a set of image points and their corresponding object points.
     """
 
@@ -73,14 +74,21 @@
             all_images = []
             image_formats = ["*.jpg", "*.png"]
             if not os.path.exists(calibrationDir):
                 raise FileNotFoundError("CalibrationDir path does not exit!")
             for image_format in image_formats:
                 images = glob.glob(os.path.join(calibrationDir, image_format))
                 all_images.extend(images)
+
+            print("Processing image and find chessboard corners ", end="", flush=True)
+            for _ in range(5):
+                print(".", end="", flush=True)
+                time.sleep(0.25)
+            print()
+
             for image in all_images:
 
                 img = cv.imread(image)
                 gray = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
 
                 # Find the chess board corners
                 cornersFound, cornersOrg = cv.findChessboardCorners(
@@ -105,14 +113,19 @@
                         cv.waitKey(1000)
             cv.destroyAllWindows()
             if not valid_data_flag:
                 raise Exception(
                     "All data is not valid, needs to be clearer to be able to identify the chessboard corners!"
                 )
             # CALIBRATION
+            print("Calculating ", end="", flush=True)
+            for _ in range(5):
+                print(".", end="", flush=True)
+                time.sleep(0.25)
+            print()
             repError, cameraMatrix, distCoeff, rvecs, tvecs = cv.calibrateCamera(
                 objpoints, imgpoints, framesize, None, None
             )
             if show_calibration_data:
                 print("Camera Matrix: ", cameraMatrix)
                 print("\nDistortion Coefficent: ", distCoeff)
             self.cameraMatrix = cameraMatrix
@@ -304,21 +317,21 @@
 
 
 if __name__ == "__main__":
 
     calibrator = CameraCalibration()
     calibrator.calculate_calibration_data(
         run=True,
-        chessboardSize=(9, 6),
-        size_of_chessboard_squares_mm=25,
+        chessboardSize=(7, 4),
+        size_of_chessboard_squares_mm=100,
         framesize=(1280, 720),
         calibrationDir=r"image\calibration_dir",
         savepath="",
         saveformat="npz",
-        show_process_img=False,
+        show_process_img=True,
         show_calibration_data=True,
     )
     calibrator.read_calibration_data(r"calibration.npz", "npz", True)
 
     ################ Test undistortion img ###########################
     # img = cv.imread(r"image\results\frame_36.jpg")
     # distortion_img = calibrator.remove_distortion(img, verbose=True)
```

