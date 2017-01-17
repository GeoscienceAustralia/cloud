---
title: SSL & HTTPS
layout: page
permalink: ssl_sub.html
---

### https by default

Your site should use https by default, and should redirect http to https. This is especially true for a \*.ga.gov.au site.

*Why https?*
Unencrypted http doesn't protect data from interception or alteration. The user is vulnerable to man-in-the-middle attacks or snooping. For more details, check out the [HTTPS Only Standard](https://https.cio.gov/) from the US Government's CIO Council.

*How do I make this happen?*
If your site is on AWS, use [ACM](https://aws.amazon.com/certificate-manager/). If not, use [LetsEncrypt](https://letsencrypt.org/).
