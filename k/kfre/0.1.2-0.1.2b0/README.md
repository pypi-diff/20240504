# Comparing `tmp/kfre-0.1.2.tar.gz` & `tmp/kfre-0.1.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kfre-0.1.2.tar", last modified: Sun Apr 28 01:16:20 2024, max compression
+gzip compressed data, was "kfre-0.1.2b0.tar", last modified: Sat May  4 06:22:36 2024, max compression
```

## Comparing `kfre-0.1.2.tar` & `kfre-0.1.2b0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 01:16:20.129324 kfre-0.1.2/
--rw-rw-rw-   0        0        0    28206 2024-04-28 01:16:20.128262 kfre-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    24261 2024-04-28 01:16:09.000000 kfre-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 01:16:20.129324 kfre-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1286 2024-04-28 01:08:27.000000 kfre-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 01:16:20.088129 kfre-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-28 01:16:20.090130 kfre-0.1.2/src/kfre/
--rw-rw-rw-   0        0        0     1872 2024-04-28 00:46:44.000000 kfre-0.1.2/src/kfre/__init__.py
--rw-rw-rw-   0        0        0    26880 2024-04-28 00:46:36.000000 kfre-0.1.2/src/kfre/main.py
-drwxrwxrwx   0        0        0        0 2024-04-28 01:16:20.127135 kfre-0.1.2/src/kfre.egg-info/
--rw-rw-rw-   0        0        0    28206 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:22:36.505899 kfre-0.1.2b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 06:22:28.000000 kfre-0.1.2b0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-04 06:22:36.505899 kfre-0.1.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-05-04 06:22:28.000000 kfre-0.1.2b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:22:36.505899 kfre-0.1.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-04 06:22:28.000000 kfre-0.1.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:22:36.501899 kfre-0.1.2b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:22:36.501899 kfre-0.1.2b0/src/kfre/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-04 06:22:28.000000 kfre-0.1.2b0/src/kfre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-04 06:22:28.000000 kfre-0.1.2b0/src/kfre/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:22:36.505899 kfre-0.1.2b0/src/kfre.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-04 06:22:36.000000 kfre-0.1.2b0/src/kfre.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 06:22:36.000000 kfre-0.1.2b0/src/kfre.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:22:36.000000 kfre-0.1.2b0/src/kfre.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 06:22:36.000000 kfre-0.1.2b0/src/kfre.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 06:22:36.000000 kfre-0.1.2b0/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.2/PKG-INFO` & `kfre-0.1.2b0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,433 +1,414 @@
-Metadata-Version: 2.1
-Name: kfre
-Version: 0.1.2
-Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
-Home-page: UNKNOWN
-Author: Leonid Shpaner
-Author-email: Lshpaner@ucla.edu
-License: UNKNOWN
-Project-URL: Author Website, https://www.leonshpaner.com
-Project-URL: Source Code, https://github.com/lshpaner/kfre
-Description: # KFRE: Kidney Failure Risk Estimator
-        
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/lshpaner/kfre/main/LICENSE.md)
-        ![PyPI](https://img.shields.io/pypi/v/kfre.svg)
-        [![PyPI](https://img.shields.io/badge/PyPi-Page-blue)](https://pypi.org/project/kfre/)
-        [![Downloads](https://pepy.tech/badge/kfre)](https://pepy.tech/project/kfre)
-        
-        `kfre` is a Python library designed to estimate the risk of chronic kidney disease (CKD) progression over two distinct timelines: 2 years and 5 years. Using Tangri's Kidney Failure Risk Equation (KFRE), the library provides tools for healthcare professionals and researchers to predict CKD risk based on patient data. It supports predictions for both males and females and includes specific adjustments for individuals from North American and non-North American regions.
-        
-        --------
-        ## Table of Contents
-        
-        1. [Features](#Features)
-        2. [Prerequisites](#Prerequisites)
-        3. [Installation](#installation)
-        4. [Usage Guide](#usage-guide)
-           - [Single Patient Risk Calculation](#single-patient-risk-calculation)
-           - [Batch Risk Calculation for Multiple Patients](#batch-risk-calculation-for-multiple-patients)
-           - [Conversion of Clinical Parameters](#conversion-of-clinical-parameters)
-                - [uPCR to uACR](#upcr-to-uacr)
-                - [Calcium](#calcium)
-                - [Phosphate](#phosphate)
-                - [Albumin](#albumin)
-        5. [Contributor/Maintainer](#contributormaintainer)
-        6. [License](#license)
-        7. [Support](#acknowledgements)
-        8. [References](#references)
-        --------
-        
-        
-        ## Features
-        
-        - **Risk Prediction**: Utilize Tangri's validated risk prediction model to estimate kidney failure risk using
-            - 4 variables: sex, age, eGFR, uACR (log-normalized)
-            - 6 variables: sex, age, eGFR, uACR (log-normalized), diabetes mellitus, hypertension
-            - 8 variables: sex, age, eGFR, uACR (log-normalized), serum albumin, serum phosphorous, serum calcium, and serum bicarbonate.
-        - **Data Flexibility**: Handles various input data formats and maps them to required model parameters.
-        - **Conversion Utilities**: Includes functions to convert common laboratory results to the required units for risk prediction.
-        
-        ### Important Note on Data Units
-        The kfre library requires precise data input, with clear specification of the units for each variable. The variables can be expressed in multiple units, and it's crucial that the data being used clearly delineates which units the variables are expressed in. For instance:
-        
-        - uACR (Urinary Albumin-Creatinine Ratio) can be expressed in either mg/g or mg/mmol.
-        - Albumin levels can be measured in g/dL or g/L.
-        - Phosphorous levels can be noted in mg/dL or mmol/L.
-        - Bicarbonate can be recorded in mEq/L or mmol/L.
-        - Calcium can be documented in mg/dL or mmol/L.
-        
-        This flexibility allows the library to be used with a variety of clinical data sources, enhancing its applicability across different healthcare settings.
-        
-        ## Prerequisites
-        Before you install `kfre`, ensure you have the following:
-        
-        - **Python**: Python 3.6 or higher is required to run `kfre`.
-        
-        Additionally, kfre has the following package dependencies:
-        
-        - **NumPy**: Version 1.18.5 or higher
-        - **Pandas**: Version 1.0.5 or higher
-        
-        These dependencies will be automatically installed when you install kfre using pip.
-        
-        ## Installation
-        
-        You can install `kfre` directly from PyPI:
-        
-        ```bash
-        pip install kfre
-        ```
-        
-        ## Usage Guide
-        
-        ## Single Patient Risk Calculation
-        The kfre library offers a flexible and user-friendly interface to estimate the risk of kidney failure for individual patients using Tangri's KFRE model. With `kfre`, you can calculate the risk using the classic 4-variable model, the detailed 8-variable model, and, uniquely, a 6-variable model that is not commonly found in online calculators.
-        
-        ## `kfre_person`
-        
-        ```python
-        risk_percentage = kfre_person(
-            age=57.28,
-            is_male=False,
-            eGFR=15.0,
-            uACR=1762.001840,
-            is_north_american=False,
-            years=2,
-            dm=None,
-            htn=None,
-            albumin=None,
-            phosphorous=None,
-            bicarbonate=None,
-            calcium=None
-        ) * 100  # Convert to percentage
-        
-        ```
-        
-        Parameters: 
-        
-        - `age` (float): The age of the patient in years.
-        - `is_male` (bool): Indicates if the patient is male. False indicates a female patient.
-        - `eGFR` (float): Estimated Glomerular Filtration Rate in mL/min/1.73 mÂ², indicating kidney function.
-        - `uACR` (float): Urinary Albumin to Creatinine Ratio in mg/g, indicating kidney damage.
-        - `is_north_american` (bool): Specifies whether the patient is from North America, affecting model constants.
-        - `years` (int): The time frame in years (2 or 5) over which the risk assessment is projected.
-        - `dm` (float, optional): Diabetes mellitus status (1 if present, 0 if not). Required for the 6-variable model.
-        - `htn` (float, optional): Hypertension status (1 if present, 0 if not). Required for the 6-variable model.
-        - `albumin` (float, optional): Serum albumin level in g/dL. Required for the 8-variable model.
-        - `phosphorous` (float, optional): Serum phosphorus level in mg/dL. Required for the 8-variable model.
-        - `bicarbonate` (float, optional): Serum bicarbonate level in mEq/L. Required for the 8-variable model.
-        - `calcium` (float, optional): Serum calcium level in mg/dL. Required for the 8-variable model.
-        
-        Returns:
-        
-        `float`: The risk of developing CKD within the specified timeframe, as a decimal. Multiply by 100 to convert to a percentage.
-        
-        Description:
-        
-        The `kfre_person` function allows for detailed, personalized risk assessments based on a range of clinical parameters. Depending on the completeness of the data provided, the function can apply a basic 4-variable model or more comprehensive models incorporating additional risk factors like diabetes, hypertension, and various biochemical markers.
-        
-        The function is designed for ease of use in clinical settings or research, providing immediate risk estimations that are crucial for patient management or further analysis.
-        
-        ### Example Calculation for 2-year and 5-year Risk
-        Here's how to estimate the 2-year and 5-year kidney failure risk for a hypothetical 57.28-year-old female who is not from North America and has specific clinical characteristics:
-        
-        ```python
-        from kfre import kfre_person
-        
-        for years in [2, 5]:
-            risk_percentage = (
-                kfre_person(
-                    age=57.28,
-                    is_male=False,  # is the patient male?
-                    eGFR=15.0,  # ml/min/1.73 m^2
-                    uACR=1762.001840,  # mg/g
-                    is_north_american=False,  # is the patient from North America?
-                    years=years,
-                    ####################################################################
-                    # Uncomment "dm" and "htn" for the 6-variable model:
-                    ####################################################################
-                    # dm=0,
-                    # htn=1,
-                    ####################################################################
-                    # Comment out "dm" and "htn" and uncomment the following lines for
-                    # the 8-variable model:
-                    ####################################################################
-                    # albumin=3.0, # g/dL
-                    # phosphorous=3.162, # mg/dL
-                    # bicarbonate=21.3, # mEq/L
-                    # calcium=9.72, # mg/dL
-                )
-                * 100  # multiply by 100 to convert to percentage
-            )
-        
-            message = f"The {years}-year risk of kidney failure for this patient is"
-            print(f"{message} {risk_percentage:.2f}%.")
-        ```
-        ```
-        The 2-year risk of kidney failure for this patient is 44.66%.
-        The 5-year risk of kidney failure for this patient is 89.89%.
-        ```
-        
-        Ensure to:
-        - Uncomment `dm` and `htn` if you are using the 6-variable KFRE model.
-        - For the 8-variable KFRE, keep `dm` and `htn` commented out and instead, uncomment the `albumin`, `phosphorous`, `bicarbonate`, and `calcium` variables.
-        
-        
-        ## Batch Risk Calculation for Multiple Patients
-        The kfre library provides the functionality to perform batch processing of patient data, allowing for the computation of kidney failure risk predictions across multiple patients in a single operation. This capability is especially valuable for researchers and clinicians needing to assess risks for large cohorts or patient groups.
-        
-        **Key Features**
-        
-        When using the `add_kfre_risk_col` function, the library will append new columns for each specified variable model (4-variable, 6-variable, 8-variable) and each time frame (2 years, 5 years) directly to the original DataFrame. This facilitates a seamless integration of risk predictions into existing patient datasets without the need for additional data manipulation steps.
-        
-        ***Disclaimer***
-        
-        The `kfre` library is designed to facilitate risk prediction using Tangri's KFRE model based on a given set of patient data. It is crucial to ensure that all patient data within a batch calculation are consistent in terms of regional categorizationâ€”that is, either all North American or all non-North American. To this end, it is crucial to ensure that all patient data within a batch calculation are consistent in terms of regional categorization. Mixing patient data from different regions within a single batch is not supported, as the function is set to apply one regional coefficient set at a time. This approach ensures the accuracy and reliability of the risk predictions.
-        
-        Example Usage:
-        
-        Here is how to perform batch risk calculations for a group of non-North American patients. Note the importance of maintaining consistency in regional data:
-        
-        ***Note***: The following is a mock example using simulated DataFrame structures to illustrate the function usage.
-        
-        ```python
-        ## Note: Ensure that the units for each laboratory value are consistent with
-        # your model's requirements.
-        
-        # mock dataframe example
-        data = pd.DataFrame(
-            {
-                "Age": [65, 70, 60, 75, 80],
-                "Sex": ["male", "female", "female", "male", "female"],
-                "eGFR": [19, 50, 45, 22, 30],  # eGFR in mL/min/1.73 m^2
-                "uACR": [30, 35, 25, 40, 50],  # uACR in mg/g
-                "Diabetes": [1, 0, 0, 1, 1],  # 1 for diabetes, 0 for no diabetes
-                "Hypertension": [1, 1, 0, 1, 0],  # 1 for hypertension, 0 for no hypertension
-                "Albumin": [3.5, 4.0, 3.8, 3.3, 3.7],  # Serum albumin in g/dL
-                "Phosphorus": [3.5, 4.1, 3.9, 4.5, 3.2],  # Serum phosphorus in mg/dL
-                "Bicarbonate": [24, 22, 25, 21, 23],  # Serum bicarbonate in mEq/L
-                "Calcium": [9.5, 9.7, 9.4, 8.8, 9.6],  # Serum calcium in mg/dL
-            }
-        )
-        
-        # Assuming 'data' and 'columns' are already defined as per your data structure
-        data_with_risks = add_kfre_risk_col(
-            df=data,
-            age_col="Age",
-            sex_col="Sex",
-            eGFR_col="eGFR",
-            uACR_col="uACR",
-            dm_col="Diabetes",
-            htn_col="Hypertension",
-            albumin_col="Albumin",
-            phosphorous_col="Phosphorus",
-            bicarbonate_col="Bicarbonate",
-            calcium_col="Calcium",
-            num_vars=[4, 6, 8],  # can also be a tuple
-            years=(2, 5),  # can also be a list
-            is_north_american=False,
-            copy=True,  # Work on a copy of the DataFrame
-        )
-        
-        
-        # The resulting DataFrame 'data' now includes new columns with risk predictions
-        # for each model and time frame
-        data_with_risks
-        ```
-        
-        | **Age** | **Sex** | **eGFR** | **uACR** | **Diabetes** | **Hypertension** | **Albumin** | **Phosphorus** | **Bicarbonate** | **Calcium** | **kfre_4var_2year** | **kfre_4var_5year** | **kfre_6var_2year** | **kfre_6var_5year** | **kfre_8var_2year** | **kfre_8var_5year** |
-        |---------|:-------:|:--------:|:--------:|:------------:|:----------------:|:-----------:|:--------------:|:---------------:|:-----------:|:-------------------:|:-------------------:|:-------------------:|:-------------------:|:-------------------:|:-------------------:|
-        | 65      |   male  |    19    |    30    |       1      |         1        |     3.5     |       3.5      |        24       |     9.5     |       0.063123      |       0.223128      |       0.060014      |       0.209336      |       0.069774      |       0.277728      |
-        | 70      |  female |    50    |    35    |       0      |         1        |      4      |       4.1      |        22       |     9.7     |       0.00155       |       0.005987      |       0.001717      |       0.006501      |       0.00303       |       0.013559      |
-        | 60      |  female |    45    |    25    |       0      |         0        |     3.8     |       3.9      |        25       |     9.4     |       0.002893      |       0.011156      |       0.002773      |       0.010484      |       0.004705      |       0.020993      |
-        | 75      |   male  |    22    |    40    |       1      |         1        |     3.3     |       4.5      |        21       |     8.8     |       0.041757      |       0.152247      |       0.039731      |       0.142611      |       0.09375       |       0.357774      |
-        | 80      |  female |    30    |    50    |       1      |         0        |     3.7     |       3.2      |        23       |     9.6     |       0.013457      |       0.051111      |       0.011059      |       0.041325      |       0.016574      |       0.072424      |
-        
-        
-        ## `add_kfre_risk_col`
-        
-        Purpose:
-        
-        This function is designed to compute the risk of chronic kidney disease (CKD) over specified or all possible models and time frames, directly appending the results as new columns to the provided DataFrame. It organizes the results by model (4-variable, 6-variable, 8-variable) first, followed by the time frame (2 years, 5 years) for each model type.
-        
-        Usage: 
-        
-        ```python
-        df = add_kfre_risk_col(
-            df=df,
-            age_col="Age",
-            sex_col="SEX",
-            eGFR_col="eGFR-EPI",
-            uACR_col="uACR",
-            dm_col="Diabetes (1=yes; 0=no)",
-            htn_col="Hypertension (1=yes; 0=no)",
-            albumin_col="Albumin_g_dl",
-            phosphorous_col="Phosphate_mg_dl",
-            bicarbonate_col="Bicarbonate (mmol/L)",
-            calcium_col="Calcium_mg_dl",
-            num_vars=8,
-            years=(2, 5),
-            is_north_american=False,
-            copy=False  # Modify the original DataFrame directly
-        )
-        ```
-        
-        Parameters: 
-        
-        - `df` (DataFrame): The patient data containing required clinical parameters.
-        - `age_col`, `sex_col`, `eGFR_col`, `uACR_col`, `dm_col`, `htn_col`, `albumin_col`, `phosphorous_col`, `bicarbonate_col`, `calcium_col` (str): Column names in df that correspond to the clinical parameters required for risk calculation.
-        - `num_vars` (int or list): Specifies the number of variables to use for the risk calculations (4, 6, or 8). It determines the complexity of the model applied.
-        - `years` (tuple, list, or int): Specifies the time frames over which to calculate the risk. Valid inputs include combinations of 2 and 5 years.
-        - `is_north_american` (bool): Flag indicating whether the patient data should be analyzed with coefficients specific to the North American population.
-        - `copy` (bool): If set to True, operates on and returns a copy of the DataFrame. If False, modifies the original DataFrame directly.
-        
-        Returns: 
-        
-        - `DataFrame`: The modified DataFrame with new columns added for each model and time frame specified. Columns are named following the pattern `pred_{model_var}var_{year}year`, where `{model_var}` is the number of variables (4, 6, or 8) and `{year}` is the time frame (2 or 5).
-        
-        ## Conversion of Clinical Parameters
-        
-        The `kfre` library includes a utility function `perform_conversions` designed to convert clinical measurement units. This function is especially useful when preparing data for analyses that require specific units. It can handle conversions for multiple parameters, such as urinary protein-creatinine ratio (uPCR), calcium, phosphate, and albumin levels.
-        
-        **Key Features**
-        
-        - **Flexible Conversion:** The function supports both standard and reverse conversions, allowing users to switch between units as needed.
-        - **Batch Processing:** It can process entire columns of data, making it suitable for datasets with multiple patients.
-        - **Custom Column Names:** Users can specify which columns to convert, providing flexibility in handling datasets with varied naming conventions.
-        
-        **Parameters**
-        
-        - `df` (DataFrame): The DataFrame containing the data to be converted.
-        - `reverse` (bool): If True, performs the reverse conversion (e.g., mmol/L to mg/dL). If False, performs the standard conversion (e.g., mg/dL to mmol/L).
-        - `convert_all` (bool): If True, attempts to automatically identify and convert all recognized columns.
-        - `upcr_col`, `calcium_col`, `phosphate_col`, `albumin_col` (str, optional): Column names in the DataFrame that contain the values to be converted.
-        
-        ### Convert Specific Variables from mmol/L to mg/g and/or g/dL
-        
-        #### uPCR to uACR
-        The conversion of uPCR from mg/mmol to mg/g involves understanding that both mg/mmol and mg/g are ratios that can be related through their units.
-        
-        - mg/mmol is a ratio of mass (in milligrams) to molar concentration (in millimoles), while
-        - mg/g is a ratio of mass (in milligrams) to mass (in grams).
-        
-        To convert mg/mmol to mg/g, we need to know the molar mass of creatinine, because uPCR is the ratio of the mass of protein to the mass of creatinine. The molar mass of creatinine is approximately 113.12 g/mol. Therefore, 1 mmol of creatinine is 113.12 mg.
-        
-        Here's the conversion:
-        
-        1 mg/mmol means that you have 1 mg of protein for every 1 mmol of creatinine. Since 1 mmol of creatinine is 113.12 mg:
-        
-        $$ \frac{\text{1 mg}}{\text{1 mmol creatinine}} \times \frac{\text{113.12 mg creatinine}}{\text{1 g creatinine}} = 113.12 \text{ mg/g} $$
-        
-        However, since we are interested in a ratio where the denominator is 1 g (or 1000 mg) rather than 113.12 mg, we use the following calculation:
-        
-        $$ \frac{\text{1 mg protein}}{\text{0.11312 g creatinine}} \approx 8.84  {\text{ mg/g}} $$
-        
-        #### Calcium
-        
-        Calcium is often measured in millimoles per liter (mmol/L) and needs to be converted to milligrams per deciliter (mg/dL) for certain clinical applications or study comparisons.
-        - Molecular weight of Calcium (Ca): Calcium's atomic weight is approximately 40.08 g/mol.
-        - Conversion factor: To convert mmol/L to mg/dL for calcium, you multiply by 4. This is derived as follows:
-        
-        $$ \text{1 mmol/L} \times  \frac{\text{40.08 mg}}{{\text{1 mmol}}} \times \frac{\text {1L} } {\text{10 dL}} = 4.008 \text{ mg/dL}$$
-        
-        #### Phosphate
-        
-        Phosphate concentrations are similarly reported in mmol/L but often need to be expressed in mg/dL.
-        
-        - Molecular weight of Phosphate $(PO_4^{3-})$: The molar mass of phosphate as an ion (considering phosphorus and oxygen) is approximately 94.97 g/mol.
-        - Conversion factor: To convert mmol/L to mg/dL for phosphate:
-        
-        $$ \text{1 mmol/L} \times  \frac{\text{94.97 mg}}{{\text{1 mmol}}} \times \frac{\text {1L} } {\text{10 dL}} \approx 9.497 \text{ mg/dL}$$
-        
-        The clinical conversion factor used is slightly simplified to 3.1, likely a rounded approximation or specific to the binding state of phosphate in clinical assays.
-        
-        #### Albumin
-        
-        Albumin measurements are often made in grams per liter (g/L) and converted to grams per deciliter (g/dL) for standard reporting in many clinical contexts.
-        
-        Conversion factor: Converting g/L to g/dL is straightforward as it involves shifting the decimal point:
-        
-        $$ 1\text{ g/L} \div 10 = 0.1 \text { g/dL} $$
-        
-        These conversions help ensure consistency in reporting and interpreting lab values across different systems and studies, facilitating better comparison and understanding of patient data.
-        
-        **Usage Example**
-        
-        The following is a mock example to illustrate the usage of the perform_conversions function. This example shows how to convert values from mmol to mg for various clinical parameters within a DataFrame.
-        
-        ```python
-        # Sample DataFrame
-        df = pd.DataFrame(
-            {
-                "uPCR (mmol)": [0.5, 0.7, 0.2],  # Example values that need conversion
-                "Calcium (mmol)": [2.5, 2.0, 2.2],
-                "Phosphate": [1.2, 1.3, 1.1],
-                "Albumin": [0.45, 0.50, 0.47],
-            }
-        )
-        
-        # Perform conversions using the wrapper function, specifying all parameters
-        # Perform conversions and specify new column names
-        converted_df = perform_conversions(
-            df=df,
-            reverse=False,
-            upcr_col="uPCR (mmol)",
-            calcium_col="Calcium",
-            albumin_col="Albumin",
-            convert_all=True,
-        )
-        
-        # Print the DataFrame to see the changes
-        converted_df
-        ```
-        ```
-        Converted 'uPCR (mmol)' to new column 'uPCR_mg_g' with factor 8.84016973125884
-        Converted 'Calcium (mmol)' to new column 'Calcium_mg_dl' with factor 4
-        Converted 'Phosphate' to new column 'Phosphate_mg_dl' with factor 3.1
-        Converted 'Albumin' to new column 'Albumin_g_dl' with factor 0.1
-        ```
-        
-        | **uPCR   (mmol)** | **Calcium (mmol)** | **Phosphate** | **Albumin** | **uPCR_mg_g** | **Calcium_mg_dl** | **Phosphate_mg_dl** | **Albumin_g_dl** |
-        |:-----------------:|:------------------:|:-------------:|:-----------:|:-------------:|:-----------------:|:-------------------:|:----------------:|
-        |        0.5        |         2.5        |      1.2      |     0.45    |    4.420085   |         10        |         3.72        |       0.045      |
-        |        0.7        |          2         |      1.3      |     0.5     |    6.188119   |         8         |         4.03        |       0.05       |
-        |        0.2        |         2.2        |      1.1      |     0.47    |    1.768034   |        8.8        |         3.41        |       0.047      |
-        
-        
-        ## Contributor/Maintainer
-        
-        <img align="left" width="150" height="150" src="https://www.leonshpaner.com/author/leon-shpaner/avatar_hu48de79c369d5f7d4ff8056a297b2c4c5_1681850_270x270_fill_q90_lanczos_center.jpg">
-        
-        [Leonid Shpaner](https://github.com/lshpaner) is a Data Scientist at UCLA Health. With over a decade experience in analytics and teaching, he has collaborated on a wide variety of projects within financial services, education, personal development, and healthcare. He serves as a course facilitator for Data Analytics and Applied Statistics at Cornell University and is a lecturer of Statistics in Python for the University of San Diegoâ€™s M.S. Applied Artificial Intelligence program.
-        
-        <br><br>
-        
-        ## License
-        `kfre` is distributed under the MIT License. See [`LICENSE`](LICENSE.md) for more information.
-        
-        ## Support
-        If you have any questions or issues with `kfre`, please open an issue on this GitHub repository.
-        
-        ## Acknowledgements
-        Tangri's KFRE model and its contributions to kidney disease research.
-        
-        ## References
-        The `kfre` library is based on the risk prediction models developed in the following studies:
-        
-        1. Tangri N, Grams ME, Levey AS, Coresh J, Appel LJ, Astor BC, Chodick G, Collins AJ, Djurdjev O, Elley CR, Evans M, Garg AX, Hallan SI, Inker LA, Ito S, Jee SH, Kovesdy CP, Kronenberg F, Heerspink HJL, Marks A, Nadkarni GN, Navaneethan SD, Nelson RG, Titze S, Sarnak MJ, Stengel B, Woodward M, Iseki K, for the CKD Prognosis Consortium. (2016). *Multinational assessment of accuracy of equations for predicting risk of kidney failure: A meta-analysis. JAMA,* **315**(2), 164â€“174. doi: 10.1001/jama.2015.18202.
-        
-        2. Tangri, N., Stevens, L. A., Griffith, J., Tighiouart, H., Djurdjev, O., Naimark, D., Levin, A., & Levey, A. S. (2011). *A predictive model for progression of chronic kidney disease to kidney failure. JAMA,* **305**(15), 1553-1559. doi: 10.1001/jama.2011.451.  
-        
-        3. Sumida K, Nadkarni GN, Grams ME, Sang Y, Ballew SH, Coresh J, Matsushita K, Surapaneni A, Brunskill N, Chadban SJ, Chang AR, Cirillo M, Daratha KB, Gansevoort RT, Garg AX, Iacoviello L, Kayama T, Konta T, Kovesdy CP, Lash J, Lee BJ, Major RW, Metzger M, Miura K, Naimark DMJ, Nelson RG, Sawhney S, Stempniewicz N, Tang M, Townsend RR, Traynor JP, Valdivielso JM, Wetzels J, Polkinghorne KR, Heerspink HJL, for the Chronic Kidney Disease Prognosis Consortium. (2020). Conversion of urine protein-creatinine ratio or urine dipstick protein to urine albumin-creatinine ratio for use in chronic kidney disease screening and prognosis. *Ann Intern Med,* ***173***(6), 426-435. doi: 10.7326/M20-0529.
-        
-        
-        Please refer to these studies for an in-depth understanding of the kidney failure risk prediction models used within this library.
-        
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# KFRE: Kidney Failure Risk Estimator
+
+[![PyPI](https://img.shields.io/pypi/v/kfre.svg)](https://pypi.org/project/kfre/)
+[![Downloads](https://pepy.tech/badge/kfre)](https://pepy.tech/project/kfre)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/lshpaner/kfre/tree/main?tab=License-1-ov-file)
+[![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.11100223.svg)](https://doi.org/10.5281/zenodo.11100222)
+
+`kfre` is a Python library designed to estimate the risk of chronic kidney disease (CKD) progression over two distinct timelines: 2 years and 5 years. Using Tangri's Kidney Failure Risk Equation (KFRE), the library provides tools for healthcare professionals and researchers to predict CKD risk based on patient data. It supports predictions for both males and females and includes specific adjustments for individuals from North American and non-North American regions.
+
+--------
+## Table of Contents
+
+1. [Features](#Features)
+2. [Prerequisites](#Prerequisites)
+3. [Installation](#installation)
+4. [Usage Guide](#usage-guide)
+   - [Single Patient Risk Calculation](#single-patient-risk-calculation)
+   - [Batch Risk Calculation for Multiple Patients](#batch-risk-calculation-for-multiple-patients)
+   - [Conversion of Clinical Parameters](#conversion-of-clinical-parameters)
+        - [uPCR to uACR](#upcr-to-uacr)
+        - [Calcium](#calcium)
+        - [Phosphate](#phosphate)
+        - [Albumin](#albumin)
+5. [Contributor/Maintainer](#contributormaintainer)
+6. [License](#license)
+7. [Support](#acknowledgements)
+8. [References](#references)
+--------
+
+
+## Features
+
+- **Risk Prediction**: Utilize Tangri's validated risk prediction model to estimate kidney failure risk using
+    - 4 variables: sex, age, eGFR, uACR (log-normalized)
+    - 6 variables: sex, age, eGFR, uACR (log-normalized), diabetes mellitus, hypertension
+    - 8 variables: sex, age, eGFR, uACR (log-normalized), serum albumin, serum phosphorous, serum calcium, and serum bicarbonate.
+- **Data Flexibility**: Handles various input data formats and maps them to required model parameters.
+- **Conversion Utilities**: Includes functions to convert common laboratory results to the required units for risk prediction.
+
+### Important Note on Data Units
+The kfre library requires precise data input, with clear specification of the units for each variable. The variables can be expressed in multiple units, and it's crucial that the data being used clearly delineates which units the variables are expressed in. For instance:
+
+- uACR (Urinary Albumin-Creatinine Ratio) can be expressed in either mg/g or mg/mmol.
+- Albumin levels can be measured in g/dL or g/L.
+- Phosphorous levels can be noted in mg/dL or mmol/L.
+- Bicarbonate can be recorded in mEq/L or mmol/L.
+- Calcium can be documented in mg/dL or mmol/L.
+
+This flexibility allows the library to be used with a variety of clinical data sources, enhancing its applicability across different healthcare settings.
+
+## Prerequisites
+Before you install `kfre`, ensure you have the following:
+
+- **Python**: Python 3.6 or higher is required to run `kfre`.
+
+Additionally, kfre has the following package dependencies:
+
+- **NumPy**: Version 1.18.5 or higher
+- **Pandas**: Version 1.0.5 or higher
+
+These dependencies will be automatically installed when you install kfre using pip.
+
+## Installation
+
+You can install `kfre` directly from PyPI:
+
+```bash
+pip install kfre
+```
+
+## Usage Guide
+
+## Single Patient Risk Calculation
+The kfre library offers a flexible and user-friendly interface to estimate the risk of kidney failure for individual patients using Tangri's KFRE model. With `kfre`, you can calculate the risk using the classic 4-variable model, the detailed 8-variable model, and, uniquely, a 6-variable model that is not commonly found in online calculators.
+
+## `kfre_person`
+
+```python
+risk_percentage = kfre_person(
+    age=57.28,
+    is_male=False,
+    eGFR=15.0,
+    uACR=1762.001840,
+    is_north_american=False,
+    years=2,
+    dm=None,
+    htn=None,
+    albumin=None,
+    phosphorous=None,
+    bicarbonate=None,
+    calcium=None
+) * 100  # Convert to percentage
+
+```
+
+Parameters: 
+
+- `age` (float): The age of the patient in years.
+- `is_male` (bool): Indicates if the patient is male. False indicates a female patient.
+- `eGFR` (float): Estimated Glomerular Filtration Rate in mL/min/1.73 m², indicating kidney function.
+- `uACR` (float): Urinary Albumin to Creatinine Ratio in mg/g, indicating kidney damage.
+- `is_north_american` (bool): Specifies whether the patient is from North America, affecting model constants.
+- `years` (int): The time frame in years (2 or 5) over which the risk assessment is projected.
+- `dm` (float, optional): Diabetes mellitus status (1 if present, 0 if not). Required for the 6-variable model.
+- `htn` (float, optional): Hypertension status (1 if present, 0 if not). Required for the 6-variable model.
+- `albumin` (float, optional): Serum albumin level in g/dL. Required for the 8-variable model.
+- `phosphorous` (float, optional): Serum phosphorus level in mg/dL. Required for the 8-variable model.
+- `bicarbonate` (float, optional): Serum bicarbonate level in mEq/L. Required for the 8-variable model.
+- `calcium` (float, optional): Serum calcium level in mg/dL. Required for the 8-variable model.
+
+Returns:
+
+`float`: The risk of developing CKD within the specified timeframe, as a decimal. Multiply by 100 to convert to a percentage.
+
+Description:
+
+The `kfre_person` function allows for detailed, personalized risk assessments based on a range of clinical parameters. Depending on the completeness of the data provided, the function can apply a basic 4-variable model or more comprehensive models incorporating additional risk factors like diabetes, hypertension, and various biochemical markers.
+
+The function is designed for ease of use in clinical settings or research, providing immediate risk estimations that are crucial for patient management or further analysis.
+
+### Example Calculation for 2-year and 5-year Risk
+Here's how to estimate the 2-year and 5-year kidney failure risk for a hypothetical 57.28-year-old female who is not from North America and has specific clinical characteristics:
+
+```python
+from kfre import kfre_person
+
+for years in [2, 5]:
+    risk_percentage = (
+        kfre_person(
+            age=57.28,
+            is_male=False,  # is the patient male?
+            eGFR=15.0,  # ml/min/1.73 m^2
+            uACR=1762.001840,  # mg/g
+            is_north_american=False,  # is the patient from North America?
+            years=years,
+            ####################################################################
+            # Uncomment "dm" and "htn" for the 6-variable model:
+            ####################################################################
+            # dm=0,
+            # htn=1,
+            ####################################################################
+            # Comment out "dm" and "htn" and uncomment the following lines for
+            # the 8-variable model:
+            ####################################################################
+            # albumin=3.0, # g/dL
+            # phosphorous=3.162, # mg/dL
+            # bicarbonate=21.3, # mEq/L
+            # calcium=9.72, # mg/dL
+        )
+        * 100  # multiply by 100 to convert to percentage
+    )
+
+    message = f"The {years}-year risk of kidney failure for this patient is"
+    print(f"{message} {risk_percentage:.2f}%.")
+```
+```
+The 2-year risk of kidney failure for this patient is 44.66%.
+The 5-year risk of kidney failure for this patient is 89.89%.
+```
+
+Ensure to:
+- Uncomment `dm` and `htn` if you are using the 6-variable KFRE model.
+- For the 8-variable KFRE, keep `dm` and `htn` commented out and instead, uncomment the `albumin`, `phosphorous`, `bicarbonate`, and `calcium` variables.
+
+
+## Batch Risk Calculation for Multiple Patients
+The kfre library provides the functionality to perform batch processing of patient data, allowing for the computation of kidney failure risk predictions across multiple patients in a single operation. This capability is especially valuable for researchers and clinicians needing to assess risks for large cohorts or patient groups.
+
+**Key Features**
+
+When using the `add_kfre_risk_col` function, the library will append new columns for each specified variable model (4-variable, 6-variable, 8-variable) and each time frame (2 years, 5 years) directly to the original DataFrame. This facilitates a seamless integration of risk predictions into existing patient datasets without the need for additional data manipulation steps.
+
+***Disclaimer***
+
+The `kfre` library is designed to facilitate risk prediction using Tangri's KFRE model based on a given set of patient data. It is crucial to ensure that all patient data within a batch calculation are consistent in terms of regional categorization—that is, either all North American or all non-North American. To this end, it is crucial to ensure that all patient data within a batch calculation are consistent in terms of regional categorization. Mixing patient data from different regions within a single batch is not supported, as the function is set to apply one regional coefficient set at a time. This approach ensures the accuracy and reliability of the risk predictions.
+
+Example Usage:
+
+Here is how to perform batch risk calculations for a group of non-North American patients. Note the importance of maintaining consistency in regional data:
+
+***Note***: The following is a mock example using simulated DataFrame structures to illustrate the function usage.
+
+```python
+## Note: Ensure that the units for each laboratory value are consistent with
+# your model's requirements.
+
+# mock dataframe example
+data = pd.DataFrame(
+    {
+        "Age": [65, 70, 60, 75, 80],
+        "Sex": ["male", "female", "female", "male", "female"],
+        "eGFR": [19, 50, 45, 22, 30],  # eGFR in mL/min/1.73 m^2
+        "uACR": [30, 35, 25, 40, 50],  # uACR in mg/g
+        "Diabetes": [1, 0, 0, 1, 1],  # 1 for diabetes, 0 for no diabetes
+        "Hypertension": [1, 1, 0, 1, 0],  # 1 for hypertension, 0 for no hypertension
+        "Albumin": [3.5, 4.0, 3.8, 3.3, 3.7],  # Serum albumin in g/dL
+        "Phosphorus": [3.5, 4.1, 3.9, 4.5, 3.2],  # Serum phosphorus in mg/dL
+        "Bicarbonate": [24, 22, 25, 21, 23],  # Serum bicarbonate in mEq/L
+        "Calcium": [9.5, 9.7, 9.4, 8.8, 9.6],  # Serum calcium in mg/dL
+    }
+)
+
+data_with_risks = add_kfre_risk_col(
+    df=data,
+    age_col="Age",
+    sex_col="Sex",
+    eGFR_col="eGFR",
+    uACR_col="uACR",
+    dm_col="Diabetes",
+    htn_col="Hypertension",
+    albumin_col="Albumin",
+    phosphorous_col="Phosphorus",
+    bicarbonate_col="Bicarbonate",
+    calcium_col="Calcium",
+    num_vars=[4, 6, 8],  # can also be a tuple
+    years=(2, 5),  # can also be a list
+    is_north_american=False,
+    copy=True,  # Work on a copy of the DataFrame
+)
+
+
+# The resulting DataFrame 'data' now includes new columns with risk predictions
+# for each model and time frame
+data_with_risks
+```
+
+| **Age** | **Sex** | **eGFR** | **uACR** | **Diabetes** | **Hypertension** | **Albumin** | **Phosphorus** | **Bicarbonate** | **Calcium** | **kfre_4var_2year** | **kfre_4var_5year** | **kfre_6var_2year** | **kfre_6var_5year** | **kfre_8var_2year** | **kfre_8var_5year** |
+|---------|:-------:|:--------:|:--------:|:------------:|:----------------:|:-----------:|:--------------:|:---------------:|:-----------:|:-------------------:|:-------------------:|:-------------------:|:-------------------:|:-------------------:|:-------------------:|
+| 65      |   male  |    19    |    30    |       1      |         1        |     3.5     |       3.5      |        24       |     9.5     |       0.063123      |       0.223128      |       0.060014      |       0.209336      |       0.069774      |       0.277728      |
+| 70      |  female |    50    |    35    |       0      |         1        |      4      |       4.1      |        22       |     9.7     |       0.00155       |       0.005987      |       0.001717      |       0.006501      |       0.00303       |       0.013559      |
+| 60      |  female |    45    |    25    |       0      |         0        |     3.8     |       3.9      |        25       |     9.4     |       0.002893      |       0.011156      |       0.002773      |       0.010484      |       0.004705      |       0.020993      |
+| 75      |   male  |    22    |    40    |       1      |         1        |     3.3     |       4.5      |        21       |     8.8     |       0.041757      |       0.152247      |       0.039731      |       0.142611      |       0.09375       |       0.357774      |
+| 80      |  female |    30    |    50    |       1      |         0        |     3.7     |       3.2      |        23       |     9.6     |       0.013457      |       0.051111      |       0.011059      |       0.041325      |       0.016574      |       0.072424      |
+
+
+## `add_kfre_risk_col`
+
+Purpose:
+
+This function is designed to compute the risk of chronic kidney disease (CKD) over specified or all possible models and time frames, directly appending the results as new columns to the provided DataFrame. It organizes the results by model (4-variable, 6-variable, 8-variable) first, followed by the time frame (2 years, 5 years) for each model type.
+
+Usage: 
+
+```python
+df = add_kfre_risk_col(
+    df=df,
+    age_col="Age",
+    sex_col="SEX",
+    eGFR_col="eGFR-EPI",
+    uACR_col="uACR",
+    dm_col="Diabetes (1=yes; 0=no)",
+    htn_col="Hypertension (1=yes; 0=no)",
+    albumin_col="Albumin_g_dl",
+    phosphorous_col="Phosphate_mg_dl",
+    bicarbonate_col="Bicarbonate (mmol/L)",
+    calcium_col="Calcium_mg_dl",
+    num_vars=8,
+    years=(2, 5),
+    is_north_american=False,
+    copy=False  # Modify the original DataFrame directly
+)
+```
+
+Parameters: 
+
+- `df` (DataFrame): The patient data containing required clinical parameters.
+- `age_col`, `sex_col`, `eGFR_col`, `uACR_col`, `dm_col`, `htn_col`, `albumin_col`, `phosphorous_col`, `bicarbonate_col`, `calcium_col` (str): Column names in df that correspond to the clinical parameters required for risk calculation.
+- `num_vars` (int or list): Specifies the number of variables to use for the risk calculations (4, 6, or 8). It determines the complexity of the model applied.
+- `years` (tuple, list, or int): Specifies the time frames over which to calculate the risk. Valid inputs include combinations of 2 and 5 years.
+- `is_north_american` (bool): Flag indicating whether the patient data should be analyzed with coefficients specific to the North American population.
+- `copy` (bool): If set to True, operates on and returns a copy of the DataFrame. If False, modifies the original DataFrame directly.
+
+Returns: 
+
+- `DataFrame`: The modified DataFrame with new columns added for each model and time frame specified. Columns are named following the pattern `pred_{model_var}var_{year}year`, where `{model_var}` is the number of variables (4, 6, or 8) and `{year}` is the time frame (2 or 5).
+
+## Conversion of Clinical Parameters
+
+The `kfre` library includes a utility function `perform_conversions` designed to convert clinical measurement units. This function is especially useful when preparing data for analyses that require specific units. It can handle conversions for multiple parameters, such as urinary protein-creatinine ratio (uPCR), calcium, phosphate, and albumin levels.
+
+**Key Features**
+
+- **Flexible Conversion:** The function supports both standard and reverse conversions, allowing users to switch between units as needed.
+- **Batch Processing:** It can process entire columns of data, making it suitable for datasets with multiple patients.
+- **Custom Column Names:** Users can specify which columns to convert, providing flexibility in handling datasets with varied naming conventions.
+
+**Parameters**
+
+- `df` (DataFrame): The DataFrame containing the data to be converted.
+- `reverse` (bool): If True, performs the reverse conversion (e.g., mmol/L to mg/dL). If False, performs the standard conversion (e.g., mg/dL to mmol/L).
+- `convert_all` (bool): If True, attempts to automatically identify and convert all recognized columns.
+- `upcr_col`, `calcium_col`, `phosphate_col`, `albumin_col` (str, optional): Column names in the DataFrame that contain the values to be converted.
+
+### Convert Specific Variables from mmol/L to mg/g and/or g/dL
+
+#### uPCR to uACR
+The conversion of uPCR from mg/mmol to mg/g involves understanding that both mg/mmol and mg/g are ratios that can be related through their units.
+
+- mg/mmol is a ratio of mass (in milligrams) to molar concentration (in millimoles), while
+- mg/g is a ratio of mass (in milligrams) to mass (in grams).
+
+To convert mg/mmol to mg/g, we need to know the molar mass of creatinine, because uPCR is the ratio of the mass of protein to the mass of creatinine. The molar mass of creatinine is approximately 113.12 g/mol. Therefore, 1 mmol of creatinine is 113.12 mg.
+
+Here's the conversion:
+
+1 mg/mmol means that you have 1 mg of protein for every 1 mmol of creatinine. Since 1 mmol of creatinine is 113.12 mg:
+
+$$ \frac{\text{1 mg}}{\text{1 mmol creatinine}} \times \frac{\text{113.12 mg creatinine}}{\text{1 g creatinine}} = 113.12 \text{ mg/g} $$
+
+However, since we are interested in a ratio where the denominator is 1 g (or 1000 mg) rather than 113.12 mg, we use the following calculation:
+
+$$ \frac{\text{1 mg protein}}{\text{0.11312 g creatinine}} \approx 8.84  {\text{ mg/g}} $$
+
+#### Calcium
+
+Calcium is often measured in millimoles per liter (mmol/L) and needs to be converted to milligrams per deciliter (mg/dL) for certain clinical applications or study comparisons.
+- Molecular weight of Calcium (Ca): Calcium's atomic weight is approximately 40.08 g/mol.
+- Conversion factor: To convert mmol/L to mg/dL for calcium, you multiply by 4. This is derived as follows:
+
+$$ \text{1 mmol/L} \times  \frac{\text{40.08 mg}}{{\text{1 mmol}}} \times \frac{\text {1L} } {\text{10 dL}} = 4.008 \text{ mg/dL}$$
+
+#### Phosphate
+
+Phosphate concentrations are similarly reported in mmol/L but often need to be expressed in mg/dL.
+
+- Molecular weight of Phosphate (PO₄³⁻): The molar mass of phosphate as an ion (considering phosphorus and oxygen) is approximately 94.97 g/mol.
+- Conversion factor: To convert mmol/L to mg/dL for phosphate:
+
+$$ \text{1 mmol/L} \times  \frac{\text{94.97 mg}}{{\text{1 mmol}}} \times \frac{\text {1L} } {\text{10 dL}} \approx 9.497 \text{ mg/dL}$$
+
+The clinical conversion factor used is slightly simplified to 3.1, likely a rounded approximation or specific to the binding state of phosphate in clinical assays.
+
+#### Albumin
+
+Albumin measurements are often made in grams per liter (g/L) and converted to grams per deciliter (g/dL) for standard reporting in many clinical contexts.
+
+Conversion factor: Converting g/L to g/dL is straightforward as it involves shifting the decimal point:
+
+$$ 1\text{ g/L} \div 10 = 0.1 \text { g/dL} $$
+
+These conversions help ensure consistency in reporting and interpreting lab values across different systems and studies, facilitating better comparison and understanding of patient data.
+
+**Usage Example**
+
+The following is a mock example to illustrate the usage of the `perform_conversions` function. This example shows how to convert values from mmol to mg for various clinical parameters within a DataFrame.
+
+```python
+# Sample DataFrame
+df = pd.DataFrame(
+    {
+        "uPCR (mmol)": [0.5, 0.7, 0.2],  # Example values that need conversion
+        "Calcium (mmol)": [2.5, 2.0, 2.2],
+        "Phosphate": [1.2, 1.3, 1.1],
+        "Albumin": [0.45, 0.50, 0.47],
+    }
+)
+
+# Perform conversions using the wrapper function, specifying all parameters
+# Perform conversions and specify new column names
+converted_df = perform_conversions(
+    df=df,
+    reverse=False,
+    upcr_col="uPCR (mmol)",
+    calcium_col="Calcium",
+    albumin_col="Albumin",
+    convert_all=True,
+)
+
+# Print the DataFrame to see the changes
+converted_df
+```
+```
+Converted 'uPCR (mmol)' to new column 'uPCR_mg_g' with factor 8.84016973125884
+Converted 'Calcium (mmol)' to new column 'Calcium_mg_dl' with factor 4
+Converted 'Phosphate' to new column 'Phosphate_mg_dl' with factor 3.1
+Converted 'Albumin' to new column 'Albumin_g_dl' with factor 0.1
+```
+
+| **uPCR   (mmol)** | **Calcium (mmol)** | **Phosphate** | **Albumin** | **uPCR_mg_g** | **Calcium_mg_dl** | **Phosphate_mg_dl** | **Albumin_g_dl** |
+|:-----------------:|:------------------:|:-------------:|:-----------:|:-------------:|:-----------------:|:-------------------:|:----------------:|
+|        0.5        |         2.5        |      1.2      |     0.45    |    4.420085   |         10        |         3.72        |       0.045      |
+|        0.7        |          2         |      1.3      |     0.5     |    6.188119   |         8         |         4.03        |       0.05       |
+|        0.2        |         2.2        |      1.1      |     0.47    |    1.768034   |        8.8        |         3.41        |       0.047      |
+
+
+## Contributor/Maintainer
+
+<img align="left" width="150" height="150" src="https://www.leonshpaner.com/author/leon-shpaner/avatar_hu48de79c369d5f7d4ff8056a297b2c4c5_1681850_270x270_fill_q90_lanczos_center.jpg">
+
+[Leonid Shpaner](https://github.com/lshpaner) is a Data Scientist at UCLA Health. With over a decade experience in analytics and teaching, he has collaborated on a wide variety of projects within financial services, education, personal development, and healthcare. He serves as a course facilitator for Data Analytics and Applied Statistics at Cornell University and is a lecturer of Statistics in Python for the University of San Diego’s M.S. Applied Artificial Intelligence program.
+
+<br><br>
+
+## License
+`kfre` is distributed under the MIT License. See [`LICENSE`](LICENSE.md) for more information.
+
+## Support
+If you have any questions or issues with `kfre`, please open an issue on this GitHub repository.
+
+## Acknowledgements
+Tangri's KFRE model and its contributions to kidney disease research.
+
+The `kfre` library is based on the risk prediction models developed in the following studies. Please refer to these studies for an in-depth understanding of the kidney failure risk prediction models used within this library.
+
+
+## References
+
+1. Tangri N, Grams ME, Levey AS, Coresh J, Appel LJ, Astor BC, Chodick G, Collins AJ, Djurdjev O, Elley CR, Evans M, Garg AX, Hallan SI, Inker LA, Ito S, Jee SH, Kovesdy CP, Kronenberg F, Heerspink HJL, Marks A, Nadkarni GN, Navaneethan SD, Nelson RG, Titze S, Sarnak MJ, Stengel B, Woodward M, Iseki K, for the CKD Prognosis Consortium. (2016). *Multinational assessment of accuracy of equations for predicting risk of kidney failure: A meta-analysis. JAMA,* **315**(2), 164–174. doi: 10.1001/jama.2015.18202.
+
+2. Tangri, N., Stevens, L. A., Griffith, J., Tighiouart, H., Djurdjev, O., Naimark, D., Levin, A., & Levey, A. S. (2011). *A predictive model for progression of chronic kidney disease to kidney failure. JAMA,* **305**(15), 1553-1559. doi: 10.1001/jama.2011.451.  
+
+3. Sumida K, Nadkarni GN, Grams ME, Sang Y, Ballew SH, Coresh J, Matsushita K, Surapaneni A, Brunskill N, Chadban SJ, Chang AR, Cirillo M, Daratha KB, Gansevoort RT, Garg AX, Iacoviello L, Kayama T, Konta T, Kovesdy CP, Lash J, Lee BJ, Major RW, Metzger M, Miura K, Naimark DMJ, Nelson RG, Sawhney S, Stempniewicz N, Tang M, Townsend RR, Traynor JP, Valdivielso JM, Wetzels J, Polkinghorne KR, Heerspink HJL, for the Chronic Kidney Disease Prognosis Consortium. (2020). Conversion of urine protein-creatinine ratio or urine dipstick protein to urine albumin-creatinine ratio for use in chronic kidney disease screening and prognosis. *Ann Intern Med,* ***173***(6), 426-435. doi: 10.7326/M20-0529.
+
+
```

### Comparing `kfre-0.1.2/src/kfre/main.py` & `kfre-0.1.2b0/src/kfre/main.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,690 +1,690 @@
-################################################################################
-############################### Library Imports ################################
-import pandas as pd
-import numpy as np
-
-################################################################################
-
-
-class RiskPredictor:
-    """
-    A class to represent a risk predictor for chronic kidney disease (CKD).
-
-    This class implements the Tangri risk prediction model, which is based on the
-    multinational assessments described in Tangri N, Grams ME, Levey AS, et al.
-    "Multinational assessment of accuracy of equations for predicting risk of kidney
-    failure: A meta-analysis." JAMA, 315(2), 164–174, doi: 10.1001/jama.2015.18202.
-
-    This class uses the Tangri risk prediction model, which calculates risk
-    based on various patient parameters. Results are accurate for both males
-    and females, but the original paper calculated risk specifically for males.
-
-    Attributes:
-    data (DataFrame): The patient data.
-    columns (dict): Dictionary to map expected parameter names to actual column
-    names in the data.
-
-    Methods:
-    predict(years, use_extra_vars): Predicts the risk of CKD for the given
-    number of years, optionally using extra variables for the prediction.
-    """
-
-    def __init__(
-        self,
-        df=None,
-        columns=None,
-    ):
-        """
-        Constructs the necessary attributes for the RiskPredictor object.
-
-        Parameters:
-        data (DataFrame): The patient data.
-        columns (dict): A dictionary specifying the column names in the dataset
-        that correspond to the required parameters.
-        Example: {'age': 'Age', 'sex': 'Gender', 'eGFR': 'eGFR',
-        'uACR': 'Albumin_Ratio', 'region': 'Region', 'dm': 'Diabetes',
-        'htn': 'Hypertension'}
-        apply_conversions (bool, optional): Flag to apply unit conversions.
-        Default is False.
-        """
-        self.df = df
-        self.columns = columns
-
-    def predict_kfre(
-        self,
-        years,
-        is_north_american,
-        use_extra_vars=False,
-        num_vars=4,
-    ):
-        """
-        Predicts the risk of chronic kidney disease (CKD) over a specified
-        number of years using the Tangri risk prediction model. This method
-        supports the basic 4-variable model as well as the extended 6-variable
-        and 8-variable models if additional patient data is available.
-
-        Parameters:
-        - years (int): The number of years over which the risk assessment is
-          projected.
-        - is_north_american (bool): Flag indicating whether the patient is from
-          North America, which affects the model's constants.
-        - use_extra_vars (bool, optional): Determines if additional variables
-          (such as diabetes and hypertension status for the 6-variable model, or
-          biochemical markers for the 8-variable model) should be used in the
-          risk calculation. Defaults to False.
-        - num_vars (int, optional): Specifies the number of variables to use in
-          the prediction model (4, 6, or 8). Defaults to 4.
-
-        Returns:
-        - float: A probability value between 0 and 1 representing the patient's
-          risk of CKD development within the specified timeframe.
-
-        Raises:
-        - ValueError: If `num_vars` is set to an unsupported number.
-
-        Notes:
-        - The 6-variable model includes diabetes and hypertension status in
-          addition to the base parameters.
-        - The 8-variable model includes serum albumin, phosphorous, bicarbonate,
-          and calcium levels in addition to the parameters used in the
-          6-variable model.
-        - It is important to provide accurate mappings in the `columns`
-          dictionary upon class instantiation for the method to correctly locate
-          the necessary data in the DataFrame.
-        """
-        # Basic required columns
-        necessary_cols = [
-            self.columns["age"],
-            self.columns["sex"],
-            self.columns["eGFR"],
-            self.columns["uACR"],
-        ]
-
-        # Retrieve data only once
-        df = self.df[necessary_cols].copy()
-
-        # Convert sex to numeric in a vectorized way
-        df[self.columns["sex"]] = (
-            df[self.columns["sex"]].str.lower() == "male"
-        ).astype(int)
-
-        # Extract basic parameters from the DataFrame
-        age = df[self.columns["age"]]
-        sex = df[self.columns["sex"]]
-        eGFR = df[self.columns["eGFR"]]
-        uACR = df[self.columns["uACR"]]
-
-        if use_extra_vars:
-            if num_vars == 6:
-                # Extend columns for 6-variable model
-                necessary_cols.extend([self.columns["dm"], self.columns["htn"]])
-                df = self.df[necessary_cols].copy()
-                dm = df[self.columns["dm"]]
-                htn = df[self.columns["htn"]]
-                return risk_pred(
-                    age, sex, eGFR, uACR, is_north_american, dm, htn, years=years
-                )
-            elif num_vars == 8:
-                # Extend columns for 8-variable model
-                necessary_cols.extend(
-                    [
-                        self.columns["albumin"],
-                        self.columns["phosphorous"],
-                        self.columns["bicarbonate"],
-                        self.columns["calcium"],
-                    ]
-                )
-                df = self.df[necessary_cols].copy()
-                albumin = df[self.columns["albumin"]]
-                phosphorous = df[self.columns["phosphorous"]]
-                bicarbonate = df[self.columns["bicarbonate"]]
-                calcium = df[self.columns["calcium"]]
-                return risk_pred(
-                    age,
-                    sex,
-                    eGFR,
-                    uACR,
-                    is_north_american,
-                    None,
-                    None,
-                    albumin,
-                    phosphorous,
-                    bicarbonate,
-                    calcium,
-                    years=years,
-                )
-        else:
-            # Call the function with basic parameters for the 4-variable model
-            return risk_pred(age, sex, eGFR, uACR, is_north_american, years=years)
-
-    def kfre_person(
-        self,
-        age,
-        is_male,
-        eGFR,
-        uACR,
-        is_north_american,
-        years=2,
-        dm=None,
-        htn=None,
-        albumin=None,
-        phosphorous=None,
-        bicarbonate=None,
-        calcium=None,
-    ):
-        """
-        Predicts CKD risk for an individual patient based on provided clinical
-        parameters.
-
-        Parameters:
-        - age (float): Age of the patient.
-        - is_male (bool): True if the patient is male, False if female.
-        - eGFR (float): Estimated Glomerular Filtration Rate.
-        - uACR (float): Urinary Albumin to Creatinine Ratio.
-        - is_north_american (bool): True if the patient is from North America,
-          False otherwise.
-        - years (int): Time horizon for the risk prediction (default is 2 years).
-        - dm (float, optional): Diabetes mellitus indicator (1=yes; 0=no).
-        - htn (float, optional): Hypertension indicator (1=yes; 0=no).
-        - albumin (float, optional): Serum albumin level.
-        - phosphorous (float, optional): Serum phosphorous level.
-        - bicarbonate (float, optional): Serum bicarbonate level.
-        - calcium (float, optional): Serum calcium level.
-
-        Returns:
-        - float: The computed risk of developing CKD.
-        """
-        # Use is_male directly, since it's already a boolean
-        # Call the risk prediction function with the parameters
-        risk_prediction = risk_pred(
-            age=age,
-            sex=is_male,
-            eGFR=eGFR,
-            uACR=uACR,
-            is_north_american=is_north_american,
-            years=years,
-            dm=dm,
-            htn=htn,
-            albumin=albumin,
-            phosphorous=phosphorous,
-            bicarbonate=bicarbonate,
-            calcium=calcium,
-        )
-        return risk_prediction
-
-
-################################################################################
-################################ uPCR to uACR ##################################
-################################################################################
-
-
-def upcr_uacr(df, sex_col, diabetes_col, hypertension_col, upcr_col, female_str):
-    """
-    Converts urinary protein-creatinine ratio (uPCR) to urinary
-    albumin-creatinine ratio (uACR) for an entire DataFrame using vectorized
-    operations to enhance performance. This function is designed to handle large
-    datasets efficiently by applying the conversion formula across columns,
-    rather than row-by-row.
-
-    The conversion uses patient-specific factors such as sex, presence of
-    diabetes, and presence of hypertension to adjust the uACR calculation
-    according to a specified logarithmic and exponential formula. This approach
-    is critical in clinical settings where accurate adjustments based on
-    demographic factors are essential for proper diagnosis and treatment planning.
-
-    Parameters:
-    - df (pd.DataFrame): The DataFrame containing the patient data.
-    - sex_col (str): Column name in 'df' that contains the patient's gender.
-    - diabetes_col (str): Column name in 'df' that indicates whether the
-      patient has diabetes (1=yes; 0=no).
-    - hypertension_col (str): Column name in 'df' that indicates whether the
-      patient has hypertension (1=yes; 0=no).
-    - upcr_col (str): Column name in 'df' that contains the urinary
-      protein-creatinine ratio.
-    - female_str (str): The string used in the dataset to identify female patients.
-
-    Returns:
-    - pd.Series: A pandas Series object containing the computed urinary
-      albumin-creatinine ratio (uACR) for each patient in the DataFrame.
-
-    This function ensures that all calculations respect the integrity of the
-    original data by not modifying any existing columns and only adding the
-    resulting uACR as a new column. It handles NaN values by excluding them
-    from the calculation, thus retaining them in the resulting uACR values to
-    reflect the lack of information for certain patients.
-
-    Notes: Conversion from uPCR to uACR can be independently verified using the
-    calculator on `https://ckdpcrisk.org/pcr2acr/`
-
-    This function converts urine protein-creatinine ratio or urine dipstick
-    protein to urine albumin-creatinine ratio, based on the method outlined in
-    Sumida K, Nadkarni GN, Grams ME, et al. "Conversion of urine protein-creatinine
-    ratio or urine dipstick protein to urine albumin-creatinine ratio for use in
-    chronic kidney disease screening and prognosis."
-    Ann Intern Med, 173(6), 426-435, doi: 10.7326/M20-0529.
-
-    """
-    # Convert to float and get the female mask
-    upcr = df[upcr_col].astype(float)
-    female = (df[sex_col] == female_str).astype(int)
-
-    # Masks to identify valid data for diabetes and hypertension
-    diabetic_mask = ~df[diabetes_col].isna()
-    hypertensive_mask = ~df[hypertension_col].isna()
-
-    # Only calculate uACR where we have complete information
-    valid_mask = diabetic_mask & hypertensive_mask
-
-    # Initialize uACR with NaNs
-    uacr = np.full(df.shape[0], np.nan)
-
-    # Calculate uACR only for valid data
-    uacr[valid_mask] = np.exp(
-        5.2659
-        + 0.2934 * np.log(np.minimum(upcr[valid_mask] / 50, 1))
-        + 1.5643 * np.log(np.maximum(np.minimum(upcr[valid_mask] / 500, 1), 0.1))
-        + 1.1109 * np.log(np.maximum(upcr[valid_mask] / 500, 1))
-        - 0.0773 * female[valid_mask]
-        + 0.0797 * df[diabetes_col][valid_mask].astype(int)
-        + 0.1265 * df[hypertension_col][valid_mask].astype(int)
-    )
-
-    return pd.Series(uacr, index=df.index)
-
-
-################################################################################
-#################################  Wrappers  ###################################
-################################################################################
-
-
-# convenience function as wrapper for method with the same name
-def predict_kfre(
-    df, columns, years, is_north_american, use_extra_vars=False, num_vars=4
-):
-    """
-    A convenience function to predict CKD risk using the Tangri risk prediction
-    model without directly creating an instance of the RiskPredictor class.
-
-    Parameters:
-    - df (DataFrame): The DataFrame containing patient data.
-    - columns (dict): Maps clinical parameter names to DataFrame column names.
-    - years (int): Number of years for the risk prediction.
-    - is_north_american (bool): True if the data is from North America.
-    - use_extra_vars (bool): If True, use additional clinical variables for the
-      prediction.
-    - num_vars (int): Number of variables used in the model (4, 6, or 8).
-
-    Returns:
-    - Series: CKD risk probabilities for each patient.
-    """
-
-    predictor = RiskPredictor(df=df, columns=columns)
-    return predictor.predict_kfre(
-        years=years,
-        is_north_american=is_north_american,
-        use_extra_vars=use_extra_vars,
-        num_vars=num_vars,
-    )
-
-
-def add_kfre_risk_col(
-    df,
-    age_col=None,
-    sex_col=None,
-    eGFR_col=None,
-    uACR_col=None,
-    dm_col=None,
-    htn_col=None,
-    albumin_col=None,
-    phosphorous_col=None,
-    bicarbonate_col=None,
-    calcium_col=None,
-    num_vars=8,
-    years=(2, 5),
-    is_north_american=False,
-    copy=True,
-):
-    """
-    Calculate CKD risks for specified variable num_vars and time frames or for
-    all num_vars and years, grouping the results by model first and then by time
-    frame in the output DataFrame. Optionally creates a copy of the DataFrame to
-    avoid modifying the original data.
-
-    Parameters:
-    - df (DataFrame): The patient data.
-    - age_col, sex_col, ..., calcium_col (str): Column names for the patient
-      parameters.
-    - num_vars (int or list): Specifies the number of variables to use (4, 6, 8).
-    - years (tuple or list): Time frames to calculate risk for.
-    - is_north_american (bool): True if the calculation is for the North
-      American region.
-    - copy (bool): If True, operates on a copy of the DataFrame. If False,
-      modifies the DataFrame in place.
-
-    Returns:
-    - DataFrame: The modified or new DataFrame with added risk prediction columns.
-    """
-    # Use a copy if requested for safety
-    df_used = df.copy() if copy else df
-
-    column_map = {
-        "age": age_col,
-        "sex": sex_col,
-        "eGFR": eGFR_col,
-        "uACR": uACR_col,
-        "dm": dm_col,
-        "htn": htn_col,
-        "albumin": albumin_col,
-        "phosphorous": phosphorous_col,
-        "bicarbonate": bicarbonate_col,
-        "calcium": calcium_col,
-    }
-
-    model_requirements = {
-        4: ["age", "sex", "eGFR", "uACR"],
-        6: ["age", "sex", "eGFR", "uACR", "dm", "htn"],
-        8: [
-            "age",
-            "sex",
-            "eGFR",
-            "uACR",
-            "albumin",
-            "phosphorous",
-            "bicarbonate",
-            "calcium",
-        ],
-    }
-
-    # Adjust 'num_vars' and 'years' handling to accept 'all', integer, or iterable
-    num_vars = (
-        [4, 6, 8]
-        if num_vars == "all"
-        else ([num_vars] if isinstance(num_vars, int) else num_vars)
-    )
-    years = (
-        [2, 5]
-        if years == "all"
-        else ([years] if isinstance(years, int) else list(years))
-    )
-
-    for model in num_vars:
-        missing = [req for req in model_requirements[model] if column_map[req] is None]
-        if missing:
-            required_cols = ", ".join(missing)
-            raise ValueError(
-                f"{required_cols} needed to complete calculation for {model}var model"
-            )
-
-    # Initialize the predictor with the data and columns
-    predictor = RiskPredictor(
-        df_used, {k: v for k, v in column_map.items() if v is not None}
-    )
-
-    # Calculate risks for each model and time frame
-    for model_vars in num_vars:
-        if all(column_map[req] is not None for req in model_requirements[model_vars]):
-            for time_frame in years:
-                risk_column = f"kfre_{model_vars}var_{time_frame}year"
-                df_used[risk_column] = predictor.predict_kfre(
-                    years=time_frame,
-                    is_north_american=is_north_american,
-                    use_extra_vars=(model_vars > 4),
-                    num_vars=model_vars,
-                )
-
-    return df_used
-
-
-def perform_conversions(
-    df,
-    reverse=False,
-    convert_all=False,
-    upcr_col=None,
-    calcium_col=None,
-    phosphate_col=None,
-    albumin_col=None,
-):
-    """
-    Convert specified units of columns in a dataframe and create new columns
-    for the results, with specific suffixes based on the conversion direction.
-    Original columns are preserved.
-
-    Parameters:
-    - df (DataFrame): The dataframe containing the data.
-    - reverse (bool): If True, revert to original units by dividing; if False,
-      perform the standard conversion by multiplying.
-    - convert_all (bool): If True, automatically convert all recognized columns.
-    - upcr_col (str, optional): Column name for urine protein-creatinine ratio.
-    - calcium_col (str, optional): Column name for calcium.
-    - phosphate_col (str, optional): Column name for phosphate.
-    - albumin_col (str, optional): Column name for albumin.
-    """
-    # Define the conversion factors and the suffixes for the converted units
-    conversion_factors = {
-        "uPCR": 1 / 0.11312,  # From mg/g to mmol/L
-        "Calcium": 4,  # From mg/dL to mmol/L
-        "Phosphate": 3.1,  # From mg/dL to mmol/L
-        "Albumin": 1 / 10,  # From g/dL to g/L
-    }
-
-    # Define the suffixes for new column names based on conversion direction
-    conversion_suffix = {
-        "uPCR": "mg_g" if not reverse else "mmol_L",
-        "Calcium": "mg_dl" if not reverse else "mmol_L",
-        "Phosphate": "mg_dl" if not reverse else "mmol_L",
-        "Albumin": "g_dl" if not reverse else "g_L",
-    }
-
-    # Initialize columns_to_convert with provided column names or defaults
-    columns_to_convert = {
-        "uPCR": upcr_col,
-        "Calcium": calcium_col,
-        "Phosphate": phosphate_col,
-        "Albumin": albumin_col,
-    }
-
-    # If convert_all is True, automatically identify columns for conversion
-    if convert_all:
-        columns_to_convert = {
-            key: next((col for col in df.columns if key.lower() in col.lower()), None)
-            for key in conversion_factors
-        }
-
-    # Perform conversions
-    for key, orig_col in columns_to_convert.items():
-        if orig_col and orig_col in df.columns:
-            factor = conversion_factors[key]
-            suffix = conversion_suffix[key]
-            # Calculate the converted values
-            converted_values = (
-                df[orig_col] / factor if reverse else df[orig_col] * factor
-            )
-            # Create the new column name
-            new_col = f"{key}_{suffix}"
-            # Add the converted values as a new column to the dataframe
-            df[new_col] = converted_values
-            print(
-                f"Converted '{orig_col}' to new column '{new_col}' with factor {factor}"
-            )
-        else:
-            print(
-                f"Warning: Column '{orig_col}' not found in DataFrame. "
-                f"No conversion performed for this column."
-            )
-
-    return df
-
-
-################################################################################
-############################## KFRE Risk Predictor #############################
-################################################################################
-
-
-def risk_pred(
-    age,
-    sex,
-    eGFR,
-    uACR,
-    is_north_american,
-    dm=None,
-    htn=None,
-    albumin=None,
-    phosphorous=None,
-    bicarbonate=None,
-    calcium=None,
-    years=2,
-):
-    """
-    Calculates the risk of chronic kidney disease progression based on a range
-    of clinical parameters using the Tangri risk prediction model. This model
-    can use 4, 6, or 8 variables for prediction based on the data available.
-    The coefficients and constants used in the calculations are selected based
-    on the geographic region of the patient (North American or not) and the time
-    horizon for the risk prediction (2 or 5 years).
-
-    Parameters:
-    - age (float): Age of the patient in years.
-    - sex (int): Biological sex of the patient (0 for female, 1 for male).
-    - eGFR (float): Estimated Glomerular Filtration Rate, indicating kidney
-      function.
-    - uACR (float): Urinary Albumin to Creatinine Ratio, showing kidney damage
-      level.
-    - is_north_american (bool): Indicates if the patient is from North America.
-    - dm (float, optional): Indicates if the patient has diabetes (0 or 1).
-    - htn (float, optional): Indicates if the patient has hypertension (0 or 1).
-    - albumin (float, optional): Serum albumin level, required for the
-      8-variable model.
-    - phosphorous (float, optional): Serum phosphorous level, required for the
-      8-variable model.
-    - bicarbonate (float, optional): Serum bicarbonate level, required for the
-      8-variable model.
-    - calcium (float, optional): Serum calcium level, required for the
-      8-variable model.
-    - years (int, default=2): The number of years over which the risk is
-      redicted (2 or 5 years).
-
-    Returns:
-    - risk_prediction (float): A probability value between 0 and 1 representing
-      the patient's risk of developing chronic kidney disease within the
-      specified number of years.
-
-    Notes:
-    The function accounts for the patient's geographic location by adjusting the
-    alpha constants in the risk calculation. It defaults to coefficients for the
-    4-variable model unless additional parameters are provided, in which case it
-    switches to the 6-variable or 8-variable models.
-    """
-
-    # Define the alpha values and risk factor coefficients for each model
-    if dm is not None and htn is not None:
-        # 6-variable model
-        alpha_values = {
-            (True, 2): 0.9750,
-            (True, 5): 0.9240,
-            (False, 2): 0.9830,
-            (False, 5): 0.9370,
-        }
-        risk_factors = {
-            "age": -0.2218,  # Adjusted for 6-var model
-            "sex": 0.2553,  # Adjusted for 6-var model
-            "eGFR": -0.5541,  # Adjusted for 6-var model
-            "uACR": 0.4562,  # Adjusted for 6-var model
-        }
-        dm_factor = -0.1475  # DM risk factor coefficient
-        htn_factor = 0.1426  # HTN risk factor coefficient
-    elif (
-        albumin is not None
-        and phosphorous is not None
-        and bicarbonate is not None
-        and calcium is not None
-    ):
-        # 8-variable model
-        alpha_values = {
-            (True, 2): 0.9780,
-            (True, 5): 0.9301,
-            (False, 2): 0.9827,
-            (False, 5): 0.9245,
-        }
-        risk_factors = {
-            "age": -0.1992,  # Adjusted for 8-var model
-            "sex": 0.1602,  # Adjusted for 8-var model
-            "eGFR": -0.4919,  # Adjusted for 8-var model
-            "uACR": 0.3364,  # Adjusted for 8-var model
-        }
-        # Extra risk factors for the 8-variable model
-        albumin_factor = -0.3441
-        phosph_factor = +0.2604
-        bicarb_factor = -0.07354
-        calcium_factor = -0.2228
-    else:
-        # 4-variable model
-        alpha_values = {
-            (True, 2): 0.9750,
-            (True, 5): 0.9240,
-            (False, 2): 0.9832,
-            (False, 5): 0.9365,
-        }
-        risk_factors = {
-            "age": -0.2201,
-            "sex": 0.2467,
-            "eGFR": -0.5567,
-            "uACR": 0.4510,
-        }
-
-    # Ensure uACR is positive to avoid log(0)
-    uACR = np.maximum(uACR, 1e-6)
-    log_uACR = np.log(uACR)
-
-    # Compute the base risk score using the coefficients
-    risk_score = (
-        risk_factors["age"] * (age / 10 - 7.036)
-        + risk_factors["sex"] * (sex - 0.5642)
-        + risk_factors["eGFR"] * (eGFR / 5 - 7.222)
-        + risk_factors["uACR"] * (log_uACR - 5.137)
-    )
-
-    # Adjust risk score for the 6-variable model if DM and HTN data is provided
-    if dm is not None and htn is not None:
-        risk_score += dm_factor * (dm - 0.5106) + htn_factor * (htn - 0.8501)
-
-    # Adjust risk score for the 8-variable model if additional data is provided
-    if (
-        albumin is not None
-        and phosphorous is not None
-        and bicarbonate is not None
-        and calcium is not None
-    ):
-        risk_score += (
-            albumin_factor * (albumin - 3.997)
-            + phosph_factor * (phosphorous - 3.916)
-            + bicarb_factor * (bicarbonate - 25.57)
-            + calcium_factor * (calcium - 9.355)
-        )
-
-    # Select alpha based on region and years
-    alpha = alpha_values[(is_north_american, years)]
-
-    # Compute the risk prediction
-    risk_prediction = 1 - alpha ** np.exp(risk_score)
-    return risk_prediction
-
-
-################################################################################
-# References
-# ------------------------------------------------------------------------------
-#
-# Tangri N, Grams ME, Levey AS, Coresh J, et al. (2016). Multinational assessment
-# of accuracy of equations for predicting risk of kidney failure: A meta-analysis.
-# JAMA, 315(2), 164–174. doi: 10.1001/jama.2015.18202.
-#
-# Tangri, N., Stevens, L. A., Griffith, J., Tighiouart, H., Djurdjev, O.,
-# Naimark, D., Levin, A., & Levey, A. S. (2011). A predictive model for
-# progression of chronic kidney disease to kidney failure. JAMA, 305(15),
-# 1553-1559. doi: 10.1001/jama.2011.451.
-#
-# Sumida K, Nadkarni GN, Grams ME, Sang Y, et al. (2020). Conversion of urine
-# protein-creatinine ratio or urine dipstick protein to urine albumin-creatinine
-# ratio for use in chronic kidney disease screening and prognosis. Ann Intern Med,
-# 173(6), 426-435. doi: 10.7326/M20-0529.
-# ------------------------------------------------------------------------------
-################################################################################
+################################################################################
+############################### Library Imports ################################
+import pandas as pd
+import numpy as np
+
+################################################################################
+
+
+class RiskPredictor:
+    """
+    A class to represent a risk predictor for chronic kidney disease (CKD).
+
+    This class implements the Tangri risk prediction model, which is based on the
+    multinational assessments described in Tangri N, Grams ME, Levey AS, et al.
+    "Multinational assessment of accuracy of equations for predicting risk of kidney
+    failure: A meta-analysis." JAMA, 315(2), 164–174, doi: 10.1001/jama.2015.18202.
+
+    This class uses the Tangri risk prediction model, which calculates risk
+    based on various patient parameters. Results are accurate for both males
+    and females, but the original paper calculated risk specifically for males.
+
+    Attributes:
+    data (DataFrame): The patient data.
+    columns (dict): Dictionary to map expected parameter names to actual column
+    names in the data.
+
+    Methods:
+    predict(years, use_extra_vars): Predicts the risk of CKD for the given
+    number of years, optionally using extra variables for the prediction.
+    """
+
+    def __init__(
+        self,
+        df=None,
+        columns=None,
+    ):
+        """
+        Constructs the necessary attributes for the RiskPredictor object.
+
+        Parameters:
+        data (DataFrame): The patient data.
+        columns (dict): A dictionary specifying the column names in the dataset
+        that correspond to the required parameters.
+        Example: {'age': 'Age', 'sex': 'Gender', 'eGFR': 'eGFR',
+        'uACR': 'Albumin_Ratio', 'region': 'Region', 'dm': 'Diabetes',
+        'htn': 'Hypertension'}
+        apply_conversions (bool, optional): Flag to apply unit conversions.
+        Default is False.
+        """
+        self.df = df
+        self.columns = columns
+
+    def predict_kfre(
+        self,
+        years,
+        is_north_american,
+        use_extra_vars=False,
+        num_vars=4,
+    ):
+        """
+        Predicts the risk of chronic kidney disease (CKD) over a specified
+        number of years using the Tangri risk prediction model. This method
+        supports the basic 4-variable model as well as the extended 6-variable
+        and 8-variable models if additional patient data is available.
+
+        Parameters:
+        - years (int): The number of years over which the risk assessment is
+          projected.
+        - is_north_american (bool): Flag indicating whether the patient is from
+          North America, which affects the model's constants.
+        - use_extra_vars (bool, optional): Determines if additional variables
+          (such as diabetes and hypertension status for the 6-variable model, or
+          biochemical markers for the 8-variable model) should be used in the
+          risk calculation. Defaults to False.
+        - num_vars (int, optional): Specifies the number of variables to use in
+          the prediction model (4, 6, or 8). Defaults to 4.
+
+        Returns:
+        - float: A probability value between 0 and 1 representing the patient's
+          risk of CKD development within the specified timeframe.
+
+        Raises:
+        - ValueError: If `num_vars` is set to an unsupported number.
+
+        Notes:
+        - The 6-variable model includes diabetes and hypertension status in
+          addition to the base parameters.
+        - The 8-variable model includes serum albumin, phosphorous, bicarbonate,
+          and calcium levels in addition to the parameters used in the
+          6-variable model.
+        - It is important to provide accurate mappings in the `columns`
+          dictionary upon class instantiation for the method to correctly locate
+          the necessary data in the DataFrame.
+        """
+        # Basic required columns
+        necessary_cols = [
+            self.columns["age"],
+            self.columns["sex"],
+            self.columns["eGFR"],
+            self.columns["uACR"],
+        ]
+
+        # Retrieve data only once
+        df = self.df[necessary_cols].copy()
+
+        # Convert sex to numeric in a vectorized way
+        df[self.columns["sex"]] = (
+            df[self.columns["sex"]].str.lower() == "male"
+        ).astype(int)
+
+        # Extract basic parameters from the DataFrame
+        age = df[self.columns["age"]]
+        sex = df[self.columns["sex"]]
+        eGFR = df[self.columns["eGFR"]]
+        uACR = df[self.columns["uACR"]]
+
+        if use_extra_vars:
+            if num_vars == 6:
+                # Extend columns for 6-variable model
+                necessary_cols.extend([self.columns["dm"], self.columns["htn"]])
+                df = self.df[necessary_cols].copy()
+                dm = df[self.columns["dm"]]
+                htn = df[self.columns["htn"]]
+                return risk_pred(
+                    age, sex, eGFR, uACR, is_north_american, dm, htn, years=years
+                )
+            elif num_vars == 8:
+                # Extend columns for 8-variable model
+                necessary_cols.extend(
+                    [
+                        self.columns["albumin"],
+                        self.columns["phosphorous"],
+                        self.columns["bicarbonate"],
+                        self.columns["calcium"],
+                    ]
+                )
+                df = self.df[necessary_cols].copy()
+                albumin = df[self.columns["albumin"]]
+                phosphorous = df[self.columns["phosphorous"]]
+                bicarbonate = df[self.columns["bicarbonate"]]
+                calcium = df[self.columns["calcium"]]
+                return risk_pred(
+                    age,
+                    sex,
+                    eGFR,
+                    uACR,
+                    is_north_american,
+                    None,
+                    None,
+                    albumin,
+                    phosphorous,
+                    bicarbonate,
+                    calcium,
+                    years=years,
+                )
+        else:
+            # Call the function with basic parameters for the 4-variable model
+            return risk_pred(age, sex, eGFR, uACR, is_north_american, years=years)
+
+    def kfre_person(
+        self,
+        age,
+        is_male,
+        eGFR,
+        uACR,
+        is_north_american,
+        years=2,
+        dm=None,
+        htn=None,
+        albumin=None,
+        phosphorous=None,
+        bicarbonate=None,
+        calcium=None,
+    ):
+        """
+        Predicts CKD risk for an individual patient based on provided clinical
+        parameters.
+
+        Parameters:
+        - age (float): Age of the patient.
+        - is_male (bool): True if the patient is male, False if female.
+        - eGFR (float): Estimated Glomerular Filtration Rate.
+        - uACR (float): Urinary Albumin to Creatinine Ratio.
+        - is_north_american (bool): True if the patient is from North America,
+          False otherwise.
+        - years (int): Time horizon for the risk prediction (default is 2 years).
+        - dm (float, optional): Diabetes mellitus indicator (1=yes; 0=no).
+        - htn (float, optional): Hypertension indicator (1=yes; 0=no).
+        - albumin (float, optional): Serum albumin level.
+        - phosphorous (float, optional): Serum phosphorous level.
+        - bicarbonate (float, optional): Serum bicarbonate level.
+        - calcium (float, optional): Serum calcium level.
+
+        Returns:
+        - float: The computed risk of developing CKD.
+        """
+        # Use is_male directly, since it's already a boolean
+        # Call the risk prediction function with the parameters
+        risk_prediction = risk_pred(
+            age=age,
+            sex=is_male,
+            eGFR=eGFR,
+            uACR=uACR,
+            is_north_american=is_north_american,
+            years=years,
+            dm=dm,
+            htn=htn,
+            albumin=albumin,
+            phosphorous=phosphorous,
+            bicarbonate=bicarbonate,
+            calcium=calcium,
+        )
+        return risk_prediction
+
+
+################################################################################
+################################ uPCR to uACR ##################################
+################################################################################
+
+
+def upcr_uacr(df, sex_col, diabetes_col, hypertension_col, upcr_col, female_str):
+    """
+    Converts urinary protein-creatinine ratio (uPCR) to urinary
+    albumin-creatinine ratio (uACR) for an entire DataFrame using vectorized
+    operations to enhance performance. This function is designed to handle large
+    datasets efficiently by applying the conversion formula across columns,
+    rather than row-by-row.
+
+    The conversion uses patient-specific factors such as sex, presence of
+    diabetes, and presence of hypertension to adjust the uACR calculation
+    according to a specified logarithmic and exponential formula. This approach
+    is critical in clinical settings where accurate adjustments based on
+    demographic factors are essential for proper diagnosis and treatment planning.
+
+    Parameters:
+    - df (pd.DataFrame): The DataFrame containing the patient data.
+    - sex_col (str): Column name in 'df' that contains the patient's gender.
+    - diabetes_col (str): Column name in 'df' that indicates whether the
+      patient has diabetes (1=yes; 0=no).
+    - hypertension_col (str): Column name in 'df' that indicates whether the
+      patient has hypertension (1=yes; 0=no).
+    - upcr_col (str): Column name in 'df' that contains the urinary
+      protein-creatinine ratio.
+    - female_str (str): The string used in the dataset to identify female patients.
+
+    Returns:
+    - pd.Series: A pandas Series object containing the computed urinary
+      albumin-creatinine ratio (uACR) for each patient in the DataFrame.
+
+    This function ensures that all calculations respect the integrity of the
+    original data by not modifying any existing columns and only adding the
+    resulting uACR as a new column. It handles NaN values by excluding them
+    from the calculation, thus retaining them in the resulting uACR values to
+    reflect the lack of information for certain patients.
+
+    Notes: Conversion from uPCR to uACR can be independently verified using the
+    calculator on `https://ckdpcrisk.org/pcr2acr/`
+
+    This function converts urine protein-creatinine ratio or urine dipstick
+    protein to urine albumin-creatinine ratio, based on the method outlined in
+    Sumida K, Nadkarni GN, Grams ME, et al. "Conversion of urine protein-creatinine
+    ratio or urine dipstick protein to urine albumin-creatinine ratio for use in
+    chronic kidney disease screening and prognosis."
+    Ann Intern Med, 173(6), 426-435, doi: 10.7326/M20-0529.
+
+    """
+    # Convert to float and get the female mask
+    upcr = df[upcr_col].astype(float)
+    female = (df[sex_col] == female_str).astype(int)
+
+    # Masks to identify valid data for diabetes and hypertension
+    diabetic_mask = ~df[diabetes_col].isna()
+    hypertensive_mask = ~df[hypertension_col].isna()
+
+    # Only calculate uACR where we have complete information
+    valid_mask = diabetic_mask & hypertensive_mask
+
+    # Initialize uACR with NaNs
+    uacr = np.full(df.shape[0], np.nan)
+
+    # Calculate uACR only for valid data
+    uacr[valid_mask] = np.exp(
+        5.2659
+        + 0.2934 * np.log(np.minimum(upcr[valid_mask] / 50, 1))
+        + 1.5643 * np.log(np.maximum(np.minimum(upcr[valid_mask] / 500, 1), 0.1))
+        + 1.1109 * np.log(np.maximum(upcr[valid_mask] / 500, 1))
+        - 0.0773 * female[valid_mask]
+        + 0.0797 * df[diabetes_col][valid_mask].astype(int)
+        + 0.1265 * df[hypertension_col][valid_mask].astype(int)
+    )
+
+    return pd.Series(uacr, index=df.index)
+
+
+################################################################################
+#################################  Wrappers  ###################################
+################################################################################
+
+
+# convenience function as wrapper for method with the same name
+def predict_kfre(
+    df, columns, years, is_north_american, use_extra_vars=False, num_vars=4
+):
+    """
+    A convenience function to predict CKD risk using the Tangri risk prediction
+    model without directly creating an instance of the RiskPredictor class.
+
+    Parameters:
+    - df (DataFrame): The DataFrame containing patient data.
+    - columns (dict): Maps clinical parameter names to DataFrame column names.
+    - years (int): Number of years for the risk prediction.
+    - is_north_american (bool): True if the data is from North America.
+    - use_extra_vars (bool): If True, use additional clinical variables for the
+      prediction.
+    - num_vars (int): Number of variables used in the model (4, 6, or 8).
+
+    Returns:
+    - Series: CKD risk probabilities for each patient.
+    """
+
+    predictor = RiskPredictor(df=df, columns=columns)
+    return predictor.predict_kfre(
+        years=years,
+        is_north_american=is_north_american,
+        use_extra_vars=use_extra_vars,
+        num_vars=num_vars,
+    )
+
+
+def add_kfre_risk_col(
+    df,
+    age_col=None,
+    sex_col=None,
+    eGFR_col=None,
+    uACR_col=None,
+    dm_col=None,
+    htn_col=None,
+    albumin_col=None,
+    phosphorous_col=None,
+    bicarbonate_col=None,
+    calcium_col=None,
+    num_vars=8,
+    years=(2, 5),
+    is_north_american=False,
+    copy=True,
+):
+    """
+    Calculate CKD risks for specified variable num_vars and time frames or for
+    all num_vars and years, grouping the results by model first and then by time
+    frame in the output DataFrame. Optionally creates a copy of the DataFrame to
+    avoid modifying the original data.
+
+    Parameters:
+    - df (DataFrame): The patient data.
+    - age_col, sex_col, ..., calcium_col (str): Column names for the patient
+      parameters.
+    - num_vars (int or list): Specifies the number of variables to use (4, 6, 8).
+    - years (tuple or list): Time frames to calculate risk for.
+    - is_north_american (bool): True if the calculation is for the North
+      American region.
+    - copy (bool): If True, operates on a copy of the DataFrame. If False,
+      modifies the DataFrame in place.
+
+    Returns:
+    - DataFrame: The modified or new DataFrame with added risk prediction columns.
+    """
+    # Use a copy if requested for safety
+    df_used = df.copy() if copy else df
+
+    column_map = {
+        "age": age_col,
+        "sex": sex_col,
+        "eGFR": eGFR_col,
+        "uACR": uACR_col,
+        "dm": dm_col,
+        "htn": htn_col,
+        "albumin": albumin_col,
+        "phosphorous": phosphorous_col,
+        "bicarbonate": bicarbonate_col,
+        "calcium": calcium_col,
+    }
+
+    model_requirements = {
+        4: ["age", "sex", "eGFR", "uACR"],
+        6: ["age", "sex", "eGFR", "uACR", "dm", "htn"],
+        8: [
+            "age",
+            "sex",
+            "eGFR",
+            "uACR",
+            "albumin",
+            "phosphorous",
+            "bicarbonate",
+            "calcium",
+        ],
+    }
+
+    # Adjust 'num_vars' and 'years' handling to accept 'all', integer, or iterable
+    num_vars = (
+        [4, 6, 8]
+        if num_vars == "all"
+        else ([num_vars] if isinstance(num_vars, int) else num_vars)
+    )
+    years = (
+        [2, 5]
+        if years == "all"
+        else ([years] if isinstance(years, int) else list(years))
+    )
+
+    for model in num_vars:
+        missing = [req for req in model_requirements[model] if column_map[req] is None]
+        if missing:
+            required_cols = ", ".join(missing)
+            raise ValueError(
+                f"{required_cols} needed to complete calculation for {model}var model"
+            )
+
+    # Initialize the predictor with the data and columns
+    predictor = RiskPredictor(
+        df_used, {k: v for k, v in column_map.items() if v is not None}
+    )
+
+    # Calculate risks for each model and time frame
+    for model_vars in num_vars:
+        if all(column_map[req] is not None for req in model_requirements[model_vars]):
+            for time_frame in years:
+                risk_column = f"kfre_{model_vars}var_{time_frame}year"
+                df_used[risk_column] = predictor.predict_kfre(
+                    years=time_frame,
+                    is_north_american=is_north_american,
+                    use_extra_vars=(model_vars > 4),
+                    num_vars=model_vars,
+                )
+
+    return df_used
+
+
+def perform_conversions(
+    df,
+    reverse=False,
+    convert_all=False,
+    upcr_col=None,
+    calcium_col=None,
+    phosphate_col=None,
+    albumin_col=None,
+):
+    """
+    Convert specified units of columns in a dataframe and create new columns
+    for the results, with specific suffixes based on the conversion direction.
+    Original columns are preserved.
+
+    Parameters:
+    - df (DataFrame): The dataframe containing the data.
+    - reverse (bool): If True, revert to original units by dividing; if False,
+      perform the standard conversion by multiplying.
+    - convert_all (bool): If True, automatically convert all recognized columns.
+    - upcr_col (str, optional): Column name for urine protein-creatinine ratio.
+    - calcium_col (str, optional): Column name for calcium.
+    - phosphate_col (str, optional): Column name for phosphate.
+    - albumin_col (str, optional): Column name for albumin.
+    """
+    # Define the conversion factors and the suffixes for the converted units
+    conversion_factors = {
+        "uPCR": 1 / 0.11312,  # From mg/g to mmol/L
+        "Calcium": 4,  # From mg/dL to mmol/L
+        "Phosphate": 3.1,  # From mg/dL to mmol/L
+        "Albumin": 1 / 10,  # From g/dL to g/L
+    }
+
+    # Define the suffixes for new column names based on conversion direction
+    conversion_suffix = {
+        "uPCR": "mg_g" if not reverse else "mmol_L",
+        "Calcium": "mg_dl" if not reverse else "mmol_L",
+        "Phosphate": "mg_dl" if not reverse else "mmol_L",
+        "Albumin": "g_dl" if not reverse else "g_L",
+    }
+
+    # Initialize columns_to_convert with provided column names or defaults
+    columns_to_convert = {
+        "uPCR": upcr_col,
+        "Calcium": calcium_col,
+        "Phosphate": phosphate_col,
+        "Albumin": albumin_col,
+    }
+
+    # If convert_all is True, automatically identify columns for conversion
+    if convert_all:
+        columns_to_convert = {
+            key: next((col for col in df.columns if key.lower() in col.lower()), None)
+            for key in conversion_factors
+        }
+
+    # Perform conversions
+    for key, orig_col in columns_to_convert.items():
+        if orig_col and orig_col in df.columns:
+            factor = conversion_factors[key]
+            suffix = conversion_suffix[key]
+            # Calculate the converted values
+            converted_values = (
+                df[orig_col] / factor if reverse else df[orig_col] * factor
+            )
+            # Create the new column name
+            new_col = f"{key}_{suffix}"
+            # Add the converted values as a new column to the dataframe
+            df[new_col] = converted_values
+            print(
+                f"Converted '{orig_col}' to new column '{new_col}' with factor {factor}"
+            )
+        else:
+            print(
+                f"Warning: Column '{orig_col}' not found in DataFrame. "
+                f"No conversion performed for this column."
+            )
+
+    return df
+
+
+################################################################################
+############################## KFRE Risk Predictor #############################
+################################################################################
+
+
+def risk_pred(
+    age,
+    sex,
+    eGFR,
+    uACR,
+    is_north_american,
+    dm=None,
+    htn=None,
+    albumin=None,
+    phosphorous=None,
+    bicarbonate=None,
+    calcium=None,
+    years=2,
+):
+    """
+    Calculates the risk of chronic kidney disease progression based on a range
+    of clinical parameters using the Tangri risk prediction model. This model
+    can use 4, 6, or 8 variables for prediction based on the data available.
+    The coefficients and constants used in the calculations are selected based
+    on the geographic region of the patient (North American or not) and the time
+    horizon for the risk prediction (2 or 5 years).
+
+    Parameters:
+    - age (float): Age of the patient in years.
+    - sex (int): Biological sex of the patient (0 for female, 1 for male).
+    - eGFR (float): Estimated Glomerular Filtration Rate, indicating kidney
+      function.
+    - uACR (float): Urinary Albumin to Creatinine Ratio, showing kidney damage
+      level.
+    - is_north_american (bool): Indicates if the patient is from North America.
+    - dm (float, optional): Indicates if the patient has diabetes (0 or 1).
+    - htn (float, optional): Indicates if the patient has hypertension (0 or 1).
+    - albumin (float, optional): Serum albumin level, required for the
+      8-variable model.
+    - phosphorous (float, optional): Serum phosphorous level, required for the
+      8-variable model.
+    - bicarbonate (float, optional): Serum bicarbonate level, required for the
+      8-variable model.
+    - calcium (float, optional): Serum calcium level, required for the
+      8-variable model.
+    - years (int, default=2): The number of years over which the risk is
+      redicted (2 or 5 years).
+
+    Returns:
+    - risk_prediction (float): A probability value between 0 and 1 representing
+      the patient's risk of developing chronic kidney disease within the
+      specified number of years.
+
+    Notes:
+    The function accounts for the patient's geographic location by adjusting the
+    alpha constants in the risk calculation. It defaults to coefficients for the
+    4-variable model unless additional parameters are provided, in which case it
+    switches to the 6-variable or 8-variable models.
+    """
+
+    # Define the alpha values and risk factor coefficients for each model
+    if dm is not None and htn is not None:
+        # 6-variable model
+        alpha_values = {
+            (True, 2): 0.9750,
+            (True, 5): 0.9240,
+            (False, 2): 0.9830,
+            (False, 5): 0.9370,
+        }
+        risk_factors = {
+            "age": -0.2218,  # Adjusted for 6-var model
+            "sex": 0.2553,  # Adjusted for 6-var model
+            "eGFR": -0.5541,  # Adjusted for 6-var model
+            "uACR": 0.4562,  # Adjusted for 6-var model
+        }
+        dm_factor = -0.1475  # DM risk factor coefficient
+        htn_factor = 0.1426  # HTN risk factor coefficient
+    elif (
+        albumin is not None
+        and phosphorous is not None
+        and bicarbonate is not None
+        and calcium is not None
+    ):
+        # 8-variable model
+        alpha_values = {
+            (True, 2): 0.9780,
+            (True, 5): 0.9301,
+            (False, 2): 0.9827,
+            (False, 5): 0.9245,
+        }
+        risk_factors = {
+            "age": -0.1992,  # Adjusted for 8-var model
+            "sex": 0.1602,  # Adjusted for 8-var model
+            "eGFR": -0.4919,  # Adjusted for 8-var model
+            "uACR": 0.3364,  # Adjusted for 8-var model
+        }
+        # Extra risk factors for the 8-variable model
+        albumin_factor = -0.3441
+        phosph_factor = +0.2604
+        bicarb_factor = -0.07354
+        calcium_factor = -0.2228
+    else:
+        # 4-variable model
+        alpha_values = {
+            (True, 2): 0.9750,
+            (True, 5): 0.9240,
+            (False, 2): 0.9832,
+            (False, 5): 0.9365,
+        }
+        risk_factors = {
+            "age": -0.2201,
+            "sex": 0.2467,
+            "eGFR": -0.5567,
+            "uACR": 0.4510,
+        }
+
+    # Ensure uACR is positive to avoid log(0)
+    uACR = np.maximum(uACR, 1e-6)
+    log_uACR = np.log(uACR)
+
+    # Compute the base risk score using the coefficients
+    risk_score = (
+        risk_factors["age"] * (age / 10 - 7.036)
+        + risk_factors["sex"] * (sex - 0.5642)
+        + risk_factors["eGFR"] * (eGFR / 5 - 7.222)
+        + risk_factors["uACR"] * (log_uACR - 5.137)
+    )
+
+    # Adjust risk score for the 6-variable model if DM and HTN data is provided
+    if dm is not None and htn is not None:
+        risk_score += dm_factor * (dm - 0.5106) + htn_factor * (htn - 0.8501)
+
+    # Adjust risk score for the 8-variable model if additional data is provided
+    if (
+        albumin is not None
+        and phosphorous is not None
+        and bicarbonate is not None
+        and calcium is not None
+    ):
+        risk_score += (
+            albumin_factor * (albumin - 3.997)
+            + phosph_factor * (phosphorous - 3.916)
+            + bicarb_factor * (bicarbonate - 25.57)
+            + calcium_factor * (calcium - 9.355)
+        )
+
+    # Select alpha based on region and years
+    alpha = alpha_values[(is_north_american, years)]
+
+    # Compute the risk prediction
+    risk_prediction = 1 - alpha ** np.exp(risk_score)
+    return risk_prediction
+
+
+################################################################################
+# References
+# ------------------------------------------------------------------------------
+#
+# Tangri N, Grams ME, Levey AS, Coresh J, et al. (2016). Multinational assessment
+# of accuracy of equations for predicting risk of kidney failure: A meta-analysis.
+# JAMA, 315(2), 164–174. doi: 10.1001/jama.2015.18202.
+#
+# Tangri, N., Stevens, L. A., Griffith, J., Tighiouart, H., Djurdjev, O.,
+# Naimark, D., Levin, A., & Levey, A. S. (2011). A predictive model for
+# progression of chronic kidney disease to kidney failure. JAMA, 305(15),
+# 1553-1559. doi: 10.1001/jama.2011.451.
+#
+# Sumida K, Nadkarni GN, Grams ME, Sang Y, et al. (2020). Conversion of urine
+# protein-creatinine ratio or urine dipstick protein to urine albumin-creatinine
+# ratio for use in chronic kidney disease screening and prognosis. Ann Intern Med,
+# 173(6), 426-435. doi: 10.7326/M20-0529.
+# ------------------------------------------------------------------------------
+################################################################################
```

