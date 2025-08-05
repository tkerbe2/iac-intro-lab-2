![tkdev_space_200](https://github.com/user-attachments/assets/31af05be-97b5-4d4e-82ef-4f23203eb7ac)

<br>


# 🧪 Lab 2 - AWS New Account Setup

In this lab you will setup your brand new AWS account with an IAM User, MFA, and create an access portal. If you have not yet created an AWS account please do so before starting this lab.

- [AWS Free Tier](https://aws.amazon.com/free/)

### Resources Created:
This demo creates the following resources:

- An IAM Account
- MFA 
- Custom access portal URL
- Access key and secret key

<br>

# 💡 Terms and Concepts

Before we get started I want to discuss some key terms and concepts about AWS and accounts. This is not meant to be an AWS course or AWS specific guide but I realize many who take this will be new to AWS so I want to cover it. If this information is not new to you, feel free to skip this and the suggested reading.

### AWS Accounts

In AWS your account is like a container that all your resources you build such as VMs, buckets, etc, get attached to. Inside your account you can have users and roles with defined permissions, etc. All of this still lives within your account and your account will have a unique account ID that is tied to the email you used when you created it. Initially you will log into the AWS console with your root account (the account you created when you signed up) this will be your email. Root has unrestricted access to the entire AWS account and you rarely want to use this for day-to-day acitivity and creating infrastructure. This lab will walk through how to more tightely secure your root account with MFA and then create other accounts that you can use for this lab.

<br>


# 📖 Suggested Reading 
- [What is an AWS account?](https://docs.aws.amazon.com/accounts/latest/reference/accounts-welcome.html)
- [Terminology and concepts for AWS Organizations](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_getting-started_concepts.html)

<br>

# Lab Steps

### 1. Log into AWS

- Log into AWS with your root account [AWS](https://aws.amazon.com/)

![image](https://github.com/user-attachments/assets/464af956-2c61-487d-bbef-acce4a9378f0)

<br>

***

### 2. Open Identity and Access Management (IAM)

![image](https://github.com/user-attachments/assets/27f8a292-70a5-4475-9628-fd0c0ddda89c)

- You can favorite it so it's easier to find later

<br>

***

### 3. Create and assign access to the user

- On the left pane you will find users and click on create user

![image](https://github.com/user-attachments/assets/42972e56-3d4e-4202-b972-f2f3cbb6c65d)

- We're going to create a specific account for our Terraform code to use when it deploys

![image](https://github.com/user-attachments/assets/2b4e63bd-523b-45e9-aeb0-68e2e8ce05a5)

- We need to give this account access to perform actions in certain services like creating a VM in EC2

![image](https://github.com/user-attachments/assets/fa52a954-38fd-47f6-8cc8-c92c82a55e6b)

- Find the two built-in roles you see in the screenshot (AmazonEC2FullAccess, AmazonVPCFullAccess)

![image](https://github.com/user-attachments/assets/3f86448c-3355-40a9-b973-457928d5efee)

<br>

***

### 4. Create access keys

- Open the newly created iac-user account

![image](https://github.com/user-attachments/assets/a958e31f-c1dc-4ada-b2e1-d7f50e2a3ed8)

- You can create an access key on the top right pane

![image](https://github.com/user-attachments/assets/192a7969-fcdf-47a2-ad1e-7fcd03bb8e23)

- Select the other option for use case

![image](https://github.com/user-attachments/assets/cc8abd0f-101e-4b28-bf84-26220b0cc1bc)

- Give it a name to remember it by

![image](https://github.com/user-attachments/assets/424dead8-aa49-44e3-b134-d9d0d56b9eed)

- I recommend downloading the CSV
- Once an access key is created you can never read the secret again if you lose it

![image](https://github.com/user-attachments/assets/ad6795b8-9b01-4cb9-be07-b98b87707e87)

<br>





# ✨ Congratulations!

***

You've finished this lab and have completed the following items:
- ✅ Created a new AWS account.
- ✅ Logged into your AWS root account.
- ✅ Created an AWS IAM user that will be used for Terraform.
- ✅ Created an access key and secret key with the new user.

***

