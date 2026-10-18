# Retail Banking Customer Analytics Dashboard (Excel)

Interactive Excel dashboard built on a 100,000-customer retail banking dataset (45 fields), covering customer profile, financial performance, and marketing campaign results.

## Dashboard

![Dashboard top](screenshots/dashboard_top.png)
![Customer segments](screenshots/dashboard_segments.png)
![Dashboard charts](screenshots/dashboard_charts.png)
![Dashboard bottom](screenshots/dashboard_bottom.png)

## What I did
- Added Age Group, Credit Score Category, and Balance Category columns using nested IF formulas
- Built pivot tables and 14 charts, connected to slicers for Region, Age Group, Segment, Channel, Gender, Education, Risk Rating, and Contact Month
- Tracked KPIs: 100,000 customers, 30.02% term-deposit conversion rate, average credit score of 620, total account balance of ₹194.84 Cr

## Pivot analysis

![Pivot analysis 1](screenshots/pivot_analysis_1.png)
![Pivot analysis 2](screenshots/pivot_analysis_2.png)

## Key findings
- 35-44 is the largest age group (32,170 customers)
- Digital is the preferred channel for 50% of customers
- 68% of customers have a Poor credit score
- Metro has the highest average account balance (₹22,787); East has the lowest (₹17,570)
- Term-deposit conversion is similar across regions (29% to 32%), with Metro the highest

## Data cleaning formulas
- Age Group: `=IF(B2<25,"18-24",IF(B2<35,"25-34",IF(B2<45,"35-44",IF(B2<55,"45-54","55+"))))`
- Credit Score Category: `=IF(M2>=750,"Excellent",IF(M2>=700,"Good",IF(M2>=650,"Fair","Poor")))`
- Balance Category: `=IF(R2<10000,"Low",IF(R2<30000,"Medium","High"))`

## Excel file
[Open the Excel file (data, cleaning, pivot analysis, dashboard)](https://docs.google.com/spreadsheets/d/12Bff5jtHTWWLBgCnPi-6URPbGyqa3aUx/edit?usp=sharing)

The file is view-only. For the full dashboard with slicers and charts, please download it (File > Download > Microsoft Excel) and open it in Excel. Google Sheets does not display slicers and some charts.

## Tools
Advanced Excel, Pivot Tables, Slicers, Charts, Nested IF formulas
