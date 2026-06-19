# Student-Revenue-Enrolment-Analytics-System  
# Student Revenue & Enrolment Analytics System

A data analytics engine built with **Python**, **Pandas**, and **NumPy** designed to process student enrollment profiles, automate tax calculations, and reconcile transaction ledgers to flag financial outstanding balances.

---

## 📌 Core Architecture & Capabilities

This system functions as a modular pipeline designed to manage corporate data integrity across disjointed operational inputs (Student Academic Registries vs. Accounts Receivable Ledgers). 

### Key Analytical Features:
* **Dynamic Fee Structuring:** Vectorized financial manipulation applying localized regulatory taxes (18% Goods and Services Tax).
* **Ledger Reconciliation:** Programmatic application of full algebraic relational joins to bridge isolated transactional histories using identification matching keys (`roll`).
* **Multi-Conditional Risk Filtering:** Automated risk flagging to pinpoint collections gaps based on complex, combined conditional thresholds.

---

## 📂 Structural Breakdown & Tasks

### 📊 Module 1: Ingestion & Schema Evaluation
* **File Creation & Parsing:** Generation of structured schema sets (`students.csv`) mapping student identifiers, names, course tracks, base fees, and operational locations.
* **Positional Index Slicing:** Clean extraction of subsets of entries using performance-oriented index lookup methods (`.iloc` boundary indexing).

### 📐 Module 2: Financial Matrix Modifications
* **Tax Invoicing:** Multi-column feature scaling processing raw fees to populate distinct columns for dynamic tax amounts ($\text{GST} = \text{Fees} \times 0.18$) and final combined obligations ($\text{Total} = \text{Fees} + \text{GST}$).
* **Database Maintenance:** Structural schema validation enabling secure row data injection and strategic header namespace updates (`.rename()`).

### 🔍 Module 3: Vectorized Query Masking
* **Compound Logical Slicing:** Constructing optimized bitwise queries (`&` / `|`) parsing geo-demographic patterns (e.g., assessing specific regions or target subject groups).
* **Multi-Level Value Ordering:** Row prioritization arranging large datasets across secondary dependent matrices (e.g., sorting across location categories, then grouping inside by total course prices).

### 🧾 Module 4: Relational Merging & Accounts Reconciliation
* **Payment Processing Integration:** Ingestion of separate flat accounting tables (`payments.csv`) recording historical cash inflows per identifier.
* **Exhaustive Merging Operations:** Implementation and validation of all baseline relational data join structures (Inner, Full Outer, Left-hand, Right-hand).
* **Revenue Gap Identification:** Final programmatic evaluation tracking immediate outstanding collection vulnerability points:
  $$\text{Remaining Fees} = \text{Base Course Fees} - \text{Paid Fees}$$

---

## 📋 System Data Modeling

### 1. Student Academic Directory (`students.csv`)

| roll | name | course | fees | city |
| :--- | :--- | :--- | :--- | :--- |
| 1 | Amit | Python | 25000 | Pune |
| 2 | Neha | Data Science | 45000 | Mumbai |

### 2. Transaction Accounts Ledger (`payments.csv`)

| roll | paid_fees |
| :--- | :--- |
| 1 | 20000 |
| 2 | 40000 |

---

## 🚀 Execution & Setup Guide

1. **Clone the repository:**
   ```bash
   git clone https://github.com/GithubRakesh-hue/Student-Revenue-Enrolment-Analytics-System.git 
   ```
2. **Install systemic dependency requirements:**
   ```bash
   pip install pandas numpy
   ```
3. **Execute the processing pipeline script:**
   ```bash
   python analytics_pipeline.py
   ```

---
## 💻 Built With
* **Python 3.x**
* **Pandas** - Fast, flexible, and expressive data structures
* **NumPy** - Vectorized array handling and core mathematics
