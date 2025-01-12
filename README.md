# Breast-Cancer-Prediction-Model
A Breast Cancer Prediction Model is a machine learning system designed to classify breast tumors as benign (non-cancerous) or malignant (cancerous) using patient data. 
# Breast Cancer Prediction and Diagnosis Report

## 1. Introduction
This report presents a comprehensive analysis of the Breast Cancer Wisconsin Diagnostic dataset to predict and diagnose breast cancer using various machine learning techniques. The dataset contains 569 samples with 33 features, including measurements of cell nuclei and a diagnosis label indicating whether the tumor is malignant or benign.

## 2. Data Loading and Exploration
The dataset was loaded using the Pandas library and explored to understand its structure and contents.

### Dataset Overview:
- **Total Samples:** 569
- **Total Features:** 33 (including the target variable 'diagnosis')
- **Target Variable:** 'diagnosis' (M: Malignant, B: Benign)

### Data Insights:
- An unnecessary column `Unnamed: 32` containing only NaN values was dropped.
- The target variable 'diagnosis' was label-encoded: Malignant (1) and Benign (0).

## 3. Data Preprocessing

### Missing Values:
- No missing values in relevant features.
- Dropped the `Unnamed: 32` column due to all values being null.

### Feature Scaling:
- StandardScaler was used to normalize the features, ensuring consistent data scaling for model training.

### Data Splitting:
- The dataset was split into training and testing sets using an 80-20 ratio.

## 4. Exploratory Data Analysis (EDA)

### Diagnosis Distribution:
- Visualization of the diagnosis variable revealed class imbalance:
  - Malignant: 212
  - Benign: 357

### Correlation Analysis:
- Strong correlations observed between certain features, e.g., `radius_mean` and `perimeter_mean`.
- High correlation between `concave points_mean` and the diagnosis label.

## 5. Machine Learning Models
Various machine learning models can be trained on this dataset, including:
- K-Nearest Neighbors (KNN)
- Random Forest Classifier
- Logistic Regression
- Decision Tree Classifier
- Support Vector Machine (SVM)

### Model Training Process:
- Training and testing datasets were used to evaluate model performance.
- Standard metrics such as accuracy, precision, recall, and F1-score were used for evaluation.

## 6. Key Findings
- Support Vector Machine (SVM) achieved the highest classification accuracy (97.2%) in previous analysis.
- Features like `radius_mean`, `perimeter_mean`, and `concave points_mean` are significant indicators of malignancy.

## 7. Conclusion
This analysis highlights the effectiveness of machine learning models in predicting breast cancer. Feature scaling and proper preprocessing significantly contribute to improved model performance. Among the models, SVM demonstrated the best accuracy, making it a promising choice for breast cancer diagnosis.

## 8. References
- Breast Cancer Wisconsin Diagnostic Dataset (UCI Machine Learning Repository)
- Scikit-learn Documentation
- Pandas and Numpy Libraries
- Matplotlib and Seaborn for Visualization

