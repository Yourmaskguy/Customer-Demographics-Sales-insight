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
2. Sales by Customer Type and Branch: How do total sales compare between members and non-members in each branch?
3. Customer Satisfaction by Gender: What is the average customer satisfaction rating by gender?
4. Average Purchase Amount by Gender: Is there a significant difference in the average total purchase amount between male and female customers?
5. Quantity Purchased by Customer Type: How does the quantity of products purchased vary by customer type (member vs. non-member)?
6. Peak Shopping Hours by Gender: What are the peak shopping hours for male and female customers?
7. Payment Method by Total Sales: Which payment method (Cash, Credit card, Ewallet) is most popular based on total sales?
