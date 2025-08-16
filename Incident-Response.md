
## **What is Incident Response?**

**Incident Response (IR)** is the structured approach to handle and manage the aftermath of a **security breach or cyberattack**, also known as an incident. It includes steps to:
- Detect the incident
- Contain the damage
- Investigate the root cause
- Recover normal operations
- Report and document findings
## **Incident Response Process

The NIST Incident Response Lifecycle includes **4 main phases**:

| **Phase**                         | **Description**                                                                 |
|----------------------------------|---------------------------------------------------------------------------------|
| **1. Preparation**               | Establish policies, train team, and set up tools and logging mechanisms.       |
| **2. Detection and Analysis**    | Identify potential incidents using logs, alerts, and anomaly detection systems.|
| **3. Containment, Eradication, and Recovery** | Isolate threats, remove malware/artifacts, and restore systems securely.       |
| **4. Post-Incident Activity**    | Conduct lessons learned, create reports, and improve incident response plans.  |
## **Common Types of Incidents on Windows:**

| **Platform** | **Incident Type**                             | **Description**                                                                 |
|--------------|-----------------------------------------------|---------------------------------------------------------------------------------|
| **Windows**  | Unauthorized Login Attempts                   | Multiple failed logins or brute-force via RDP or local access.                  |
|              | PowerShell-based Attacks                      | Obfuscated or encoded PowerShell commands for exploitation or lateral movement. |
|              | Malware/Ransomware Execution                  | Malicious EXE/DLL files executed, causing encryption or data theft.             |
|              | Credential Dumping                            | Use of tools like Mimikatz to extract credentials from LSASS memory.            |
|              | Lateral Movement via WMI or RDP               | Internal system traversal using Windows services and accounts.                  |
| **Linux**    | SSH Brute Force or Unauthorized Access        | Repeated login attempts or access from unknown IPs via SSH.                     |
|              | Malicious Cron Jobs for Persistence           | Scheduled tasks created by attackers to maintain access.                        |
|              | Sudo Abuse / Privilege Escalation             | Exploiting weak sudo rules or known vulnerabilities to gain root privileges.    |
|              | Web Shell Upload                              | Attackers upload backdoors via vulnerable web applications.                     |
|              | Crypto Miner Installation                     | Hidden mining software running under compromised user accounts.                 |
| **AWS**      | IAM Credential Misuse                         | Leaked API keys used from unknown geographies.                                  |
|              | Root User Console Access                      | Suspicious login or activity from the AWS root account.                         |
|              | Unusual S3 Bucket Access                      | Public or unauthorized access to private storage.                               |
|              | CloudTrail or Logging Disabled                | Logging service turned off to hide attacker activity.                           |
|              | EC2 Abuse for Command and Control             | EC2 instances being used as a staging point or C2 server.                       |
| **Network**  | DDoS Attack                                   | Flood of traffic targeting public-facing services.                              |
|              | Port Scanning / Reconnaissance                | Continuous scanning of open ports across network segments.                      |
|              | ARP Spoofing / Man-in-the-Middle (MitM)       | Tampering with traffic flows for interception.                                  |
|              | DNS Tunneling                                 | Covert data exfiltration using DNS queries.                                     |
|              | Unauthorized VPN Access                       | Compromised VPN credentials used for internal access.                           |
| **Email**    | Phishing / Credential Harvesting              | Fake emails with links to steal user credentials.                               |
|              | Malware via Attachments                       | Office or ZIP files with embedded malware.                                      |
|              | Business Email Compromise (BEC)               | Attacker impersonates an executive to trick employees.                          |
|              | Spoofed Email Domains                         | Sending emails from domains that look like legitimate ones.                     |
|              | Internal Account Compromise                   | Compromised internal mailbox used to spread phishing internally.                |
## **Common Types of Incidents Across Platforms**
## **How SOC Analysts Respond to Incidents:**
- Monitor logs and alerts (via SIEM)
- Investigate suspicious behavior
- Contain and isolate infected systems
- Coordinate with other teams
- Document and report the incident


