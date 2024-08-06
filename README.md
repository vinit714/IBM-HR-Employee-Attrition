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
* From the Tableau plots we can conclude that the mentioned category has higher attrition rates:
* * Sales department among all the departments
* * Human Resources and Technical Degree in Education
* * Single’s in Marital status (Will not use this due to GDPR)
* * Male in comparison to females in Gender (Will not use this due to GDPR)
* * Employee with job satisfaction value 1
* * Job level 1 in job level
* * Life balance having value 1
* * Employee staying at a distant place
* * Environment Satisfaction value 1
 
## Modeling for prediction
To find a model that could help with the prediction process we ran several data-mining models
* [Decision Tree and Random forest](https://github.com/vinit714/IBM-HR-Employee-Attrition/blob/main/ModelingDtree_Final.ipynb)
* [Artificial Neural Networks](https://github.com/vinit714/IBM-HR-Employee-Attrition/blob/main/ANN.ipynb)

## Future Work
Train and test more models.



