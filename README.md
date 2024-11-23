# Wjindani-Upgrad-MelanomaDetectionAssignment
# Melanoma-Detection

> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
 
## Table of Contents
* [Problem Statement](#problem-statement)
* [Project Pipeline](#project-pipeline)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)

## Problem Statement

### Business Understanding

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

* Actinic keratosis
* Basal cell carcinoma
* Dermatofibroma
* Melanoma
* Nevus
* Pigmented benign keratosis
* Seborrheic keratosis
* Squamous cell carcinoma
* Vascular lesion

### Business Goal:

You are required to build a multiclass classification model using a custom convolutional neural network in TensorFlow. 

### Business Risk:

- Predicting an incorrect class of skin cancer

# Project Pipeline

### 1. Data Preparation
- **Data Reading & Understanding**: Specify the paths for train and test image directories.  
- **Dataset Creation**:  
  - Generate training and validation datasets from the training directory with a batch size of 32.  
  - Ensure all images are resized to `180x180` pixels.  

---

### 2. Dataset Visualization
- Implement functionality to visualize one example from each of the nine classes in the dataset.  

---

### 3. Initial Model Building & Training
- **Model Creation**:  
  - Develop a CNN capable of classifying the nine classes in the dataset.  
  - Normalize pixel values by rescaling images between 0 and 1.  
- **Training Configuration**:  
  - Select an appropriate optimizer and loss function.  
  - Train the model for approximately 20 epochs.  
- **Evaluation**:  
  - Analyze the training results to check for signs of overfitting or underfitting.  
  - Document observations and findings.  

---

### 4. Addressing Overfitting/Underfitting
- Apply suitable data augmentation strategies to tackle any overfitting or underfitting issues identified earlier.  

---

### 5. Model Training with Augmented Data
- **Model Creation**:  
  - Rebuild the CNN, ensuring images are rescaled to normalize pixel values between 0 and 1.  
- **Training Configuration**:  
  - Choose a relevant optimizer and loss function.  
  - Train the model for about 20 epochs.  
- **Evaluation**:  
  - Reassess model performance and verify if the augmentation resolved previous issues.  

---

### 6. Class Distribution Analysis
- Examine the distribution of samples across all nine classes in the training dataset:  
  - Identify the class with the least samples.  
  - Determine which classes dominate the dataset in terms of sample proportions.  

---

### 7. Handling Class Imbalances
- Use the **Augmentor** library to address imbalances in the training dataset.  

---

### 8. Model Training with Balanced Data
- **Model Creation**:  
  - Build a CNN designed to classify all nine classes. Normalize image pixel values between 0 and 1.  
- **Training Configuration**:  
  - Select a suitable optimizer and loss function.  
  - Train the model for approximately 30 epochs.  
- **Evaluation**:  
  - Document findings to confirm whether the class imbalance issues have been resolved.  

---

## Technologies Used
- pandas - 1.3.4
- numpy - 1.20.3
- matplotlib - 3.4.3
- seaborn - 0.11.2
- plotly - 5.8.0
- sklearn - 1.1.2
- statsmodel - 0.13.2
- tensorflow - 2.11.0



## Acknowledgements
- This project was independent case study for MS in AI & ML.
- https://www.geeksforgeeks.org/
- https://seaborn.pydata.org/
- https://plotly.com/
- https://pandas.pydata.org/
- https://learn.upgrad.com/
- https://www.tensorflow.org/


## Contact
Created by Wjindani for Upgrad Assignment. 


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
