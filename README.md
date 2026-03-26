# Credit Card Fraud Detection: A Comparative ML Approach  

---

## Project Overview  

In the financial domain, detecting fraudulent transactions is critical, as even a single missed fraud can lead to significant financial loss, while excessive false alerts can harm customer experience.  

This project develops a **robust Machine Learning pipeline** to detect fraudulent credit card transactions using a highly imbalanced dataset and evaluates multiple models to balance **fraud detection (Recall)** and **user trust (Precision)**.

---

## Business Objective  

- Detect fraudulent transactions with high recall  
- Minimize false positives to protect customer experience  
- Enable scalable fraud detection systems for financial institutions  

---

## Model Performance  

| Model | Accuracy | Recall (Fraud) | Precision (Fraud) | ROC-AUC |
|------|----------|----------------|-------------------|--------|
| **XGBoost** | **99.92%** | **85%** | **73%** | **0.980** |
| Random Forest | 99.96% | 82% | **94%** | 0.963 |
| Logistic Regression | 97.41% | **92%** | 06% | 0.971 |

---

## Key Technical Components  

### 1. Class Imbalance Handling  
- Applied **SMOTE (Synthetic Minority Over-sampling Technique)**  
- Improved model’s ability to learn rare fraud patterns (~0.17% class)  

### 2. Feature Scaling  
- Used `StandardScaler` for normalization  
- Improved convergence for gradient-based models  

### 3. Model Comparison Strategy  
- Evaluated **Logistic Regression, Random Forest, and XGBoost**  
- Focused on **ROC-AUC and F1-score** instead of accuracy  

---

## Key Insights  

- Logistic Regression achieves **highest recall (92%)** → best at catching fraud  
- Random Forest achieves **highest precision (94%)** → minimizes false alarms  
- XGBoost provides **best overall performance (ROC-AUC: 0.98)**  
- Trade-off between recall and precision is critical in fraud detection  

---

## Business Impact  

- **85% fraud detection rate** using XGBoost improves financial security  
- **94% precision (Random Forest)** significantly reduces false alerts and manual workload  
- Prevents financial losses while maintaining customer trust  
- Enables data-driven fraud monitoring systems in production environments  

---

## Tech Stack  

- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost  
- **Imbalance Handling:** SMOTE  
- **Visualization:** Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  

---

## Conclusion  

This project demonstrates that no single model is universally optimal for fraud detection.  

- **Logistic Regression** → Best for sensitivity (recall)  
- **Random Forest** → Best for precision (customer experience)  
- **XGBoost** → Best overall performance  

A production system should balance these trade-offs based on business priorities.

---

## Author  

**Aniket Yadav**  
Aspiring Data Analyst | Machine Learning Enthusiast  

---

If you found this project useful, feel free to star the repository!
