# Fraud Detection with XGBoost and Machine Learning

## 📊 Project Overview
This project implements a comprehensive fraud detection system using machine learning models to identify fraudulent financial transactions in the PaySim synthetic financial dataset. The notebook compares multiple classification algorithms including XGBoost, Random Forest, Decision Tree, and Logistic Regression to determine the most effective approach for fraud detection.

## 🚀 Features
- **Data Exploration & Visualization**: Comprehensive EDA with heatmaps, violin plots, and transaction type analysis
- **Data Preprocessing**: Label encoding, feature scaling, and class imbalance handling with SMOTE
- **Multiple ML Models**: 
  - XGBoost Classifier
  - Random Forest Classifier  
  - Decision Tree Classifier
  - Logistic Regression
- **Model Evaluation**: Performance comparison using Accuracy, Precision, Recall, F1-Score, and ROC-AUC
- **Feature Importance Analysis**: Identifies key factors contributing to fraudulent transactions
- **Visual Results**: Confusion matrices, ROC curves, and performance comparison charts

## 📁 Dataset
The project uses the **PaySim** synthetic financial dataset from Kaggle:
- **File**: `PS_20174392719_1491204439457_log.csv`
- **Size**: 6,362,620 transactions with 11 features
- **Target Variable**: `isFraud` (0=Legitimate, 1=Fraudulent)
- **Fraud Rate**: Only 0.13% of transactions are fraudulent (highly imbalanced dataset)

## 🔧 Key Steps
1. **Data Loading & Initial Exploration**
2. **Visual Analysis** of transaction patterns and fraud distribution
3. **Data Preprocessing**: Encoding categorical variables and feature scaling
4. **Class Imbalance Handling**: Using SMOTE to balance the dataset
5. **Train-Test Split**: 80-20 split with stratification
6. **Model Training & Evaluation**: Four different ML models
7. **Performance Comparison**: Comprehensive metrics analysis
8. **Feature Importance**: Identifying critical fraud indicators

## 📈 Results
The models are evaluated on multiple metrics with a focus on recall and F1-score due to the high cost of false negatives in fraud detection. The notebook identifies which model performs best for this specific fraud detection task.

## 🛠️ Requirements
```
numpy
pandas
scikit-learn
imbalanced-learn
xgboost
seaborn
matplotlib
```

## 💡 Key Insights
- Transaction type plays a significant role in fraud patterns
- Certain features show clear separation between fraudulent and legitimate transactions
- Class balancing techniques are crucial for effective fraud detection in imbalanced datasets
- Ensemble methods like XGBoost and Random Forest generally outperform traditional classifiers

## 📝 Usage
Run the Jupyter notebook cells sequentially. The notebook is self-contained and includes all necessary steps from data loading to model evaluation. Results are automatically displayed with visualizations.

## 🔍 Applications
- Financial institution fraud monitoring systems
- Credit card fraud detection
- Mobile payment security
- Anomaly detection in transaction data

## ⚠️ Note
This is a synthetic dataset designed for research purposes. While it mimics real transaction patterns, results should be validated on real-world data before production deployment.

## 📄 License
This project is intended for educational and research purposes. The dataset is publicly available on Kaggle.
