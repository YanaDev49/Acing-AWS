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


