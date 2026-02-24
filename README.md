#🏥 Hospital Emergency Room Dashboard (Excel Project)
📌 Project Overview

The Hospital Emergency Room Dashboard is an interactive Excel-based analytics project designed to monitor and evaluate emergency department performance.
This dashboard provides monthly insights into patient flow, service efficiency, demographics, and departmental workload to support data-driven decision-making.

🎯 Objective
The goal of this project is to:
Monitor total patient visits
Analyze average waiting time
Track patient satisfaction score
Identify delays in service
Understand patient demographics
Analyze department referrals
Improve hospital operational efficiency

📊 Key Performance Indicators (KPIs)
Total Patients
Average Wait Time (Minutes)
Patient Satisfaction Score
On-time vs Delayed Attendance

📈 Dashboard Features
🔹 Patient Attendance Status
Pie chart comparing:
On-time patients
Delayed patients

🔹 Gender-wise Analysis
Donut chart showing:
Male patients

Female patients
🔹 Patients by Age Group
Bar chart categorizing patients into age segments:
0–9
10–19
20–29
30–39
40–49
50–59
60–69
70–79

🔹 Department Referral Analysis
Horizontal bar chart displaying patient referrals to:
General
Orthopedics
Cardiology
Neurology
Physiotherapy
Gastroenterology
Renal

🧮 Data Modeling & Formulas Used
📅 Calendar Table (Power Query)
= List.Dates(#date(2023,01,01),731,#duration(1,0,0,0))
📊 Age Group (DAX Formula)
=IF([Patient Age]>=70,"70-79",
IF([Patient Age]>=60,"60-69",
IF([Patient Age]>=45,"45-59",
IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",
IF([Patient Age]>=5,"05-14","0-4"))))))
⏱ Patient Attend Status (DAX)
=IF([Patient Waittime]<30,"Within Time","Delay")
🎛 Interactivity
📅 Month-wise filter
📆 Year toggle (2023 / 2024)
Dynamic KPI updates
Fully interactive visual dashboard

🛠 Tools & Skills Demonstrated
Microsoft Excel
Power Query
DAX Formulas
KPI Tracking
Healthcare Data Analysis
Dashboard Design
Data Visualization
Interactive Reporting

💡 Business Impact
This dashboard helps hospital management:
Reduce patient wait time
Improve service quality
Optimize department workload
Enhance patient satisfaction
Make data-driven operational decisions

📂 Files Included
Hospital Emergency Room Dashboard.xlsx
Hospital Emergency Room Data.csv
Dashboard Screenshot
