# Project 05: HR Analytics & Workforce Readiness Logistics

## 📄 Business Scenario
Maintaining operational delivery targets requires deep insight into organizational capacity. This project tracks human resources metrics, evaluating current workforce strength, identifying regional personnel distribution, and monitoring turnover risks that threaten client milestones.

## 🗢 Data Architecture & Schema
* **Staging Table:** `staging_hr_workforce` hosted on Supabase PostgreSQL.
* **Structure:** Employee lifecycle tracking mapping unique IDs, department affiliations, regional assignments (Luzon, Visayas, Mindanao), contract status, and tenure milestones.

## 📐 Key Analytical DAX Metrics
* **Active Headcount:** Filters the absolute workforce database down to currently active staff.
* **Total Separated:** Aggregates staff turnover counts across the historical timeline.
* **Enterprise Attrition Rate %:** Measures organization stability using the formula:
  $$\text{Attrition Rate \%} = \frac{\text{Total Separated}}{\text{Active Headcount} + \text{Total Separated}}$$

## 📊 Visual Insights
* **Workforce Capacity Matrix:** Provides cross-filtering across structural departments and regional outposts, giving senior leadership the exact capacity visibility required for strategic workforce planning.
