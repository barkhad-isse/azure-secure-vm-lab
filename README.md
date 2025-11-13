# Azure Secure VM Lab

## Overview

This project demonstrates how to securely deploy, monitor, and audit a Linux virtual machine in Microsoft Azure. The lab follows Microsoft best practices to restrict access, enable logging, and integrate security monitoring.

## Setup Summary

- **Resource Group:** `rg-securevm-swiss`
- **Region:** Switzerland North
- **Subscription:** Azure for Students
- **Virtual Machine:** Ubuntu Server 24.04 LTS (B1s)
- **Public Inbound Ports:** None (restricted by NSG)
- **Disk Type:** Standard HDD
- **Boot Diagnostics:** Enabled
- **Auto-Shutdown:** Enabled (19:00)

## Network Security Configuration

1. Created a Network Security Group (`nsg-securevm`) in the same resource group and region.
2. Added a custom inbound rule to allow SSH (TCP port 22) only from my public IP address.
3. Associated the NSG with the VM’s network interface.






## Monitoring & Logging

1. Provisioned a Log Analytics workspace (`law-securevm`) in the same resource group and region.
2. Created a Data Collection Rule (`dcr-securevm`) to install the Azure Monitor Agent on the VM and send performance counters and logs to the workspace.
3. Verified that data ingestion started via Azure Monitor.






## Defender for Cloud

1. Enabled Microsoft Defender for Servers in Azure Defender for Cloud.
2. Confirmed that the VM is protected and monitored for vulnerabilities and threats.
3. Reviewed Defender recommendations, such as enabling disk encryption.




## Mock Security Audit

After all services were configured, I performed a brief security audit:

- **Network Access:** SSH restricted to a single IP address via NSG.
- **Monitoring:** Azure Monitor Agent installed; performance and syslog data collected in Log Analytics.
- **Defender for Cloud:** enabled; no critical alerts were detected.
- **Recommendations:** Non‑critical suggestion to enable disk encryption.

## Learnings

- How to design granular NSG rules to restrict access.
- Integrating Log Analytics and Azure Monitor Agent for centralized monitoring.
- Enabling Microsoft Defender for Cloud to assess security posture.
- Importance of regular audits and following recommendations to enhance security.
