**Intro to Data Governance with SCD2: A Practical Data Engineering Notebook**

##### Overview

This notebook provides a practical, code-driven exploration of Slowly Changing Dimension Type 2 (SCD2) modeling, using a reduced and self contained dataset and business scenarios with a narrative tone. 

It demonstrates how SCD2 dimensional modeling ensures historical accuracy, regulatory compliance, and auditability key requirements for any enterprise data platform.

##### Key Features

- **Simplified Dataset with real world relevance:**  
  The notebook uses a simple customer dimension table , a static FICA alert threshold table, and a fact table of customer deposits,  modeled after a fintech scenario.

- **SCD1 vs. SCD2 Comparison:**  
  The notebook illustrates the pitfalls of SCD1 (overwriting history) by showing how alert logic can silently misclassify historical transactions when customer attributes change. It then demonstrates how SCD2 preserves the full change history, enabling correct, context-aware compliance checks.

- **Data Governance and Auditability:**  
  SCD2 is implemented to ensure that every transaction is evaluated against the correct historical dimension values, supporting robust data governance and regulatory audit requirements.

##### Why SCD2 Matters

- **Historical Integrity:**  
  SCD2 maintains a complete record of all changes to dimension data (e.g., customer address), allowing accurate reconstruction of business context for any point in time.

- **Audit-Readiness:**  
  By preserving change history, SCD2 enables organizations to answer critical audit questions, such as whether a transaction was compliant at the time it occurred.

- **Business Value:**  
  SCD2 modeling prevents silent data errors, supports transparent reporting, and enables reliable compliance logic - capabilities essential for regulated industries.
