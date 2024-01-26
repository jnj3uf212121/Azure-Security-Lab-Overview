1. Infrastructure Setup: Established a honeynet in Azure with two virtual machines (one Linux, one Windows), configured with VNets, resource groups, and open network security groups (NSGs) to welcome all internet traffic.

2. Lab Enhancement and Attack Simulation: Integrated MS SQL and Studio Manager on the Windows VM for detailed log oversight, and deployed an attack VM to simulate threats, analyzing the resulting event and authentication logs.

3. User and Log Management: Utilized Azure Active Directory to create users with varied permissions, exploring their log activities, and implemented centralized log management with Log Analytics Workspace, integrated with Azure Sentinel for enhanced security intelligence.

4. Security and Log Analysis: Activated Microsoft Defender for Cloud for consolidated security alerts, set up a dedicated storage account for NSG flow logs, and used KQL for in-depth log analysis.

5. Incident Response and Compliance: Adhered to NIST 800-61 guidelines for a comprehensive incident response lifecycle and enforced NIST 800-53 controls, especially SC-7, to strengthen cloud security through strategic NSG placements and network topology analysis.
