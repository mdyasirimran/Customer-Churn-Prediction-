# Customer-Churn-Prediction-

Project Title: Customer Churn Prediction for a Telecom Company
Dataset Used:
Telco Customer Churn Dataset (from Kaggle)

Tools & Libraries:
Python, Pandas, Scikit-learn, Seaborn, Matplotlib, Joblib

✅ Objective:
To build a predictive model that identifies customers who are likely to churn (i.e., stop using the telecom service) and understand the key factors influencing churn behavior.

🔹 Step 1: Data Loading & Preprocessing
Loaded the dataset and removed irrelevant columns like customerID.

Converted categorical variables into numerical format using One-Hot Encoding.

Handled missing values (if any).

Final dataset split into features (X) and target (y = Churn).

🔍 Step 2: Exploratory Data Analysis (EDA)
Analyzed distribution of Churn, Contract, and MonthlyCharges.

Visualizations:

Count plots of churned vs non-churned customers.

Boxplots showing MonthlyCharges by churn status.

Count plot of Contract Type vs Churn.

Correlation heatmap for numeric variables.

Found that contract type and monthly charges are important predictors of churn.

🤖 Step 3: Model Training
Trained two classification models:

Decision Tree Classifier

Gradient Boosting Classifier

Evaluated models using Accuracy, Classification Report, and Confusion Matrix.

🔧 Step 4: Hyperparameter Tuning
Used GridSearchCV for Gradient Boosting and RandomizedSearchCV for HistGradientBoostingClassifier.

Performed cross-validation (cv=3) for better generalization.

Selected the best model based on performance.

📊 Step 5: Evaluation & Visualization
Evaluated the final optimized model on the test set.

Plotted confusion matrix for clarity.

Displayed Top 10 Important Features using bar plots (from Gradient Boosting).

Features like Contract_Two year, MonthlyCharges, tenure had high importance.

💾 Step 6: Model Saving
Saved the final best model as:

Copy
Edit
best_hist_gradient_boosting_model.pkl
📌 Key Takeaways:
Customers with month-to-month contracts and high monthly charges are more likely to churn.

Contract type and monthly charges are among the top churn predictors.

Boosting models outperformed basic decision trees in accuracy and precision.

📎 This project successfully followed the required steps:
✅ Data Preprocessing
✅ EDA & Visualization
✅ Model Training & Evaluation
✅ Hyperparameter Tuning
✅ Result Interpretation & Saving
