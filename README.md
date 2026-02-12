# bank
This project demonstrates how risk analytics can be applied in the banking sector to support data-driven lending decisions.
Using Power BI, I built an interactive dashboard that analyzes customer financial behavior, loan exposure, deposits, and engagement metrics to help financial institutions:<br>
-  Reduce lending risk<br>
-  Identify high-value and high-risk customers<br>
-  Monitor financial KPIs<br>
-  Optimize strategic decision-making<br>
-  This project highlights strong skills in data modeling, DAX, KPI development, and business storytelling.<br>

🎯 Business Problem<br>
Banks face significant financial risk when lending to customers without proper analysis of:<br>
-  Income segmentation<br>
-  Loan exposure<br>
-  Engagement history<br>
-  Deposit patterns<br>

The objective was to build a dashboard that enables stakeholders to evaluate client profiles and make informed lending decisions.
🛠️ Technical Implementation
🔹 Data Modeling
-  Designed relational data model using multiple tables:
-  Clients
-  Client-Banking
-  Banking Relationship
-  Gender
-  Investment Advisor
-  Period
-  Established relationships using primary and foreign keys.
-  Optimized model for performance and scalability.

🔹 Data Transformation
Created calculated columns for:
-  Engagement Timeframe
-  Engagement Days
-  Income Band segmentation
-  Processing Fees logic
-  Cleaned and structured financial fields.
-  Applied income binning strategy for segmentation analysis.

🔹 Advanced DAX Measures
Total Clients
Total Clients = DISTINCTCOUNT('Clients - Banking'[Client ID])

Total Loan
Total Loan = [Bank Loan] + [Business Lending] + [Credit Cards Balance]


Total Deposit
Total Deposit = [Bank Deposit] + [Savings Account] + [Foreign Currency Account] + [Checking Accounts]


Total Fees
Total Fees = SUMX('Clients - Banking', [Total Loan] * 'Clients - Banking'[Processing Fees])


Engagement Days
Engagement Days = DATEDIFF('Clients - Banking'[Joined Bank], TODAY(), DAY)

📊 Key Business KPIs
-  KPI	Value
-  Total Clients	188
-  Total Loan Exposure	$139.9M
-  Total Deposits	$111.49M
-  Total Fees Generated	$5.17M
-  Total Engagement Value	$18.26K
-  Total Credit Card Exposure	$135
📈 Dashboard Breakdown
🏠 Executive Overview

-  Financial health summary
-  High-level KPI monitoring
-  Strategic snapshot for decision-makers

💰 Loan Risk Analysis
-  Loan distribution by Income Band
-  Loan exposure by Nationality
-  Business vs Retail lending breakdown
-  Credit card balance insights

💳 Deposit Analysis
-  Checking vs Savings breakdown
-  Foreign currency exposure
-  Deposit concentration trends

📊 Strategic Summary
-  Client segmentation insights
-  Engagement impact on financial performance
-  Cross-analysis between loan and deposit behavior

🔍 Key Insights Generated
-  Higher income bands correlate with increased loan exposure.
-  Private banks hold a larger client base compared to others.
-  Certain nationalities show higher lending concentration.
-  Deposit-to-loan ratio reveals potential liquidity risk areas.
-  Engagement duration influences overall financial value.

💼 Skills Demonstrated

✔ Data Modeling (Star Schema Concepts)
✔ Advanced DAX (SUMX, SWITCH, DISTINCTCOUNT, DATEDIFF)
✔ KPI Design & Business Metrics
✔ Financial Data Analysis
✔ Risk Analytics Fundamentals
✔ Data Cleaning & Transformation
✔ Business Storytelling with Visualization

🚀 Business Impact
This dashboard enables banks to:
-  Make smarter lending decisions
-  Monitor financial exposure in real-time
-  Identify high-risk customer segments
-  Improve strategic financial planning

🔮 Future Enhancements
-  Integration of predictive loan default model
-  Risk scoring system using probability modeling
-  Real-time data integration
-  Automated alert system for high-risk profiles
-  Drill-through risk profiling dashboard

📂 Project Assets
-  Banking Dashboard.pbix
-  Banking.xlsx
-  Banking.csv
-  Banking Report.docx
-  Banking.pptx

👤 Author

Tarun Yadav
Aspiring Data Analyst | Power BI Developer | DAX Specialist

📍 India
📊 Focus: Financial Analytics | Business Intelligence | Risk Analytics
