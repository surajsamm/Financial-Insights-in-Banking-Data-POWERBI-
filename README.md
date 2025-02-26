# Financial-Insights-in-Banking-Data-POWERBI-

![image](https://github.com/user-attachments/assets/f8621e03-6fff-4e2f-9cb4-210447f9cb9c)             ![image](https://github.com/user-attachments/assets/c5924945-2aec-42e5-a498-3e157f4e2354)    ![image](https://github.com/user-attachments/assets/aaa7c822-f33e-4a48-bc74-fa6ce39953d0)




# Banking

### **Case Study: Unlocking Financial Insights in Banking Data**

### **Background**

As a data analyst at FinInsight Group, a consultancy specializing in banking analytics, you are equipped with two comprehensive datasets: 'Banking Transactions' and 'Customer Account Details'. The 'Banking Transactions' dataset records detailed transaction data, including types, amounts, dates, and branch information. The 'Customer Account Details' dataset provides insights into account holders, covering account types, balances, interest rates, credit scores, and loan amounts. Your expertise is crucial in a sector where financial data drives strategic decisions in customer relationship management, risk assessment, and product offerings.

### **Objective**

Your task is to employ Power BI to analyze these banking datasets, aiming to unravel the intricate patterns and behaviors within the data. This involves in-depth data cleaning, robust data modeling, and strategic use of DAX for complex analytics. Your goal is to create a comprehensive, interactive dashboard that not only illustrates transactional trends and customer profiles but also offers a holistic view of the banking ecosystem. This analysis should include understanding customer transaction behaviors, identifying relationships between account characteristics and financial health, and exploring factors influencing credit scores and loan management. Your insights will guide FinInsight Group in advising banking institutions on optimizing their services, enhancing customer satisfaction, and managing financial risks effectively.

### **Data Source:**

[BankingDataset1.xlsx](https://prod-files-secure.s3.us-west-2.amazonaws.com/d1e1bc70-9ede-4c69-84fd-42c5605803a0/a5a65b8a-cbbd-40f7-90e8-dbf57cb41048/BankingDataset1.xlsx)

The "BankingDataset1.xlsx" file contains the following columns:

1. **TransactionID**: A unique identifier for each transaction. 
2. **AccountNumber**: The account number associated with the transaction. (Foreign Key)
3. **TransactionType**: The type of transaction (e.g., Transfer, Deposit, Withdrawal, Payment).
4. **Amount**: The amount of money involved in the transaction.
5. **TransactionDate**: The date when the transaction occurred.
6. **BranchCode**: The code of the bank branch where the transaction took place.
7. **Currency**: The currency in which the transaction was made.
8. **TransactionTime**: The time of day when the transaction occurred (in hours).

[BankingDataset2.xlsx](https://prod-files-secure.s3.us-west-2.amazonaws.com/d1e1bc70-9ede-4c69-84fd-42c5605803a0/c32057d2-f4bf-491f-aaaf-25b20f52eb8e/BankingDataset2.xlsx)

The "BankingDataset2.xlsx" file contains the following columns:

1. **AccountNumber**: A unique identifier for each account, corresponding to 'AccountNumber' in "BankingDataset1.xlsx". (Primary Key)
2. **AccountHolder**: The name of the account holder.
3. **AccountType**: The type of account (e.g., Credit, Loan, Checking).
4. **Balance**: The current balance of the account.
5. **InterestRate**: The interest rate applicable to the account.
6. **CreditScore**: The credit score of the account holder.
7. **OpeningDate**: The date when the account was opened.
8. **LoanAmount**: The amount of loan associated with the account (if applicable).
9. **AccountHolderDetails:** Details about account holders - employment sector, years at current residence, and city of residence etc.

### **Part 1: Data Cleaning, Modeling, and DAX in Power BI**

1. **Data Importing and Initial Examination**
    - Import both datasets into Power BI. Perform a preliminary examination of the data. Identify any data quality issues or inconsistencies.
2. **Merging and Relating Datasets**
    - Merge the datasets using a suitable column as a key. Ensure that the merge is accurate and retains all necessary information.
3. **Cleaning: Handling Missing and Irrelevant Data**
    - Identify and address missing data in both datasets. Address duplicate entries and irrelevant data points, ensuring data quality.
4. **Data Type Conversion**
    - Transform and normalize data where necessary for consistency across datasets.
5. **Categorizing Transaction Types**
    - Create a new column categorizing transactions into broader categories based on 'TransactionType'. What categories did you create?
6. **Analysis of Account Balances**
    - Calculate the average account balance for each account type. Which account type has the highest average balance?
7. **Currency Exchange Rate Impact**
    - Analyze the impact of currency exchange rates on transaction amounts. Convert all transactions to a standard currency for comparison.
8. **Branch Activity Analysis**
    - Investigate which branch (identified by 'BranchCode') has the highest number of transactions.
9. **Interest Rate and Balance Correlation**
    - Using DAX, analyze the correlation between interest rates and account balances. Does a higher interest rate correlate with higher balances?
10. **Loan Amount and Credit Score Relation**
    - Examine the relationship between loan amount and credit score. Do higher credit scores correlate with larger loan amounts?
11. **Transaction Trends Over Time**
    - Analyze transaction trends over time. Are there any noticeable patterns or seasonal fluctuations?
12. **Customer Loyalty Analysis**
    - Calculate the duration of each account's relationship with the bank (from 'OpeningDate' to the most recent transaction date). Who are the longest-standing customers?
13. **High-Value Transaction Analysis**
    - Identify high-value transactions and analyze their characteristics. What constitutes a high-value transaction in your analysis?
14. **Analysis of Transaction Time Patterns**
    - Investigate if there are patterns in the times of day when different types of transactions are made.
15. **Credit Score Distribution**
    - Analyze the distribution of credit scores among account holders. What insights can you gather?
16. **Correlation Between Account Age and Balance**
    - Explore if there's a correlation between the age of an account (time since opening) and its current balance.
17. **Performance Rating of Branches**
    - Create a measure to rate branches based on transaction volume and value.
18. **Extracting Key Information**
    - Create new columns in the dataset that extract the employment sector, years at current residence, and city of residence from the 'AccountHolderDetails' column. Each piece of information should be in its own separate column.
19. **Advanced DAX: Risk Assessment Model**
    - Using DAX, develop a risk assessment model based on transaction patterns, account balances, and credit scores.
20. **Customer Demographics and Transaction Behavior**
    - Analyze transaction behavior based on customer demographics inferred from account data.
21. **Branch and Account Type Influence on Transactions**
    - Investigate if certain branches or account types have a significant influence on the types and values of transactions.
22. **Predictive Modeling for Account Growth**
    - Use DAX to create a predictive model estimating future account growth based on historical transaction and balance data.
23. **Data Modeling: Time Series Forecasting of Transactions**
    - Perform time series forecasting of transaction volumes using historical data. What are the predicted transaction volumes for the next quarter?
24. **Advanced Data Transformation: Identifying Unusual Transactions**
    - Using Power BI's data transformation capabilities, identify any unusual transactions (e.g., unusually high amounts, rare transaction types).

### **Part 2: Dashboard Building**

1. **Comprehensive Banking Dashboard**
    - Create a dashboard in Power BI showcasing key metrics such as transaction volumes, account balances, loan amounts, and credit scores. Include filters for account types, branches, and currencies.
2. **Dashboard Design and Functionality**
    - Focus on the dashboard's design and functionality. Ensure it is user-friendly, visually appealing, and provides interactive elements.
3. **Time-Based Analysis in Dashboard**
    - Incorporate time-based analysis in your dashboard, such as trends in account opening and transaction patterns over time.
4. **Interactive Analysis of Loan Data**
    - Create an interactive section for analyzing loan data, including loan amounts, interest rates, and credit scores.
5. **Visualization of Transaction and Account Data**
    - Implement visualizations that display transaction and account data effectively, providing insights into customer behavior and bank operations.
6. **Key Insights and Data Storytelling**
    - Provide a section summarizing key insights or stories from the data. Highlight significant findings or trends that emerged from your analysis.
