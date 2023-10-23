# tableau_Customer_churn


Customer churn, often referred to as customer attrition or customer defection, is a business metric that calculates the number of customers who leave or stop using a company's product or service over a specific time period. It's a crucial metric for businesses in various industries as it directly impacts revenue and profitability. Customer churn can occur for various reasons, and understanding and managing it is essential for maintaining a healthy customer base and sustaining a business's growth.


Customer churn analysis is a common and valuable use case for businesses to understand why customers leave and what can be done to retain them.


 Reasons for Churn: Customer churn can result from a variety of factors, including:

          Dissatisfaction with the product or service.
          Competitive offerings or better alternatives.
          Changes in the customer's circumstances.
          Poor customer service or support.
          Pricing issues.
          Lack of engagement or utilization.

Impact on Business: High churn rates can have a significant negative impact on a business's revenue and profitability. Acquiring new customers is often more expensive than retaining existing ones, so reducing churn is cost-effective.


 Retention Strategies: To reduce customer churn, businesses often implement retention strategies, such as improving product quality, offering loyalty programs, providing excellent customer service, and tailoring marketing efforts to re-engage customers.


 Feedback and Customer Surveys: Collecting feedback from departing customers can be valuable for understanding why they're leaving and making improvements based on their input.

 

Identify what factors contribute to churn, and can you predict which customers are likely to churn? 
the insights you gain can help businesses make data-driven decisions to retain customers and improve their overall satisfaction

Data Collection:
customer demographics, transaction history, support interactions, and any other data that might be related to customer behavior.

Data Preprocessing:
- Clean and preprocess your data.
    - This involves dealing with missing values, outliers, and any other data anomalies.
- Feature engineering:
    - Create new features or transform existing ones that could be useful for your analysis, like customer tenure, usage patterns, or customer segment.


Exploratory Data Analysis (EDA):

- Visualize and analyze the data to gain insights into customer behavior.
- Identify patterns and correlations that may be related to churn.


Communication:

Prepare a tableau dashboard to summarizing findings and recommendations
Communicate your results to stakeholders.


### Steps

1.  Load data sheet to **Tableau**.
2.  Create **Calculated Fields**.
   
    - No of Customers: **COUNT([Customer Id])**
    - No of Unique Customers: **COUNTD([Customer Id])**
    - Number of Churned Customers: **SUM([Exited])**
    - Churned rate: **[3 Number of Churned Customers]/[1 Number of Customers]**

3.  Check **Avg Num of Products** and **Avg Age**. then change number format(Decimal) 
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/6d384de8-8673-4ba6-81c1-3090e53edfbe)
![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/4a12bb86-a2dd-42be-82e4-aa9a7e69c6f1)






![image](https://github.com/hashinil/tableau_Customer_churn/assets/33922245/c8233868-4070-41a7-92cf-f7a1f0946baa)
