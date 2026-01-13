# 🏢 AI Solutions for Real Estate Agencies (Showcase Workflows)

This repository shares a **public showcase** of selected n8n workflows used to automate real-estate operations.  
While the **full workflow library** is not displayed, here we highlight sanitized examples to illustrate our approach.  

---

## 📂 Included Workflows

### 1. 🏦 **Rent Payment Reconciliation**
- **Input**: A bank statement and a table of expected rents.  
- **Process**:  
  - Uses **fuzzy matching with scoring** to identify tenants and match payments to expected rents.  
  - Calls a **LLM** to improve ambiguous matches and handle edge cases.  
- **Output**: A Google Sheet automatically filled with the list of received rents and an email to the landlord that sums up the received rents for the current month.  
- **Extended version** (private): includes an automation that **sends email reminders** to tenants for unpaid rents.

---

### 2. 🤖 **Agent Manager Orchestration**
This workflow coordinates and supervises **multiple specialized AI agents** to handle real-estate tasks.  
- **Core Logic**:  
  - A **main manager node** decides which sub-agent to activate based on the request.  
  - Sub-agents include:
    - **Lead Generation Agent** (scrapes portals, filters prospects, enriches data).  
    - **Email Reply Agent** (drafts and personalizes responses using context).  
    - **Voicebot Agent** (schedules appointments, answers FAQs).  
    - **Data Logger Agent** (records all activity into a database/CRM).  
  - Results are consolidated and sent back to the manager for validation.  
- **Goal**: Provide a **modular, scalable orchestration system** where agents work in parallel but remain centrally supervised.

---

## 🔒 About This Repo
- Workflows here are **simplified and sanitized** (no secrets, no sensitive data).  
- This repo is for **showcase purposes**.

---

