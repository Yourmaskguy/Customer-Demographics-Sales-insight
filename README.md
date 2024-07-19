# Customer Demographics and Sales insight

### Project Overview

This project involves analyzing customer demographics and sales data to uncover key insights and trends. The primary objectives are to understand customer behavior, identify high-value customer segments, and improve sales strategies based on data-driven insights.

### Data Source

Capstone Data: The primary dataset used for this analysis is the "capstone data.csv" file, containing detailed information about customer demographics and sales records.The dataset is provided as part of a capstone project and is available for download [here](https://docs.google.com/spreadsheets/d/1SCc8RT-ckz2B5BhcDQ8DOarPRgIWmU7S/edit?usp=drive_link&ouid=105676808417011957014&rtpof=true&sd=true)

### Data Description:

The dataset comprises the following columns:

•	Invoice id: Computer generated sales slip invoice identification number.


•	Branch: Branch of supercenter (A, B, and C).

•	City: Location of supercenters.

•	Customer type: Type of customers (1 for Members, 0 for Normal customers).

•	Gender: Gender of customer (M for Male, F for Female).

•	Product line: General item categorization groups.

•	Unit price: Price of each product in $.

•	Quantity: Number of products purchased by customer.

•	Tax: 5% tax fee for customer buying.

•	Total: Total price including tax.

•	Date: Date of purchase (January 2019 to March 2019).

•	Time: Purchase time (10am to 8pm).

•	Payment: Payment method used by customer (Cash, Credit card, Ewallet).

•	COGS: Cost of goods sold.

•	Gross margin percentage: Gross margin percentage.

•	Gross income: Gross income.

•	Rating: Customer satisfaction rating (scale of 1 to 10).

### Tool

-Excel [Download-here](https://www.microsoft.com/en-us/microsoft-365/excel)

### Microsoft Excel Skills/Concepts applied:

1. Data Cleaning
2. Excel Formulas (IF etc.)
3. Conditional Formatting
4. Cell Referencing
5. Pivot Tables/Charts
6. Slicers
7. Data Visualization
8. Dashboard Building

### Data Cleaning/Preparation

Data Cleaning
The data cleaning process involved several steps to ensure data quality and consistency. The following actions were performed:

1. Checking for Spelling Errors, Duplicate Values, and Null Values:
- Ensured there were no spelling mistakes in categorical fields.
- Removed duplicate entries from the dataset.
- Identified and handled null values appropriately.

2. Changing Customer Type Values:

I used the IF function to change the customer type values from 0 and 1 to Members and Normal Customers, respectively.
Formula used: 

```excel
=IF(A1 = 1, "Member", "Normal Customer")
```

![Customer Type](https://github.com/user-attachments/assets/39813c92-13ff-4acb-a5b5-fa7ce0202609)


3. Replacing Gender Abbreviations:

I used the Find and Replace tool in Excel to change the gender abbreviations:
FM to Female
M to Male

![gender](https://github.com/user-attachments/assets/94792a3c-bc5e-41de-b1fb-7ff3b0b53412)


4. Formatting Numerical Values as Currency:

Converted the Unit Price, Tax 5%, Total, COGS, and Gross Income columns to currency format.

![currency](https://github.com/user-attachments/assets/b760925c-2484-4575-a195-8ac26b0e70d3)


### Exploratory Data Analysis (EDA)

In this project, Exploratory Data Analysis (EDA) was performed to gain insights into customer demographics, purchasing behaviors, and sales performance. The following key questions guided the analysis:
1. Customer Distribution by Gender and Branch: What is the distribution of customers by gender across different branches?
2. Total Sales by Customer Type and Branch: How do total sales compare between members and normal customer in each branch?
3. Customer Satisfaction by Gender: What is the average customer satisfaction rating by gender?
4. Average Total Purchase Amount by Gender: Is there a significant difference in the average total purchase amount between male and female customers?
5. Total Quantity Purchased by Customer Type: How does the quantity of products purchased vary by customer type (member vs. normal customer)?
6. Peak Shopping Hours by Gender: What are the peak shopping hours for male and female customers?
7. Payment Method by Total Sales: Which payment method (Cash, Credit card, Ewallet) is most popular based on total sales?

### Detailed Overview Of The Analysis

1. Customer Distribution by Gender and Branch

Description: Analyzed the distribution of customers by gender across different branches.

Visualization: Clustered Column chart showing the number of male and female customers in each branch.

Branch A: 179 males, 161 females  
Branch B: 170 males, 162 females 
Branch C: 150 males, 178 females 

![git 1](https://github.com/user-attachments/assets/ce24a29f-7c64-4365-8434-de641a0fd5fe)


Key Insight: 

Branches attract both genders fairly equally, with Branch C having more female customers.

2. Total Sales by Customer Type and Branch

Description: Compared total sales between members and normal customer in each branch.

Visualization: Pivot table and clustered bar chart showing sales figures for each customer type across branches.

Branch A: 
- Normal Customer: $52,562.90
- Members: $53,637.48  

Branch B:
- Normal Customer: $52,492.99
- Members: $53,704.69 

Branch C:
- Normal Customer: $53,687.42
- Members: $56,881.28 

![git 2](https://github.com/user-attachments/assets/5b49f472-b0d7-4402-af31-c2d5dd3f4e27)

Key Insights:

Membership programs positively impact sales, with members spending more.

3. Customer Satisfaction by Gender

Description: Calculated the average customer satisfaction rating by gender.

Visualization: Clustered Column chart showing average satisfaction ratings for male and female customers.

Female: 6.96  

Male: 6.98  

![git 3](https://github.com/user-attachments/assets/f1f06932-449d-4238-8cb5-7d2f34439b9d)

Key Insights:

Both genders report similar satisfaction levels, indicating consistent service quality.

4. Average Total Purchase Amount by Gender

Description: Analyzed the difference in average total purchase amounts between male and female customers.

Visualization: Pie chart showing average purchase amounts for each gender.

Female: $335.10 

Male: $310.79  

![git 4](https://github.com/user-attachments/assets/796ff3f2-d210-4bf0-a2fa-d4aff964ac3e)

Key Insights:
Female customers have a higher average transaction value.

5. Total Quantity Purchased by Customer Type

Description: Examined how the quantity of products purchased varies by customer type.

Visualization: Pivot table and bar chart showing average quantity purchased by each customer type.

Normal Customer: 2,725  

Members: 2,785  

![git 55](https://github.com/user-attachments/assets/65cc4112-94d1-4dbc-9d3e-250b962706e4)


Key Insights:

Members purchase slightly more products on average.


6. Peak Shopping Hours by Gender

Description: Identified peak shopping hours for male and female customers.

Visualization: Line graph showing shopping frequency by hour for each gender.

10 AM: Female - 62, Male - 39  

11 AM: Female - 47, Male - 43  

12 PM: Female - 46, Male - 43  

1 PM:   Female - 61, Male - 42

2 PM:   Female - 39, Male - 44 

3 PM:   Female - 42, Male - 60

4 PM:   Female - 36, Male - 41

5 PM:   Female - 38, Male - 36

6 PM:   Female - 45, Male - 48 

7 PM:   Female - 54, Male - 59

8 PM:   Female - 31, Male - 44

![git 6](https://github.com/user-attachments/assets/b8afa608-e9cd-4ee5-9aad-5a7470c251fb)


Key Insights:

Peak shopping times vary, with the highest activity around 3 PM for males and 10 AM for females.


7. Payment Method by Total Sales

Description: Analyzed which payment method (Cash, Credit card, Ewallet) is most popular based on total sales.

Ewallet: $109,993 

Credit Card: $100,767

Cash: $112,207

Key Insight:  

Cash is the most popular payment method, followed by Ewallet and then credit card.



### Dashboard Overview

![final](https://github.com/user-attachments/assets/4e77960e-7d61-45bb-84f7-51147215247b)

### Key Findings

Gender Distribution: Branches attract both genders equally, with a slight preference for females in Branch C.

Sales by Customer Type: Members contribute more to sales than normal customer across all branches.

Customer Satisfaction: Similar satisfaction levels for both genders. 

Average Purchase Amount: Female customers spend more on average than male customers.

Quantity Purchased: Members purchase slightly more products than normal customer.

Peak Shopping Hours: Peak times vary by gender, with females shopping more in the morning and males in the afternoon.

Payment Methods: Cash is the most popular, followed by Ewallet and credit cards.

### Recommendation

- Enhance Membership Programs: Leverage the higher spending and product quantity purchased by members to drive membership sign-ups.  
- Optimize Store Staffing: Adjust staffing levels to match peak shopping hours for males and females.  
- Targeted Promotions: Create gender-specific promotions to capitalize on spending habits.  
- Improve Payment Options: Encourage the use of cash and Ewallets with targeted incentives.

### Conclusion

By leveraging these insights and recommendations, the company can optimize its operations, improve customer satisfaction, and drive higher sales, positioning itself for sustained growth and success.

