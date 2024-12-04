# Pneumonia Image Classification - Machine Learning ![Project Views](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FBrunosCodeLab%2FPneumoniaImageClassification-ML&count_bg=%235C9CFF&title_bg=%23008FC9&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)


## Project Description
The theme of this project is **classification of pneumonia X-ray images**. The goal was to develop an ML model capable of detecting pneumonia based solely on chest X-ray images.

The use of machine learning models in diagnostics offers the following advantages:
- Automated analysis of large volumes of X-ray images.
- Faster diagnosis processes.
- Reduced risk of human error.
- Improved accuracy in identifying pneumonia.

## Dataset
We used the **Chest X-Ray Images (Pneumonia)** dataset available on [Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia).

The dataset contains:
- 1341 images of normal lungs (class 0).
- 3875 images of lungs with pneumonia (class 1).

## Development Environment
The project was developed using **Google Colab**, leveraging TensorFlow and Keras libraries for building a convolutional neural network (CNN).

## Key Implementation Steps

### 1. Data Preprocessing
- **Image Augmentation:** We used `ImageDataGenerator` for scaling images, horizontal flipping, and other augmentations.
- **Class Balance Analysis:** The dataset was examined for class imbalance.
- **Class Weighting:** Class weights were calculated to address data imbalance and improve training focus.
- **Image Scaling:** Pixel values were normalized between 0 and 1.

### 2. CNN Model Development
The CNN model was built using a **Sequential** architecture with the following key components:
- **Convolutional Layers:** Extract features from the images.
- **MaxPooling Layers:** Reduce dimensionality and focus on dominant features.
- **Flatten Layer:** Converts multidimensional input into a one-dimensional vector.
- **Dense Layers:** Facilitate final classification.

The output layer uses a **sigmoid** activation function for binary classification (normal vs. pneumonia).

### 3. Evaluation
The model was evaluated on validation and test datasets to assess its performance.

## Results
The classification results demonstrated high accuracy in detecting pneumonia from chest X-ray images.

## Conclusion
This project highlights the potential of machine learning in medical diagnostics. The developed model could serve as an assistive tool for physicians, enabling faster and more accurate diagnoses.
