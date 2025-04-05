## 🧪 Lab Scenario Summary

This lab takes place in a simulated enterprise network environment where **internal traffic is unrestricted**, and tools like PowerShell are **not governed by any execution policy restrictions**.

The **Server Operations team** has reported **degraded performance** on aging infrastructure within the `10.0.0.0/16` subnet. After ruling out **external DDoS or upstream provider issues**, the **Security Operations Center (SOC)** has been tasked with investigating internal traffic patterns for signs of misconfiguration, malicious activity, or resource exhaustion.

As the analyst, your goal is to **identify the root cause** of this internal performance issue by analyzing logs, correlating network and process activity, and building a timeline of suspicious behavior.

---

## 📌 Lab Objectives

| Objective ID | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| OBJ-01       | Analyze internal traffic in the `10.0.0.0/16` subnet                        |
| OBJ-02       | Identify devices with the highest connection counts                         |
| OBJ-03       | Correlate process-level activity with network events                        |
| OBJ-04       | Detect any scripting abuse (e.g., PowerShell used for automation/beaconing) |
| OBJ-05       | Determine root cause of degraded network performance                        |
| OBJ-06       | Provide a summary of key findings and remediation recommendations           |

---

## 📁 Repository Contents

| File                              | Description                                                  |
|-----------------------------------|--------------------------------------------------------------|
| `Investigation.txt`              | Queries and logic used during investigation          |
| `Report_Findings.txt`            | MITRE ATT&CK-style analysis of findings                      |
| `TotalDeviceNetworkEvents.csv`   | Raw output of device-level network connection logs           |
| `TotalConnectionsPerDeviceNetworkEvents.csv` | Summary of top connection counts by device         |
| `felix-win10-investigation.csv`  | Detailed filtered activity on `felix-win10`                  |
| `felix-win10.csv`                | Correlation between process and network behavior             |

---

## 🛠️ Tools Used

- Microsoft Sentinel (Log Analytics Workspace)
- Microsoft Defender for Endpoint
- Kusto Query Language (KQL)
