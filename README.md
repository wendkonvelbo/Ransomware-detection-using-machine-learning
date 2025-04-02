# Ransomware-detection-using-machine-learning
This project detects ransomware using Random Forest, GBM, and Logistic Regression. It preprocesses data, applies cross-validation, and evaluates models with confusion matrices and classification reports. Visualizations include model comparisons and performance metrics. 
Ransomware Detection with Machine Learning

📌 Overview

This project detects ransomware using machine learning models: Random Forest, Gradient Boosting Machines (GBM), and Logistic Regression. It preprocesses data, performs cross-validation, and evaluates models using confusion matrices and classification reports.

🛠️ Features

Data preprocessing:

Dropping irrelevant columns (e.g., file names, hashes)

Encoding categorical values into numerical representations

Standardizing features for Logistic Regression

Model training and evaluation using:

Random Forest Classifier

Gradient Boosting Machines (GBM)

Logistic Regression

Cross-validation (5-fold) to assess model performance

Confusion matrix visualization for better interpretability

Classification report analysis (precision, recall, F1-score)

Comparison of model accuracy using bar charts

📊 Models Used

Random Forest Classifier: Ensemble learning method that improves prediction accuracy by combining multiple decision trees.

Gradient Boosting Machines (GBM): Boosting technique that builds models sequentially to correct previous errors.

Logistic Regression: A statistical model used for binary classification after feature scaling.

📌 Dependencies

Ensure you have the following Python libraries installed:

pip install pandas scikit-learn matplotlib mlxtend

🚀 Usage

Clone the repository:

git clone https://github.com/yourusername/ransomware-detection.git
cd ransomware-detection

Install dependencies (if not installed):

pip install -r requirements.txt

Run the script:

python ransomware_detection.py

View evaluation results, classification reports, and confusion matrices.

📈 Results

Random Forest

Cross-Validation Scores: [0.9942, 0.9961, 0.9952, 0.9966, 0.9963]

Mean Accuracy: 0.9957

Confusion Matrix:

[[7094   13]
 [  27 5363]]

Classification Report:

Precision    Recall  F1-score   Support

0       1.00      1.00      1.00      7107
1       1.00      0.99      1.00      5390

Accuracy                          1.00     12497
Macro avg       1.00      1.00      1.00     12497
Weighted avg   1.00      1.00      1.00     12497

Gradient Boosting Machines (GBM)

Cross-Validation Scores: [0.9864, 0.9927, 0.9919, 0.9903, 0.9879]

Mean Accuracy: 0.9899

Confusion Matrix:

[[7071   36]
 [  87 5303]]

Classification Report:

Precision    Recall  F1-score   Support

0       0.99      0.99      0.99      7107
1       0.99      0.98      0.99      5390

Accuracy                          0.99     12497
Macro avg       0.99      0.99      0.99     12497
Weighted avg   0.99      0.99      0.99     12497

Logistic Regression

Cross-Validation Scores: [0.8853, 0.8962, 0.7466, 0.8856, 0.8726]

Mean Score: 0.8573

Confusion Matrix:

[[6571  536]
 [2080 3310]]

Classification Report:

Precision    Recall  F1-score   Support

0       0.76      0.92      0.83      7107
1       0.86      0.61      0.72      5390

Accuracy                          0.79     12497
Macro avg       0.81      0.77      0.78     12497
Weighted avg   0.80      0.79      0.78     12497

🔍 Future Improvements

Experimenting with additional machine learning models (e.g., SVM, XGBoost)

Implementing real-time detection with streaming data

Enhancing feature engineering for better accuracy

📜 License

This project is open-source and available under the MIT License.

