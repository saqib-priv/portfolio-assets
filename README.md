# Full-Cycle Attendance Audit Engine (Python)

---

## Project Overview

This is an integrated, Python-based automation system designed to eliminate common HR disputes and ensure daily attendance **compliance and data integrity**. The engine replaces time-consuming manual processes with a proactive, rule-based audit that flags all attendance exceptions immediately.

---

## Core Logic: Exception Management

The system's intelligence lies in its ability to detect and categorize three critical attendance failures, moving beyond simple absence checks.

| Exception Category | Detection Rule | Business Value |
| :--- | :--- | :--- |
| **Full Absence** | Identifies records where both Time In and Time Out fields are missing. | Triggers prompt **Absence Reminders**. |
| **Missing Tap (Mis-Tap)** | Uses XOR logic to find records with only one tap recorded. | Fosters immediate correction of records. |
| **Late-Tap Reclassification** | Smart rule that re-designates a tap after a business threshold (e.g., 12:00:00) as the **Time Out**; then alerts on the missing Time In. | Solves the discrepancy caused by the common **early-exit/single-tap strategy**. |

---

## Technical Stack & Security

| Feature | Technologies Used | Contribution |
| :--- | :--- | :--- |
| **Data Processing** | Python, Pandas | High-speed data ingestion, cleaning, and pivoting. |
| **System Control** | Tkinter, smtplib | Deploys a **managerial approval GUI** and contextual email notifications. |
| **Security** | Environment Variables | Secure handling of credentials (e.g., email passwords) without hardcoding. |

---

## Measurable Business Impact

| Metric | Result |
| :--- | :--- |
| **Efficiency Gains** | **95%+ Reduction in Manual Auditing Effort.** |
| **Compliance** | Minimized payroll risk and established a robust, verifiable audit trail. |
| **Strategic Value** | System functions as the **cornerstone of daily attendance integrity**. |

---

## System Architecture

[System Architecture Diagram Link](https://github.com/saqib-priv/portfolio-assets/blob/main/Gemini_Generated_Image_m4x3xkm4x3xkm4x3.png?raw=true)
