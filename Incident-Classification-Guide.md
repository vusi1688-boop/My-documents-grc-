# Incident Classification Guide
## MediCare Connect (Pty) Ltd

**Classification:** Internal  
**Version:** 1.0  
**Date:** June 2025  
**Author:** Patrick Mohlala, GRC Analyst  
**Review Date:** June 2026

---

## 1. Purpose

This guide ensures all staff classify security incidents consistently so the correct response is triggered at the correct speed every time.

Misclassifying a CRITICAL incident as LOW is one of the most common causes of missed POPIA notification deadlines.

---

## 2. Incident Definition

An information security incident is any event that actually or potentially:

- Compromises the confidentiality of patient or staff personal information
- Affects the integrity of medical records
- Disrupts availability of clinical systems
- Violates POPIA obligations
- Breaches MediCare Connect security policies

An event that could have caused harm but did not is called a **NEAR MISS** and must also be reported and logged.

---

## 3. Severity Tiers

### Tier 1 - Critical

**Definition:**
Confirmed breach of patient medical records or personal information. Active attack in progress. Full system compromise. Clinical operations halted.

**Examples:**
- Ransomware encrypting patient database
- Confirmed unauthorized access to PHRS
- Stolen unencrypted laptop with patient data
- Attacker actively inside the network
- Accidental disclosure of records to wrong recipient (mass scale)

**POPIA Reportable:** Yes - Always  
**Response time:** Immediate (within 1 hour)  
**Escalation:** CEO, IT Manager, Information Officer notified simultaneously  
**Notification:** Information Regulator within 72 hours of discovery  
**Patient notification:** Required if high risk  
**External support:** Cyber insurer activated  
**Management action:** Clinical operations continuity plan activated

---

### Tier 2 - High

**Definition:**
Suspected breach under investigation. Significant system degradation. Single user account compromised. Malware detected and contained but origin unknown.

**Examples:**
- Phishing email clicked, credentials entered on suspicious site
- Single staff account compromised
- Malware detected and quarantined
- Unusual access patterns detected in patient record system
- Laptop lost but encryption status unknown

**POPIA Reportable:** Possibly - assess impact  
**Response time:** Within 4 hours  
**Escalation:** IT Manager and Information Officer notified  
**Notification:** Prepare notification in case breach confirmed  
**Management action:** Increased monitoring, containment measures

---

### Tier 3 - Medium

**Definition:**
Security policy violation without confirmed data exposure. Isolated malware blocked. System performance degradation. Minor physical security breach.

**Examples:**
- Staff member sharing password (caught before exploitation)
- Phishing email received but not clicked
- Antivirus blocked malware download
- Visitor found in restricted area
- Single misdirected email with non-sensitive information

**POPIA Reportable:** Unlikely - document only  
**Response time:** Within 24 hours  
**Escalation:** IT Manager notified  
**Notification:** Log in incident register only  
**Management action:** Remind staff of policy, review access if needed

---

### TIER 4 - Low

**Definition:**
Near miss or policy awareness issue. No systems affected. No data at risk. Procedural error caught early.

**Examples:**
- Staff left workstation unlocked (discovered and locked by colleague)
- Suspected phishing email reported before any action taken
- Password reset required
- Visitor badge not returned
- Software licence expired

**POPIA Reportable:** NO  
**Response time:** Within 5 business days  
**Escalation:** Logged only  
**Notification:** None  
**Management action:** Log, trend analysis, training reminder

---

## 4. POPIA Reportability Decision Tree

**Ask these questions in order :**

### Question 1:
Was personal information accessed, acquired, used or disclosed without authorization OR lost?

- **NO** → Document as internal incident. POPIA notification not required
- **YES** → Go to Question 2

### Question 2:
Does the personal information belong to an identifiable living person?

- **No** → Document as internal incident
- **Yes** → Go to Question 3

### Question 3:
Could the breach cause harm to the affected persons? (Financial loss, reputation damage, discrimination, physical harm, identity theft, distress)

- **No** → Document internally. Consider voluntary notification
- **Yes** → **POPIA Section 22 Applies.** Notify Information Regulator within 72 hours. Notify affected data subjects as soon as reasonably possible

---

## 5. Incident Category Types

| Code | Category |
|------|----------|
| CAT-01 | Malware and Ransomware |
| CAT-02 | Phishing and Social Engineering |
| CAT-03 | Unauthorised Access |
| CAT-04 | Data Loss or Exposure |
| CAT-05 | Physical Security Breach |
| CAT-06 | Insider Threat |
| CAT-07 | Third Party or Vendor Incident |
| CAT-08 | System Availability Failure |
| CAT-09 | Policy Violation |
| CAT-10 | Near Miss |

---

## 6. Who Can Declare an Incident

**ANY Staff Member** can and must report a suspected incident.

**Only the following can classify and formally declare an incident:**
- IT Manager
- Information Officer
- GRC Analyst
- CEO (in absence of above)

> **When in Doubt: Classify higher.**  
> It is better to escalate a LOW as a HIGH than to miss a CRITICAL.

---

**Document Control**  
Prepared by: Patrick Mohlala, GRC Analyst  
Version: 1.0  
Status: Final  
Review: June 2026
