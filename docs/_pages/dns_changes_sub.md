---
title: Making DNS Changes
layout: page
permalink: cloud/dns_changes_sub.html
---

### Creating a \*.ga.gov.au domain

[Create a hosted zone](http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/CreatingHostedZone.html) in AWS Route 53. When the zone is created, you will be given a list of four AWS nameservers.

Raise a support request to delegate control of this subdomain to these nameservers. Mark this request as "Attn: Networks, Windows, Linux". This request should be automatically sent to Products & Promotions for approval. Once done, this will make these nameservers the authority for this zone, so make sure your records are in place before raising the request.

The content of the request should:

1. Request a ticket be raised to our upstream DNS provider to make these changes to their DNS configuration. ("Attn: Networks")
2. Request an update to internal DNS to reflect these external changes. ("Attn: Windows")
3. Request an update to internal proxy to ensure routing is performed correctly. ("Attn: Linux")

### Creating a \*.gov.au website

You'll need to raise a request with the [gov.au domain registrar](https://www.domainname.gov.au/). (The Aubots have an account.) The request will undergo some serious scrutiny, so you'll need a business case.

### Creating a test domain

You could purchase your own test domain, or you could contact the Autobots to use their existing test domain.
