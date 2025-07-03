![tkdev_space_200](https://github.com/user-attachments/assets/31af05be-97b5-4d4e-82ef-4f23203eb7ac)

<br>


# 🧪 AWS New Account Setup - Guided Lab

In this lab you will setup your brand new AWS account with an IAM User, MFA, and create an access portal. If you have not yet created an AWS account please do so before starting this lab.

- [AWS Free Tier](https://aws.amazon.com/free/)

### Resources Created:
This demo creates the following resources:

- An IAM Account
- MFA 
- Custom access portal URL
- Access key and secret key

<br>

# Some Theory

Before we get started I want to discuss some terms and theory about AWS and accounts. This is not meant to be an AWS course or AWS specific guide but I realize many who take this will be new to AWS so I want to cover it. If this information is not new to you, feel free to skip this and the suggested reading.

### AWS Accounts

In AWS your account is like a container that all your resources you build such as VMs, buckets, etc, get attached to. Inside your account you can have users and roles with defined permissions, etc. All of this still lives within your account and your account will have a unique account ID that is tied to the email you used when you created it. Initially you will log into the AWS console with your root account (the account you created when you signed up) this will be your email. Root has unrestricted access to the entire AWS account and you rarely want to use this for day-to-day acitivity and creating infrastructure. This lab will walk through how to more tightely secure your root account with MFA and then create other accounts that you can use for this lab.

<br>



> 📖 Suggested Reading:
- [What is an AWS account?](https://docs.aws.amazon.com/accounts/latest/reference/accounts-welcome.html)
- [Terminology and concepts for AWS Organizations](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_getting-started_concepts.html)

<br>

# Lab Steps

### 1. Log into AWS

- Log into AWS with your root account [AWS](https://aws.amazon.com/)

![image](https://github.com/user-attachments/assets/464af956-2c61-487d-bbef-acce4a9378f0)

<br>

***

### 2. Once you're in AWS open up Identity and Access Management (IAM)

![image](https://github.com/user-attachments/assets/27f8a292-70a5-4475-9628-fd0c0ddda89c)

- You can favorite it so it's easier to find later

<br>

***

### 3. Once you're in AWS open up Identity and Access Management (IAM)

![image](https://github.com/user-attachments/assets/27f8a292-70a5-4475-9628-fd0c0ddda89c)

- On the left pane you will find users and click on create user

![image](https://github.com/user-attachments/assets/42972e56-3d4e-4202-b972-f2f3cbb6c65d)

<br>

***

### 4. Once you're in AWS open up Identity and Access Management (IAM)


- We're going to create a specific account for our Terraform code to use when it deploys

![image](https://github.com/user-attachments/assets/2b4e63bd-523b-45e9-aeb0-68e2e8ce05a5)

- We need to give this account access to perform actions in certain services like creating a VM in EC2

![image](https://github.com/user-attachments/assets/fa52a954-38fd-47f6-8cc8-c92c82a55e6b)


<br>

***








# ✨ Congratulations!

***

You've finished this lab and have completed the following items:
- ✅ Launched a bash Cloud Shell environment.
- ✅ Saved your Subscription ID to a variable and exported it for Terraform.
- ✅ Cloned the GitHub repo.
- ✅ Modified some Terraform variables in the terraform.tfvars file.
- ✅ Initialized your directory.
- ✅ Ran a Terraform plan and applied the changes.
- ✅ Verified your resources in the Azure UI.
- ✅ Ran a Terraform destroy and unset your variables

***

