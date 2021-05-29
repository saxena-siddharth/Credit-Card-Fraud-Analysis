
# Credit Card Fruad Detection Analysis

Credit card fraud can be stated as unauthorized use of credit or a debit card, or similar kind of payment to fraudulently obtain money or property. 

This project will involve making predictions by modeling past credit card transactions. Also, based on this model we detect whether the new transaction made is fraudulent or not. In this manner, we can help business owners, merchandisers to minimize fraud.

**Introduction**

The dataset contains data of credit card transactions made in September 2013 by the European cardholders. This dataset it states that 492 frauds have been detected out of 284,807 transactions in two days. This interprets that the data is highly imbalanced. The percentage of positive frauds of all transactions are 0.172%. As it involves confidential data, we just have following features V1 to V28 which are termed as the principal components. Apart from this we are been provided with time and transaction amount.

Standard Scaler is a typical tool when working with classification issues this way. It changes the data to where there is a mean of 0 and a standard deviation of 1, in this way, normalizing the information into a typical conveyance takes place. Particularly with taking a shot at such a wide scope of sums and time, we saw that scaling data before running the tests gave better outcomes.

Another issue to address is the profoundly imbalanced dataset. With numerous non-fraudulent transactions set up, we can actualize Random Under sampling to diminish the quantity of non-fraudulent transactions and match it to the measure of fraudulent transactions.

**Implementation**

With our dataset, we tried to implement our data analysis through CNN, heat maps and correlation matrix. This data analysis is in respect to the time, amount w.r.t V1 and V3. Our main goal was to understand how heat maps work with our dataset when convoluted with neural networks. In pre-processing and cleaning our dataset, we followed the following steps:

Gathering data.
Importing dataset and their respective libraries.
Remove missing values.
Dividing the dataset into dependent and independent variables.
Dealing categorical values and split into test and training sets.
Feature Scaling.
Exploratory Data Analysis


We then followed with XGBoost where we used both train-validation split and cross-validation to evaluate the model's effectiveness to predict class, wherein achieved AUC score 0.974 for validation set and 0.93 for the cross-validation set. We also performed random forest to test the accuracy of the train and test dataset.
