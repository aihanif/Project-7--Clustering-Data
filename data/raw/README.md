# Raw Data Directory

## Purpose
This directory contains the original, unprocessed data files before any cleaning or preprocessing.

## Contents
- **Data_cleaned_3.pickle**: Original system monitoring dataset (671 records, 43 features)
- **Data_PCA_2.pickle**: PCA processed data for dimensionality reduction

## Data Description
- **Source**: System monitoring logs and user behavior tracking
- **Format**: Pickle files (.pickle)
- **Size**: Approximately 2-5 MB
- **Last Updated**: December 2024

## Usage Notes
- These files are the starting point for all analysis
- Do not modify these files directly
- Always work with copies in the processed/ directory
- Keep backups of original data

## Data Dictionary
Key features include:
- PAGE_NO: Page identifier
- TOTAL_ANNOTATION: Number of annotations
- YEAR/MONTH: Temporal information
- DEVICE_NAME: Device type
- IS_WEEKEND: Weekend indicator
- BROWSER_VERSION: Browser information
- CATEGORY_ERROR: Error classification

## File Naming Convention
- `Data_[processing_step]_[version].pickle`
- Version numbers indicate processing iterations
