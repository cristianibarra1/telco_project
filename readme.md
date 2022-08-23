![logo@2x.png](attachment:logo@2x.png)


```python
!jt -t oceans16 
```

# Telco_ Project
by cristian ibarra 

# Project Goals:

Find drivers for customer churn at Telco. Why are customers churning?

Construct a ML classification model that accurately predicts customer churn.

Deliver a report that a non-data scientist can read through and understand what steps were taken, why and what was the outcome?

# Project steps:

Step 1: Understanding the Problem.

Step 2: Data Extraction.

Step 3: Data Cleaning.

Step 4: Exploratory Data Analysis.

Step 5: Feature Selection.

Step 6: Testing the Models.

Step 7: Deploying the Model.
# Project Planning:

•Create README.md with data dictionary, project and business goals, come up with initial hypotheses.

•Acquire data from the Codeup Database and create a function to automate this process. Save the function in an acquire.py file to import into the Final Report Notebook.

•Clean and prepare data for the first iteration through the pipeline, MVP preparation. Create a function to automate the process, store the function in a prepare.py module, and prepare data in Final Report Notebook by importing and using the funtion.

•Clearly define two hypotheses, set an alpha, run the statistical tests needed, reject or fail to reject the Null Hypothesis, and document findings and takeaways.

•Establish a baseline accuracy and document well.

•Evaluate models on train and validate datasets.

•Choose the model with that performs the best and evaluate that single model on the test dataset.

•Create csv file

•Document conclusions, takeaways, and next steps in the Final Report Notebook.

# Hypotheses:
`Hypothesis 1 - Monthly charge`:

`Ho` -> Does the higher the monthly charge effect churn?

`Ha`-> The higher the monthly charge doesnt effect churn?

`Hypothesis 2 - Contract type `:

`Ho` -> There is no association between churn and a customer having a longer contract type 

`Ha`-> There is an association between churn and a customer having shorter contract type 


`Hypothesis 3 - Contract type and Monthly charge`:

`Ho` -> There is no association between churn and a customer having high monthly with low contract 

`Ha`-> There is no association between churn and a customer having high monthly with high contract.

# Goal:
Churn — Whether the customer churned or not (Yes or No)

# Data Dictionary/Findings:

### Data Used-Telco
| Attribute        |        Data type    |       Definition    |
| -------- | -------- | -------- |
|Gender |int |0-female and 1-male |
|Tenure |int |years customer has been with telco |
|Monthly_charges   |float |price of monthly services charged to the customer each month |
|Total_charges |float |price of the total months  | 
|Churn |int |0 if the customer is still with the company, 1 if they have left/churned |
|Contract_type  |int |12 for month-to-month contract, 1 for 1 year contract, 2 for 2 year contract |
|Paperless_billing |int |0 if customer does not have paperless billing, 1 if they do |


# Modeling:
---
# VALIDATE:
|MODEL | ACCURACY/VALIDATE | F1 SCORE/VALIDATE |
| ----- | ----- | ----- |
|K-Nearest Neighbor|.77|.53|
|Random Forest |.80|.58|
|Logistic Regression |.80|0.63|



# TRAIN:
|MODEL | ACCURACY/TRAIN | F1 SCORE/TRAIN |
| ----- | ----- | ----- |
|K-Nearest Neighbor|.83|.65|
|Random Forest |.90|.79|
|Logistic Regression |.80|0.63|

# Project description
1)Why this project-
This project would help determind if customer are churning based on contract lenght or monthly charge

2)Why is important-
So we could change the outcome before it happens to more customers 

3)How does this help you- 
This would help all of us on understanding how,who,why our customers are leaving to better companies.

# Conclusions & Next Steps

•With baseline of 73%. We identified on why customer are turning away from staying with us or joining our company. As per our analysis the main issues were customers with short term contracts,and customers with higher monthly charge tenth to turn away from stay in the contract longer.

• Short term contract tent to be the highest churn rate out of all our categories

`Next step`

•investigated why customers are leaving within the 12month period of a contract,and if there's another reason why our clientel are leaving more often.

`Recommendations`

• I recommned that we either lower the price for our longer contracts so that would incourage more customer to stay in a longer commitment or we lower the month to month for more customer to stay in the loing term.

• Our monthly cost should offer deal or sale to increase our customer line up

• Reccommned more contrat lenght instead of just 3. The sweet spot seem to be arround the 3-12 month part so we could make a 6month contract or 4 month contract 

• I reccommend we check this every 6month to make sure our prediction of churn customers is going in the right place

# Deliverables:
To access the correct MySQL database, you will need credentials to access to the CodeUp database. This database is accessed in this project via an env.py file. Add the below to your env.py and fill in your individual access information as strings:

user = 'your_user_name'
password = 'your_password'
host = 'the_codeup_db'

1-Readme (.md)

2-Final Report (.ipynb) 

3-Acquire (.py)

4-Model (.py)

5-Prepare Modules (.py)

6-Predictions (.csv).
