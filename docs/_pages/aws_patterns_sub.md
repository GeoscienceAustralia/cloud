---
title: AWS Patterns
layout: page
permalink: cloud/aws_patterns_sub.html
---

### Creating an AMI

[Simple webserver](https://github.com/GeoscienceAustralia/packer/tree/master/simple-webserver)

This will create an Amazon Machine Image running Apache. This AMI can then be used to create a running EC2 instance.

### Creating AWS infrastructure

[Two-tier webserver](https://github.com/GeoscienceAustralia/terraform/tree/master/two-tier-vpc)

This will create:

 * An autoscaling web server group
 * An elastic load-balancer
 * A VPC with a NAT gateway and a jump host

[Webserver with a database](https://github.com/GeoscienceAustralia/terraform/tree/master/three-tier-rds)

This will create:

 * An autoscaling web server group
 * An elastic load-balancer
 * A Postgres database
 * A VPC with a NAT gateway and a jump host

[Static website with S3 and Cloudfront](https://github.com/GeoscienceAustralia/terraform/tree/master/s3-www-cloudfront)

This will create

 * A static website on S3
 * A Cloudfront distribution for content delivery
