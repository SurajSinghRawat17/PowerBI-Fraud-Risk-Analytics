## Fraud and Risk Analytics Dashboard - Personal Portfolio Project 

**This project was developed independently for learning and portfolio purposes using a synthetic dataset. It does not contain any proprietary, confidential, client or employer data**

Power BI dashboard analyzing 60,000 global transactions (10 countries, full year 2024) to identify fraud risk patterns across geography, channel, device, and customer behavior.

DATA MODEL
- Star schema built in Power BI (Power Query + DAX): Fact_Transactions joined to Dim_Date, Dim_Geography, Dim_Device, Dim_Payment_Method, Dim_Transaction_Type, Dim_Customer_Segment, Dim_Hour_Bucket.

KEY FEATURES
- Dynamic metric selector using a disconnected table + SWITCH measure (no relationship to the model)
- Conditional-formatted risk matrices (Country x Transaction Type)
- 4 pages: Overview, Geography, Risk Deep-Dive, CEO Summary
- Bookmark-driven navigation and All Transactions / Fraud Only toggle
- Role-based view design (Team / Manager / CEO)

KEY FINDINGS
- Wire Transfer is the highest-risk channel: 9.0% fraud rate, roughly 3x higher than POS Payment (2.8%)
- New/unrecognized devices carry meaningfully higher risk: 4.89% fraud rate vs 3.23% for known devices
- Risk factors compound: combining a high-risk channel (Wire Transfer) with a high-risk country pushes fraud rate above 13% in some cells, vs the 3.36% overall baseline
- Monthly fraud rate is fairly stable year-round (3.1%-3.8% range), suggesting no strong seasonal fraud pattern in this data - risk is driven more by channel/device/behaviour than time of year

TOOLS
 - Power BI Desktop (Power Query, DAX, bookmarks, custom buttons, conditional formatting)
 - MS Excel
