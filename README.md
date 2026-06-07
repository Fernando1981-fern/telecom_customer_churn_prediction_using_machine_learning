# Telecom Customer Churn Prediction

## 📋 Project Overview

This project aims to build a machine learning model to predict customer churn in the telecom industry. The goal is to help **Interconnect**, a telecom provider, identify customers who are likely to cancel their services so they can take proactive retention measures such as offering personalized promotions or special plans.

Customer retention is critical in the highly competitive telecom industry, and retaining existing customers is typically more cost-effective than acquiring new ones. By predicting which customers are at risk of churning, the company can implement targeted interventions to improve customer satisfaction and reduce customer loss.

## 🎯 Project Objectives

- Analyze customer behavior patterns and characteristics
- Perform exploratory data analysis (EDA) to understand customer data
- Engineer relevant features from raw data
- Build and train multiple machine learning models
- Evaluate model performance using appropriate metrics
- Identify key factors influencing customer churn
- Provide actionable insights for retention strategies

## 📊 Dataset

The project uses data from four main sources, each containing customer information:

1. **contract.csv** - Contract details and churn information
2. **personal.csv** - Personal customer demographics
3. **internet.csv** - Internet service information
4. **phone.csv** - Phone service details

All datasets are merged using the `customerID` column as the primary key.

### Key Features:
- **Customer ID**: Unique customer identifier
- **Churn**: Binary target variable (0 = retained, 1 = churned)
- **BeginDate**: Contract start date
- **EndDate**: Contract end date (if churned)
- **Contract type**: Length and type of contract
- **Services**: Internet, phone, and other service subscriptions
- **Demographics**: Age, gender, and family status
- **Billing information**: Monthly charges, total charges

## 🔧 Tech Stack

### Libraries & Tools
- **Data Processing**: pandas, numpy
- **Visualization**: matplotlib, seaborn
- **Machine Learning**: scikit-learn, LightGBM, CatBoost
- **Preprocessing**: LabelEncoder, StandardScaler

### Models Used
The project implements and compares multiple machine learning algorithms:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier
- LightGBM Classifier
- CatBoost Classifier

## 📈 Methodology

### 1. Data Loading & Exploration
- Load data from CSV files
- Merge datasets on `customerID`
- Explore dataset structure and statistics

### 2. Feature Engineering
- Create binary `Churn` target variable from `EndDate`
- Convert `BeginDate` to proper datetime format
- Handle categorical variables
- Normalize/scale numerical features

### 3. Exploratory Data Analysis (EDA)
- Analyze customer demographics
- Visualize churn distribution
- Examine relationships between features and churn
- Identify correlations and patterns

### 4. Model Development
- Split data into training and testing sets
- Train multiple machine learning models
- Compare model performance using ROC-AUC and accuracy metrics
- Select the best performing model

### 5. Model Evaluation
- Use ROC-AUC score for model comparison
- Calculate accuracy metrics
- Analyze feature importance
- Generate insights from model predictions

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- Jupyter Notebook
- Required libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, lightgbm, catboost

### Installation
```bash
pip install pandas numpy matplotlib seaborn scikit-learn lightgbm catboost
```

### Running the Project
1. Open `final_project.ipynb` in Jupyter Notebook
2. Ensure data files are in the correct `/datasets/final_provider/` path
3. Run cells sequentially from top to bottom
4. Review visualizations and model results

## 📊 Project Structure

```
final_project.ipynb
├── Project Overview & Business Context
├── Data Loading & Import
├── Data Exploration & Merging
├── Feature Engineering & Preprocessing
├── Exploratory Data Analysis
│   ├── Customer demographics analysis
│   ├── Service usage patterns
│   ├── Churn distribution analysis
│   └── Correlation analysis
├── Model Development
│   ├── Data splitting
│   ├── Feature scaling
│   ├── Model training
│   └── Model evaluation
├── Results & Insights
└── Recommendations
```

## 🔍 Key Findings

*Results and key insights will be generated after running the models, including:*
- Customer segments most prone to churn
- Most important features predicting churn
- Best performing model and its metrics
- Actionable recommendations for customer retention

## 📈 Model Performance Metrics

The models are evaluated using:
- **ROC-AUC Score**: Measures the model's ability to distinguish between churn and non-churn
- **Accuracy**: Percentage of correct predictions
- **Feature Importance**: Identifies which features are most influential in predicting churn

## 💡 Recommendations for Stakeholders

Based on the model predictions, Interconnect can:
1. **Identify high-risk customers** for proactive outreach
2. **Offer targeted promotions** to at-risk customer segments
3. **Improve service quality** in identified problem areas
4. **Optimize retention budgets** by focusing on highest-value customers at risk
5. **Personalize retention strategies** based on customer profiles

## 📝 Notes

- All data manipulation and preprocessing is performed within the notebook
- Models are compared to determine the best approach
- Results and insights are documented throughout the notebook
- The project can be extended with additional features or more sophisticated ensemble methods

## 👤 Author

Created by: Fernando Gnone de Oliveira

## 📄 License

This project is provided as-is for educational and business analysis purposes.

---

**Last Updated**: June 2026
