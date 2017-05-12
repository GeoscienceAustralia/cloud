---
title: AWS Patterns
layout: page
permalink: cloud/aws_patterns_sub.html
---

### Creating an AMI

Example AMI builds are located in the [Packer project](https://bitbucket.org/account/user/geoscienceaustralia/projects/PAC). These include:

[Simple webserver](https://bitbucket.org/geoscienceaustralia/simple-webserver)

This will create a security-hardened Amazon Machine Image running Apache. This AMI can then be used to create a running EC2 instance.
 
[Tomcat](https://bitbucket.org/geoscienceaustralia/tomcat-packer)

This will create a security-hardened Amazon Machine Image running Tomcat. This can be used as a basis to run any Java web container, including applications running on Geoserver.

### Creating AWS infrastructure

Example Terraform architectures are located in the [Terraform project](https://bitbucket.org/account/user/geoscienceaustralia/projects/TF).

If you're just getting started, look at the various workshop examples ([Workshop 1](https://bitbucket.org/geoscienceaustralia/workshop_ec2), [Workshop 2](https://bitbucket.org/geoscienceaustralia/workshop_ec2-userdata), [Workshop 3](https://bitbucket.org/geoscienceaustralia/workshop_asg)).

If you're looking for something more advanced, look at the example architectures:

[Two-tier webserver](https://bitbucket.org/geoscienceaustralia/two-tier-www)

This will create:

 * An autoscaling web server group
 * An elastic load-balancer
 * A VPC with a NAT gateway and a jump host

[Webserver with a database](https://bitbucket.org/geoscienceaustralia/three-tier-rds)

This will create:

 * An autoscaling web server group
 * An elastic load-balancer
 * A Postgres database
 * A VPC with a NAT gateway and a jump host

[Static website with S3 and Cloudfront](https://bitbucket.org/geoscienceaustralia/s3-cloudfront)

This will create

 * A static website on S3
 * A Cloudfront distribution for content delivery

[Two-tier webserver with shared storage](https://bitbucket.org/geoscienceaustralia/two-tier-efs)

This will create:

 * An autoscaling web server group
 * An elastic load-balancer
 * A VPC with a NAT gateway and a jump host
 * An EFS file system
