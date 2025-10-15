# Telco Customer Churn Prediction

A machine learning project analyzing customer churn patterns and building a predictive model using Random Forest.

## 📊 Project Overview

- **Exploratory Data Analysis** to understand churn patterns
- **Random Forest Classifier** for churn prediction
- **Model Evaluation** with comprehensive metrics

## 🛠️ Installation

```bash
git clone https://github.com/Nabin15/telco-customer-churn.git
cd telco-customer-churn
pip install -r requirements.txt
```

### Required Libraries
- pandas, numpy, matplotlib, seaborn, scikit-learn

## 📁 Project Structure

```
telco-customer-churn/
├── data/
│   └── telco_churn.csv
├── notebooks/
│   ├── eda.ipynb
│   └── modeling.ipynb
├── models/
│   └── random_forest_model.pkl
├── requirements.txt
└── README.md
```

## 🔍 Key EDA Findings

- **Month-to-month contracts** have higher churn rates
- **Higher monthly charges** correlate with increased churn
- **Longer tenure** customers are less likely to churn
- **Fiber optic** internet users show higher churn
- **Electronic check** payment method has higher churn

## 🤖 Model Performance

- **Accuracy**: [0.81]
- **Precision(macro_average)**: [0.76] 
- **Recall(macro_average)**: [0.72]
- **F1-Score(macro_average)**: [0.73]
- **ROC-AUC**: [0.84]

### Top Features
1. Tenure
2. Total Charges  
3. Monthly Charges 
4. Internet Service Type
5. Payment Method Elec. Check

## 🚀 Usage

```python
import joblib

# Load model and make predictions
model = joblib.load('models/random_forest_model.pkl')
predictions = model.predict(new_data)
```

## 📈 Business Insights

**High-Risk Customers:**
- Month-to-month contracts
- Fiber optic internet  
- Electronic check payments
- Higher monthly charges

**Recommendations:**
- Target customers in first 6 months
- Encourage longer contracts
- Review fiber optic pricing
