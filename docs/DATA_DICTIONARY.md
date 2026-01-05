# Data Dictionary: Breast Cancer Dataset

## Overview

This document describes all features in the Wisconsin Breast Cancer Dataset used for tumor classification.

## Target Variable

| Column    | Type        | Description     | Values                    |
| --------- | ----------- | --------------- | ------------------------- |
| diagnosis | Categorical | Tumor diagnosis | M = Malignant, B = Benign |

## Feature Categories

Features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image.

### Feature Types

Each of the 10 base measurements has three statistical measures:

- **\_mean**: Mean value for the cells
- **\_se**: Standard error (variability)
- **\_worst**: Mean of the three largest values

## Complete Feature List

### Base Measurements (Mean Values)

| Feature                | Type  | Unit | Description                                          |
| ---------------------- | ----- | ---- | ---------------------------------------------------- |
| radius_mean            | Float | μm   | Mean distance from center to points on the perimeter |
| texture_mean           | Float | -    | Standard deviation of gray-scale values              |
| perimeter_mean         | Float | μm   | Perimeter of the cell nucleus                        |
| area_mean              | Float | μm²  | Area of the cell nucleus                             |
| smoothness_mean        | Float | -    | Local variation in radius lengths                    |
| compactness_mean       | Float | -    | perimeter² / area - 1.0                              |
| concavity_mean         | Float | -    | Severity of concave portions of the contour          |
| concave_points_mean    | Float | -    | Number of concave portions of the contour            |
| symmetry_mean          | Float | -    | Symmetry of the cell                                 |
| fractal_dimension_mean | Float | -    | "Coastline approximation" - 1                        |

### Standard Error Measurements

| Feature              | Type  | Description                         |
| -------------------- | ----- | ----------------------------------- |
| radius_se            | Float | Standard error of radius            |
| texture_se           | Float | Standard error of texture           |
| perimeter_se         | Float | Standard error of perimeter         |
| area_se              | Float | Standard error of area              |
| smoothness_se        | Float | Standard error of smoothness        |
| compactness_se       | Float | Standard error of compactness       |
| concavity_se         | Float | Standard error of concavity         |
| concave_points_se    | Float | Standard error of concave points    |
| symmetry_se          | Float | Standard error of symmetry          |
| fractal_dimension_se | Float | Standard error of fractal dimension |

### Worst (Largest) Measurements

| Feature                 | Type  | Description             |
| ----------------------- | ----- | ----------------------- |
| radius_worst            | Float | Worst (largest) radius  |
| texture_worst           | Float | Worst texture           |
| perimeter_worst         | Float | Worst perimeter         |
| area_worst              | Float | Worst area              |
| smoothness_worst        | Float | Worst smoothness        |
| compactness_worst       | Float | Worst compactness       |
| concavity_worst         | Float | Worst concavity         |
| concave_points_worst    | Float | Worst concave points    |
| symmetry_worst          | Float | Worst symmetry          |
| fractal_dimension_worst | Float | Worst fractal dimension |

## Removed Columns

| Column      | Reason                            |
| ----------- | --------------------------------- |
| id          | Unique identifier, not predictive |
| Unnamed: 32 | Empty column with all NaN values  |

## Data Statistics Summary

| Statistic      | Value                          |
| -------------- | ------------------------------ |
| Total Samples  | 569                            |
| Total Features | 30 (after cleaning)            |
| Missing Values | 0 (after removing Unnamed: 32) |
| Feature Type   | All numerical (float64)        |

## Source

Wisconsin Breast Cancer Dataset  
Creators: Dr. William H. Wolberg, W. Nick Street, Olvi L. Mangasarian  
Source: University of Wisconsin Hospitals, Madison  
UCI Machine Learning Repository
