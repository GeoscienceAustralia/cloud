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

If you're just getting started, look at the various workshop examples ([Workshop 1](https://bitbucket.org/geoscienceaustralia/tutorial-1-ec2), [Workshop 2](https://bitbucket.org/geoscienceaustralia/tutorial-2-ec2-userdata), [Workshop 3](https://bitbucket.org/geoscienceaustralia/tutorial-3-asg)) or have a look at [18F's fantastic walkthrough](https://github.com/jezhumble/cloud-native-aws-terraform-workshop).

If you're looking for something more advanced, look at the approved example architectures:

[Webserver Architecture](https://bitbucket.org/geoscienceaustralia/webserver)

This will create:

 * An autoscaling web server group
 * An elastic load-balancer
 * A VPC with a NAT gateway and a jump host

[Webserver + EFS Architecture](https://bitbucket.org/geoscienceaustralia/webserver-efs)

This will create:

 * An autoscaling web server group
 * An EFS network drive for shared storage
 * An elastic load-balancer
 * A VPC with a NAT gateway and a jump host

[Webserver with a database](https://bitbucket.org/geoscienceaustralia/webserver-db)

This will create:

 * An autoscaling web server group
 * An elastic load-balancer
 * A Postgres database
 * A VPC with a NAT gateway and a jump host

[Webserver + EFS with a database](https://bitbucket.org/geoscienceaustralia/webserver-efs-db)

This will create:

 * An autoscaling web server group
 * An EFS network drive for shared storage
 * An elastic load-balancer
 * A Postgres database
 * A VPC with a NAT gateway and a jump host

[Static website](https://bitbucket.org/geoscienceaustralia/static-website)

This will create

 * A static website on S3
 * A Cloudfront distribution for caching and content delivery
 
