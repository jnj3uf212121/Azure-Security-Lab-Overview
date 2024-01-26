**Lab Report: Development and Analysis of a Mini Honeynet in Microsoft Azure**

**Introduction**

This report details the creation, configuration, and analysis of a mini honeynet within Microsoft Azure. The project's primary objectives were to integrate various log sources into a Log Analytics workspace, utilize Microsoft Sentinel for generating attack maps, triggering alerts, and creating incidents, and to observe the effectiveness of security metrics before and after the implementation of security controls.

**Lab Overview**

The project comprised several key phases, each contributing to the overall setup and analysis of the honeynet:

1. **Honeynet Creation**
   - Developed two Virtual Machines (VMs) - one Linux, one Windows - and exposed them to the internet.
   - Set up virtual networks and resource groups for the VMs, assigned them to the same region, and configured Network Security Groups (NSGs) to permit inbound internet traffic.
   - Disabled the internal firewall on the Windows VM.

2. **MS SQL Server Installation**
   - Installed MS SQL and Studio Manager on the Windows VM.
   - Configured SQL logs to integrate with Windows Event Manager logs.

3. **Attack Simulation**
   - Created an attack VM to simulate attacks on the Windows and Linux VMs and the SQL database.
   - Analyzed the resulting logs in the Event Manager and Authentication logs.

4. **Azure Active Directory Management**
   - Reviewed Azure Active Directory (AAD), created users with various permissions, and observed user activities at different levels.

5. **Logging and Monitoring**
   - Conducted a session on logging at different Azure layers.
   - Established a Log Analytics workspace as a centralized log aggregator and connected it to Sentinel.

6. **Microsoft Defender Integration**
   - Enabled Microsoft Defender for Cloud to funnel all security alerts from the VMs and SQL database into the Log Analytics workspace.

7. **NSG Flow Log and Data Collection**
   - Created a storage account for NSG flow logs to enter the Log Analytics workspace.
   - Configured and tested data collection rules manually and through cloud-based settings.

8. **KQL Deep Dive**
   - Provided an in-depth lesson on KQL (Kusto Query Language) and its application in analyzing logs.

9. **Azure Sentinel Implementation**
   - Utilized the imported logs in Sentinel to create attack maps, simulate attack traffic, and define alerts for malicious activities.
   - Worked through incidents in alignment with NIST 800-61 and hardened the environment following NIST 800-53 guidelines.

10. **Incident Response and Compliance**
    - Responded to incidents using NIST 800-61, documenting and closing incidents in Sentinel.
    - Enabled NIST 800-53 compliance in Microsoft Defender for Cloud and reviewed the secure score.
    - Implemented NIST 800-53 SC-7 (Boundary Protection), configured NSGs on subnets, enabled built-in firewalls, and configured private links.

**Additional Activities**

- Conducted detailed logging at the tenant, subscription, and resource levels using Azure Active Directory, Activity Logs, and Resource Logs.
- Simulated security incidents, such as brute force attacks and privilege escalations, and utilized NIST 800-61 for effective incident response.

**Metrics and Attack Maps**

*Pre- and Post-Hardening Metrics*: 
(See previous tables for specific metric counts before and after hardening)

- Notable reduction in security events and incidents post-hardening.
- Attack maps indicated a significant decrease in malicious activity after security measures were implemented.

**Conclusion**

This project effectively demonstrated the construction and analysis of a honeynet within Azure. The implementation of security controls, as guided by NIST 800-61 and 800-53 standards, led to a marked reduction in security events and incidents. The integration of tools like Microsoft Defender for Cloud and Azure Sentinel was pivotal in managing security within the cloud environment. This initiative not only highlighted the effectiveness of Azure's security features but also underscored the importance of proactive security measures in network management.
