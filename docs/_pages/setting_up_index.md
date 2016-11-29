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

If you have an application that will eventually become a production service, you should create a stand-alone account.  

1. Information you will need:  
  * Approval from the relevant section leader/financial delegate  
  * A valid GA Credit Card for step 6.  
  * GA Cost and Activity Codes  
  * The name for your Account - this should be 'GA-AWS-xxxxxxxxxx'. For example, 'ga-aws-bumblebee' for the Bumblebee project. Maximum of 10 characters for a total of 17 characters overall. The Account Name can also be used as an email at step 2.  
  * This information will need to be sent to the Cloud Enablement team (the 'Autobots') for them to complete the Consolidated Bill process:  
  * tesmtina.s:  
 
   > testing 2  
   

2. Create an [AWS account](https://aws.amazon.com/resources/create-account/):  
 * Click on the "Sign Up Now" button - then select the "I am a new user" option.  
 * Enter a valid email address - this should be either:  
 
   > A shared GA mailbox (contact the Service Desk - note that this can take some time to create).  
   > The IT Service Desk will need the following information:    
   > Mailbox Name: this should be the Account Name from step 1 with the GA domain - eg. ga-aws-bumblebee@ga.gov.au  
   > Mailbox Members: should include the relevant Divisional Information Officer (DIO) for the project, The Business Team or Section Lead, the Tecnical Lead, and the Autobots (James Kingsmill and Scott McLauchlan)
   >  
   > **OR**  
   >
   > ga.autobots+______@gmail.com (e.g. ga.autobots+bumblebee@gmail.com).  
   > Email from this account forwards to the Autobots.  
   >
   > The Contact Email and some other details can be changed later on the My Account page/Account Settings using the root account.  
  
 * Click the "Sign in using our secure server" button to creat a new account.  
 
3. Login Credentials:
 * My Name is: this will be the **Account Name** from step 1.  
   
 * My e-mail address: same as used in previous step  
 * Enter a password (and remember it for later!)
 * Click "Create Account" button
  
4. Contact Information:
 * Select "Company Account" radio button
 * Full Name is the **Account Name** from step 1.
 * Company Name and Details as below:  
   > Company Name: Geoscience Australia  
   > Country: Australia  
   > Address: GPO Box 378  
   > City: Canberra  
   > State: ACT  
   > Post Code: 2601  
   > Phone: +61 2 6249 9111  
   
 * Complete the Captcha Image test and tick the "AWS Customer Agreement" check box - and click "Create Account and Contine"  
 * Welcome to Amazon Web Services page - click 'Launch Management Console' button  

5. Sign In to new account:
 * My e-mail address: same as used previously  
 * Select 'I am a returning user' and enter the password  
 * click 'Sign in using our secure server'  
 
6. Add Credit Card to secure charges:  
 > To cover any charges, AWS requires a credit card to secure the account initially. 
 > The next step will request the new account to be assigned to GA's Consolidated Billing account. 
 > Any credit charges should be minimal (less than $10 in the first month) however this needs to be agreed to by the GA Credit Card holder and the relevant financial delegate.
 
 * Step 1 of 2 - Enter Credit Card Details  
 * Step 2 of 2 - select 'use contact address' tick box and click 'Continue'  

7. Sign up for Consolidated Billing:  
 * Select 'My Billing Dashboard' from drop down menu under the Account Name - top right of window.  
 * Select the 'Consolidated Billing' menu option and click 'Sign up for Consolidated Billing'  
 * You may be asked to Verify your Identity - this is done via an automated phone call
   > A new browser tab will be opened  
   > Enter the Captcha text and a valid phone number  
   > A Code Number will be displayed and AWS will call the number provided.
   > Enter the code number via the key pad - the web page will automatically update  
   > Click the 'Continue to Support Plan' button, select the default 'Basic' option and click 'Continue'  
   > Registration should now be complete - close this window and click back to the Billing Management Tab
   
 * Refresh the page and click 'Sign up for Consolidated Billing'  
   > An email will be sent to the 'Autobots' Cloud Enablement team who will login to the GA Consolidated Billing account and add the new AWS Account.  
   > At this point the 'Autobots' will need information about the account detailed in step 1 and the Account Number...  
   > Once they have actioned the request you will receive an email to accept Consolidated Billing for the account.
   
8.  

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
