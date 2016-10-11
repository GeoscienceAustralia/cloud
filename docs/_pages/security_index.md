---
title: Security
layout: page
permalink: security_index.html
---

<h2>Cyber security incidents</h2>

We recommend that you implement a process to identify, report and contain any cyber security incident that could affect GA information. We suggest you deploy and manage tools (**list of tools link**) in such a way that they are capable of detecting and responding to information security incidents. Regular system integrity checks must be performed to detect deviation from the expected configuration.

Consider some of the following tools for detecting potential cyber security incidents:

    anomaly detection system
    intruder prevention system
    log analysis
    network and host-intrusion detection systems
    system integrity verification.

Report cyber security incidents to GA cloud manager, including the cause of the incident and what remediation has occurred. Reporting must occur within 48 hours of the incident occurring.

It is recommended the cyber security incidents are recorded in a register. At a minimum, the register should include:

    the date the incident was discovered
    the date the incident occurred
    a description of the incident, including the personnel and locations involved
    the action taken
    the date reported
    the file reference.



<h2>Cloud Computing Security Mitigation</h2>


| Risk                  | Mitigation reference number       | Mitigations
| ---                   | ---                               | ---
| Overarching failure to maintain the confidentiality, integrity and availability of the Geoscience Australia’s data   | 1 - General  | Obtain certification of the cloud service and underlying infrastructure (explicitly addressing mitigations in this document) against the Australian Government Information Security Manual (ISM) at the appropriate classification level required to handle the Geoscience Australia’s data. |
| -                                                                                                      | 2 - General  | Implement security governance involving senior management directing and coordinating security-related activities including robust change management, as well as having technically skilled staff in defined security roles. |
| -                                                                                                      | 3 - General  | Implement and annually test an incident response plan providing the Geoscience Australia with emergency contact details, the ability to access forensic evidence otherwise inaccessible to the Geoscience Australia, and contractual notification of incidents. |
| Geoscience Australia’s data compromised in transit by malicious third party                                          | 4 - General  | Support and use ASD-approved cryptographic controls to protect data in transit between the Geoscience Australia and the Cloud Service Provider e.g. application layer TLS or IPsec VPN with approved algorithms, key length and key management. |
| -                                                                                                      | 5 - General  | Use ASD-approved cryptographic controls to protect data in transit between the Cloud Service Provider’s data centres over insecure communication channels such as public Internet infrastructure. |
| -                                                                                                      | 6 - General  | Support and use ASD-approved cryptographic controls to protect data at rest on storage media in transit via post/courier between the Geoscience Australia and the Cloud Service Provider when transferring data as part of on-boarding or off-boarding. |
| Geoscience Australia’s cloud service account credentials compromised by malicious third party                        | 7 - General  | Provide Identity and Access Management e.g. multi-factor authentication and account roles with varying privileges for the Geoscience Australia to use and administer the cloud service via the Cloud Service Provider’s website control panel and API. |
| -                                                                                                      | 8 - General  | Support and use ASD-approved cryptographic controls to protect credentials and administrative activity in transit when the Geoscience Australia uses and administers the cloud service via the Cloud Service Provider’s website control panel and API. |
| -                                                                                                      | 9 - General  | Enable the Geoscience Australia to download detailed time-synchronised logs and obtain real-time alerts generated for the Geoscience Australia’s cloud service accounts used to access, and especially to administer, the cloud service. |
| Geoscience Australia’s data compromised by malicious Cloud Service Provider staff or malicious third party                              | 10 - General  | Enable the Geoscience Australia to download detailed time-synchronised logs and obtain real-time alerts generated by the cloud service used by the Geoscience Australia e.g. operating system, web server and application logs. |
| -                                                                                                      | 11 - General  | Disclose the countries and legal jurisdictions where Geoscience Australia data is (or will be in the coming months) stored, backed up, processed and accessed by Cloud Service Provider staff for troubleshooting, remote administration and customer support. |
| -                                                                                                      | 12 - General  | Perform background checks of Cloud Service Provider staff commensurate with their level of access to systems and data. Maintain security clearances for staff with access to highly sensitive data. |
| -                                                                                                      | 13 - General  | Use physically-secure data centres and offices that store Geoscience Australia data or that can access Geoscience Australia data15. Verify and record the identity of all staff and visitors. Escort visitors to mitigate them accessing data without authorisation.  |
| -                                                                                                      | 14 - General  | Restrict CSP staff privileged access to systems and data based on their job tasks12. Require re-approval every three months for CSP staff requiring privileged access. Revoke access upon termination of Cloud Service Provider staff employment. |
| -                                                                                                      | 15 - General  | Promptly analyse logs of Cloud Service Provider staff actions that are logged to a secured and isolated log server. Implement separation of duties by requiring log analysis to be performed by Cloud Service Provider staff who have no other privileges or job roles. |
| -                                                                                                      | 16 - General  | Perform a due diligence review of suppliers before obtaining software, hardware or services, to assess the potential increase to the Cloud Service Provider’s security risk profile. |
| -                                                                                                      | 17 - General  | Use ASD-approved cryptographic controls to protect highly sensitive data at rest. Sanitise storage media prior to repair, disposal, and Geoscience Australia off-boarding with a non-disclosure agreement for data in residual backups. |
| Geoscience Australia’s data compromised by another malicious/compromised Geoscience Australia                                      | 18 - General  | Implement multi-tenancy mechanisms to prevent the Geoscience Australia’s data being accessed by other Geoscience Australias. Isolate network traffic, storage, memory and computer processing. Sanitise storage media prior to its reuse. |
| Geoscience Australia’s data unavailable due to corruption, deletion, or Cloud Service Provider terminating the account/service         | 19 - General  | Enable the Geoscience Australia to perform up-to-date backups in a format that avoids Cloud Service Provider lock-in. If an account or cloud service is terminated, immediately notify the Geoscience Australia and provide them with at least a month to download their data. |
| Geoscience Australia’s data unavailable or compromised due to Cloud Service Provider bankruptcy or other legal action                   | 20 - General  | Contractually ensure that the Geoscience Australia retains legal ownership of their data. |
| Cloud service unavailable due to Cloud Service Provider’s inadequate network connectivity                                 | 21 - General  | Support adequately high bandwidth, low latency, reliable network connectivity between the Geoscience Australia and the cloud service to meet the claimed level of availability as required by the Geoscience Australia. |
| Cloud service unavailable due to Cloud Service Provider error, planned outage, failed hardware or act of nature           | 22 - General  | Architect to meet the claimed level of availability as required by the Geoscience Australia e.g. minimal single points of failure, clustering and load balancing, data replication, automated failover and real-time availability monitoring. |
| -                                                                                                      | 23 - General  | Develop and annually test a disaster recovery and business continuity plan to meet the claimed level of availability as required by the Geoscience Australia, e.g. enacted for incidents that cause enduring loss of Cloud Service Provider staff or infrastructure. |
| Cloud service unavailable due to genuine spike in demand or bandwidth/CPU denial of service            | 24 - General  | Implement denial of service mitigations to meet the claimed level of availability as required by the Geoscience Australia e.g. redundant high bandwidth external and internal network connectivity with traffic throttling and filtering. |
| -                                                                                                      | 25 - General  | Provide infrastructure capacity and responsive automated scaling to meet the claimed level of availability as required by the Geoscience Australia. |
| Financial consequences of a genuine spike in demand or bandwidth/CPU denial of service                 | 26 - General  | Enable the Geoscience Australia to manage the cost of a genuine spike in demand or denial of service via contractual spending limits, real-time alerts, and configurable maximum limits for their use of the Cloud Service Provider’s infrastructure capacity. |
| Cloud Service Provider’s infrastructure compromised by malicious Geoscience Australia or malicious third party                          | 27 - General  | Use corporately approved and secured computers, jump servers, dedicated accounts, strong passphrases and multi-factor authentication, to provide customer support and administer cloud services and infrastructure. |
| -                                                                                                      | 28 - General  | Use ASD-approved cryptographic controls to protect credentials and administrative activity in transit over insecure communication channels between the Cloud Service Provider’s data centre and Cloud Service Provider administrator / customer support staff. |
| -                                                                                                      | 29 - General  | Implement network segmentation and segregation26 between the Internet, CSP infrastructure used by Geoscience Australias, the network that the CSP uses to administer cloud services and infrastructure, and the Cloud Service Provider’s corporate LAN. |
| -                                                                                                      | 30 - General  | Utilise secure programming practices for software developed by the Cloud Service Provider.  |
| -                                                                                                      | 31 - General  | Perform secure configuration, ongoing vulnerability management, prompt patching, annual third party security reviews and penetration testing of cloud services and underlying infrastructure. |
| -                                                                                                      | 32 - General  | Train all CSP staff, especially administrators, on commencement of employment and annually, to protect Geoscience Australia data, maintain cloud service availability, and proactively identify security incidents e.g. via prompt log analysis. |
| Geoscience Australia’s Virtual Machine (VM) compromised by malicious third party                                    | 1 - LaaS      | Provide network access controls enabling the Geoscience Australia to implement network segmentation and segregation26, including a network filtering capability to disallow remote administration of their VMs except from their IP address. |
| -                                                                                                      | 2 - LaaS      | Provide the tenant with securely configured and patched VM template images. Avoid assigning a weak administrative passphrase to newly provisioned VMs. |
| Geoscience Australia’s data compromised by malicious third party                                                     | 1 - PaaS      | Harden and securely configure operating system, web server and platform software. Limit inbound and outbound network connectivity to only required ports/protocols. Promptly perform patching and log analysis. |
| Geoscience Australia’s data compromised by malicious third party                                                     | 1 - SaaS      | Implement security controls specific to the cloud service e.g. for email delivered as a service, provide features including whitelisted content filtering with automated dynamic analysis of emails and email attachments. |
| -                                                                                                      | 2 - SaaS      | Implement general security controls e.g. limited inbound and outbound network connectivity to only required ports/protocols, antivirus software updated daily, intrusion prevention systems and prompt log analysis. |


