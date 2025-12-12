# Film Sales Profitability & Operations Analysis (R)

This project showcases a comprehensive data analysis focusing on **customer retention** and **supply chain optimization** for a medical equipment distributor's film sales. The goal was to transform raw sales data into **actionable business strategies** for both the sales team and the inventory management team.

---

## **View the Final Report**

The full analysis, including interactive visualizations, methodology, and detailed recommendations, is best viewed in the live HTML format.

---

## **Key Business Insights & Strategy**

The analysis utilizes two distinct models to address both the revenue side (Customer Segmentation) and the cost side (Inventory Management) of the business.

### 1. Customer Segmentation (Revenue Focus)

A **Recency, Frequency, Quantity (RFQ) Model** was implemented to group customers based on their purchasing behavior, enabling targeted marketing efforts.

| Segment | Strategic Action | Key Finding |
| :--- | :--- | :--- |
| **Most Valuable** | **Premium Service:** Focus on retention and cross-selling. | **RSIPA** and **LPRDA** are stable, high-volume purchasers. |
| **At-Risk/Long IPI** | **Win-back Campaigns:** Prioritize engagement before churn. | Identified customers with **Inter-Purchase Intervals (IPI) > 180 days** who require immediate follow-up. |
| **Churned** | **Diagnostic Outreach:** Determine the root cause of departure. | Customers positioned furthest to the right on the Recency axis represent lost revenue potential. |

### 2. Inventory Optimization (Cost Focus)

**Safety Stock (SS)** and **Reorder Point (ROP)** formulas were calculated to establish a predictive, service-level driven inventory policy.

* **Service Level Goal:** 95%
* **Actionable Outcome:** Calculated precise ROPs based on a **15-day lead time** to minimize stockouts and reduce excess working capital.
* **Risk Mitigation:** The analysis flagged **Small film** as having the highest demand volatility (standard deviation), requiring the largest Safety Stock (39 units) to mitigate inventory risk.

---

## **Technical Stack & Methodology**

| Component | Detail |
| :--- | :--- |
| **Language** | R |
| **Libraries** | `tidyverse` (data wrangling), `ggplot2` (visualization), `ggrepel` (labeling), `janitor`, `lubridate` |
| **Modeling** | **Customer:** RFQ Segmentation, Inter-Purchase Interval (IPI) analysis. <br> **Operations:** Safety Stock (SS) & Reorder Point (ROP) calculation based on Normal Distribution. |
| **Data Source** | Anonymized historical film sales data (2023–2025). |

### **Code Integrity Note**

The source code (`film_sales_analysis.Rmd`) was developed using an AI-assisted, **human-in-the-loop** approach. All code, logic, and output were thoroughly reviewed and validated to ensure analytical integrity and accuracy.
