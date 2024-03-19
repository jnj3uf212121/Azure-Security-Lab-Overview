![SOC TOPOLOGY](https://github.com/jnj3uf212121/Azure-Security-Lab-Overview/assets/148787196/11aec0a1-bfe3-44c8-aed3-cf77a71802cb)

## Overview

Developed and executed a comprehensive security lab focused on Azure cloud services, encompassing setup, attack simulation, logging, monitoring, compliance, and incident response.

### 1. Lab Setup

- **Virtual Machine Configuration**: Two virtual machines (VMs) were created, one running Linux and the other Windows. These VMs were opened to the internet, creating a honeynet environment to attract potential attacks.
- **Networking**: Virtual networks were set up for each VM to ensure controlled communication channels. Additionally, resource groups were created for organizational purposes, with all resources assigned to the same geographical region for consistency.
- **Security Groups and Firewall Settings**: Network Security Groups (NSGs) were configured to allow any inbound internet traffic, simulating a vulnerable network environment. The Windows VM's firewall was specifically disabled to increase its exposure to potential attacks.

### 2. Software Installation and Configuration

- **Microsoft SQL and Studio Manager**: These were installed on the Windows VM to add complexity to the lab environment and provide additional targets for the simulated attacks.
- **Log Integration**: SQL logs were integrated with the Windows Event Manager to centralize logging and facilitate analysis.

### 3. Attack Simulation

- **Attack VM Setup**: A separate VM was configured to simulate attacks on the Windows and Linux VMs, as well as the SQL database. This allowed for practical experience in detecting and analyzing malicious activities.
- **Log Analysis**: Logs from the Event Manager and authentication logs were scrutinized to identify and understand the nature of the simulated attacks.

### 4. Azure Active Directory and Permissions

- **Azure AD Overview**: The lab included an exploration of Azure Active Directory, focusing on the relationships between tenants, subscriptions, and resource groups.
- **User Permissions**: Different users were created and assigned varying levels of permissions to observe and understand the effects of permission levels on resource access and security.

### 5. Logging and Monitoring

- **Log Analytics Workspace**: A central log aggregator was set up to consolidate logs from various sources for analysis.
- **Microsoft Defender for Cloud**: This feature was enabled to push all security alerts from VMs, the SQL database, and other resources into the log analytics workspace for centralized monitoring.

### 6. Security Incident and Event Management (SIEM)

- **Azure Sentinel**: This tool was used to analyze logs, create attack maps for visualizing malicious events, and generate alerts for detected malicious activities.
- **Incident Response**: Using NIST 800-61 guidelines, incidents were worked through to completion, including detection, analysis, containment, eradication, recovery, and documentation of findings.

### 7. Compliance and Security Hardening

- **NIST 800-53 Implementation**: Security controls from NIST 800-53 were applied to harden the environment against future attacks. This included configuring NSGs, enabling built-in firewalls, and setting up private links for public internet-exposed resources like storage accounts and key vaults.
- **Regulatory Compliance and Secure Score**: The Microsoft Defender for Cloud secure score was utilized to evaluate and improve the security posture of the cloud environment.

### Additional Activities

- **Logging at Different Levels**: Custom KQL queries were used to analyze logs at the tenant, subscription, and resource levels.
- **Scheduled Queries and Alert Testing**: Scheduled queries were set up to test alerts for brute force attacks and other malicious activities, with custom incident response playbooks developed for handling detected incidents.

### Conclusion

This lab provided a hands-on experience with setting up, attacking, and defending cloud-based environments using Azure's security tools and services. Through simulated attacks and the use of Azure's logging, monitoring, and compliance features, participants gained valuable insights into cloud security best practices and incident response strategies.

### Disclaimer:  Please note that the availability of images within this project is limited due to its proprietary nature. This project is not open source as it involves components for which licensing fees have been paid. I extend my gratitude to Josh Makador for his exceptional work in developing this fascinating lab!


