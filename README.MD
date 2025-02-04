"" 
"#Overview#" 
"" 

"This project aims to predict customer churn using various machine learning techniques. Churn prediction is crucial for businesses to retain customers by identifying those at risk of leaving." 

"" 

"# Dataset Description#" 


"" 

"The dataset \`Train_data.csv\` contains customer information and the target variable indicating whether a customer has churned. The columns are:" 

"- \`Unnamed: 0\`: Index" 

"- \`RowNumber\`: Customer's row number" 

"- \`CustomerId\`: Customer ID" 

"- \`Surname\`: Customer surname" 

"- \`CreditScore\`: Credit score of the customer" 

"- \`Geography\`: Country of the customer" 

"- \`Gender\`: Gender of the customer" 

"- \`Age\`: Age of the customer" 

"- \`Tenure\`: Number of years the customer has been with the bank" 

"- \`Balance\`: Account balance of the customer" 

"- \`NumOfProducts\`: Number of bank products the customer is using" 

"- \`HasCrCard\`: Does the customer have a credit card? (1 = Yes, 0 = No)" 

"- \`IsActiveMember\`: Is the customer an active member? (1 = Yes, 0 = No)" 

"- \`EstimatedSalary\`: Estimated salary of the customer" 

"- \`Exited\`: Did the customer churn? (1 = Yes, 0 = No)" 

"- \`Complain\`: Did the customer complain? (1 = Yes, 0 = No)" 

"- \`Satisfaction_Score\`: Customer satisfaction score" 

"- \`Card_Type\`: Type of card the customer has" 

"- \`Point_Earned\`: Points earned by the customer" 

"- \`ReceivedPromotion\`: Did the customer receive a promotion? (1 = Yes, 0 = No)" 

"- \`AgeGroup\`: Age group of the customer" 

"- \`InterventionType\`: Type of intervention used for the customer" 

"" 

"## Data Preprocessing ## " 

"" 

"The data preprocessing steps include:" 

"1. Replacing whitespace in column names with underscores." 

"2. Converting categorical features to dummy/indicator variables." 

"3. Dropping unnecessary columns." 

"4. Splitting the data into training and testing sets." 

"" 

"## Model Building and Training ##" 

"" 

"### Models Used: ###" 
  
"- **Random Forest**" 

"- **Gradient Boosting (XGBoost)**"

"- **LightGBM**" 

"### Hyperparameter Tuning: ##" 

"Grid Search with Cross-Validation was used to find the best hyperparameters." 

""

"### LightGBM Model with Class Weighting:###" 

"" 

"#### Parameter Grid: ###" 

"\`\`\`python" 

"param_grid_lgbm = {" 

"    'n_estimators': [50, 100, 200]," 

"    'learning_rate': [0.01, 0.05, 0.1]," 

"    'max_depth': [3, 4, 5]," 

"    'subsample': [0.6, 0.7, 0.8],"

"    'colsample_bytree': [0.6, 0.7, 0.8]," 

"    'reg_alpha': [0.0, 0.1, 0.5]," 

"    'reg_lambda': [0.0, 0.1, 0.5],"

"    'class_weight': ['balanced']"

"}" 

"\`\`\`" 

"" 

"## Installation ##"

"" 

"To run the notebooks, you will need to have Python and Jupyter Notebook installed. You can install the required packages using the following commands:" 

"" 

"pip install jupyter"

"pip install pandas" 

"pip install numpy"

"pip install matplotlib" 

"pip install seaborn" 

"pip install scikit-learn"

"pip install xgboost"

"pip install lightgbm" 

"\`\`\`"

"" 

"## Usage  ##" 

""

"1. Clone the repository to your local machine:" 

"   \`\`\`bash" 

"   git clone https://github.com/yourusername/your-repo-name.git" 

"   cd your-repo-name" 

"   \`\`\`" 

"" 

"2. Navigate to the project directory:" 

"   \`\`\`bash" 

"   cd MyProject" 

"   \`\`\`" 

""

"3. Start the Jupyter Notebook server:" 

"   \`\`\`bash" 

"   jupyter notebook" 

"   \`\`\`" 

"" 

"4. Open the notebooks \`predictive Modeling.ipynb\` and \`ExploratoryDataAnalysis.ipynb\` to explore the content." 

"" 

"## Files ##" 

"" 

"- **predictive Modeling.ipynb**: This notebook contains predictive modeling work including data preprocessing, model training, and evaluation." 

"- **ExploratoryDataAnalysis.ipynb**: This notebook contains exploratory data analysis, visualizations, and insights drawn from the dataset." 

"" 

"## Contributing ##" 

"" 

"Contributions are welcome! If you would like to contribute, please follow these steps:" 

"" 

"1. Fork the repository." 

"2. Create a new branch: \`git checkout -b my-feature-branch\`" 

"3. Make your changes and commit them: \`git commit -m 'Add some feature'\`"

"4. Push to the branch: \`git push origin my-feature-branch\`" 

"5. Submit a pull request." 

"" 
