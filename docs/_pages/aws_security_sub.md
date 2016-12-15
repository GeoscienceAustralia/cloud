---
title: AWS Security
layout: page
permalink: aws_security_sub.html
---

### AWS keys
Don't commit your AWS keys to git repositories!

### So I've got an AWS space...

* Don't commit your AWS credentials to public repositories. One solution could be [git-secrets](https://github.com/awslabs/git-secrets). If you do commit a key, delete the key from AWS immediately. You might also want to look into [BFG](https://github.com/IBM-Swift/BluePic/wiki/Using-BFG-Repo-Cleaner-tool-to-remove-sensitive-files-from-your-git-repo) to delete content from git permanently.
* Enable [Multi-Factor Authentication](https://aws.amazon.com/iam/details/mfa/) on all user accounts in your space.
* Run [Cloudsploit](https://github.com/GeoscienceAustralia/cloudsploit-lambda) regularly to audit the security of the infrastructure in your space.
* Have a read of the [AWS security whitepapers](https://aws.amazon.com/whitepapers/).
* If you have [premium support](https://aws.amazon.com/premiumsupport/) enabled on your AWS account, you can use [AWS Trusted Advisor](https://aws.amazon.com/premiumsupport/trustedadvisor/), which can help you reduce cost, increase performance, and improve security by optimizing your AWS environment. Note that business support incurs an additional fee on your account.
* Familiarise yourself with GA security policies on the intranet. Remember you can get in touch with the ICTIS Security team if you have any questions about IT security.

### And seriously...
Don't commit your AWS keys to git repositories!
