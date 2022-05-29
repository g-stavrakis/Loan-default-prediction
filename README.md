## Business Context

A major bank wants to pilot a new product, a short-term credit line with the limit of £25,000 and line of 1 month with interest of 2% per month. Then assume that the client who was issued credit and repaid it will more likely use your bank for similar short-term financing needs in the future, which has an additional lifetime value (CLV) of £1,000. However, if the client will default, then you will be able to recover only £20,000 out of £25,000 granted.

- Potential profits for bank if client does not default:  25,000*2% + 1,000 = £1,500
- Potential losses for bank if client default:  25,000 - 20,000 = £5,000
- If the credit is not issued to the client:  profit = loss = 0

 ## Aim of the project
The bank wants to better predict the likelihood of default for its customers, as well as identify the key drivers that determine this likelihood, to inform its future strategy, including their planning of issuing its new short-term credit line to its more reliable customers. 


## Data

The dataset that was provided for this project contained various information about 25,000 bank clients, including demographic factors, credit data, history of payment, and bill statements from April to September, as well as information on whether the customer default or not in October.
Of those 25,000 clients, 1,000 were randomly selected as the test set and stored on “New_applications.csv” file and the remain 24,000 on “Credit_data.csv”, which was used to train and validate the model. 


## Overview of the analysis

-	Creating Prediction Model based on existing clients
  - Importing and inspecting the data
  -	Pre-processing the data
  -	Feature engineering 
  -	Building the logistic regression model
  -	Selecting a Threshold that maximize bank’s profits
  -	Retraining the model with combined train and validation set
-	Using the Model on new applicants of the pilot
  -	Importing and inspecting the data for new applicants 
  -	Pre-processing the data
  -	Predicting default clients in the new applicants
