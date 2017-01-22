---
title: Setting Up AWS Account
layout: page
permalink: setting_up_aws_sub.html
---

# First steps

1. Join [Slack](https://geoscience-australia.slack.com/signup), our messaging app. It's a great place to ask questions.
2. Join the #awscop and #autobots channels to chat with experts from across GA.
3. Talk with your Divisional Information Officer (DIO) and/or the Autobots about what you wish to achive. If you are just looking to have a play with AWS or try out a specific service, then the GA AWS Development environment may be suitable for your needs.

# Create an AWS space

If you have an application that will eventually become a production service, you should create a stand-alone account.  

## 1. Information you will need:

  * Documented approval from your section leader/financial delegate with GA Cost and Activity Codes. Approval needs be documented (e.g. in an email) as it is supporting the expenditure of Government funds - and will be needed to support adding the account to GA's Consolidated Billing account.

  * A valid GA Credit Card - for step 6. Initial spend should be quite small (less than $10 for the first month) however signing up with a credit card makes the process very much faster and easier.  

  * The name for your Account - this should be 'GA-AWS-XXXXXXXXXX'. For example, 'GA-AWS-BUMBLEBEE' for the Bumblebee project. A maximum of 23 characters are shown in many AWS reports, however more are allowed. The Account Name can also be used as an email address at step 2.  
  
  * When you create a new space you will receive root credentials - these will need to be supplied to the GA Cloud Enablement Team (the Autobots) to ensure that there is another way for GA staff to get into the account in the event of an emergency such as a security breach, or development staff leaving GA.

## 2. Create an [AWS account](https://aws.amazon.com/resources/create-account/):

 * Click on the "Sign Up Now" button
 * If you see the "I am a new user" option select it - otherwise click on the "Sign-in using root account credentials" link. 
 * Enter a valid email address (dont use a mobile number) - this should be either the autobots email address (with a unique tag) or a shared GA mailbox. You can use the same email address for multiple AWS accounts provided you provide a unique name for each account. Generally easier to use the autobots email account with a unique tag.  
 
   > **Speedy Option**
   >
   > ga.autobots+**uniqueTag**@gmail.com (e.g. ga.autobots+bumblebee@gmail.com).  
   > Email from this account will be forward to the Autobots (the uniqueTag part after the '+' symbol will be ignored by gamail - but can be used for filtering etc).  
   >
   > **OR - Slower Option**  
   > 
   > A shared GA mailbox (contact the Service Desk - note that this can take some time to create).  
   > The IT Service Desk will need the following information:    
   > Mailbox Name: this should be the Account Name from step 1 with the GA domain - eg. ga-aws-bumblebee@ga.gov.au  
   > Mailbox Members: should include the relevant Divisional Information Officer (DIO) for the project, The Business Team or Section Lead, the Technical Lead, and the Autobots
   >
   > The Contact Email and some other details can be changed later on the My Account page/Account Settings using the root account.  
  
 * Click the "Sign in using our secure server" button to create a new account.  
 
## 3. Login Credentials:

 * My Name is: this will be the **Account Name** from step 1 - e.g. "GA-AWS-BUMBLEBEE"
 * My e-mail address: same as used in previous step  
 * Enter a password - this will need to be stored in GA's password management solution (the Cloud Enablement Team has access to this) - see step 8.
 * Click "Create Account" button
  
## 4. Contact Information:

 * Select "Company Account" radio button
 * Full Name is the **Account Name** from step 1 (e.g. 'GA-AWS-BUMBLEBEE').
 * Company Name and Details as below:  
 
   > Company Name: Geoscience Australia  
   > Country: Australia  
   > Address: GPO Box 378  
   > City: Canberra  
   > State: ACT  
   > Post Code: 2601  
   > Phone: +61 2 6249 9111
   
 * Complete the Captcha Image test and tick the "AWS Customer Agreement" check box - and click "Create Account and Continue"  
 * Welcome to Amazon Web Services page - click 'Launch Management Console' button  

## 5. Sign In to new account:

 * My e-mail address: same as used previously  
 * Select 'I am a returning user' and enter the password  
 * Click 'Sign in using our secure server'  
 
## 6. Add Credit Card to secure charges (optional):

 * To cover any charges, AWS requests a credit card to secure the account initially. This is absolutly, but avoiding it can be tricky.
 * Any credit charges should be minimal (less than $10 in the first month) however this needs to be agreed to by the GA Credit Card holder and the relevant financial delegate.
 
 **Speedy Option**
 
 * Step 1 of 2 - Enter Credit Card Details  
 * Step 2 of 2 - select 'Use contact address' tick box and click 'Continue'  
 * Sign into the root account and select EC2 from the Services menu> Compute option. It will ask you to verify your identity. Follow the steps outlined in 7. below.

**OR - Slower Option**

 * Contact the Autobots to add the account to Consolidated Billing. They will need the account name and number.
 * Wait for confirmation that your account has been added...
 * Sign into the root account and select EC2 from the Services menu> Compute option. It will ask you to verify your identity. Follow the steps outlined in 7. below.

## 7. Verify your Itentity:

 * You will now be asked to Verify your Identity - this is done via an automated phone call
   > Follow the instructions...
   > Click the 'Continue to Support Plan' button, select the default (Free) 'Basic' or 'Developer' or 'Business' option and click 'Continue'  
   > Registration should now be complete - close this window. 
   > You should now be ready to use your AWS account

## 7. Ask to be added to GA's Consolidated Billing:

 * Forward the approval email to the Cloud Enablement Team (the Autobots - include email [TP]) with the following message:
 
   > *Hi Autobots!  
   > I have created a new AWS Space called: GA-AWS-BUMBLEBEE
   > The AWS Account Number is: 1234567891011
   > The email address used is: ga.autobots+ga-aws-bumblebee@gmail.com
   > The space will be used for: Developing a application to monitor bumblebee flightpaths...  
   > The section lead is:  Janet Beekeeper
   > Cost/Activity Codes: 1234/5678  
   > Regards, Account Owner...*

 * Once the request has been actioned you will receive an email to accept Consolidated Billing for the account.
   
## 8. Clean up steps 
[TP to confirm with Autobots]

 * Contact the Cloud Enablement Team to arrange to store root credentials and MFA Key for safekeeping
 
 [for example]

 * [Customise your sign-in link](http://docs.aws.amazon.com/IAM/latest/UserGuide/console_account-alias.html).  
 * Add Multi Factor Authentication (MFA) to your root account.
 * Send Root Account details and MFA Key to Cloud Enablement Team (for safekeeping).
 * Set up Admin Account users and discontinue use of root account.
 * Update your contact email addresses if necessary.
 * Do steps to set IAM Security Status to Green 
 
 * Run [space-provisioner](https://bitbucket.org/geoscienceaustralia/space-provisioner/) on your new account.
