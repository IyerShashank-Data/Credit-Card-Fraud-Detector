# Credit-Card-Fraud-Detector
## Description
In this project, I applied **three anomaly detection techniques**:
- Isolation Forest
- One-Class SVM
- Z-Score

Then I combined them using an ensemble approach to detect fraud in real-world credit card transactions.

### 📁 Dataset
Kaggle: [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

### Techniques
- Ensemble Anomaly Detection
- PCA Visualization
- Scikit-learn, Seaborn, Matplotlib

### Results
Out of 284,807 transactions:
- ~492 labeled frauds
- Ensemble detected ~88% of frauds with minimal false positives

-Class 0: Legitimate Transactions
    Precision: 1.00 – The model is perfect at identifying genuine transactions.
    Recall: 0.96 – It correctly identifies 96% of all genuine transactions.
    F1-Score: 0.98 – Strong balance between precision and recall.

-Class 1: Fraudulent Transactions",
    Precision: 0.04 – Of all predicted frauds, only 4% were fraud.
    Recall: 0.85 – However, it captured 85% of all actual frauds, which is crucial in fraud detection
    F1-Score: 0.08 – Very low due to low precision.
    
-Overall Performance
    Accuracy: 96% – Dominated by Class 0, so not meaningful alone.
    Macro Avg F1-Score: 0.53 – Averages both classes equally; fair given class imbalance.
    Weighted Avg F1-Score: 0.98 – Skewed toward Class 0 due to class imbalance.
  
-Final Thoughts:
  Despite the low precision for fraud detection, the model achieved a high recall rate (85%), indicating that it successfully flagged most fraudulent transactions. 
    In high-risk domains like credit card fraud:
    Recall is more important than precision, since missing a fraud is costlier than a false alarm.
    This makes our model practically useful, especially when paired with human review.
    
 ### Best use case
 Semi-automated fraud detection, where flagged transactions are reviewed manually.

### Tools Used
- Python (Pandas, Scikit-learn, Matplotlib, Seaborn)
- Jupyter Notebook
