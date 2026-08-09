# Incident Response Plan
## MediCare Connect (Pty) Ltd

**Aligned to ISO 27035:2023 and POPIA Section 22**

**Classification:** Confidential  
**Version:** 1.0  
**Date:** June 2025  
**Author:** Patrick Mohlala, GRC Analyst  
**Approved by:** [Pending - CEO]  
**Review Date:** June 2026

---

## 1. Purpose

This Incident Response Plan (IRP) defines how MediCare Connect detects, responds to, contains and recovers from information security incidents affecting patient data, clinical systems and business operations.

It ensures the organisation meets its obligations under:
- POPIA Section 22 (72 hour notification)
- ISO 27001:2022 Annex A.5.24 to A.5.28
- ISO 27035:2023 (Incident Management)
- National Health Act 61 of 2003

---

## 2. Scope

This plan applies to:
- All information systems within the ISMS
- All 45 MediCare Connect staff members
- All third party providers with system access
- All incident types from Tier 1 to Tier 4

---

## 3. IR Team Roles and Responsibilities

### Incident Response Manager
**Role:** IT Manager  
**Responsibilities:**
- Declare and classify the incident
- Coordinate technical response team
- Brief CEO and Information Officer
- Make containment decisions
- Document technical actions taken
- Authorise evidence collection

**Contact:** [IT Manager mobile - 24/7]

### Information Officer (POPIA Lead)
**Role:** Appointed Information Officer  
**Responsibilities:**
- Assess POPIA reportability
- Prepare Information Regulator notification
- Coordinate affected person notification
- Maintain POPIA breach register
- Liaise with Information Regulator

**Contact:** [Information Officer mobile]

### GRC Analyst
**Role:** Patrick Mohlala (portfolio context)  
**Responsibilities:**
- Document all incident actions and timeline
- Maintain chain of custody for evidence
- Track POPIA notification deadlines
- Prepare post incident review report
- Update risk register and controls

**Contact:** [GRC Analyst contact]

### CEO
**Role:** Executive Sponsor  
**Responsibilities:**
- Ultimate decision authority
- Approve regulatory notifications
- Communicate with media if required
- Approve external support spend
- Board and stakeholder communication

**Contact:** [CEO mobile - 24/7]

### Clinical Lead
**Role:** Senior Doctor or Practice Manager  
**Responsibilities:**
- Activate clinical continuity procedures
- Communicate with clinical staff
- Maintain patient safety during incident
- Approve any patient communication

**Contact:** [Clinical Lead contact]

### External Support
- **Cyber Insurer:** [Policy number and hotline]
- **Legal Counsel:** [Attorney contact]
- **Forensic IR Firm:** [Vendor contact]
- **Microsoft Support:** [M365 admin portal]

---

## 4. The Six Phases of Incident Response

### PHASE 1: PREPARATION

Actions completed before any incident:

- [ ] This IR plan documented and approved
- [ ] IR team trained and contacts confirmed
- [ ] Incident classification guide distributed
- [ ] All staff trained to report incidents
- [ ] Emergency contact list printed and stored offline (not only on systems that may be compromised)
- [ ] Cyber insurance policy activated
- [ ] Forensic IR vendor pre-contracted
- [ ] Backups tested and verified restorable
- [ ] Legal counsel retained and briefed
- [ ] POPIA notification templates prepared
- [ ] Information Regulator portal access confirmed by Information Officer
- [ ] Tabletop exercise conducted annually

### PHASE 2: DETECTION AND REPORTING

**How incidents are detected:**
- Staff report to IT Manager or IR email
- Automated alerts from security tools
- Patient or third party notification
- System monitoring alerts
- External threat intelligence

**Staff Reporting Procedure:**
1. Do not ignore it or try to fix it
2. Do not turn off the affected device (preserves evidence)
3. Note the time you discovered it
4. Call IT Manager immediately
5. Complete Incident Report Form
6. Do not discuss on WhatsApp or email

**Initial Information to Capture:**
- Date and time of discovery
- Who discovered it and how
- What systems or data are affected
- What actions have already been taken
- Is the incident still ongoing

### PHASE 3: ASSESSMENT AND CLASSIFICATION

**IT Manager actions within first hour:**

1. Receive incident report
2. Gather initial information
3. Classify severity (Tier 1-4) using Incident Classification Guide
4. Notify appropriate team members based on tier
5. Open incident log with unique ID. Format: `INC-YYYY-MM-NNN` (Example: `INC-2025-06-001`)
6. Assess POPIA reportability with Information Officer
7. If POPIA reportable start **72 HOUR CLOCK IMMEDIATELY**
8. Brief CEO if Tier 1 or 2

**POPIA Clock Notification:**
- Time of discovery: ____________
- 72 hour deadline: ____________ (Add exactly 72 hours to discovery time)
- Responsible: Information Officer
- Escalation if missed: CEO and Legal

