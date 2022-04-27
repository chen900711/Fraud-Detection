# Fraud-Detection
### Credit Card Fraud Detection
In this project, we are using SQL skills to analyze historical credit card transactions and consumption patterns in order to identify possible fraudulent transactions.

### Data Modeling:
First of all, we created on MySQL a database called frauddetectingproject, then imported five CSV data files to MySQL. Then, we created some Views according to the consumption patterns.

### Data Engineering:
We created a database schema on MySQL and imported our database from the CSV files provided. Using our database model as a blueprint, we created a database schema for each of our tables and relationships. We specified data types, primary keys and foreign keys. After creating the database schema, we imported the data from the corresponding CSV files.

### Data Analysis:
In this part, we will analyze the data and then create some views to show our findings. We will make some consumption patterns according to following scenarios:

According to time, which time frame the fraud transaction might be happended? Consider the time period 7:00 a.m. to 9:00 a.m.
  1. What are the 100 highest transactions during this time period?
  2. Do we see any fraudulent or anomalous transactions?

According to transaction amount, some fraudsters hack a credit card by making several small payments (we consider the transaction amout less than $2.00), which are typically ignored by cardholders. Count the transactions that are less than $2.00 per cardholder. 
   1. Is there any evidence to suggest that a credit card has been hacked?
   2. What are the top five merchants prone to being hacked using small transactions?

Once we have a query that can be reused, we will create a view for each of the previous queries. Then, we will analyze our findings to verify our consumption patterns.

### Improvement
In the future, we could detecting fraud transactions according to two main sections client's background and consumption habits. In the client's background, we should analyze the suspicious transaction according to client's age, education background, position, location, and gender. In the client's consumption habits, we need to consider the client's shopping area, stores, and time. Based on those two sections, we could create some grading system to detect and flag the suspicious transactions to verified with client.
