# Melanoma Detection Project
> This project aimed to develop a machine learning model to accurately classify different types of skin lesions.

**Table of Contents**
1. Problem Statement
2. Project Pipeline
3. [General Info](#GeneralInfo)
4. [Technologies Used](#TechnologiesUsed)
5. [Conclusions](#Conclusions)
6. [Acknowledgements](#Acknowledgements)
7. [Contact](#Contact)

## Problem Statement
In this project, we will build a multiclass classification model using a custom convolutional neural network in TensorFlow. 

To build a CNN-based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

## Project Pipeline
- **Data Reading/Data Understanding** → Defining the path for train and test images 
- **Dataset Creation** → Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
- **Dataset visualization** → Create a code to visualize one instance of all the nine classes present in the dataset 
- **Model Building & training :**
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
  - Choose an appropriate optimizer and loss function for model training
  - Train the model for ~20 epochs
  - Write your findings after the model fit. You must check if there is any evidence of model overfit or underfit.
- Chose an appropriate data augmentation strategy to resolve underfitting/overfitting 
- Model Building & training on the augmented data :
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
  - Choose an appropriate optimizer and loss function for model training
  - Train the model for ~20 epochs
  - Write your findings after the model fit, and see if the earlier issue is resolved or not?
- Class distribution: Examine the current class distribution in the training dataset 
  - Which class has the least number of samples?
  - Which classes dominate the data in terms of the proportionate number of samples?
-  Handling class imbalances: Rectify class imbalances present in the training dataset with the Augmentor library.
-  Model Building & training on the rectified class imbalance data :
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
  - Choose an appropriate optimizer and loss function for model training
  - Train the model for ~30 epochs
  - Write your findings after the model fit, and see if the issues are resolved or not?

## General Information
This project is focused on addressing the challenge of classifying skin lesions into various categories, including pigmented benign keratosis, melanoma, basal cell carcinoma, nevus, squamous cell carcinoma, vascular lesion, actinic keratosis, dermatofibroma, and seborrheic keratosis. The dataset used in this project initially suffered from class imbalance, which could potentially impact the model's performance. Therefore, data augmentation techniques were applied to address this issue.

The project aimed to develop a model that could accurately classify skin lesions and provide valuable insights for healthcare professionals in diagnosing and treating skin conditions. The dataset used for training and evaluation included images of skin lesions, along with corresponding labels indicating the lesion type.

## Technologies Used
- Python - version 3.10
- TensorFlow - version 2.6
- Keras - version 2.6
- Augmentor - version 0.2

## Conclusions
Based on the analysis of the trained model, the following conclusions can be drawn:

- The deep learning model achieved promising results with a training accuracy of approximately 95% and a validation accuracy of around 83%.

- The application of data augmentation techniques helped mitigate the impact of class imbalance, resulting in improved performance on underrepresented classes.

- Further analysis, such as evaluating precision, recall, and F1-score for each class, would provide a more comprehensive assessment of the model's performance on imbalanced data.

## Acknowledgements
This project was inspired by the need for accurate skin lesion classification to support dermatological diagnosis and treatment. The methodology and techniques used were adapted from various machine learning and deep learning resources. Special thanks to the developers and contributors of the open-source libraries used in this project.

## Contact
Created by [@jamesalvin49](https://github.com/jamesalvin49) - feel free to contact me!

Please let me know if you need any further details or if there's anything else I can assist you with!
