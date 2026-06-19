Daniyal Aziz_TC-INT-20260602-358
TASK 01
CUSTOMER BEHAVIOR ANALYTICS & CHURN PREDICTION DASHBOARD
Teyzix Core Internship — Task DA-INT-1
DESCRIPTION:
This project builds an end-to-end churn analytics system on the IBM Telco
Customer Churn dataset (7,043 customers). It covers data cleaning,
exploratory analysis, feature engineering, customer segmentation, and churn
prediction using three ML models (Logistic Regression, Random Forest,
XGBoost), with SHAP explainability and a risk-scored customer output.

Key outputs:
- 13 visualizations (churn distribution, correlations, model comparison,
  SHAP, etc.)
- Model performance report (Accuracy, Precision, Recall, F1, ROC-AUC)
- customer_risk_scores.csv — every customer scored with churn probability
  and risk category (Low / Medium / High)
- Printed business insights report (top churn drivers, revenue impact,
  recommendations)
FILES:
churn_analysis.ipynb  (Main notebook , run this)
WA_Fn-UseC_-Telco-Customer-Churn.csv (Input dataset)
customer_risk_scores.csv (Output , generated after running)
viz.png (Output charts , generated after running)
REQUIREMENTS:
Python 3.9+
Packages: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, shap
PROCESS:
OPTION 1 : Local (Jupyter / VS Code)
Install dependencies:
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost shap jupyter

2. Place WA_Fn-UseC_-Telco-Customer-Churn.csv in the same folder as the
   notebook.

3. Open churn_analysis.ipynb in Jupyter or VS Code.

4. Run all cells top to bottom (Run All).

OPTION 2 : Google Colab

1. Upload churn_analysis.ipynb to Colab.

2. Upload the dataset CSV in the first cell:
   from google.colab import files
   files.upload()

3. Install the one missing package (Colab has the rest pre-installed):
   !pip install xgboost shap

4. Run all cells.
NOTEBOOK STRUCTURE:
1. Setup & Imports
2. Load & Inspect Data
3. Data Cleaning
4. Exploratory Data Analysis
5. Feature Engineering
6. Customer Segmentation
7. Correlation Heatmap
8. Revenue Analysis
9. Preprocessing for ML
10. Model Training & Evaluation
11. Feature Importance & SHAP
12. Churn Probability & Risk Categorization
13. Business Insights Report
SUMMARY:
Overall churn rate: 26.5%
Best model (ROC-AUC): Logistic Regression — 0.848
High-risk customers identified: 1,030 (~$83K/month revenue at risk)
Top churn drivers: month-to-month contracts, electronic check payment,
low tenure, no tech support / online security add-ons