### PHASE 4: CONTAINMENT

**Short Term Containment (first 4 hours):**  
Goal: Stop the bleeding immediately

- [ ] Isolate affected systems from network (unplug network cable, disable WiFi). **DO NOT power off unless instructed**
- [ ] Revoke compromised user credentials
- [ ] Block suspicious IP addresses on firewall
- [ ] Enable additional logging on all systems
- [ ] Notify all staff not to use affected systems until cleared
- [ ] Preserve all evidence before changes
- [ ] Screenshot all error messages and alerts
- [ ] Do not wipe or rebuild any system yet

**Evidence Preservation:**
Every action taken must be documented with timestamp, person responsible and outcome. This is your chain of custody.

Format for each action:
`[TIME] [WHO] [ACTION TAKEN] [OUTCOME]`

Example:
`[14:32] IT Manager - Isolated PHRS server from network by disabling switch port. System remains powered on. Logs preserved.`

**Long Term Containment (4-72 hours):**
- [ ] Deploy additional monitoring
- [ ] Implement temporary compensating controls
- [ ] Maintain clinical operations using continuity procedures if systems offline
- [ ] Prepare clean systems for restoration
- [ ] Continue evidence collection

### PHASE 5: ERADICATION AND RECOVERY

**Eradication Steps:**
- [ ] Identify root cause of incident
- [ ] Remove malware or attacker access
- [ ] Close the vulnerability that was exploited
- [ ] Reset all potentially compromised credentials
- [ ] Patch affected systems before restoration
- [ ] Verify eradication with forensic evidence
- [ ] Document all eradication actions

**Recovery Steps:**
- [ ] Restore systems from verified clean backup
- [ ] Confirm backup integrity before restoration
- [ ] Test restored systems before reconnecting
- [ ] Monitor restored systems intensively
- [ ] Gradually restore services starting with lowest risk systems first
- [ ] Confirm patient record integrity
- [ ] Clinical Lead to approve return to normal clinical operations
- [ ] IT Manager to sign off technical recovery
- [ ] CEO to approve full service restoration

**Recovery Criteria:**  
Systems may return to production only when:
-  Root cause identified and eliminated
-  All malware or attacker access removed
-  Systems patched and hardened
-  Credentials reset across all accounts
-  Backup integrity confirmed
-  Monitoring confirmed active
-  Clinical Lead approved return

### PHASE 6: POST INCIDENT REVIEW

**Timeline:** Within 14 days of incident closure

**Review Meeting Attendees:**
- IT Manager
- Information Officer
- GRC Analyst
- CEO (for Tier 1 incidents)
- Clinical Lead (if clinical impact)

**Questions to Answer:**
1. What exactly happened and when?
2. How was the incident detected?
3. Was detection fast enough?
4. Were response procedures followed?
5. Was the POPIA timeline met?
6. What evidence was collected well?
7. What evidence was missed?
8. What would have prevented this?
9. What controls need updating?
10. Were staff communications clear?

**Outputs Required:**
- [ ] Post Incident Review Report
- [ ] Updated risk register entries
- [ ] Corrective action plan with owners
- [ ] Policy or procedure updates identified
- [ ] Training gaps identified
- [ ] Lessons learned documented

**Risk Register Update:**
GRC Analyst must update the risk register within 7 days of incident closure to reflect any new risks identified or changes to existing risk scores.

---

## 5. Scenario Specific Procedures

### SCENARIO A: Ransomware Attack
**Classification:** TIER 1 CRITICAL  
**POPIA Reportable:** YES

**Immediate actions (first 30 minutes):**
- [ ] Do not pay the ransom (yet - CEO decision)
- [ ] Isolate ALL systems from the network including clinical workstations
- [ ] Disconnect all network shares
- [ ] Activate clinical continuity plan (paper based records, manual processes)
- [ ] Notify CEO and Information Officer
- [ ] Start POPIA 72 hour clock
- [ ] Call cyber insurer hotline
- [ ] Call forensic IR firm
- [ ] Preserve ransom note and all screens
- [ ] Do not restart any affected machines

**Clinical continuity during ransomware:**
- Revert to paper prescription pads
- Use offline appointment book
- Defer non-urgent telehealth appointments
- Critical patients to be seen in person
- Clinical Lead manages patient communications

**Recovery sequence:**
1. Forensic investigation completed
2. Ransom decision by CEO and insurer
3. Systems rebuilt from clean backups
4. Patient record integrity verified
5. Clinical Lead approves return
6. Intensive monitoring for 30 days

### SCENARIO B: Phishing and Account Compromise
**Classification:** TIER 1 or 2  
**POPIA Reportable:** ASSESS IMPACT

