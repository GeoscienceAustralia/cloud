---
title: General Security
layout: page
permalink: general_security_sub.html
---

### ISM

Have a read of the [Australian Government Information Security Manual](http://www.asd.gov.au/publications/Information_Security_Manual_2016_Controls.pdf) (pdf). Especially useful are the top 4 strategies:

1. Application whitelisting
2. Patch applications
3. Patch operating systems
4. Restrict administrative privileges.

### https by default

Your site should use https by default, and should redirect http to https. This is especially true for a \*.ga.gov.au site.

*Why https?*
Unencrypted http doesn't protect data from interception or alteration. The user is vulnerable to man-in-the-middle attacks or snooping. For more details, check out the [HTTPS Only Standard](https://https.cio.gov/) from the US Government's CIO Council.

*How do I make this happen?*
If your site is on AWS, use [ACM](https://aws.amazon.com/certificate-manager/). If not, use [LetsEncrypt](https://letsencrypt.org/).
