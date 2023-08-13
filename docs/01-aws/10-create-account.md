---
title            : AWS - Create Account
sidebar_label    : Create Account
---

# AWS - Create Account

If you have an AWS account, you can proceed to create a new user or add permissions to an existing user. This guide is designed for beginners, providing step-by-step instructions. It's important to note that you need an AWS account to link it with your **DeployPRO** account. 

1. Access the AWS Website: Navigate to the official [AWS homepage.](https://aws.amazon.com/)
2. Click the `Create an AWS Account` button located in the top-right corner of the AWS homepage to commence the account registration process.
3. Provide your valid email address in the designated field, serving as the unique username for your AWS account.
4. For enhanced security, AWS may necessitate a verification code delivered to your designated email address, validating your account ownership. 
5. Choose a robust and secure password, consisting of alphanumeric characters and special symbols, to safeguard your AWS account.
6. Complete essential personal and contact details, including your full name, postal address, and phone number, as part of the AWS account registration procedure.
7. Optionally, submit valid payment particulars, such as credit card details, to enable access to specific AWS services. 
    - AWS will exclusively charge you for the actual resources and services you utilize, allowing you to configure billing alerts and limits to manage expenditures effectively.
8. Carefully review the terms and conditions, along with the data processing agreement, and consent to the stated terms by selecting `Create Account and Continue`.
9. Upon completing the registration process, AWS will conduct a brief review of your submitted information. 
    - Once account verification is completed, you will receive an email confirmation, confirming the activation of your AWS account.

## ROOT User 

The AWS Root User represents the foundational administrative account within your AWS account, offering unparalleled control over all resources and services. Instead, employing IAM users with tailored permissions enhances security and aligns with the principle of least privilege. In summary, the root user possesses wide-ranging, unrestricted access to your entire AWS account, making it a **high-security risk if not used carefully**. 

1. Open your web browser and go to the [AWS Management Console](https://aws.amazon.com/console/). Click the `Sign In to the Console` button and enter your AWS account credentials.
2. After signing in, look for your account name in the top-right corner of the console. Click on it. From the drop-down menu, choose `Security Credentials`.
3. In the `Security Credentials` page, scroll down to the `Access keys` section.
4. To generate a new access key for the root user, click the `Create Access Key` button.
5. Tick the box to confirm you understand the above recommendation to proceed.
6. Once the access key is created, a pop-up window will appear displaying the access key ID and secret access key.

These are sensitive credentials⚠️, so make sure to copy and save them in a secure location or you can download it as a CSV file by clicking the "Download .csv file" button.

## IAM User 

IAM allows you to securely control access to **specific AWS services and resources** in your AWS account. For more information about AWS Account and Access Keys, visit https://docs.aws.amazon.com/

1. Access the AWS Management Console by visiting the official [AWS website](https://aws.amazon.com/) and clicking on `Sign in to the Console` in the top-right corner. Enter your AWS account credentials to log in.
2. In the AWS Management Console, search for `IAM` (Identity and Access Management) in the services search bar, and select `IAM` from the results. This will take you to the IAM dashboard. 
3. In the IAM dashboard, locate and click on `Users` in the left-hand navigation pane. This will display a list of IAM users in your account.
4. To add a user, Click the `Add users` button.
5. Name your user application and click `Next`. The checkbox confirmation is optional.
6. Make the permission options become `Attach policies directly`. This will show you the list of permission policies. 
7. Search for **`AmazonEC2FullAccess`** and then tick the checkbox to continue the process.
8. Make the third step configuration default. So, directly click the `Create user` button.

### IAM User - Permissions 

If you'd like to utilize an existing IAM user, you can adjust their permissions to enable connection with DeployPRO using the Access Key and Secret Key. Here's how:

1. Head to the IAM dashboard and select `Users` from the left sidebar. Click on the username of the user you want to modify.
2. Go to the `Permissions` tab on the user's details page.
3. Click the `Add permissions` button under the `Permissions` tab to start adding permission policies.
4. Choose the `Attach policies directly` option from the available choices.
5. Use the search bar to find and select **`AmazonEC2FullAccess`**. Confirm your choice by checking the checkbox.
6. Review the attached policies and click `Add permissions`.

<br />

## Resources

- 👉 [Deploy Projects](https://deploypro.dev/) using your preferred provider: `AWS`, `GCP`, `Azzure`
- 👉 Get [Deployment Support](https://deploypro.dev/support/) from the team behind this service
- 👉 Join the [Community](https://discord.gg/qQhjQZhnur) and chat with the team behind `DeployPRO`
