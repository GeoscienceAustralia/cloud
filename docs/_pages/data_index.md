---
title: Data & records Policy
layout: page
permalink: data_index.html
---

<h2> things to include</h2>
* data retention 
* data archiving
* data sharing
* data classification
* data backup

<h2>Protecting Data at Rest</h2>
GA recommends that you protect your data at rest stored in Amazon S3, on Amazon EBS, Amazon RDS, or other services from AWS.

consider when you are implementing protection of data at rest on the cloud.

| Concern | Recommended Protection Approach | Strategies | 
| --- | --- | --- |
| Accidental information disclosure | Designate data as confidential and limit the number of users who can access it. Use AWS permissions to manage access to resources for services such as Amazon S3. Use encryption to protect confidential data on Amazon EBS, or Amazon RDS. |Permissions. File, partition, volume or application-level encryption  |
| Data integrity compromise | To ensure that data integrity is not compromised through deliberate or accidental modification, use resource permissions to limit the scope of users who can modify the data. Even with resource permissions, accidental deletion by a privileged user is still a threat (including a potential attack by a Trojan using the privileged user’s credentials), which illustrates the importance of the principle of least privilege. Perform data integrity checks, such as Message Authentication Codes (SHA-1/SHA-2), or Hashed Message Authentication Codes (HMACs), digital signatures, or authenticated encryption (AES-GCM), to detect data integrity compromise. If you detect data compromise, restore the data from backup, or, in the case of Amazon S3, from a previous object version. | Permissions. Data integrity checks (MAC/HMAC/Digital Signatures/Authenticated Encryption). Backup. Versioning (Amazon S3) |
| Accidental deletion | Using the correct permissions and the rule of the least privilege is the best protection against accidental or malicious deletion. For services such as Amazon S3, you can use MFA Delete to require multi-factor authentication to delete an object, limiting access to Amazon S3 objects to privileged users. If you detect data compromise, restore the data from backup, or, in the case of Amazon S3, from a previous object version. | Permissions Backup. Versioning (Amazon S3). MFA Delete (Amazon S3) |
| System, infrastructure, hardware or software availability | In the case of a system failure or a natural disaster, restore your data from backup, or from replicas. Some services, such as Amazon S3 and Amazon DynamoDB, provide automatic data replication between multiple Availability Zones within a region. Other services require you to configure replication or backups. | Backup Replication |


<h2>Australian Government security classification system</h2>
https://www.protectivesecurity.gov.au/informationsecurity/Pages/AustralianGovernmentSecurityClassificationSystem.aspx

The Australian Government information security management guidelines—Australian Government security classification system gives guidance in identifying and grading the confidentiality requirements of official information.

The guidelines assist agencies to identify the value of information and in turn apply a suitable protective marking.

These guidelines cover:

    types of official information:

        information not requiring additional protection
        information requiring security classifications:
            PROTECTED
            CONFIDENTIAL
            SECRET
            TOP SECRET
        information requiring dissemination limiting markers (DLMs):
            For Official Use Only
            the four Sensitive DLMs (Sensitive: Cabinet, Sensitive: Personal, Sensitive: Legal and Sensitive)
        types of caveats

    who applies protective markings
    when protective markings are applied
    altering protective markings
    managing over-classification
    duration of classifications.
