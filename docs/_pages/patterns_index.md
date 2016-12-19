---
title: Patterns & Examples
layout: page
permalink: patterns_index.html
---

## AWS

### Guides

[The Open Source Guide to AWS](https://github.com/open-guides/og-aws/blob/master/README.md)

### Creating an AMI

[Simple webserver](https://github.com/GeoscienceAustralia/cloud-examples/tree/master/simple-webserver)

This will create an Amazon Machine Image running Apache. This AMI can then be used to create a running EC2 instance.

### Creating AWS infrastructure

[Two-tier webserver](https://github.com/GeoscienceAustralia/cloud-examples/tree/master/two-tier-vpc)

This will create:

 * An autoscaling web server group
 * An elastic load-balancer
 * A VPC with a NAT server and a jump host

[Webserver with a database](https://github.com/GeoscienceAustralia/cloud-examples/tree/master/three-tier-rds)

This will create:

 * An autoscaling web server group
 * An elastic load-balancer
 * A Postgres database
 * A VPC with a NAT server and a jump host

[Static website with S3 and Cloudfront](https://github.com/GeoscienceAustralia/cloud-examples/tree/master/s3-www-cloudfront)

This will create a static website on S3 with a Cloudfront distribution for content delivery.

[VPC](https://github.com/GeoscienceAustralia/cloud-examples/tree/master/vpc)

This will create a virtual private cloud.

## NCI

In progress.

## CSC Cloud

In progress.
