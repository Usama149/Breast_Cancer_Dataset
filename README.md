## Breast Cancer Classification with Machine Learning

### Overview
This project applies multiple **classification algorithms** to the **Breast Cancer Wisconsin Diagnostic dataset** in order to predict whether a tumor is:

- **M** = Malignant
- **B** = Benign

The goal was to compare the performance of different classifiers on the same dataset and identify which model performed best.

---

### Models Tested
The following classification models were trained and evaluated:

- Logistic Regression
- K-Nearest Neighbors (K-NN)
- Support Vector Machine (Linear)
- Kernel SVM
- Naive Bayes
- Decision Tree
- Random Forest

---

### Data Preparation
Before training the models, the dataset was prepared as follows:

- the **ID column** was removed
- the **diagnosis column** was used as the target variable
- diagnosis labels were encoded into numeric form
- the dataset was split into **training** and **test** sets
- **feature scaling** was applied where necessary, such as for Logistic Regression, K-NN, and SVM

---

### Model Comparison

#### Test Set Results

| Model | Accuracy |
|------|------:|
| Logistic Regression | 95.80% |
| K-NN (k = 3) | 94.41% |
| K-NN (k = 5) | 95.10% |
| K-NN (k = 7) | 95.10% |
| Linear SVM | 93.71% |
| Kernel SVM | 95.80% |
| Naive Bayes | 91.61% |
| Decision Tree | 95.10% |
| Random Forest | 98.60% |

---

### Best Performing Model
The **Random Forest** classifier achieved the highest accuracy on the selected test set:

- **Accuracy:** 98.60%
- **Correct predictions:** 141 out of 143
- **Misclassifications:** 2

#### Confusion Matrix for Random Forest

```text
[[90  0]
 [ 2 51]]

 ## Model Comparison Chart

<img width="1189" height="590" alt="Model Comparison" src="https://github.com/user-attachments/assets/b335d718-4376-4657-a31a-e075bbe94ceb" />

