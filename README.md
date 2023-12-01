# Pace_telecom


## East Coast Retention

GitHub repositery for the east cost retention project. 

Repositery Structure

- Executive Summary
    - Business Problem
    - Proposed Solution
- Data
    - Statistics
    - Data exclusion
    - Data Assumption
- EDA
    - Analysis
- Modeling
    - Outcome variable
    - Features
    - Random Forest
    - Training, testing and predicting data
- Findings
    - Model Findings
    - Analysis Findings
- Recommendations
    
## Executive Summary 

#### - Business Problem
Pace Telecom is facing challenges in establishing a significant Market Share in the East Coast region, despite successfully acquiring new customers.

#### - Proposed Solution
Accelerating customer acquisition without maintaining market share may lead to underperformance in the East Coast region. Given the current scenario, customer retention would possibly be the optimal solution.


## Data

- Source: Marketing Team
- Size: 7032 customers * 20 characteristics
- Time Period: 1st January,2023 - 1st October, 2023

#### Data Exclusion
- Considering the ethnicity concern, sensitive details such as name, address, banking details and joining date are excluded by the HR team.
- Information this sensitive can lead to biases by any data operator. 
- Information like address and name must be preserved because incase of a data breach, customers can get on the verge of identity theft.

#### Data Assumption
The dataset was provided by our marketing team which was extracted directly from the service dealers, so it is assumed that the dataset contains all the customers as its mandatory to register a customer before providing the service and the details in the dataset are correct.


## Exploratory Data Analysis

#### Exploring Churn pattern with types of Contract.

{image link}

Key Takeaways
- Majority of customers choose Monthly contracts. 
- Probably because they were new to the company and unsure about the service so chose monthly plan and kept using the same

---
#### Exploring Churn pattern with types of Contract. -2 

{image link}

Key Takeaways
- Maximum churn happens in customers who choose monthly contract at 42.7%.
- Churn rate for customers with yearly contract is significantly lower at 11.28% and 2.85%.

---
#### Exploring Churn pattern with monthly charges

{image link}

Graph Notes
- Blue plots | No Churn         
- Red plots | Churn


Key Takeaways
- Customers who churned had higher on-average monthly charges.

---
#### Exploring Churn pattern with Tenure.

{image link}

Key notes

- Chances of customer turning down the service during the first year of operation are highest at 47.68%
- The longer the customer keeps using the service, the lesser are their chances of churning.

## Modeling

#### Outcome variable
- Using this model, we are trying to predict what amount of our customers may churn by the end of this year.
- Predicting the future churn can be used in targeting retention to customers likely to churn. 
- Retaining customers and acquiring new ones can help business achieve the solution proposed by marketing and data team.


#### Features
While predicting customer churn, we found following variables to be highly important,
- Contract : The duration of contract. (monthly, 1 year or 2 year)
- Tenure: Fow how long the customer has been using the service.
- Online Security: has customer opted for online security or not.
-  Monthly Charges: the monthly billed amount.

Refer this File for full list of features.


#### Random Forest
Random Forest will be a perfect fit for our problem as
- The dataset is showcasing complex relationships among multiple features.
- It provides feature importance which can be used to understand the factors driving customer to churn.
- The ensemble effect will result in more stable and reliable model.

#### Training, testing and predicting data
- The data acquired from 1st january, 2023 – 1st october, 2023 will be used to train the model.
- A 20% randomly selected section of that data will be used to evaluate the model, to check whether the model is performing upto mark or not.
- Using the trained model, we will predict churn among customers who joined out service from october 1st to november 10th, 2023.
