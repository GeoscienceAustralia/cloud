---
title: Setting Up AWS Account
layout: page
permalink: cloud/setting_up_aws_sub.html
---

# First steps

1. Join [Slack](https://geoscience-australia.slack.com/signup), our messaging app. It's a great place to ask questions.
2. Join the #awscop and #autobots channels to chat with experts from across GA.
3. Talk with your Divisional Information Officer (DIO) and/or the Autobots about what you wish to achive. If you are just looking to have a play with AWS or try out a specific service, then the GA AWS Development environment may be suitable for your needs.

# Create an AWS account

If you have an application that will eventually become a production service, you should create a stand-alone account. The steps for creating a new AWS account are:

## 1. Email the [Autobots](mailto:autobots@ga.gov.au)

Include this information in your email:

  * Documented approval from your section leader/financial delegate with GA Cost and Activity Codes. Approval needs be documented (e.g. in an email) as it is supporting the expenditure of Government funds - and will be needed to support adding the account to GA's Consolidated Billing account.
  
  * The name for your Account.
  
  * A valid group email address, we can create one if you don't have one.
  
  * The name of the technical owner of the account. This user will receive credentials to log into the new account, and they will be responsible for the security of the account.

## 2. Log in

The technical owner of the account will receive an email with:
* A link to the new account
* A temporary password

They will need to log in and set a new password.
  
## 3. Secure it!

The technical owner of the account will need to:
 * Reset the password of the root account

## 4. Clean up steps 

 * Add [Multi Factor Authentication (MFA) to your root account](http://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_mfa_enable_virtual.html#enable-virt-mfa-for-root)
 * Contact the Cloud Enablement Team to arrange to store root credentials and MFA Key for safekeeping
 * Update your contact email addresses if necessary
 * Do steps to set IAM Security Status to Green
 * [Customise your sign-in link](http://docs.aws.amazon.com/IAM/latest/UserGuide/console_account-alias.html)
 
## 5. Configure security baseline

 * Run [space-provisioner](https://bitbucket.org/geoscienceaustralia/space-provisioner/) on your new account to configure minimum security settings like password policies, logging, etc.
 * Run [cloudsploit](https://github.com/GeoscienceAustralia/cloudsploit-lambda) on your account to set up automatic security auditing
 
## 6. Add other users
 
 * [Create IAM users](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html) for other users of the account
 * Make sure to [enable MFA](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_mfa.html) for these users
 * Add the users to the groups created by [space-provisioner](https://bitbucket.org/geoscienceaustralia/space-provisioner/) above, or create your own policies/groups
 * Discontinue use of the root account
