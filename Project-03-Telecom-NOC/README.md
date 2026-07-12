# Project 03: Telecom Network Operations Center (NOC) Dashboard

## 📄 Business Scenario
In large-scale telecommunications operations, maintaining high network availability across diverse client portfolios is critical. This project addresses the challenge of monitoring real-time incident responses, track operational efficiency, and mitigating financial contract penalties resulting from Service Level Agreement (SLA) breaches.

## 🗢 Data Architecture & Schema
The data is hosted in a cloud-based **Supabase PostgreSQL** database, streamed directly into Power BI Desktop via an **ODBC DSN connection**. 
* **Fact Table:** `staging_noc_tickets` (Tracks individual network faults, severities, timestamps, and SLA metrics).

## 📐 Key Analytical DAX Metrics
* **Mean Time to Repair (MTTR):** Calculates the precise average hours elapsed between incident generation and successful field resolution.
* **SLA Breach Rate %:** Tracks the percentage of critical and major tickets that exceeded contractually mandated restoration windows.

## 📊 Visual Insights
* **Portfolio Health Grid:** Slices ticket volume, MTTR, and SLA breach rates side-by-side for key infrastructure stakeholders (including PTCI, FTAP, LDIC, and Edgepoint).
* **Severity Matrix:** Highlights that Critical faults present the highest operational bottleneck, allowing leadership to allocate field team resources efficiently.

