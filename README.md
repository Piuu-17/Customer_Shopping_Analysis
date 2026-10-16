# Retail Supply Chain & Customer Demand Analytics Workflow

##  Project Overview
This project delivers a production-grade, end-to-end data analytics workflow designed to simulate modern business intelligence and operational workflows. By analyzing retail customer shopping trends, this repository maps data-driven insights directly to **Industrial Engineering (IE)** and **Supply Chain Management (SCM)** pillars: optimizing inventory turnover, understanding regional demand fluctuations, and refining customer segmentation to reduce operational waste.

The architecture spans data ingestion, automated cleaning, relational database warehousing, advanced querying, and executive-level visualization.

##  Tech Stack & Production Architecture
*   **Data Preprocessing:** Python (`Pandas`, `NumPy`, `Jupyter Notebook`)
*   **Database & Warehousing:** SQL (Relational Schema Design, Aggregations, Window Functions)
*   **Business Intelligence:** Power BI (DAX, Interactive Dashboards, ETL Modeling)
*   **Methodology:** CRISP-DM (Cross-Industry Standard Process for Data Mining)
 quality. 

##  Repository Structure

├── Business Problem Document.pdf          # Root cause analysis & business requirement specification
├── customer_shopping_behavior.csv         # Raw transactional retail data
├── customer_shopping_behavior_datacleaning_fixed.ipynb  # Production-ready Python ETL pipeline
├── customer_behavior.sql                  # Production SQL analytics script & database schema
├── customer_behavior_dashboard.pbix       # Executive Power BI Dashboard file
└── README.md                              # Project documentation

## Execution Workflow & Implementation

### Phase 1: Data Quality & ETL Pipeline (Python)
*   **Problem:** Raw transactional data often contains anomalies, duplicate records, or unstructured types that break downstream production databases.
*   **Solution:** Built a Python script using `Pandas` to handle missing values, validate data types, strip white spaces, and filter out noise.
*   **IE Alignment:** Implemented data validation checkpoints analogous to **Poka-Yoke (Mistake-Proofing)** in production lines to block bad data from contaminating the data warehouse.

### Phase 2: Relational Database Modeling & Analytics (SQL)
*   Designed a structured relational database schema optimizing query performance for fast analytical retrieval.
*   Utilized complex SQL techniques including **Window Functions (`RANK()`, `PARTITION BY`)**, **Common Table Expressions (CTEs)**, and **Advanced Grouping** to isolate key metrics:
    *   Customer Lifetime Value (CLV) proxies.
    *   Category-wise revenue velocities.
    *   Payment and shipping preference distributions (critical for supply chain logistics planning).

### Phase 3: Executive BI Visualizations (Power BI)
*   Developed a dynamic, fully interactive dashboard to bridge the gap between technical data and executive decision-making.
*   Engineered calculated measures using **DAX** to track KPIs such as average order value, purchase consistency, and segment penetration.
*   Designed user journeys focused on actionable insights: allowing warehouse managers to view category demand and marketing teams to filter by customer demographics.


##  Strategic Business Insights Generated
*   **Inventory Velocity:** Identified specific product categories with high seasonal variation, allowing supply chain teams to adjust safety stock and prevent capital tie-ups.
*   **Logistics Optimization:** Isolated the most frequently utilized shipping methods by demographic group, uncovering opportunities to renegotiate bulk carrier contracts for high-volume regions.
*   **Demographic Targeting:** Discovered distinct high-value customer clusters, empowering the business to pivot from generic promotions to high-margin, targeted retention strategies.
