# Restaurant-Sales-Analysis-Project
This project analyzes restaurant sales transactions using Excel, covering price, quantity, payment method, purchase type, city, and manager performance. Outliers were identified and removed to ensure data accuracy. An interactive dashboard with slicers and charts provides valuable insights into sales distribution, and overall business performance.

## 📌 Overview
This project is based on open-source data for educational purposes. It represents a complete sales analysis for a restaurant in Egypt, focusing on 262 transactions. Although the dataset is relatively small in size, it allowed us to extract a wide range of insights, tables, and visualizations. The dataset includes order details such as product, price, quantity, purchase type, payment method, city, and manager. Data cleaning was performed to detect and remove outliers, ensuring accurate results. An interactive Excel dashboard with slicers and charts provides clear insights into sales performance, trends, and managerial impact across different branches.

## 📊 Project Details

**Tools Used:**
- Microsoft Excel  

**Dataset:**
- Sales data including:  
  `Order ID, Date, Day, Product, Correct Price, Price, Quantity, Revenue, Purchase Type, Payment Method, Manager, City`  

**Techniques Applied:**
- Data cleaning & formatting  
- Pivot tables & charts  
- Conditional formatting  
- Data modeling  
- Dashboard design  


## 📈 Key Insights

- **Data Size:** Although the dataset contained only 262 transactions, it provided rich insights into sales behavior and management performance.  
- **Outliers:** Detected and removed unrealistic price entries that significantly affected the mean, standard deviation, and overall distribution.  
- **Manager Performance:** Sales distribution showed varying performance across managers and branches, highlighting where management impacted revenue positively or negatively.  
- **Dashboard Features:** Interactive slicers for **Payment Method, Manager, City, Product** and visualizations (bar charts, pie charts, outlier analysis).  

## 🎯 Objectives

- To analyze restaurant sales transactions and extract meaningful insights.  
- To identify and remove data outliers for more accurate results.  
- To evaluate managers’ impact on sales across different branches and cities.  
- To understand customer behavior by purchase type and payment method.  
- To design an interactive Excel dashboard with slicers and charts for better decision-making.  
- To demonstrate how even a small dataset (262 rows) can generate valuable business insights.  


## 📈 Dashboard Preview
<img width="699" height="387" alt="Dashboard" src="https://github.com/user-attachments/assets/4fecf38d-9b02-4893-8ac4-3cfc99f5d280" />



## 📊 Statistics Preview
<img width="839" height="368" alt="Statistics" src="https://github.com/user-attachments/assets/66faaa5b-62bd-4a10-9d15-21c251bdc497" />




## 📑 Pivot Tables Preview
<img width="676" height="450" alt="Pivot Table" src="https://github.com/user-attachments/assets/fe2a14f1-6e80-4b0a-80a8-cd6c11506565" />




## ⚠️ Outliers Preview
<img width="898" height="461" alt="Outliers" src="https://github.com/user-attachments/assets/aec5f569-8765-4e86-a707-f80bfeb8e4c5" />








## 📝 Notes & Observations

- **Lowest orders but highest revenue:**  
  One specific day recorded the fewest transactions but generated the highest revenue, indicating larger purchase sizes or higher-value products sold.  

- **Outliers linked to one manager:**  
  All price outliers were traced back to a single manager in one branch, selling multiple products **in-store using credit card payments**. This suggests possible data entry errors or a recurring issue with the payment system.  

- **Revenue peaks:**  
  - Highest revenue day: **13 November**  
  - Lowest revenue day: **7 November**  

- **Correct Price validation column:**  
  A new column *Correct Price* was created using the following formula to automatically flag potential outliers:  
  ```excel
  =IF(OR([@Price]>AVERAGE([Price])+3*STDEV([Price]),
         [@Price]<AVERAGE([Price])-3*STDEV([Price])),
     "Outlier","OK")
"This method allowed quick detection of invalid entries and ensured more reliable analysis."


## 💡 Recommendations:

Monitor sales trends regularly to identify peak and low-performing days.

Investigate unusual transactions to ensure data accuracy and prevent errors.

Encourage managers to review branch-specific performance and apply best practices.

Optimize product pricing and promotions based on demand patterns.

Expand analysis with larger datasets or advanced BI tools for deeper insights.




## 🗂 Files in This Repository

Original Folder → The main Excel file containing data before cleaning ( Original Data.xlsx )


The Excel file containing Data Analysis Results ( Restaurant Sales Analysis Project 3.xlsx )



