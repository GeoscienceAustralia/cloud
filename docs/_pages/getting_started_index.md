---
title: Getting Started
layout: page
permalink: getting_started_index.html
---

### Getting started

1. Join [Slack](https://geoscience-australia.slack.com/signup), our messaging app. It's a great place to ask questions.
2. Join the #awscop and #autobots channels to chat with experts from across GA.

### Getting started on AWS

If you just want to experiment with AWS, you should get an account in the AWS Dev space. Send a Slack message or an email to the Autobots to get the ball rolling.

### Create an AWS space

If you have an application that will eventually become a production service, you should:

1. Create an [AWS account](https://aws.amazon.com/resources/create-account/):

  * The name for your account should be 'ga-aws-(up to 12 characters)'. For example, 'ga-aws-bumblebee' for the Bumblebee project.
  * The email can either be a shared GA mailbox (contact the Service Desk) or ga.autobots+______@gmail.com (e.g. ga.autobots+bumblebee@gmail.com). This email address forwards to the Autobots' GA mailbox.
  * Financial approval and cost/activity code from your delegate.
 
2. Don't enter your payment information! Leave this screen and contact the Autobots to get your new account added to GA's Consolidated Billing first.
3. If you used a GA mailbox, click the link from Consolidated Billing.
4. Rename your space from its account number to 'ga-aws-_____'.
5. Add MFA to your root account.

### Getting started with Continuous Delivery

1. Make sure your code is in version control in Github or Bitbucket.
2. Get started with your pipeline:
  * If you're using Github, you'll be using [TravisCI](https://travis-ci.org/). Start by adding a .travis.yml to your repository.
  *  If you're using Bitbucket, you'll be using [Bitbucket Pipelines](https://confluence.atlassian.com/bitbucket/get-started-with-bitbucket-pipelines-792298921.html). This link has all the information you need to get started.
