Fairness-Aware Disease Risk Prediction using Machine Learning
Overview

This project investigates disease risk prediction using machine learning models with a focus on fairness and bias analysis across sensitive demographic attributes. In high-stakes domains such as healthcare, models must not only be accurate but also equitable across different population groups. This work evaluates whether predictive performance differs across subgroups and highlights the importance of fairness-aware model assessment.

Objectives

Build machine learning models for disease risk prediction

Evaluate predictive performance using standard metrics

Analyze fairness across sensitive attributes (e.g., gender, age groups)

Highlight potential biases and ethical considerations in healthcare ML

Dataset

Source: UCI Heart Disease Dataset

Description: Clinical and demographic attributes used to predict the presence of heart disease

Target Variable: Disease presence (binary classification)

Note: The dataset is publicly available and commonly used for benchmarking healthcare ML models.

Methodology

Data preprocessing and feature normalization

Model training using:

Logistic Regression

Random Forest Classifier

Performance evaluation using:

Accuracy

Precision, Recall, F1-score

Fairness analysis across demographic subgroups by comparing prediction outcomes

Results

The trained models achieved competitive predictive performance on the disease classification task. However, subgroup analysis revealed variations in prediction behavior across demographic groups, indicating potential bias. These findings demonstrate that accuracy alone is insufficient for evaluating healthcare models and motivate the need for fairness-aware evaluation.

Conclusion

This project emphasizes the importance of incorporating fairness considerations into machine learning pipelines for healthcare applications. By analyzing subgroup-level behavior, the work highlights ethical risks associated with biased predictions and underscores the necessity of transparent and responsible AI systems in medical decision-making.

Tools & Technologies

Python

NumPy, Pandas

Scikit-learn

Matplotlib, Seaborn

Jupyter Notebook

Future Work

Incorporate formal fairness metrics (e.g., demographic parity, equalized odds)

Apply bias mitigation techniques

Extend analysis to multiple healthcare datasets
