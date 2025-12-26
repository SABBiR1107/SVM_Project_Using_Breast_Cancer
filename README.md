# Breast Cancer Classification Using Support Vector Machine (SVM)

## 1. Introduction

Breast cancer is one of the most common cancers affecting women worldwide. Early and accurate detection of breast cancer can significantly improve treatment outcomes and survival rates. Machine Learning techniques can assist doctors by providing accurate predictions based on medical data.

In this project, we use the **Support Vector Machine (SVM)** algorithm to classify breast cancer tumors as **Malignant (M)** or **Benign (B)** using a real-world dataset obtained from Kaggle. The project is implemented using **Python** in **Google Colab**.

---

## 2. Objective of the Project

The main objectives of this project are:

* To understand and implement the Support Vector Machine algorithm
* To preprocess and analyze a real medical dataset
* To build an accurate classification model
* To evaluate the performance of the model using different metrics

---

## 3. Dataset Description

The dataset used in this project is the **Breast Cancer Wisconsin (Diagnostic) Dataset** from Kaggle.

### Dataset Details:

* Source: Kaggle
* Total Instances: 569
* Total Features: 30
* Target Classes:

  * Malignant (M)
  * Benign (B)

### Attributes Used:

The dataset contains features related to cell nuclei measurements such as:

* Radius
* Texture
* Perimeter
* Area
* Smoothness
* Compactness
* Concavity
* Symmetry
* Fractal Dimension

Each feature is provided as mean, standard error, and worst values.

---

## 4. Tools and Technologies Used

* Programming Language: Python
* Platform: Google Colab
* Libraries:

  * NumPy
  * Pandas
  * Matplotlib
  * Scikit-learn

---

## 5. Methodology

The project follows the below steps:

### 5.1 Data Loading

The dataset was loaded into Google Colab using a CSV file downloaded from Kaggle.

### 5.2 Data Preprocessing

* Removed unnecessary columns such as `id` and empty columns
* Converted categorical target values (M, B) into numerical values (1, 0)
* Checked for missing values

### 5.3 Train-Test Split

The dataset was split into:

* 80% Training Data
* 20% Testing Data

### 5.4 Feature Scaling

Feature scaling was applied using **StandardScaler** because SVM is sensitive to feature magnitudes.

### 5.5 Model Training

Two SVM models were trained:

* SVM with Linear Kernel
* SVM with RBF Kernel

### 5.6 Model Testing

Predictions were made on the test dataset.

---

## 6. Performance Evaluation

The model performance was evaluated using:

* Accuracy Score
* Confusion Matrix
* Classification Report (Precision, Recall, F1-score)

### Results:

* Linear Kernel Accuracy: ~97%
* RBF Kernel Accuracy: ~98%

The RBF kernel performed slightly better than the linear kernel.

---

## 7. Visualization

* Bar chart was used to compare accuracy between Linear and RBF kernels
* Confusion matrix was visualized to understand true and false predictions

These visualizations help in better interpretation of model performance.

---

## 8. Conclusion

In this project, Support Vector Machine was successfully implemented to classify breast cancer tumors. The model achieved high accuracy, proving that SVM is an effective algorithm for medical diagnosis tasks. Feature scaling and kernel selection played an important role in improving performance.

This system can assist medical professionals as a decision-support tool but should not replace expert diagnosis.

---

## 9. Future Scope

* Use hyperparameter tuning (GridSearchCV)
* Try other algorithms such as Random Forest or Neural Networks
* Deploy the model using a web application

---

## 10. References

* Kaggle Breast Cancer Dataset
* Scikit-learn Documentation
* Machine Learning textbooks and online resources

---

**End of Report**
