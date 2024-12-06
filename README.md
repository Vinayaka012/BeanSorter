# Automated Dry Bean Seed Classification System

## Objective
Developed a machine learning system for the automatic categorization of 7 distinct types of dry bean seeds using high-resolution camera-captured data. This project aims to assist farmers and researchers in classifying dry bean seeds more efficiently and accurately than manual methods.

---

## Dataset Description
- **Source**: [UCI Machine Learning Repository - Dry Bean Dataset](http://archive-beta.ics.uci.edu/dataset/602/dry+bean+dataset/)
- **Features**: 16 attributes describing size and shape, including:
  - Area
  - Perimeter
  - Eccentricity
  - Convex area
  - And more
- **Classes**: Seven varieties of dry beans:
  - Seker, Barbunya, Bombay, Cali, Dermosan, Horoz, and Sira
- **Size**: 13,611 samples

---

## Methodology

### Data Preprocessing
- Divided data into **training** and **test sets**.
- Applied feature **normalization** using `StandardScaler`.

### Models Implemented
1. **Support Vector Machine (SVM)**:
   - Optimized with a linear kernel for high-dimensional data.
   - Hyperparameter tuning with `GridSearchCV`.
   - **Accuracy**: 93.11% on the test set.

2. **Random Forest Classifier**:
   - Built as an alternative to handle non-linear relationships.
   - Hyperparameters tuned using `GridSearchCV`.
   - **Accuracy**: 92.39% on the test set.

---

## Evaluation Metrics
- **Accuracy**: Both models achieved competitive classification results.
- **Precision, Recall, F1-Score**: Assessed across all classes.
- **Confusion Matrix**: Analyzed misclassifications and model performance by class.

---

## Results
- The **SVM model** outperformed the Random Forest model in overall accuracy and had fewer misclassifications.
- Demonstrated the feasibility of using machine learning for seed classification with minimal error.

---

## Key Technologies
- **Programming Language**: Python
- **Libraries**: Scikit-learn, Pandas, Matplotlib
- **Tools**: Jupyter Notebook

---

## Future Scope
- Incorporate **deep learning methods** to enhance accuracy further.
- Test models on other agricultural datasets for broader applicability.

---

## References
1. [Dry Bean Dataset - UCI Machine Learning Repository](http://archive-beta.ics.uci.edu/dataset/602/dry+bean+dataset/)
2. Koklu, M., & Ozkan, I. A. (2020). *Multiclass classification of dry beans using computer vision and machine learning techniques.*
