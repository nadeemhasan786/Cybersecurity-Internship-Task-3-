# Cybersecurity-Internship-Task-3-
Vulnerability Scanning 


# Cybersecurity Internship - Task 3: Basic Vulnerability Scan

## Objective
Use free tools to identify common vulnerabilities on your personal computer using OpenVAS (Greenbone Community Edition).

## Tools Used
- Greenbone Community Edition (OpenVAS)
- Oracle VM VirtualBox

## Steps Performed

1.  **Setup:** Downloaded and imported the Greenbone Community Edition `.ova` file into VirtualBox.
2.  **Configuration:** Logged into the Greenbone Security Assistant (GSA) web interface and created a new target for my host PC's IP address.
3.  **Scanning:** Created and executed a "Full and fast" scan task.
4.  **Analysis:** Reviewed the generated report, focusing on High and Medium severity vulnerabilities.
5.  **Documentation:** Researched fixes for the identified vulnerabilities and documented the critical findings below.

## Scan Results & Critical Vulnerabilities

| Vulnerability Name | Severity | Description | Impact | Solution |
| :--- | :--- | :--- | :--- | :--- |
| SSL/TLS: Deprecated Version Usage | High | The scan detected support for outdated TLS 1.0/1.1 protocols. | Allows attackers to perform downgrade attacks and decrypt sensitive data. | Disable TLS 1.0 and 1.1 in the Windows registry or application settings. |
| Microsoft Windows SMB Server Unprivileged Access | Medium | An information disclosure vulnerability in the SMB file sharing protocol. | Could allow an attacker to read sensitive information remotely. | Apply the latest Windows security updates from Microsoft. |
| TCP Timestamps Potential OS Scan | Low | The system reveals TCP timestamps, which can help attackers determine the system's uptime. | Information disclosure that aids in network reconnaissance. | Disable TCP timestamps via the Windows registry. |

