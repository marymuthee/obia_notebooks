# Object-Based Image Analysis (OBIA) – Segmentation, Feature Extraction, and Classification

This repository contains three Jupyter Notebooks developed as part of my Object-Based Image Analysis (OBIA) course. The notebooks demonstrate a complete OBIA workflow, including image segmentation, object-based feature extraction, and supervised classification.

The initial notebook structure and baseline code were provided by my course instructor, Dr. Dirk Tiede, for instructional purposes. I built on this foundation by extending and adding new functionalities, particularly within the feature extraction and classification stages.

---

## Repository Structure

01_segmentation.ipynb  
02_feature_extraction.ipynb  
03_classification.ipynb  

---

## Segmentation Notebook

Purpose:  
To generate image objects (segments) from multispectral imagery and assess segmentation quality.

Functionalities:
- Multiband image stacking (RGB and NIR)
- NDVI computation
- SLIC superpixel segmentation
- Visualization of:
  - Original RGB image  
  - Segmentation boundaries  
  - Mean RGB per segment  

Most of the segmentation logic was based on the provided course material, with additional documentation and visualization improvements.

---

## Feature Extraction Notebook

Purpose:  
To compute object-level features describing spectral, shape, and textural characteristics of image segments.

Functionalities:
- Creation of a multiband feature stack (R, G, B, NIR, NDVI)
- Spectral features (mean, standard deviation)
- Shape features (solidity, compactness, rectangularity/extent)
- Textural feature based on NDVI entropy
- Compilation of all features into a single feature table

The feature extraction workflow builds on the instructor-provided template and was extended with custom feature functions and improved organization.

---

## Classification Notebook

Purpose:  
To classify image objects into tree and non-tree classes using supervised machine learning.

Functionalities:
- Manual selection and labeling of training samples
- Rule-based object classification
- Random Forest supervised classification (based on provided material)
- Additional implemented functionality:
  - Support Vector Machine (SVM) object-based classification
- Accuracy assessment using:
  - Cross-validation
  - Confusion matrix
  - Precision, recall, and F1-score
- Mapping of predicted object classes back to raster space
- Visualization of classification results

---

## Acknowledgements

Baseline tutorial code and workflow design were provided by Dr. Dirk Tiede as part of the OBIA course. All additional implementations and extensions in this repository were developed by me for learning and demonstration purposes.
