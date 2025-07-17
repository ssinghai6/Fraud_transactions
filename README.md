The following project is for determing fraud transactions

Usuage
- Ensure to have transactions.txt in folder data
- Crete a virtual env and run -> "pip install -r requirements.txt" (Installing all dependencies)
- transaction_Analysis.ipynb Jupyter notebook contains the following:
- Folder pickle_files contains (All trained ML models and processing pipeline)

WorkFlow in transaction_analysis.ipynb
    1. Data Loading  
    ↓  
    2. Transaction Analysis (Histogram & Box Plot)  
    ↓  
    3. Duplicate Transactions (Multi-swipe, Reversed)  
    ↓  
    4. Data Processing  
    - Feature Engineering  
    - Null Handling  
    - Encoding  
    - Downsampling (Class Imbalance)  
    ↓  
    Model Training  
    - Logistic Regression  
    - Random Forest  
    - XGBoost  
    - ANN  
    ↓  
    Model Evaluation (Precision, Recall, F1, AUC)  
    ↓  
    Model Selection (Best Performing Model)  
    ↓  
    Feature Importance  
    ↓  
    Conclusion


Based on the following Data Science challange:

Question 1: Load

- Programmatically download and load into your favorite analytical tool the transactions data. This data, which is in line-delimited JSON format, can be found here
- Please describe the structure of the data. Number of records and fields in each record?
- Please provide some additional basic summary statistics for each field. Be sure to include a count of null, minimum, maximum, and unique values where appropriate.


Question 2: Plot

- Plot a histogram of the processed amounts of each transaction, the transactionAmount column.
- Report any structure you find and any hypotheses you have about that structure.



Question 3: Data Wrangling - Duplicate Transactions
- You will notice a number of what look like duplicated transactions in the data set. One type of duplicated transaction is a reversed transaction, where a purchase is followed by a reversal. Another example is a multi-swipe, where a vendor accidentally charges a customer's card multiple times within a short time span.

- Can you programmatically identify reversed and multi-swipe transactions?
- What total number of transactions and total dollar amount do you estimate for the reversed transactions? For the multi-swipe transactions? (please consider the first transaction to be "normal" and exclude it from the number of transaction and dollar amount counts)
- Did you find anything interesting about either kind of transaction?

Question 4: Model
Fraud is a problem for any bank. Fraud can take many forms, whether it is someone stealing a single credit card, to large batches of stolen credit card numbers being used on the web, or even a mass compromise of credit card numbers stolen from a merchant via tools like credit card skimming devices.

- Each of the transactions in the dataset has a field called isFraud. Please build a predictive model to determine whether a given transaction will be fraudulent or not. Use as much of the data as you like (or all of it).
- Provide an estimate of performance using an appropriate sample, and show your work.
- Please explain your methodology (modeling algorithm/method used and why, what features/data you found useful, what questions you have, and what you would do next with more time)