# Diabetes-Detection-Using-Machine-Learning
This project aims to develop a machine-learning model for the detection of diabetes using a dataset that includes various health-related features. The dataset is loaded from a CSV file, and several preprocessing steps are performed to enhance the quality of the data before training a RandomForestClassifier.

The steps in the project include:

Data Loading: The dataset, presumably containing information relevant to diabetes, is loaded from a CSV file using pandas.

Data Exploration: Basic exploratory data analysis is conducted to understand the size, shape, missing values, and data types in the dataset.

Data Cleaning: Duplicate rows are removed from the dataset to ensure the quality of the data.

Descriptive Statistics: Descriptive statistics are generated to provide an overview of the central tendencies and spread of the data.

Data Visualization: A pairplot is created to visualize relationships between different features, aiding in understanding potential patterns or correlations.

Data Preprocessing: Several preprocessing steps are implemented:

Features with zero values are identified and replaced with the mean of the respective feature.
Outliers in the dataset are detected and removed using the Interquartile Range (IQR) method.
Unwanted features ('Pregnancies', 'Insulin', 'BloodPressure') are dropped from the dataset.
Data Oversampling: The SMOTE (Synthetic Minority Over-sampling Technique) algorithm is applied to address class imbalance, generating synthetic samples for the minority class.

Data Splitting: The dataset is split into training and testing sets using Stratified K-Fold to preserve class distribution.

Model Training: A RandomForestClassifier is trained on the preprocessed and oversampled data.

Model Evaluation: The trained model is evaluated on the testing set, and various metrics, including accuracy, confusion matrix, and classification report, are generated.

Feature Importance: The importance of features in the trained model is analyzed and presented in a table.

Data Visualization: Additional visualizations, such as a pairplot and a heatmap of the correlation matrix, are created to gain insights into the relationships between features.

ROC Curve and AUC Score: The Receiver Operating Characteristic (ROC) curve is plotted, and the Area Under the Curve (AUC) score is calculated to assess the model's performance.

![output](https://github.com/arun7371/Diabetes-Detection-Using-Machine-Learning/assets/86791724/a60615ae-c13f-4bf3-9534-080cd9aa498f)


Achieved Accuracy:
Remarkably, the model achieves an accuracy of 100% on the testing set. While a perfect accuracy score might raise questions about potential issues such as overfitting or data leakage, it's crucial to thoroughly investigate and validate the results. Possible considerations include the dataset size, characteristics, and the chosen evaluation metrics. Additionally, a thorough understanding of the data and model behavior is necessary to ensure the credibility of the reported accuracy.
