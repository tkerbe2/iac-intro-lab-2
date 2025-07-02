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

# Some Theory

Before we get started I want to discuss some terms and theory about AWS and accounts. This is not meant to be an AWS course or AWS specific guide but I realize many who take this will be new to AWS so I want to cover it. 

### AWS Accounts

In AWS your account is like a container that all your resources you build such as VMs, buckets, etc, get attached to. Inside your account you can have users and roles with defined permissions, etc. All of this still lives within your account and your account will have a unique account ID that is tied to the email you used when you created it. Initially you will log into the AWS console with your root account (the account you created when you signed up) this will be your email. Root has unrestricted access to the entire AWS account and you rarely want to use this for day-to-day acitivity and creating infrastructure. This lab will walk through how to more tightely secure your root account with MFA and then create other accounts that you can use for this lab.

I recommend the following reading before continuing:
- [What is an AWS account?](https://docs.aws.amazon.com/accounts/latest/reference/accounts-welcome.html)
- [Terminology and concepts for AWS Organizations](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_getting-started_concepts.html)

<br>

# Lab Steps

### 1. Log into Azure and open Cloud Shell

![cloudshell](https://github.com/user-attachments/assets/a24f345c-e380-4f54-8a4b-f6b8463c023e)

- In the top right corner of the UI there is a terminal looking icon.

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

