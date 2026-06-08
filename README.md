# 🚲 Bike Sales Dashboard
 
An interactive Excel dashboard analyzing global bike sales data across multiple countries, product categories, age groups, and years.
 
---
 
## 📌 Introduction
 
This project presents a sales analytics dashboard built entirely in Microsoft Excel. It transforms raw transactional data into meaningful visual insights, enabling quick analysis of revenue, profit, units sold, and customer demographics. The dashboard is designed to give a clear picture of business performance across geographies, products, and customer segments.
 
---

### Dashboard File
My final dashboard is in...

### Excel Skills Used
The following Excel skills were utilized for analysis:

- 📉 Charts  
- 🧮 Formulas and Functions  
- ❎ Data Validation

  ### Dataset
The dataset used for this project contains real-world data from sales of Bikes accross vaious countries. The dataset is available on Keggal.com, here is the link [Title](https://www.kaggle.com/datasets/sadiqshah/bike-sales-in-europe/discussion/252420).
It includes detailed information on:  
- 📅 Order Date  
- 👥 Age Group  
- 🚻 Customer Gender  
- 🌍 Country  
- 🚴 Product Category  
- 📦 Order Quantity  
- 💰 Revenue  

## Dashboard Build
### 📈 Charts
<img width="940" height="516" alt="image" src="https://github.com/user-attachments/assets/171b212a-51bb-4a3d-b84f-f23285121dfa" />

- 🛠️ Excel Features: Utilized bar chart feature (with formatted revenue value) and optimized layout for clarity.
- 🎨 Design Choice: Vertical bar chart for visual comparison of revenue per year.
- 📉 Data Organization: Sorted years by ascending order for improved readability.
- 💡 Insights Gained: This enables quick identification of revenue, noting that 2015 saw the hghest revenue from Bike sales in Australia.

### 🗺️ Country wise Revenue - Map Chart

Insert Map Chart Here

- 🛠️ Excel Features: Utilized Excel's map chart feature to plot revenue globally.
- 🎨 Design Choice: Color-coded map to visually differentiate revenue levels across regions.
- 📊 Data Representation: Plotted revenue for each country with available data.
- 👁️ Visual Enhancement: Improved readability and immediate understanding of geographic revenue trends.
- 💡 Insights Gained: Enables quick grasp of global revenue distribution.


### 🧮 Formulas and Functions

💰 **Median Salary by Job Titles**  
  ```excel
=SUM(
   IF(
      (Main_Table[Year]=$D2)*
      (Main_Table[Country]=Country)*
      (Main_Table[Customer_Gender]=Gender)*
      (Main_Table[Product_Category]=Product),
      Main_Table[Revenue]
   )
)
```
- 🔍 Multi-Criteria Filtering: Filters records based on selected Year, Country, Customer Gender, and Product Category.
- 📊 Array Formula Logic: Uses the `SUM()` function with a nested `IF()` statement to evaluate multiple conditions simultaneously.
- 💰 Revenue Aggregation: Calculates the total revenue generated for the specified combination of filters.
- 🎯 Dynamic Analysis: Updates automatically when different criteria are selected, providing targeted sales insights.
- 📈 Formula Purpose: Powers the dashboard metrics by returning the total revenue for a specific year, country, gender, and product category combination.

🍽️ Background Table  
<img width="224" height="142" alt="image" src="https://github.com/user-attachments/assets/9d2895df-f7a0-43c1-8cf9-f7df3d6bdee4" />

### 💵Revenue by Gender Type
```excel
=SUM(
    IF(
       (Main_Table[Customer_Gender]=$P19)*
       (Main_Table[Year]=Year)*
       (Main_Table[Country]=Country)*
       (Main_Table[Product_Category]=Product),
       Main_Table[Revenue],
    FALSE
  )
)
```
- 🔍 Multi-Criteria Filtering: Filters records based on Customer Gender, Year, Country, and Product Category.
- 💰 Revenue Summation: Uses the SUM() function with a nested IF() statement to aggregate revenue only for matching records.
- 📊 Segment-Specific Analysis: Enables analysis of sales performance across different customer demographics, regions, and product categories.

### 🍽️ Background Table
<img width="250" height="60" alt="image" src="https://github.com/user-attachments/assets/82c45233-4cf8-4023-855d-d1595bdc0c4b" />  


📉 Dashboard Implementation:  
<img width="581" height="349" alt="image" src="https://github.com/user-attachments/assets/4d5d172b-d0df-44b1-89d7-97d60a30351c" />


### ❎ Data Validation  
🔍 Filtered List  
  - 🔒 Enhanced Data Validation: Implementing the filtered list as a data validation rule under the Year, Country, Gender and product category option in the Data tab ensures:
    - 🎯 User input is restricted to predefined, validated options
    - 🚫 Incorrect or inconsistent entries are prevented
    - 👥 Overall usability of the dashboard is enhanced  
  <img width="231" height="371" alt="image" src="https://github.com/user-attachments/assets/c167f212-302c-4a60-8b55-9dc9073e586c" />


## ✅ Conclusion
 
This Excel dashboard project demonstrates how raw transactional data can be transformed into an actionable business intelligence tool using only native Excel features.















