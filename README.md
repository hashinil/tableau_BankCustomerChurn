# :runner::two_men_holding_hands::two_men_holding_hands: Bank Customer Churn Dashboard:bank::moneybag: 

[Final Dashboard](https://public.tableau.com/app/profile/hashini.liyanage/viz/BankCustomerChurn_16981592629460/Story1#1)

####

![image](https://github.com/hashinil/tableau_BankCustomerChurn/assets/33922245/c7d91b5a-9774-4d93-a038-a251b5997570)





## What is customer churn?
- Known as customer attrition/ customer defection
- Is a business metric that calculates the number of customers who leave or stop using a company's product or service over a specific time period.
  
  **Churn rate percentage = (Number of customers lost during that time period / Number of customers at the start of the time period) X 100**

## Why is churn rate important?
- Churn rates are important because losing customers means losing revenue
- It's a crucial metric for businesses in various industries as it directly impacts revenue and profitability.
- High churn rates can have a significant negative impact on a business's revenue and profitability.
- Acquiring new customers is often more expensive than retaining existing ones, so reducing churn is cost-effective.

## Reasons for Churn
- Dissatisfaction with the product or service.
- Competitive offerings or better alternatives.
- Changes in the customer's circumstances.
- Poor customer service or support.
- Pricing issues.
- Lack of engagement or utilization.

## How to reduce churn rate
- Understanding and managing churn rate is essential for maintaining a healthy customer base and sustaining a business's growth.
- Customer churn analysis is a common and valuable use case for businesses to understand why customers leave and what can be done to retain them.
- To reduce customer churn, businesses often implement retention strategies, such as improving product quality, offering loyalty programs, providing excellent customer service, and tailoring marketing efforts to re-engage customers.

---------------------------------------------------

### Customer churn analysis
##### Step 1: Data Collection:
- [Datasheet](https://github.com/hashinil/tableau_Customer_churn/blob/main/Customer-Churn-Records.csv) 
- Customer demographics, transaction history, support interactions, and any other data that might be related to customer behavior.
- Feedback and Customer Surveys: Collecting feedback from departing customers can be valuable for understanding why they're leaving and making improvements based on their input.

##### Step 2: Data Preprocessing:
- Clean and preprocess your data.
    - This involves dealing with missing values, outliers, and any other data anomalies.
- Feature engineering:
    - Create new features or transform existing ones that could be useful for your analysis, like customer tenure, usage patterns, or customer segment.

##### Step 3: Exploratory Data Analysis (EDA):
- Visualize and analyze the data to gain insights into customer behavior.
- Identify patterns and correlations that may be related to churn.
- Identify what factors contribute to churn, and can you predict which customers are likely to churn?
- **Findings:**
    - *There is high churn rates for custermers older then 50.*
    - *Their is no clear relationship with Tenure.* (Tenure: length of time a customer remains a customer)
    - *Customers who are active and not colmplain have less posibility of churn.*
    - *Almost all the Customers who colmplain have left the bank.*
    - *Customers who have 0-7 years Tenure with **Gold card type** are having less churn rate than  **Diamond card type**.*
    - *Customers who is having 3 or 4 products have more churn rate.*
    - *There is no visible relationship with Satisfaction Score and churn rate* **But it is a common fact, may be this dta set is not enough to prove it.**
    - *Customers who is having less points have more churn rate.*

##### Step 4: Communication:
- Prepare a tableau dashboard to summarizing findings and recommendations
- Communicate the insights you gain can help businesses make data-driven decisions to retain customers and improve their overall satisfaction
- [Final Dashboard](https://public.tableau.com/app/profile/hashini.liyanage/viz/BankCustomerChurn_16981592629460/Story1#1)

---------------------------------------------------

### Steps followed to create dashboard:

1.  Loaded data sheet to **Tableau**.

2.  Created **Calculated Fields**.
   
    - No of Customers: **COUNT([Customer Id])**
    - No of Unique Customers: **COUNTD([Customer Id])**
    - Number of Churned Customers: **SUM([Exited])**
    - Churned rate: **[3 Number of Churned Customers]/[1 Number of Customers]**

3.  Create WorkSheets for **No of Customers, No of Churned Customers, Churned Rate, Avg Age and No of Products**.

Checked **Avg Num of Products** and **Avg Age**. Then changed number format(Decimal). 
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/6d384de8-8673-4ba6-81c1-3090e53edfbe)
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/4a12bb86-a2dd-42be-82e4-aa9a7e69c6f1)

4.  Created bins for **Age**, size =5

5.  Created **Churn by Age** chart.

    **Findings:**
      - *There is high churn rates for custermers older then 50.*
        
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/e0e8a55a-552c-4edf-a4de-23df1506b94c)

6.  Created **Churn by Tenure** chart.
   
    **Findings:**
      - *Their is no clear relationship with Tenure.* (Tenure: length of time a customer remains a customer)
        
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/96a7b19c-4605-4ccf-83a0-4768643ea5d9)

7.  Changed **Geography** column and generate Latitude and longitude. Created **Churn by Country** chart. *Higher churn rate in GERMANY.*
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/c8233868-4070-41a7-92cf-f7a1f0946baa)
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/b8fa350c-1389-4791-8fb0-658379a25422)

8.  Changed values to **Discrete** and Marks to **Square** (Change background color)
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/9634ca8c-9d3e-4aa2-a033-a4e5e119e6ca)

9.  Created **Churn by Active Member and Complains** chart.
   
     **Findings:**
      - *Customers who are active and not colmplain have less posibility of churn.*
      - *Almost all the Customers who colmplain have left the bank.*

![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/2e9c62d6-88fe-4ac0-924e-8be9bad9b72d)

10.  Created **Churn by Card Type** chart.

     **Findings:**
      - *Customers who have 0-7 years Tenure with **Gold card type** are having less churn rate than  **Diamond card type**.*
      
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/d1f3f1b7-654d-4aa7-a57e-902ee6007ff7)

12.  Created **Churn by No of Products** chart.

     **Findings:**
      - *Customers who is having 3 or 4 products have more churn rate.*
      
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/ab86a27a-3ec5-4e53-a5c0-187d0f0d71e9)

13.  Created **Churn by Satisfaction Score** chart.

     **Findings:**
      - *There is no visible relationship with Satisfaction Score and churn rate* **But it is a common fact, may be this dta set is not enough to prove it.**
  
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/d8a4c4eb-19a6-4875-a71c-27c6f3f16d49)

14.  Created bins for **Point Earned**, size =50
15.  Created **Churn by Point Earned** chart.

     **Findings:**
      - *Customers who is having less points have more churn rate.*
  
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/063ef978-21a9-4f73-b373-ba36064b28b3)

16.  Create 3 dashboards with created sheets above.
    
18.  Created **Story** with dashboards.
