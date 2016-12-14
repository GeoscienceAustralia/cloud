---
title: Security
layout: page
permalink: security_index.html
---

### AWS keys
Don't commit your AWS keys to git repositories!

### So I'm writing code...
* Have you had a look at the [OWASP Top 10](https://www.owasp.org/index.php/OWASP_Top_Ten_Cheat_Sheet)?
* Have you checked out the [CWE Top 25](http://cwe.mitre.org/top25/index.html#Listing)?

### So I've got an AWS space...

* Enable [Multi-Factor Authentication](https://aws.amazon.com/iam/details/mfa/) on all user accounts in your space.
* Run [Cloudsploit](https://github.com/GeoscienceAustralia/cloudsploit-lambda) regularly to audit the security of the infrastructure in your space.
* Have a read of the [AWS security whitepapers](https://aws.amazon.com/whitepapers/).
* Ensure you're not committing your AWS credentials to public repositories. One solution could be [git-secrets](https://github.com/awslabs/git-secrets).
* If you have [premium support](https://aws.amazon.com/premiumsupport/) enabled on your AWS account, you can use [AWS Trusted Advisor](https://aws.amazon.com/premiumsupport/trustedadvisor/), which can help you reduce cost, increase performance, and improve security by optimizing your AWS environment. Note that business support incurs an additional fee on your account.
* Familiarise yourself with GA security policies on the intranet. Remember you can get in touch with the ICTIS Security team if you have any questions about IT security.

### But seriously...
Seriously, don't commit your AWS keys to git repositories!
