# Microsoft Purview DLP Alert Investigation

## Overview

This project demonstrates a simulated investigation of a Microsoft Purview Data Loss Prevention (DLP) alert involving sensitive data exposure in OneDrive.

The investigation focused on:
- DLP policy violations
- Sensitive information exposure
- File exfiltration activity
- User risk analysis
- Incident correlation using Microsoft Purview and Microsoft Defender

---

# Scenario

A high-severity DLP alert was triggered for the file:

`spreadsheet_2.xlsx`

The alert indicated suspicious handling of sensitive information stored in OneDrive.

---

# Tools Used

- Microsoft Purview
- Microsoft Defender
- Microsoft Copilot for Security
- Data Loss Prevention (DLP)
- Insider Risk Management

---

# Investigation Steps

## 1. Reviewed DLP Alert

Navigated to:

`Solutions > Data Loss Prevention > Alerts`

Selected the alert:

> DLP policy match for document 'spreadsheet_2.xlsx' in OneDrive

Severity:
- High

Alert Status:
- Active

---

## 2. Investigated Alert Details

Reviewed:
- Details tab
- Classifiers tab
- File activity tab
- Metadata tab

Key findings:
- Sensitive information was detected in the spreadsheet
- The file contained confidential content and regulated data
- The activity involved OneDrive downloads and USB transfers

---

## 3. Observed Suspicious Activities

The investigation identified multiple risky actions:

### Collection Activity
- Files downloaded from OneDrive

### Exfiltration Activity
- Files copied to USB devices

### Obfuscation Activity
- Sensitivity labels were downgraded

These activities strongly indicated potential data exfiltration behavior.

---

# Sensitive Data Identified

The alert referenced sensitive information including:
- U.S. Social Security Numbers (SSNs)
- Medical terms and conditions
- Confidential project information
- Internal organizational data

---

# User Risk Findings

The user involved:
- Natasha David
- Insider Risk Severity: High

Additional observations:
- User was associated with multiple active alerts
- User was in scope of several insider risk policies
- Copilot summaries highlighted suspicious file handling behavior

---

# Skills Demonstrated

- DLP alert triage
- Security investigation
- Insider risk analysis
- Incident correlation
- Microsoft Purview operations
- Microsoft Defender investigation workflow
- Security operations documentation
