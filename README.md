# 🏢 AI Solutions for Real Estate Agencies (Showcase Workflow)

## Notice
This repository contains a **highly simplified showcase version** of the original workflow.  
All data, examples, and logic have been **sanitized, minimized**.

The goal is strictly **demonstration and portfolio presentation**; illustrating the structure, reasoning steps, and high‑level automation logic without reproducing the full production system.

---
### 1. 🏦 Rent Payment Reconciliation (Showcase Version)

**Input:**  
- A bank statement  
- A table of expected rents
  
**Process:**  
- Performs fuzzy matching with scoring to identify tenants and match received payments to expected amounts.  
- Uses an LLM to refine uncertain matches and resolve ambiguous cases.  
- Applies simple heuristics to flag discrepancies (late, missing, or partial payments).  

**Output:**  
- Automatically populates a Google Sheet with reconciled rent payments for the current month.  
- Generates a summary email to the landlord listing all received payments.  

**Extended Version (Private):**  
The full workflow — not included here — also automates tenant reminders by sending emails for unpaid or partially paid rents. This functionality has been removed for privacy and security reasons.

---

