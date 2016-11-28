---
title: Setting Up
layout: page
permalink: setting_up_index.html
---

### First steps

1. Join [Slack](https://geoscience-australia.slack.com/signup), our messaging app. It's a great place to ask questions.
2. Join the #awscop and #autobots channels to chat with experts from across GA.

### Setting up AWS

If you just want to experiment with AWS, you should get an account in the AWS Dev space. Send a Slack message or an email to the Autobots to get the ball rolling.

### Create an AWS space

If you have an application that will eventually become a production service, you should:

1. Create an [AWS account](https://aws.amazon.com/resources/create-account/):
 * Click on the "Sign Up Now" button - then select the "I am a new user" option.
 * Enter a valid email address - this should be either:
 
   > A shared GA mailbox (contact the Service Desk - note that this can take some time to create), **OR**
   >
   > ga.autobots+______@gmail.com (e.g. ga.autobots+bumblebee@gmail.com). 
   > Email from this account forwards to the Autobots.
   >
   > The Contact Email and some other details can be changed later on the My Account page/Account Settings using the root account.
  
  * Click the "Sign in using our secure server" button to creat a new account.
 
2. Login Credentials:
 * My Name is: 
  
   > The name for your account should be 'GA-AWS-xxxxxxxxxx'. For example, 'ga-aws-bumblebee' for the Bumblebee project.
   
  * My e-mail address: same as used in previous step
  * Enter a password (and remember it for later!)
  * Click "Create Account" button
  
3. Contact Information:
 * Select "Company Account" radio button
 * Full Name is account name you created in prevous step - eg 'GA-AWS-BUMBLEBEE'
 * Company Name and Details as below:
 
   > Company Name: Geoscience Australia *
   > Country: Australia 

   > Address: GPO Box 378 

   > City: Canberra

   > State: ACT

   > Post Code: 2601

   > Phone: +61 2 6249 9111
  
 * Complete the Capta Image test and tick the "AWS Customer Agreement" check box - and click "Create Account and Contine"
 


* Financial approval and cost/activity code from your delegate.
2. Don't enter your payment information! Leave this screen and contact the Autobots to get your new account added to GA's Consolidated Billing first.
3. If you used a GA mailbox, click the link from Consolidated Billing.
4. Rename your space from its account number to 'ga-aws-_____'.
5. Add MFA to your root account.

### Setting up Continuous Delivery

1. Make sure your code is in version control in Github or Bitbucket.
2. Get started with your pipeline:
  * If you're using Github, you'll be using [TravisCI](https://travis-ci.org/). Start by adding a .travis.yml to your repository.
  * If you're using Bitbucket, you'll be using [Bitbucket Pipelines](https://confluence.atlassian.com/bitbucket/get-started-with-bitbucket-pipelines-792298921.html). This link has all the information you need to get started.
