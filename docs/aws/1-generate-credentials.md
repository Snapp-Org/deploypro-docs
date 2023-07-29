---
sidebar_order    : 1
title            : AWS - Generate Credentials
sidebar_label    : Generate Credentials
---

# AWS - Generate Credentials

This page explains how to optain the `Access` and `Secret KEY` for an AWS account and later use them to deploy you GitHub project using `DeployPRO` service.

## Overview

- Register on the AWS platform
- Add User in the AWS Identity and Access Management (IAM) Dashboard
- Create an `Access key` and `Secret Key` on AWS

<br />

## How to register on AWS?

1. Access the AWS Website: Navigate to the official [AWS homepage.](https://aws.amazon.com/)
2. Click the "Create an AWS Account" button located in the top-right corner of the AWS homepage to commence the account registration process.
3. Provide your valid email address in the designated field, serving as the unique username for your AWS account.
4. For enhanced security, AWS may necessitate a verification code delivered to your designated email address, validating your account ownership. 
5. Choose a robust and secure password, consisting of alphanumeric characters and special symbols, to safeguard your AWS account.
6. Complete essential personal and contact details, including your full name, postal address, and phone number, as part of the AWS account registration procedure.
7. Optionally, submit valid payment particulars, such as credit card details, to enable access to specific AWS services. 
  - AWS will exclusively charge you for the actual resources and services you utilize, allowing you to configure billing alerts and limits to manage expenditures effectively.
8. Carefully review the terms and conditions, along with the data processing agreement, and consent to the stated terms by selecting "Create Account and Continue."
9. Upon completing the registration process, AWS will conduct a brief review of your submitted information. 
  - Once account verification is completed, you will receive an email confirmation, confirming the activation of your AWS account.

<br />

## How to create an access key and secret key in AWS?

`Access keys` consist of an access key ID and a secret access key, which are used to sign programmatic requests that you make to AWS. For better security, AWS recommends using IAM access keys instead of AWS root account access keys. 

IAM allows you to securely control access to AWS services and resources in your AWS account. For more information about AWS Account and Access Keys, visit https://docs.aws.amazon.com/

<br />

### Add User

1. Access the AWS Management Console by visiting the official [AWS website](https://aws.amazon.com/) and clicking on "Sign in to the Console" in the top-right corner. Enter your AWS account credentials to log in.
2. In the AWS Management Console, search for "IAM" (Identity and Access Management) in the services search bar, and select `IAM` from the results. This will take you to the IAM dashboard. 
3. In the IAM dashboard, locate and click on `Users` in the left-hand navigation pane. This will display a list of IAM users in your account.
4. To add a user, Click the `Add users` button.
5. Name your user application and click “Next”. The checkbox confirmation is optional.
6. Make the permission options become `Attach policies directly`. This will show you the list of permission policies. 
7. Search for `AmazonEC2FullAccess` and then tick the checkbox to continue the process.
8. Make the third step configuration default. So, directly click the “Create user” button.

<br />

### Create Acces Key and Secret Key

1. Still, in the `IAM dashboard`, locate and click on "Users" in the left-hand navigation pane. This will display a list of IAM users in your account.
2. Identify the IAM user for whom you want to create an Access Key and click on their username in the user list. 
3. Within the IAM user details, navigate to the `Security credentials` tab. This tab is where you manage various security settings for the selected user.
4. Under the `Access keys` section, click on the `Create access key` button.
5. Complete the step!
    - Step 1: Access key best practices & alternatives
        Select `Command Line Interface (CLI)`. Don't forget to tick the confirmation checkbox before clicking "Next".
    - Step 2: Set description tag - optional
        This step is optional, you can directly click "Create Access Key".
    - Step 3: Retrive access key
        This picture below is how it looks when the `Access Key` and `Secrete Key` is created completely.

![AWS Access Key and Secrete Key - DeployPRO Service](https://github.com/app-generator/dummy/assets/51070104/922a0213-1e68-4c13-82b2-a67c84075ebc)


6. Download the Access Key and Secret Key CSV file using the `Download .csv file ` button. Ensure you save this file securely, as the Secret Key will not be shown again.

Treat Access Keys and Secret Keys as sensitive information. Avoid sharing them publicly or hardcoding them into your applications. Instead, use AWS-recommended practices like environment variables or AWS-specific configuration files to securely manage these credentials.

<br />

## Resources

- 👉 [Deploy Projects](https://deploypro.dev/) using your preferred provider: `AWS`, `GCP`, `Azzure`
- 👉 Get [Deployment Support](https://deploypro.dev/support/) from the team behind this service
- 👉 Join the [Community](https://discord.gg/qQhjQZhnur) and chat with the team behind `DeployPRO`
