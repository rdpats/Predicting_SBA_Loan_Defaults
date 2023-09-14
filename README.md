# Loan-Default-Prediction

**Dataset:**
You are provided with the dataset. There were several changes made to the dataset: columns dropped/added.

The dataset is from the U.S. Small Business Administration (SBA).
The U.S. SBA was founded in 1953 on the principle of promoting and assisting small enterprises in the U.S. credit market (SBA Overview and History, US Small Business Administration (2015)).

Small businesses have been a primary source of job creation in the United States; therefore, fostering small business formation and growth has social benefits by creating job opportunities and reducing unemployment. There have been many success stories of start-ups receiving SBA loan guarantees such as FedEx and Apple Computer. However, there have also been stories of small businesses and/or start-ups that have defaulted on their SBA-guaranteed loans.

More info on the original dataset: https://www.kaggle.com/mirbektoktogaraev/should-this-loan-be-approved-or-denied


**Tasks:**

1.  Load & clean the dataset. Encode, replace missing values. Replace missing values, encode categorical variables, encode numerical variables as string
2.  Add engineered features
3.  - a.Train and tune ML models
    - b.Provide final metrics using Test (hold-out) dataset:
    - c.Classification: AUC
    - d.Confusion matrix for best F1
    - e.Interpret final trained model using Test dataset:
4.  Global feature importance using both Shapley values and permutation feature importance
        Summary plot with Shapley values

Output:

Feature Engineering: Decided upon the following engineered features to be added to the data set

![image](https://github.com/rdpats/Loan-Default-Prediction/assets/145058657/ab96bc7d-4fe4-4da5-a101-50664175d761)

Light GBM Model best parameters:

![image](https://github.com/rdpats/Loan-Default-Prediction/assets/145058657/e94931a3-609d-47b9-9c4a-37f02781dff3)

Light GBM Model AUC, Accuracy and F1:

![image](https://github.com/rdpats/Loan-Default-Prediction/assets/145058657/c83accf4-75b6-4419-9bb3-75b2d8ce0dcd)


Permutation Feature Importance:
![image](https://github.com/rdpats/Loan-Default-Prediction/assets/145058657/8e5150bd-9128-4029-90ee-d3c4cccfc554)

Permutation Variable Importance:
![image](https://github.com/rdpats/Loan-Default-Prediction/assets/145058657/5e8dc2e7-8cf5-4144-9e21-a86422e52e62)

Shapley Values:
![image](https://github.com/rdpats/Loan-Default-Prediction/assets/145058657/9d249136-e7b9-44db-a643-fd5aa04bf323)

The shapley values for the whole dataset tell us that Bank is the most important variable followed by City and Loan Utilization. They impact positively in the overall model.





