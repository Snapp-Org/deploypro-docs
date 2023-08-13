---
title            : AWS - Generate Credentials
sidebar_label    : Generate Credentials
---

# AWS - Generate Credentials

This page explains how to optain the `Access` and `Secret KEY` for an AWS account and later use them to deploy your application on GitHub repository using `DeployPRO` service.

## How to create an access key and secret key in AWS?

`Access keys` consist of an access key ID and a secret access key, which are used to sign programmatic requests that you make to AWS. For better security, AWS recommends using IAM access keys instead of AWS root account access keys. 

<br />

### Create Acces Key and Secret Key

1. Still, in the `IAM dashboard`, locate and click on "Users" in the left-hand navigation pane. This will display a list of IAM users in your account.
2. Identify the IAM user for whom you want to create an Access Key and click on their username in the user list. 
3. Within the IAM user details, navigate to the `Security credentials` tab. This tab is where you manage various security settings for the selected user.
4. Under the `Access keys` section, click on the `Create access key` button.
5. Complete the step!
    
    - > Step 1: Access key best practices & alternatives

        Select `Command Line Interface (CLI)`. Don't forget to tick the confirmation checkbox before clicking "Next".

    - > Step 2: Set description tag - optional
        
        This step is optional, you can directly click "Create Access Key".

    - > Step 3: Retrive access key
        
        This picture below is how it looks when the `Access Key` and `Secrete Key` is created completely.

![AWS Access Key and Secrete Key - DeployPRO Service](https://github.com/app-generator/dummy/assets/51070104/922a0213-1e68-4c13-82b2-a67c84075ebc)


6. Download the Access Key and Secret Key CSV file using the `Download .csv file ` button. Ensure you save this file securely, as the Secret Key will not be shown again.
  
  - ⚠️ **Security Alert**
  
  Treat Access Keys and Secret Keys as sensitive information. Avoid sharing them publicly or hardcoding them into your applications. Instead, use AWS-recommended practices like environment variables or AWS-specific configuration files to securely manage these credentials.

<br />

## Resources

- 👉 [Deploy Projects](https://deploypro.dev/) using your preferred provider: `AWS`, `GCP`, `Azzure`
- 👉 Get [Deployment Support](https://deploypro.dev/support/) from the team behind this service
- 👉 Join the [Community](https://discord.gg/qQhjQZhnur) and chat with the team behind `DeployPRO`
