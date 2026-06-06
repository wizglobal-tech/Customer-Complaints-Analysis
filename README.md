# Customer-Complaints-Analysis


[![LinkedIn](https://img.shields.io/badge/LinkedIn-Post-blue)](https://www.linkedin.com/posts/eromosele-itoya_tableau-datavisualization-customerexperience-activity-7378500174664597504-TF4Y?utm_source=share&utm_medium=member_desktop&rcm=ACoAAEbDOGsBGINDr5uoWo3fkmNHZc_HI1Qst6k)

### Table of Contents
- [Project Overview](#Project-Overview)
- [Tools](#Tools)
- [Workflow](#Workflow)
- [Insights](#Insights)
- [Recommendations](#Recommendations)
- [Strategic Goals](#Strategic-Goals)
- [Dashboard](#Dashboard)

### Project Overview
This project explores CFPB consumer complaint data from 2011-2020, analyzing 72,431 banking-related entries to identify trends in products, submission channels, timelines, and geographies. Using Tableau, I crafted an interactive dashboard that empowers users to filter by year, state, or product for deep dives—e.g., spotting why Cards complaints spiked 15% YoY. Key metrics include total complaints (72K+), resolution rates (up to 37% resolved by 2020), and state distributions (CA leading). Beyond visuals, it's about actionable intel: How can banks cut disputes by targeting high-volume issues like billing errors? This scalable setup could extend to real-time feeds or multi-sector comparisons.

### Tools
- Tableau: For data ingestion, calculated fields (e.g., % of Total), LOD expressions (e.g., fixed yearly trends), parameters for dynamic filtering, and interactive viz (maps, trends, pies).

### Workflow
A structured, iterative build ensured clean data flows into insightful, user-friendly outputs.
#### 1. Data Loading and Cleaning:
- Imported the CSV dataset (~72K rows) into Tableau, covering fields like Complaint ID, Date Received, Issue, Product (e.g., Cards, Mortgages), State, Sub-issue, Submitted via (e.g., Web, Referral).
- Handled nulls/duplicates (e.g., anonymized ZIPs), parsed dates for year/month granularity, and created bins for trends (e.g., quarterly complaints).
- Filtered to focus on key products (Accounts, Cards, etc.) and added flags like "Disputed" (Yes/No) for segmentation.
    
#### 2.	Data Modelling and Processing:
- Used Tableau's data interpreter for quick joins; created relationships via Complaint ID for sub-issue drills.
- Parameters for slicers (e.g., Product dropdown: Cards, Mortgages; Year range: 2011-2020) and dynamic titles (e.g., "Complaints by [Selected Product]").
- Aggregations for KPIs: Total Complaints = COUNTD([Complaint ID]), Avg per Year = AVG([Annual Count]).

#### 3.	Data Analysis & Visualization:
- Designed core visuals: Stacked bars for yearly trends (% resolved/unresolved), pie for request channels, filled map for states (color-coded by volume), line chart for year-over-year growth.
- Added interactivity: Action filters for state drills (e.g., click CA → filter sub-issues), tooltips with details (e.g., "Top Issue: Billing Disputes – 12K cases"), and legends for product breakdowns.
- Enhancements: Conditional formatting (red for high unresolved), heatmaps for state density, and export options for raw slices.

#### 4. Dashboard Assembly:
- Single-page layout for simplicity: Top KPIs, product matrix, trends chart, state map, channel pie, and detail table.
- Tested cross-filters (e.g., select "Web" → updates all metrics) and performance (blended data for speed).
- Polished with custom colors (blues for resolved, grays for totals), icons, and navigation tooltips.

### Insights
Data-driven highlights, each tied to visuals for easy validation.
#### 1. Overall Performance:
Total Complaints: 72,431 | Peak Year: 2019 (3,567) | Avg Annual: 7,243 | Resolution Improvement: From 0% (2011) to 37% (2020).
Growth: +95% from 2012 baseline, with a 23% 2020 drop—economic recovery signal?

<img width="243" height="115" alt="Screenshot 2025-09-29 193518" src="https://github.com/user-attachments/assets/cb20b750-9d38-4aa3-…
