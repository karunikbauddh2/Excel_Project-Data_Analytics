# Project 2
## Introduction
As electric vehicles (EVs) continue to reshape the automotive industry, understanding adoption trends, manufacturer performance, vehicle types, and regional distribution has become increasingly important. This project explores EV registration data to uncover key insights into the growth and evolution of the electric vehicle market.
Using Excel's advanced data analysis capabilities, I built an interactive dashboard to analyze EV registrations, manufacturer performance, vehicle classifications, utility providers, and geographic trends.

### Questions Analyzed

To better understand the EV market, I explored the following questions:

1. How is the EV market split between Battery Electric Vehicles BEVs and PHEVs?  
2. How has EV production evolved over time? And what will the next 10 years look like for EVs?
3. What are the Top 10 manufacturers by market share?  
4. What are the Top 10 even Models?  
5. Which electric utility providers serve the largest EV owner base?  

### Excel Skills Used  
The following Excel skills were utilized for analysis:

📊 Pivot Tables  
📈 Pivot Charts  
🧮 DAX (Data Analysis Expressions)  
🔍 Power Query  
💪 Power Pivot  

### EV Dataset  

The dataset used for this project contains real-world electric vehicle registration records and includes information such as:

🚗 Vehicle Make  
🚙 Vehicle Model  
⚡ Electric Vehicle Type  
📍 State / Location  
🔋 Electric Range  
🏢 Electric Utility Provider  
📅 Model Year  
🏭 Manufacturer  

## 1️⃣ How is the EV market split between Battery Electric Vehicles BEVs and PHEVs?  
### 🔍 Skill: Power Query  
🔄 **Transform**  
I changed the query by renaming the state abbreviations, removing null values, adding index column and reordered the columns.   
<img width="243" height="217" alt="image" src="https://github.com/user-attachments/assets/8931574a-771c-44da-90d4-3920170c592c" />  

🔗**Load**  
Finally, I loaded the query into the workbook, setting the foundation for my subsequent analysis.
<img width="1366" height="728" alt="image" src="https://github.com/user-attachments/assets/bbaf8aba-2ca7-4b60-9441-fcdac3e7e9dd" />  


📊 **Analysis**  

Vehicle registrations were categorized into:  

- Battery Electric Vehicles (BEVs)  
- Plug-in Hybrid Electric Vehicles (PHEVs)  

💡 **Insights**  

- BEVs account for the majority of registered electric vehicles.  
- PHEVs represent a smaller but still significant segment of the EV market.
  <img width="477" height="288" alt="image" src="https://github.com/user-attachments/assets/ef916580-de3c-4a64-970a-7fabab094c77" />  


🤔 **So What?**  

📈The growing preference for fully electric vehicles indicates increasing consumer confidence in EV technology, charging infrastructure, and battery performance.  

## 2️⃣ How has EV production evolved over time?  And what will the next 10 years look like for EVs?

### 📈 Skill: Pivot Charts, Slicer & Forecasting  
**Pivot Chart & Slicer**  


📊 **Analysis**

Annual EV registrations were analyzed using a trend chart to identify adoption patterns over time.

💡 **Insights**  
- EV registrations have grown substantially in recent years.  
- The strongest growth occurred during the latest model years, reflecting increased consumer demand.
  
🤔 **So What?**  

The upward trend highlights the accelerating transition toward electric mobility and the increasing role EVs play in the automotive industry.  


## 3️⃣ What are the Top 10 manufacturers by market share?  
### 🧮Skills: PivotTables & DAX  
📈**Pivot Table**  

🔢 I created a PivotTable using the Data Model I created with Power Pivot.  
📊 I moved the Make to the rows area. 
🧮 Then I added new measure to calculate the count of model produced by every make.  
```excel
=COUNT(Top_10_EV_Makers[Make])
```
💡 **Insights**  
- A small group of manufacturers dominates the EV market.  
- Leading brands contribute a significant share of total EV registrations.
<img width="633" height="331" alt="image" src="https://github.com/user-attachments/assets/47f1f386-2eb7-4a27-8321-d4ad17ddab6e" />

🤔 **So What?**  

Understanding market leaders helps identify companies driving innovation and consumer adoption within the EV industry.