**Immediate actions:**
- [ ] Revoke compromised account credentials
- [ ] Enable MFA on account immediately
- [ ] Review all actions taken by account in last 30 days (audit logs)
- [ ] Check for email forwarding rules set up by attacker
- [ ] Check for new users or admin accounts created during compromise
- [ ] Assess what data the account could access
- [ ] If patient data accessed: TIER 1. Start POPIA 72 hour clock
- [ ] Scan all devices used by that account
- [ ] Check other staff for same phishing email
- [ ] Block sender and domain in email filter
- [ ] Staff-wide alert about the phishing method

**Signs attacker still has access:**
- Unexpected password reset emails
- Login alerts from unusual locations
- Email rules you did not create
- New admin accounts in the tenant
- Patient records accessed at unusual times

### SCENARIO C: Stolen or Lost Laptop
**Classification:** TIER 1 (if no encryption), TIER 2 (if encrypted)  
**POPIA Reportable:** YES if unencrypted

**Immediate actions:**
- [ ] Confirm encryption status in asset register (BitLocker on = lower risk, BitLocker off = POPIA breach confirmed)
- [ ] Remotely wipe device via Intune if enrolled in MDM
- [ ] Revoke all credentials stored on device
- [ ] Identify all patient data accessible from that device
- [ ] If unencrypted: Start POPIA 72 hour clock
- [ ] Report to SAPS (required for insurance) - Get case number
- [ ] Notify cyber insurer
- [ ] Identify last known location and circumstances of loss or theft
- [ ] Review CCTV if available

> This is why Project 1 Gap 5 was rated CRITICAL and BitLocker was the first recommended action.  
> **One encrypted stolen laptop = a TIER 2 incident.**  
> **One unencrypted stolen laptop = a TIER 1 POPIA breach.**

### SCENARIO D: POPIA Data Breach Notification Procedure
**Classification:** TIER 1  
**Triggered by:** Any confirmed unauthorised access to personal information

**72 Hour Notification Procedure:**

**HOUR 0 - DISCOVERY**
- Incident discovered and classified
- Information Officer notified immediately
- 72 hour clock starts NOW
- Deadline recorded: Discovery time ______ / Deadline ______

**HOUR 0-4 - ASSESSMENT**
- Confirm what data was affected
- Confirm how many data subjects affected
- Confirm how the breach occurred
- Confirm if breach is ongoing or contained
- Begin preparing notification documents

**HOUR 4-24 - PREPARATION**
- Draft notification to Information Regulator using prescribed Form 4 (Available at: inforegulator.org.za)
- CEO reviews and approves draft
- Legal counsel reviews if available
- Prepare affected person notification
- Document all containment actions taken

**HOUR 24-72 - NOTIFICATION**
- Submit Form 4 to Information Regulator:
  - Email: inforegulator@inforegulator.org.za
  - Portal: inforegulator.org.za
- Notify affected data subjects as soon as reasonably possible
- Keep evidence of submission
- Log submission time and confirmation

**Information Regulator Notification MUST include:**
- [ ] Description of the breach
- [ ] Date and time of breach and discovery
- [ ] Categories of personal information affected
- [ ] Approximate number of data subjects
- [ ] Likely consequences of the breach
- [ ] Measures taken or proposed to address it
- [ ] Contact details of Information Officer

**After Notification:**
- Cooperate fully with Information Regulator
- Provide updates as investigation progresses
- Do not destroy any evidence
- Legal counsel present for any meetings

---

## 6. Incident Log Format

Incident ID: INC- :______________

Date Opened       :______________

Date closed       :______________

Severity Tier     :______________

Category          :______________

POPIA Reportable  : YES / NO

POPIA Notified    : YES / NO / N-A

Notification Time : __________

Deadline Met      : YES / NO

Incident Description   :

Affected System        :

Affected Data / Person:

Timeline Of Events    :
[Time] [Action] [By Whom] [Outcome]

Root Cause            :

Containment Action    :

Eradication Action    :

Recovery Action       :

Lesson Learned        :

Risk Register Updated : YES / NO
Date Updated          : ______________
Corrective Actions Assigned : YES/NO

Incident Closed By   : ______________
Date                 : ______________

---


---

## 7. Key Contacts Quick Reference

**Print this page and store offline:**

| Contact | Number |
|---------|--------|
| IT Manager (IR Lead) | __________ |
| Information Officer | __________ |
| CEO | __________ |
| Clinical Lead | __________ |
| Cyber Insurer Hotline | __________ |
| Legal Counsel | __________ |
| Forensic IR Firm | __________ |
| Microsoft Support | __________ |
| Information Regulator | inforegulator@inforegulator.org.za / Tel: 012 406 4818 |
| SAPS (for stolen devices) | 10111 |

---

**Document Control**  
Prepared by: Patrick Mohlala, GRC Analyst  
Version: 1.0  
Status: Draft - Pending CEO Approval  
Review: June 2026
