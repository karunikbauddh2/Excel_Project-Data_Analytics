# Project 2
## Introduction
As electric vehicles (EVs) continue to reshape the automotive industry, understanding adoption trends, manufacturer performance, vehicle types, and regional distribution has become increasingly important. This project explores EV registration data to uncover key insights into the growth and evolution of the electric vehicle market.
Using Excel's advanced data analysis capabilities, I built an interactive dashboard to analyze EV registrations, manufacturer performance, vehicle classifications, utility providers, and geographic trends.

### Questions Analyzed

To better understand the EV market, I explored the following questions:

1. How is the EV market split between Battery Electric Vehicles BEVs and PHEVs?  
2. How has EV production evolved over time? And what will the next 10 years look like for EVs?
3. What are the Top 10 manufacturers by market share?  
4. What are the Top 10 EV Models?  
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
<img width="1366" height="727" alt="image" src="https://github.com/user-attachments/assets/8fd3cdc0-b5ec-47c9-bd7c-ab53dcec1a68" />  
 


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

### 📈 Skill: Pivot Chart, Slicer & Forecasting  

**Pivot Chart & Slicer**  
- 🔢 I created a Pivot Chart with Pivot Query using the Model Year.    
- 📊 I also connected a Slicer with the Pivot Chart to easily filter through different car manufaturers.   
<img width="806" height="294" alt="image" src="https://github.com/user-attachments/assets/1fdb5909-a954-47a1-bce3-868834d6af05" />  

  
⛅**Forecasting**     

- 🔢 With the same Pivot Chart I created a forecast of EV production for the next 10 years.  
<img width="650" height="314" alt="image" src="https://github.com/user-attachments/assets/99ddd9b6-b475-4034-bade-2375fff578b1" />  


📊 **Analysis**

- Annual EV registrations were analyzed using a trend chart to identify adoption patterns over time.  
- Long-term demand for EVs remains positive.

💡 **Insights**  
- EV registrations have grown substantially in recent years.  
- Forecasts indicate a recovery and steady increase in EV production through 2036.
  
🤔 **So What?**  

The upward trend highlights the accelerating transition toward electric mobility and the increasing role EVs play in the automotive industry.  


## 3️⃣ What are the Top 10 manufacturers by market share?  
### 🧮Skills: PivotTables & DAX  
📈**Pivot Table**  

- 🔢 I created a PivotTable using the Data Model I created with Power Pivot.  
- 📊 I moved the Make to the rows area. 
- 🧮 Then I added new measure to calculate the count of model produced by every make.  
```excel
=COUNT(Top_10_Manufacturers[Make])
```
💡 **Insights**  
- A small group of manufacturers dominates the EV market.  
- Leading brands contribute a significant share of total EV registrations.
<img width="660" height="319" alt="image" src="https://github.com/user-attachments/assets/54ce087e-0ad9-47af-8382-e9d180e13298" />  


🤔 **So What?**  

Understanding market leaders helps identify companies driving innovation and consumer adoption within the EV industry.  

## 4️⃣ What are the Top 10 EV Models?  
📈 **Skill: Ranking Analysis** 

- Grouped Rows together and counted each model.
- Added a custom column with Power Query Formula to get only the top model of every manufacturer.
 ```excel
 = Table.AddColumn(#"Grouped Rows", "Custom", each Table.First([Top_Model]))
```
<img width="1366" height="728" alt="image" src="https://github.com/user-attachments/assets/ef0477c9-c5c4-4611-a18c-c825b151a48a" />  

- Plotted the custom values in the Pivot Table and made a Pivot graph explaining the Top 10 ranked EV Model.
  
<img width="486" height="294" alt="image" src="https://github.com/user-attachments/assets/ae177969-8d1a-48c2-9079-effbe93ba69f" />  


💡 Insights  

- Certain EV models consistently outperform competitors in registrations.  
- Top-selling models demonstrate strong market acceptance and brand loyalty.
  
🤔 **So What?**  

Popular models provide insight into the features and vehicle segments most valued by consumers.  

## 5️⃣ Which electric utility providers serve the largest EV owner base?
