# AWS Identity And Access Management (AWS IAM) 
![image](https://github.com/user-attachments/assets/8cca882b-b630-4db8-93da-23b90ded2030) 

AWS Identity and Access Management (IAM) is a tool that helps you control who can access your AWS resources and what they 
can do with them. You can create users, groups, and roles, assign them specific permissions, and manage access securely. It ensures that
only the right people or services have access to your aws resources, whether its for developers, apps, or services.

### Its key for securing your enviroment!! 

![image](https://github.com/user-attachments/assets/d1b08254-0768-41e8-8aa9-63a3fa63c746)

## Users & Groups in AWS IAM

![image](https://github.com/user-attachments/assets/d5203f1a-c467-493b-ba56-d246263cf9b3)

- In AWS IAM, users are individual accounts created for people who need access to AWS, like yourself or individuals apart of a team. Each user has their 
own login and can be given specific permissions to access certain AWS services.

### Groups Are Collections of Users!

Instead of giving permissions to each user one by one, you can create a group like 'Developers' or 'Admins' and assign permissions to that group. Every user in the group
automatically gets those permissions. its a way to organise and manage access more easily.

![image](https://github.com/user-attachments/assets/0b45a217-874d-498d-99ce-2e7b057f44b4)

## Permissions

In AWS Identity Access Management (IAM). permissions control what actions users, groups, or roles can perform on AWS resources. These permissions are set through policies, which are written in JSON format. A JSON policy file determines what actions, like reading data from an S3 bucket or launching an EC2 instance, are allowed or denied, and on which specific resources.

- You can attach these JSON policies to users, groups, or roles, ensuring they have only the access that they need, following the principle of least privilege. This setup helps securely manage permissions and ensures users cant access services or data they dont need.

![image](https://github.com/user-attachments/assets/0fe6e301-e6a4-4317-92e5-47fa33059318)

## IAM Policies Inheritance 
![image](https://github.com/user-attachments/assets/e1be30fd-eef4-4c37-9c04-2d88001d204e)

In AWS Identity and Access Management (IAM),policy inheritance refers to how permissions are passed down to users through groups or roles. If a user is part of a group, the permissions assigned to that group will automatically apply to the user. This means you dont need to individually assign permissions to each user. Just assign policies to the group, and every member of that group will inherit those permissions.

- This makes managing access easier, especially for large teams. You can also attach multiple policies to user or group, and the permissions from all those policies combine to determine what actions are allowed or denied.

## IAM Policies Structure 
![image](https://github.com/user-attachments/assets/8ce6778d-f943-49ec-90cb-91ba4d328a13)

### Let me take you through a description of what a JSON permissions file looks like!!

### Version ### 
![image](https://github.com/user-attachments/assets/bbb650de-3e7a-436f-8493-c2cf7daa8eaf)

- At the top of your policy JSON file you will always see a version. This is the date of the current policy.

### ID ###
![image](https://github.com/user-attachments/assets/6f64290d-b0a4-4e65-8e1b-55823ebb67cd)

- This is an identifier of the policy. This is usually there to give the policy a name or some extra context

### Statement ### 
![image](https://github.com/user-attachments/assets/eaaae631-52d2-48f6-8ed6-6249788409d9)

## A policy can have one or more statements, and each one spells out exactly what the policy does:

![image](https://github.com/user-attachments/assets/5fb270c0-38e1-4c9e-84f0-d006c9faf4cb)

- The SID is like a label or tag with a statement to make it easier to identify.

![image](https://github.com/user-attachments/assets/62433ec9-6907-44de-9c50-7a678a185156)

- This is where you say whether the statement allows or denies access.

![image](https://github.com/user-attachments/assets/a4f3fe9e-4fb4-497d-a524-468ad3122347)

- The Principle tells AWS who the policy applies to. It could be the user the role or account that gets permissions.

![image](https://github.com/user-attachments/assets/8dc631d8-9a01-4e8c-a9f3-eaea1214a815)

- Actions are the specific things that the user or group is allowed or denied to do.

![image](https://github.com/user-attachments/assets/6b68a258-415c-43ec-9cfb-de7325c3656b)

- Resources define what the action applies to like an S3 bucket or an EC2 instance.

![image](https://github.com/user-attachments/assets/ff61e083-1ce1-4fac-bcc3-5ac6a6c4221a)

- Conditions are rules around when the policy is in effect. conditions are optional but especially usefull when you need extra control.

### In Summary, A policy defines what to which resource and when!! This structure gives you concise control of permissions!!

## IAM password Policy
![image](https://github.com/user-attachments/assets/10321829-30f4-4d82-904c-e9a8a1fbf4b5)

In AWS Identity and Access Management (IAM), a password policy sets rules for how strong a users password must be. It allows you to control things like the minimum password length, whether numbers, special characters, or uppercase letters are required, and how often passwords need to be changed. 

- Setting a strong password policy is crucial for security, ensuring users create hard to guess passwords. You can also enforce things like preventing password reuse and setting expiration periods, which helps protect your AWS enviroment from unauthorized access.

## MFA 

![image](https://github.com/user-attachments/assets/3b8e3a63-a93d-4b5c-b2a5-6f531a8846ac)

MFA, or Multi-Factor Authentication, In AWS Identify And Access Management (IAM), adds an extra layer of security on top of a username and password. Instead of just entering your password to sign in, you also need to provide a second piece of information, usually a temporary code from a device like your phone or hardware token.

### Heres How It Works!!

- After you enter your password, AWS prompts you for a one-time code generated by an app like Google Authenticator. Even if someone knows your password, they cant access your AWS account without this code. This makes it harder for unauthorized users to get in, adding essential protection to your AWS resources.


## MFA Devices Option In AWS!!

In AWS Identity and Access Management (IAM), the MFA Devices Options lets you set up specific devices for Multi-Factor Authentication (MFA). AWS supports a few types of devices to generate the second layer of authentication after entering your password. 

![image](https://github.com/user-attachments/assets/0373d3ba-f3d8-46d2-be2d-77ef7413bd2c)

## How can users access AWS? 
![image](https://github.com/user-attachments/assets/c2bd21fd-29b5-41ef-ae21-406e84b24893)

In AWS Identity and Access Management (IAM), users can access AWS in two main ways:

AWS Management Console – This is a web-based interface where users log in with a username, password, and optionally, a Multi-Factor Authentication (MFA) code. It provides a graphical way to interact with AWS services.

Programmatic Access – Users can interact with AWS via APIs, the AWS CLI (Command Line Interface), or SDKs (Software Development Kits). To do this, they need Access Keys, which consist of an access key ID and a secret access key.

## Access Keys

![image](https://github.com/user-attachments/assets/5839a679-9e29-48de-bd68-1ead39f70f89)

Access keys in AWS Identity And management (IAM) are a combination of an Access Key ID and a secret Access Key. These are used to make programmatic requests to AWS services, meaning theyre for things like API calls or using the AWS CLI. They're especially important for apllications that need to interact with AWS resources without logging into the AWS Management Console. 

Its important to keep access keys safe and secure, preventing from sharing with anyone to avoid hacking issues.

## IAM Roles For Services!!

![image](https://github.com/user-attachments/assets/60f9ab1a-4752-47c2-b758-5803f661301d)

AWS IAM Roles for services allow AWS services (like EC2, Lambda, or S3) to interact with other AWS resources on your behalf
, securely. Instead. of using access keys, these services use roles to assume temporary credentials with the permissions you define in the role.

For example, you can assign a role to an EC2 instance so it can access S3 buckets, nut the instance wont have permanent access keys. This reduces security risks and simplifies managing permisions.
Each role is created with specific policies that define what actions the service can perform.

