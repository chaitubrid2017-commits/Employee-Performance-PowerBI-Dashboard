# Employee-Performance-PowerBI-Dashboard
Power BI dashboard analyzing employee performance, efficiency, and productivity using KPIs and visual insights.

📊 Employee Performance Dashboard (Power BI)
🚀 End-to-End Business Intelligence Project using Power BI & DAX
________________________________________

🧭 Project Overview
This project delivers an interactive Power BI dashboard designed to analyze employee performance, efficiency, and productivity.
The dashboard transforms raw operational data into actionable insights that help business stakeholders:
•	Monitor performance trends
•	Identify top & low performers
•	Optimize time utilization
•	Improve decision-making
________________________________________

📸 Dashboard Preview

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d50266f0-f537-476e-872d-2e3d49743ec8" />

________________________________________

🎯 Business Problem

Organizations often struggle to:

•	Track employee productivity effectively
•	Measure efficiency (time vs output)
•	Identify performance gaps

👉 This dashboard solves these challenges using data-driven KPIs and visual analytics
________________________________________

📊 Key Metrics (KPIs)

KPI	Description

1) Total Leads	:-  Total leads generated
2) Leads per Hour :- 	Efficiency indicator
3) Avg Time per Lead :-	Productivity measure
4) Leads per Employee :-	Individual performance
5) Utilization %	 :- Time utilization
6) 
________________________________________

📈 Key Insights Generated

•	📌 Associate KLM is the top performer in lead generation

•	📌 Efficiency varies significantly across employees

•	📌 Declining trend observed in recent months

•	📌 Some employees show high effort but low output (inefficiency)

________________________________________

📊 Visualizations Used

•	📌 KPI Cards (Performance Summary)

•	📈 Line Chart (Trend Analysis)

•	📊 Bar Chart (Employee Comparison)

•	🔄 Combo Chart (Time vs Leads)

•	📋 Table with Conditional Formatting

________________________________________

🧠 Data Modeling & DAX

Key Measures:

1)	Total_Leads = SUM('FACT EMP TABLE'[No of Leads])

2)	Leads_per_Hour = 
DIVIDE(
    SUM('FACT EMP TABLE'[No of Leads]),
    SUM('FACT EMP TABLE'[Time Spent on LG (in mins)]) / 60
)

3)	Avg_Time_Per_Lead = 
DIVIDE(
    SUM('FACT EMP TABLE'[Time Spent on LG (in mins)]),
    SUM('FACT EMP TABLE'[No of Leads])
)

4)	Utilization % = 
DIVIDE(
    SUM('FACT EMP TABLE'[Time Spent on LG (in mins)]),
    COUNTROWS('FACT EMP TABLE') * 480
)

5)	LEADS PER EMPLOYEE = AVERAGEX(VALUES('FACT EMP TABLE'[Emp Name]),CALCULATE('FACT EMP TABLE'[TOTAL NO OF LEADS]))

________________________________________

🛠 Tools & Technologies:-

•	Power BI (Dashboard & Visualization)
•	DAX (Data Analysis Expressions)
•	Excel (Data Source)
________________________________________
🎨 Dashboard Design Highlights

•	Clean and structured layout
•	KPI-driven storytelling
•	Conditional formatting for performance
•	Interactive slicers (Month-Year)

________________________________________

📂 Repository Contents

•	📁 Employee_Performance_Dashboard.pbix
•	🖼️ dashboard.png
•	📄 README.md
________________________________________

👤 Author

Chaitanya

Aspiring Data Analyst | Power BI | SQL | Data Visualization

________________________________________

⭐ Support

If you found this project helpful, please ⭐ the repository!


