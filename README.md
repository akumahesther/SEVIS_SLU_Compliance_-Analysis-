## SEVIS F-1 Compliance Analysis — Excelerate Team 25

# Project Overview
A four-week compliance analytics project analyzing SEVIS F-1 international student data to identify enrollment, fee, and documentation risk patterns. The pipeline covers data cleaning, SQL validation, dashboard development, and a final compliance report.
Role: Research and Documentation Coordinator, Team 25.

# Tools & Stack
- PostgreSQL (Supabase) / pgAdmin — SQL validation and verification queries
Looker Studio — multi-tab compliance dashboard.
- Excel / Power Query data cleaning
- PowerPoint final stakeholder presentation.

## Project Pipeline

- Data Cleaning Cleaned a 3,524-record SEVIS dataset down to 87 verified columns.
- SQL Validation Wrote verification queries in pgAdmin to reconcile dashboard metrics against raw data.
- Dashboard Development Built a live, multi-tab Looker Studio dashboard connected to Supabase PostgreSQL.
Reporting Produced a formal compliance report with a full reconciliation table, followed by a 13-slide final presentation deck.

## Key Insights
- 53% of students had not paid the SEVIS fee the single largest compliance gap in the dataset, and the primary driver of at-risk status.
- 86.9% of the student population was concentrated at the Master's level, indicating compliance risk is not evenly spread across academic levels and outreach should be weighted accordingly.
- Two metrics  I-20 issuance rate (65.32%) and deposit-paid rate (22%) — could not be independently verified against the exported CSV due to lost derivation logic upstream, highlighting a data governance gap rather than a compliance one.
- Cross-validation between the Looker Studio dashboard and SQL queries in pgAdmin confirmed consistency across all other reconciled metrics, supporting confidence in the 53% and 86.9% figures.

  
## Recommendations
- Prioritize fee non-payment outreach. With over half the population unpaid, a targeted reminder/payment-plan workflow (e.g., automated flags at 30/60/90 days past enrollment) would address the largest single risk factor.
- Tailor compliance resources to Master's-level students given their disproportionate share of the population — generic, level-blind messaging likely under-serves this group's specific timelines (e.g., OPT/CPT windows).
- Establish a documented calculation log for derived metrics going forward, so fields like I-20 issuance and deposit status remain auditable even after the original derivation logic changes hands.
- Adopt a standing reconciliation step (dashboard vs. SQL) as a recurring QA practice rather than a one-time Week 4 exercise, to catch drift early.

  
## Deliverables
Cleaned SEVIS dataset (87 columns, 3,524 records)
SQL verification queries (pgAdmin)
Live Looker Studio compliance dashboard
Compliance report with reconciliation table

## Final presentation: SLU_Compliance_Analysis_Week4.pptx

## Author
Esther Akumah Chinomso Research and Documentation Coordinator, Team 25
