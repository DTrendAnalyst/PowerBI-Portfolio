# Project 02: Customer Behavior Analytics

## 📄 Business Scenario
Relying solely on gross sales masks critical shifts in consumer behavior. This project moves beyond standard database aggregations to deliver behavioral intelligence, evaluating how effectively the business is acquiring new accounts versus retaining high-value historical cohorts.

## 🗢 Data Architecture & Schema
* **Inheritance:** Leverages the robust Star Schema infrastructure established in the foundational data pipeline.
* **Granularity:** Customer behavior is isolated at the unique individual account grain (`customer_id`).

## 📐 Key Analytical DAX Metrics
* **Active Customers:** Dynamic `DISTINCTCOUNT` evaluation of purchasing accounts within the filtered time frame.
* **Is High Value Customer:** An advanced iterator using `AVERAGEX` and `ISINSCOPE` to dynamically classify accounts as "High Value" or "Standard" relative to the global lifetime spending baseline without hardcoding tiers.
* **New vs. Returning Cohorts:** Time-series logic utilizing table-variable patterns to track the exact date of a customer's first purchase and flag them as an acquisition or a returning customer.

## 📊 Visual Insights
* **Cohort Evolution Line Chart:** Visually details the historical shift from an acquisition-heavy startup model to a retention-driven corporate scale.
* **Customer Lifecycle Matrix:** Eliminates total-row string bugs to display precise account-level standing.
