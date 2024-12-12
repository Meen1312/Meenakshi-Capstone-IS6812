# Home Credit  Default Risk Analysis

## Table of Contents 
 
  - [Objectives](#objectives)
  - [Solution to the Business Problem ](#solution-to-the-business-problem)
  - [My Contributions](#my-contributions)
  - [Buisness Value Of The Solution](#business-value-of-the-solution)
  - [Difficulties Encounterd](#difficulties-encountered)
  - [Results And Success Metrics](#results-and-success-metrics)
  - [Recommendations](#recommendations)
  - [Limitations](#limitations)
  - [Summary](#summary)
  

### Business Problem : 
   Home Credit, founded in 1997, operates across multiple Asian and European markets with a mission to provide responsible lending. However, the challenge lies in assessing consumer trustworthiness due to limited credit history and data. This project aims to build a predictive model to enhance loan eligibility assessments, mitigate risks, and improve customer satisfaction, boosting revenue and operational efficiency. Data was extracted from Kaggle.
#### Objectives:
  -	Develop a supervised learning model to classify consumer creditworthiness.
  -	Improve loan repayment success by 30%.
  -	Increase low-risk loan approvals by 25%.
  -	Achieve a 35% improvement in customer satisfaction.

  ### Solution to the Business Problem
  #### 1 Exploratory Data Analysis:
  <img width="604" alt="Class Imbalance " src="https://github.com/user-attachments/assets/c6fe333b-a4f8-4a8f-b869-7b5803bd8271" />

  -	Analyzed class imbalance (91% non-defaults, 9% defaults)
  -  Visualized non-linear relationships between income, credit amount, and default status.
  ### 2 Data Preprocessing:
  -  Designed pipelines to clean and preprocess training and testing datasets
  -  Handled class imbalance using oversampling and under sampling techniques.
  -  Encoded categorical variables and selected predictive features
  ### 3 Model Development
  -   Built and optimized machine learning models, including Logistic Regression, Decision Trees, and XGBoost.
  -   Compared models using ROC-AUC, confusion matrices, and other performance metrics.
  ### 4 Evaluation and Visualization:
   -  Generated clear visualizations, including ROC-AUC plots, to communicate model performance effectively.
  ### 5 Documentation:
   - Created reproducible notebooks using R Markdown for transparency and easy collaboration

### My Contributions 
#### My primary contributions included:
  -  Exploratory Data Analysis (EDA): Conducted the analysis to identify class imbalances and relationships between key features and loan default status.
  -  Engineering: Designed the preprocessing pipeline, including handling missing values, transforming categorical variables, and addressing class imbalance.
  -  Model Development and Evaluation: Developed and fine-tuned the Logistic Regression and XGBoost models. Created visualizations such as ROC-AUC plots and confusion 
     matrices for model evaluation.
  -  Documentation: Authored detailed and reproducible R Markdown notebooks, ensuring clarity and usability for stakeholders.

#### Business Value of the Solution
  - The recommended XGBoost model (ROC-AUC = 0.85) has the potential to:
  - Reduce loan defaults by improving creditworthiness prediction accuracy.
  - Increase revenue by approving more low-risk loans (25% increase).
  - Enhance customer satisfaction by streamlining loan approvals and offering competitive interest rates.
  - Boost operational efficiency by automating and optimizing the credit evaluation process.

####  Difficulties Encountered
  - Class Imbalance: The dataset was heavily skewed (91% non-defaults, 9% defaults), which made it challenging to achieve high recall for the minority class. Addressed this 
    using oversampling, undersampling, and class weighting.
  - Non-Linear Data: Logistic Regression struggled with non-linear relationships, requiring feature transformations and advanced models like XGBoost.
  - Overfitting Risk: Decision Trees tended to overfit without pruning. XGBoost required extensive hyperparameter tuning to achieve optimal performance.

### Results and Success Metrics
 ####	Model Performance:
  -	Logistic Regression: ROC-AUC = 0.78<img width="607" alt="ROC" src="https://github.com/user-attachments/assets/aa5c7757-12b9-4ada-b60d-54611798c885" />
  - Decision Tree: ROC-AUC = 0.75 <img width="584" alt="Decision tree Eva" src="https://github.com/user-attachments/assets/9e183b00-5f96-40ad-9434-4c69e144f741" />
  - XGBoost: ROC-AUC = 0.85
  - Based on these results, XGBoost is recommended for deployment due to its superior performance.

### Recommendations 
  - Feature Engineering: Add interaction terms or polynomial features to better capture non-linear relationships.
  - Hyperparameter Tuning : Optimize parameters like max_depth and min_samples_split for tree-based models.
  - Model Combination: Use ensemble methods like stacking (combine predictions from Logistic Regression, Decision Tree, and XGBoost) for potentially better performance.
  - Model Interpretability: While XGBoost performs best, consider SHAP (Shapley Additive exPlanations) or feature importance plots to interpret its predictions.

### Limitations
  - Class Imbalance: The dataset is highly skewed, leading to challenges in achieving high recall for the minority class.
  - Overfitting Risk: Decision Trees may overfit without proper pruning or regularization.XGBoost, being a complex model, requires careful tuning to avoid overfitting.
  - Non-Linear Data: Logistic Regression struggles to model non-linear separable data, as evident from the scatter plot analysis.

### Summary 
   XGBoost is the recommended model for deployment based on its superior AUC (0.85), though additional interpretability measures are suggested. Addressing class imbalance 
   and enhancing interpretability through feature engineering or visualization techniques will improve outcomes. Future work should focus on exploring hybrid models and 
   reducing computational costs for scalability




     

