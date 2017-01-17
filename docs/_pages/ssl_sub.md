---
title: SSL & HTTPS
layout: page
permalink: ssl_sub.html
---

### https by default

Your site should use https by default, and should redirect http to https. This is especially true for a \*.ga.gov.au site.

Unencrypted http doesn't protect data from interception or alteration. The user is vulnerable to man-in-the-middle attacks or snooping. For more details, check out the [HTTPS Only Standard](https://https.cio.gov/) from the US Government's CIO Council.

### Certificate providers

If your site is on AWS, use [ACM](https://aws.amazon.com/certificate-manager/). If not, use [LetsEncrypt](https://letsencrypt.org/).

### ACM

* From the Certificate Manager console in AWS, request a certificate
* Add the name of your server (or servers), or add a wildcard certificate for your domain
* An approval email will be sent to [a number of email addresses](http://docs.aws.amazon.com/acm/latest/userguide/gs-acm-validate.html) to ensure that you have the approval of the domain owner. For example, for a request for a certificate for \*.server.example.com, emails will be sent to:
  * admin@server.example.com
  * administrator@server.example.com
  * hostmaster@server.example.com
  * postmaster@server.example.com
  * webmaster@server.example.com
* When the link in the email is clicked, the certificate is generated and ready for use!
* [Add an HTTPS listener to your load balancer](http://docs.aws.amazon.com/elasticloadbalancing/latest/classic/elb-https-load-balancers.html), then attach the certificate

### LetsEncrypt
