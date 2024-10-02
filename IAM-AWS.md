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
![image](https://github.com/user-attachments/assets/cc76af7a-1cd9-484f-9b33-66fc43977133)

- This is an identifier of the policy. This is usually there to give the policy a name or some extra context

### Statement ### 
![image](https://github.com/user-attachments/assets/eaaae631-52d2-48f6-8ed6-6249788409d9)

#### A policy can have one or more statements, and each one spells out exactly what the policy does:

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
