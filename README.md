#  Sales Analysis   - Dashboard

📊 Thrilled to unveil my latest endeavour: a comprehensive Sales Analysis project focused on profit and goods meticulously crafted using Power BI and Microsoft Excel! 🚀

 ## Here's what you can expect from this dashboard:

🛠️ Toolkit: Power BI, Microsoft Excel

📊 Datasets: Microsoft Excel

Project Overview:
Diving deep into sales Analysis, this project revolves around dissecting sales performance and turnover, comparison with previous year sale details with precision.

Here's what you can expect from this dashboard:

•	Sliced date time stamps scroll through select the date we can have a sales data for the particular date.	
•	Product line and average rating of the product it keeps changing according to the date.
•	Sales date wise – we can see number of products sold during the particular time. 
•	Sales type and payment mode will get. 
•	We can see which sales goes high and low per year, date, month 
•	You can see the top-notch category data.

DAX: 
How to build relations:
Using start schema design principal 
Created new table for date 
calender = CALENDAR(FIRSTDATE('Input Data'[DATE]), LASTDATE('Input Data'[DATE]))
New column - Year = YEAR(calender[Date])
New column - Month = FORMAT(calender[Date],"mmm")
Primary Key & Foreign key : 
Considered “Product ID” as Primary Key and connect with foreign key = “Product ID”
highest sale month = CALCULATE(max(calender[Month]),'Input Data'[QUANTITY]=max('Input Data'[QUANTITY]))

CY = TOTALYTD(SUM('Input Data'[QUANTITY]),calender[Date])
PY Quantity = CALCULATE(SUM('Input Data'[QUANTITY]), SAMEPERIODLASTYEAR(calender[Date]))

CY- current Year, PY – Previous Year 


![Screenshot (27)](https://github.com/Mohanasundaram-Mohi/Road-accident-Analysis-/assets/168515064/5373865c-7f59-4136-a05f-648f23d7e576)







 
