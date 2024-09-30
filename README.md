# Diabetes Prediction using SVM

This project aims to predict diabetes using Support Vector Machines (SVM) on the Pima Indians Diabetes Database. The dataset includes several medical predictor variables and one target variable, indicating the presence or absence of diabetes.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Evaluation](#model-evaluation)
- [Contributing](#contributing)


## Introduction

Diabetes is a chronic disease that occurs when the body cannot effectively use insulin. Early detection is crucial for managing the disease and preventing complications. In this project, we employ SVM, a supervised learning algorithm, to classify whether a patient is likely to have diabetes based on various medical attributes.

## Dataset

The dataset used in this project is the [Pima Indians Diabetes Database]((https://raw.githubusercontent.com/jbrownlee/Datasets/master/pima-indians-diabetes.data.csv)). It contains the following features:

| Feature                | Description                                      |
|------------------------|--------------------------------------------------|
| Pregnancies            | Number of times pregnant                         |
| Glucose                | Plasma glucose concentration                     |
| BloodPressure          | Diastolic blood pressure (mm Hg)                |
| SkinThickness          | Triceps skin fold thickness (mm)                |
| Insulin                | 2-Hour serum insulin (mu U/ml)                  |
| BMI                    | Body mass index (weight in kg/(height in m)^2) |
| DiabetesPedigreeFunction | Diabetes pedigree function                     |
| Age                    | Age (years)                                     |
| Outcome                | Class variable (1: diabetes, 0: no diabetes)   |

## Installation

To set up the project environment, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/ahmdmohamedd/svm-diabetes-prediction.git
   cd svm-diabetes-prediction
   ```

## Usage

You can adjust the parameters within the script to experiment with different kernels (linear, RBF, polynomial) and model configurations.

### Example Output

The model will output the following metrics:
- **Accuracy**: Overall accuracy of the model.
- **Confusion Matrix**: Visualization of true positive, true negative, false positive, and false negative predictions.
- **Classification Report**: Detailed metrics including precision, recall, and F1-score.

## Model Evaluation

The model's performance was evaluated using accuracy, confusion matrix, and classification report. The results from various kernels are as follows:

### Results

- **Linear Kernel**:
  - Accuracy: 70.13%
  - Confusion Matrix: 
    ```
    [[68 31]
     [15 40]]
    ```
  
- **RBF Kernel**:
  - Accuracy: 72.08%
  - Confusion Matrix: 
    ```
    [[68 31]
     [12 43]]
    ```

- **Polynomial Kernel**:
  - Accuracy: 78.57%
  - Confusion Matrix: 
    ```
    [[81 18]
     [15 40]]
    ```

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, please fork the repository and submit a pull request.
