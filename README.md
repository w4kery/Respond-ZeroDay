# Respond to a ZeroDay Attack
## What you'll learn

Learn how to address a vulnerability that may affect Product Development Staging Environment infrastructure.

## What you'll do

- Review recent publications from the Cybersecurity & Infrastructure Security Agency (CISA).
- Research the reported vulnerability.
- Draft an email to affected teams to alert them of the vulnerability and explain how to remediate.

## Background Information

You are an Information Security Analyst in the Cyber & Information Security Team.

As an information security analyst, your responsibility is to stay on top of emerging vulnerabilities to ensure timely remediation before potential exploitation by attackers.

In this task, review recent publications from the Cybersecurity & Infrastructure Security Agency (CISA) and draft an email to inform the relevant infrastructure owner at AIG of the seriousness of the reported vulnerability.

## Task Instructions

CISA has recently published two advisories:

    1. The first advisory (Log4j) outlines a serious vulnerability in one of the world’s most popular logging software.
[Mitigating Log4Shell and Other Log4j-Related Vulnerabilities](https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-356a)<br>

    2. The second advisory explores the increasing professionalization of ransomware, a concern for a large company like AIG.
[CISA, FBI, NSA and International Partners Issue Advisory on Ransomware Trends from 2021](https://www.cisa.gov/news-events/news/cisa-fbi-nsa-and-international-partners-issue-advisory-ransomware-trends-2021)<br>


Your task is to respond to the Apache Log4j zero-day vulnerability by advising affected teams of the vulnerability.

Conduct research on the vulnerability using the provided "CISA Advisory" resources as a starting point. Analyze the "Infrastructure List" to identify affected infrastructure and ownership.

## Infrastructure List
Product Team	Product Name	Team Lead	Services Installed
IT	Workstation Management System	Jane Doe (tech@email.com)	OpenSSH, dnsmasq, lighttpd
Product Development	Product Development Staging Environment	John Doe (product@email.com)	Dovecot pop3d, Apache httpd, Log4j, Dovecot imapd, MiniServ
Marketing	Marketing Analytics Server	Joe Schmoe (marketing@email.com)	Microsoft ftpd, Indy httpd, Microsoft Windows RPC, Microsoft Windows netbios-ssn, Microsoft Windows Server 2008 R2 - 2012 microsoft ds
HR	Human Resource Information System	Joe Bloggs (hr@email.com)	OpenSSH, Apache httpd, rpcbind2-4

## Example Advisory Email

**From:** AIG Cyber & Information Security Team

**To:** Product Development Team

**Subject:** Security Advisory concerning Product Development Staging Environment Log4j Vulnerability

**Body:**
Hello John Doe,

AIG Cyber & Information Security Team would like to inform you that a recent Log4j vulnerability has been discovered in the security community that may affect Product Development Staging Environment.

**Vulnerability Description:** The Log4j vulnerability poses a serious risk to the confidentiality and integrity of data.<br>
**Vulnerability Risk/Impact:** If exploited, an attacker may gain unauthorized access to sensitive information and compromise the integrity of the staging environment.<br>
**Vulnerability Remediation:** We recommend immediate action to patch the Log4j vulnerability on all affected systems. Detailed remediation steps can be found here.<br>
**Assurances:** Our team will provide support throughout the remediation process. For any questions or issues, don’t hesitate to reach out to us.<br>

Kind regards,
AIG Cyber & Information Security Team


## My Final Advisory Email
**From:** AIG Cyber & Information Security Team<br>
**To:** Product Development Team (product@email.com)<br>
**Subject:** Security Advisory concerning Product Development Staging Environment | Log4j<br>

**Body:**<br>
Hello John Doe,

AIG Cyber & Information Security Team would like to inform you that a recent Log4j vulnerability has been discovered in the security community that may affect the Product Development Staging Environment infrastructure.<br>

**Vulnerability Overview:** Log4j, a widely-used open-source tool for application logging, has recently been identified with a critical vulnerability in versions Log4j2 2.0-beta9 through 2.15.0. This vulnerability, identified as [CVE-2021-44228](https://nvd.nist.gov/vuln/detail/CVE-2021-44228) and [CVE-2021-45046](https://nvd.nist.gov/vuln/detail/CVE-2021-45046), could allow an unauthenticated attacker to execute remote code on the affected infrastructure.<br>

**Affected Products:**
- Log4j2 2.0-beta9 through 2.15.0<br>
Risk & Impact: Critical - remote code execution (RCE). Exploitation of this vulnerability could grant unauthorized access, leading to data exfiltration or malicious actions within the Product Development Staging Environment.

**Remediation Steps:**
1.	Identify any assets or infrastructure running the affected Log4j version.
2.	Update Log4j to versions 2.16.0 (Java 8) and 2.12.2 (Java 7).
3.	Remain vigilant for signs of exploitation.<br>

**Confirmation:** Once you've addressed this vulnerability, please confirm the remediation with a reply to this email.

**Additional Information:** For further details and resources, you can refer to the NIST disclosures on NVD - CVE-2021-44228 and NVD - CVE-2021-45046.

**Contact Us:** If you have any questions or concerns, feel free to reach out to our team. Your prompt attention to this matter is highly appreciated.<br>

Kind regards,<br>
AIG Cyber & Information Security Team


## **Summary:**
The **Respond-ZeroDay** project focuses on addressing the Apache Log4j zero-day vulnerability affecting the Product Development Staging Environment at AIG. Information Security Analysts are tasked with reviewing CISA advisories, conducting research, and drafting advisory emails to notify and guide affected teams. The provided infrastructure list aids in identifying the affected teams and infrastructure. The drafted email follows a concise and direct format, ensuring clarity on the vulnerability's seriousness, risks, and recommended remediation steps.
