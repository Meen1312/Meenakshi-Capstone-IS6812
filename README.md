# Home Credit  Default Risk Analysis

## Table of Contents 
 

 - [Objectives](#objectives)
 - [Exploratory Data Analysis](#exploratory-data-analysis)
 - [Results And Success Metrics](#results-and-success-metrics)
 - [Recommendations](#recommendations)
 - [Limitations](#limitations)
 - [Summary](#summary)
  

### Business Problem : 
 Home Credit, founded in 1997, operates across multiple Asian and European markets with a mission to provide responsible lending. However, the challenge lies in assessing consumer trustworthiness due to limited credit history and data. This project aims to build a predictive model to enhance loan eligibility assessments, mitigate risks, and improve customer satisfaction, boosting revenue and operational efficiency. Data was extrated from Kaggle 
#### Objectives:
-	Develop a supervised learning model to classify consumer creditworthiness.
-	Improve loan repayment success by 30%.
-	Increase low-risk loan approvals by 25%.
-	Achieve a 35% improvement in customer satisfaction.
#### Exploratory Data Analysis 
- Data Preprocessing: Designed pipelines to clean and preprocess training and testing datasets, Exploratory Data Analysis (EDA)
   1.	Analyzed class imbalance (91% non-defaults, 9% defaults).
   2. Visualized non-linear relationships between income, credit amount, and default status.<img width="610" alt="Non linear Separable check" src="https://github.com/user-attachments/assets/f112096d-8144-4b09-a9fb-ea0cca59c03f" />

  - Feature Engineering: Transformed categorical variables, handled class imbalance, and selected predictive features.
  - Model Development: Built and optimized machine learning models, including Logistic Regression, Decision Trees, and XGBoost.
  - Evaluation and Visualization: Created ROC-AUC plots, confusion matrices, and performance metrics for comparison.
  -	Documentation: Authored clear and reproducible R Markdown notebooks
### Results and Success Metrics
####	Model Performance:
-	Logistic Regression: ROC-AUC = 0.78<img width="607" alt="ROC" src="https://github.com/user-attachments/assets/aa5c7757-12b9-4ada-b60d-54611798c885" />

-  Decision Tree: ROC-AUC = 0.75 <img width="584" alt="Decision tree Eva" src="https://github.com/user-attachments/assets/9e183b00-5f96-40ad-9434-4c69e144f741" />
- 	XGBoost: ROC-AUC = 0.85 


### Recommendations 
- Feature Engineering: Add interaction terms or polynomial features to better capture non-linear relationships.
- Hyperparameter Tuning : Optimize parameters like max_depth and min_samples_split for tree-based models.
- Model Combination: Use ensemble methods like stacking (combine predictions from Logistic Regression, Decision Tree, and XGBoost) for potentially better performance.
- Model Interpretability: While XGBoost performs best, consider SHAP (Shapley Additive exPlanations) or feature importance plots to interpret its predictions.

### Limitations
- Class Imbalance: The dataset is highly skewed (91.9% non-defaults, 8.1% defaults), leading to challenges in achieving high recall for the minority class.
- Overfitting Risk: Decision Trees may overfit without proper pruning or regularization.XGBoost, being a complex model, requires careful tuning to avoid overfitting.
- Non-Linear Data: Logistic Regression struggles to model non-linear separable data, as evident from the scatter plot analysis.

### Summary 
XGBoost is the recommended model for deployment based on its superior AUC (0.85), though additional interpretability measures are suggested. Addressing class imbalance and enhancing interpretability through feature engineering or visualization techniques will improve outcomes. Future work should focus on exploring hybrid models and reducing computational costs for scalability




     

