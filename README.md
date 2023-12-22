# Ensemble of Deep Learning Architectures for Robust Cancer Diagnosis

## Overview

This project focuses on robust cancer diagnosis using an ensemble of deep learning architectures. The goal is to provide an efficient and accurate system for identifying various types of cancer from medical images. The ensemble comprises models specifically designed for oral, brain, breast, cervical, lung, and lymphoma cancers.

## Dataset

The dataset used for training and evaluation is accessible [here](https://www.kaggle.com/datasets/obulisainaren/multi-cancer). Please download the dataset before running the code.

## Preprocessing

The preprocessing phase involves the following steps:

- **Data Cleaning:** Elimination of duplicate images and resizing for consistency.
- **Data Splitting:** Stratified sampling is employed to ensure a representative distribution in the training and testing datasets.

## Models

The system incorporates different models tailored to specific cancer types, each varying in the number of convolutional neural network (CNN) layers:

- **Two Layers of CNN:**
  - Oral Cancer Model

- **Three Layers of CNN:**
  - Image Origin Model (IOM)
  - Brain Cancer Model
  - Breast Cancer Model
  - Lymphoma Cancer Model

- **Four Layers of CNN:**
  - Cervical Cancer Model
  - Lung Cancer Model

## System Workflow

The system follows a sequential process to ensure efficient utilization of resources and accurate classification:

1. **Preprocessing Pipeline:**
   - Images are resized to a standardized 128x128 dimensions.
   - Rescaling is applied to normalize pixel values, bringing them within the 0 to 1 range.

2. **Image Origin Model (IOM):**
   - The preprocessed image is fed into the IOM to determine the most suitable classification model to employ. This step is implemented to optimize resource utilization.

3. **Classification Model:**
   - The identified cancer-specific model (oral, brain, breast, cervical, lung, or lymphoma) is invoked to perform the final classification task.

By implementing this ensemble approach, the system aims to enhance the overall robustness and accuracy of cancer diagnosis, ensuring a reliable tool for medical professionals. Feel free to reach out if additional details or clarifications are needed.
