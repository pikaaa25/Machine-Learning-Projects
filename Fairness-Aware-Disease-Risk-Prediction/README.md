# Fairness-Aware Disease Risk Prediction using Machine Learning

## Overview
This project investigates disease risk prediction using machine learning models with a focus on **fairness and bias analysis** across sensitive demographic attributes. In high-stakes domains such as healthcare, models must not only be accurate but also equitable across different population groups. This work evaluates whether predictive performance differs across subgroups and highlights the importance of fairness-aware model assessment.

---

## Objectives
- Build machine learning models for disease risk prediction  
- Evaluate predictive performance using standard metrics  
- Analyze fairness across sensitive attributes (e.g., gender, age groups)  
- Highlight potential biases and ethical considerations in healthcare ML  

---

## Dataset
- **Source**: UCI Heart Disease Dataset  
- **Description**: Clinical and demographic attributes used to predict the presence of heart disease  
- **Target Variable**: Disease presence (binary classification)

> Note: The dataset is publicly available and commonly used for benchmarking healthcare machine learning models.

---

## Methodology
- Data preprocessing and feature normalization  
- Model training using:
  - Logistic Regression  
  - Random Forest Classifier  
- Performance evaluation using:
  - Accuracy  
  - Precision  
  - Recall  
  - F1-score  
- Fairness analysis by comparing model behavior across demographic subgroups  

---

## Results
The trained models achieved competitive predictive performance on the disease classification task. However, subgroup-level analysis revealed variations in prediction outcomes across demographic groups, indicating potential bias. These results demonstrate that accuracy alone is insufficient for evaluating healthcare models.

---

## Conclusion
This project emphasizes the importance of incorporating fairness considerations into machine learning pipelines for healthcare applications. By analyzing subgroup-level performance, the work highlights ethical risks associated with biased predictions and underscores the need for responsible and transparent AI systems.

---

## Tools & Technologies
- Python  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## Future Work
- Integrate formal fairness metrics such as demographic parity and equalized odds  
- Apply bias mitigation techniques  
- Extend evaluation to additional healthcare datasets  

---

## Author
**[Your Name]**  
MSc Robotics & Embedded AI
