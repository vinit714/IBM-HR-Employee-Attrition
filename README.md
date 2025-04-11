# IBM-HR-Employee-Attrition

>The data has been taken from [IBM Employee HR Attrition Kaggle](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset) 
 > The main Business problem that is being solved here is how a system can be created to help big companies control their attrition by understanding which employee could leave to provide him/her some incentives to stay back.

## Exploratory Data analysis
* Data is imbalanced by class we have 83% who have not left the company and 17% who have left the company
* The age group of IBM employees in this data set is concentrated between 25-45 years
* Attrition is more common in the younger age groups and it is more likely in females As Expected it is more common among single Employees
* People who leave the company get fewer opportunities to travel to the company
* People with very high education tend to have lower attrition
* The correlation plot was as expected
* The link to the EDA workbook in Python is [here](https://github.com/vinit714/IBM-HR-Employee-Attrition/blob/main/EDA_UnderstandingData.ipynb)

## Modeling for prediction
To find a model that could help with the prediction process we ran several data-mining models
* [Decision Tree and Random forest](https://github.com/vinit714/IBM-HR-Employee-Attrition/blob/main/ModelingDtree_Final.ipynb)
* [Artificial Neural Networks](https://github.com/vinit714/IBM-HR-Employee-Attrition/blob/main/ANN.ipynb)
* [Logistic Regression](https://github.com/vinit714/IBM-HR-Employee-Attrition/blob/main/ModelingLogisticRegression_Final.ipynb)
* [Support Vector Machines](https://github.com/vinit714/IBM-HR-Employee-Attrition/blob/main/ModelingSVM_Final.ipynb)
* [Extreme Gradient Boosting](https://github.com/vinit714/IBM-HR-Employee-Attrition/blob/main/XGBoost.ipynb)
* [Stacking a XGBOOST on a decsion tree](https://github.com/vinit714/IBM-HR-Employee-Attrition/blob/main/XGBoost_Stacker.ipynb)

Based on the results of various models applied to the IBM HR Employee Attrition dataset, several key insights emerge:

1. Random Forest with normal data achieved the highest accuracy at 87.22%, though it had a relatively low Kappa score (0.26) and ROC AUC (0.59), indicating strong predictive ability but modest agreement between predictions and true values.

2. XGBoost with SMOTE data demonstrated strong performance, achieving 86.41% accuracy, a high ROC AUC (0.68), and highest Kappa score (0.40), showing that it handled class imbalance well.

3. ANN (Artificial Neural Network) achieved a solid overall performance with 86.68% accuracy, a Kappa score of 0.36, and ROC AUC of 0.65, making it a competitive option.

4. Logistic Regression performed better with normal data (85.32% accuracy) compared to SMOTE data (73.36% accuracy), though the latter improved its ROC AUC and Kappa scores, reflecting its struggle with imbalanced data.

5. Decision Tree and Random Forest both saw a drop in performance when using SMOTE data, indicating that they may not benefit as much from resampling techniques, especially in terms of accuracy.

6. Support Vector Machine (SVM) showed moderate results, with 83.96% accuracy and a lower Kappa score (0.19) and ROC AUC (0.58), suggesting that it may not be the best choice for this dataset.

## Summary

Random Forest and XGBoost with normal data stand out in terms of accuracy, but XGBoost with SMOTE data offers a more balanced performance considering both accuracy and handling class imbalance. ANN also provides competitive results across all metrics. Models like Logistic Regression and Decision Tree tend to perform less effectively with SMOTE, while XGBoost benefits most from it.


## Future Work
1. Train and test more models.
2. Make a Tableau dashboard.



