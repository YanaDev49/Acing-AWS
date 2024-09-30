# Global Services and Region-Scoped Services in AWS!!

![image](https://github.com/user-attachments/assets/6734f3a6-740c-4eb3-a11e-5c716b4cb1fb)

### In AWS, services are categorized into two main types: Global Services And Region-Scoped Services. 

- These services operate across all AWS Regions by default, meaning they arent tied to a specific region. Theyre designed to be accessible worlwide and maintain consistency no matter where you are.

## Global Services

![image](https://github.com/user-attachments/assets/5d78f61a-61f6-4e7c-9198-b134370c4284)

### These services operate across all AWS Regions by default, meaning they arent tied to a specific region. Theyre designed to be accessible worldwide and maintain consistency no matter where you are.

## 1. IAM (Identity And Access Management):

![image](https://github.com/user-attachments/assets/aea85d10-1a52-41f5-a7ca-f4c01ad2583e)

This service allows you to manage users, groups, and permissions globally. So, When you create an IAM user, They have access to resources across all AWS regions.

## 2. Route 53:

![image](https://github.com/user-attachments/assets/8914d354-08c2-4a75-b9c5-a7aa591cfefc)

This is AWS's DNS service, and since the internet is global, Route 53 helps direct traffic to resources anywhere in the world. 

## 3. CloudFront: 

![image](https://github.com/user-attachments/assets/6aa38b0b-4fe3-4109-bb86-661dd66f2c25)

A content delivery network (CDN) service that used Edge Locations around the globe to deliver content quickly to users, no matter their location. 


## Region-Scooped Services:

### These services are tied to specific regions, meaning that resources you create in one region are isolated from other regions. If you want the same resources in another region, you have to set them up separately.

## 1. EC2 (Elastic Cloud Compute) 

![image](https://github.com/user-attachments/assets/f4cf9624-6c59-49d0-8666-23391eb97021)

When you launch an EC2 instance (virtual machine), it exists only in the region you selected. If you need an instance in another region, you have to launch it there seperately.

## 2. S3 (Simple Storage Service): 

![image](https://github.com/user-attachments/assets/e490876a-9ffb-4d29-bf01-aa664445353b)

Buckets in S3 are region-specific. You choose the region where the data is stored to improve performance or meet compliance requirements.

## 3. RDS (Relational Database Service): 

![image](https://github.com/user-attachments/assets/822c680d-9638-4fa0-95b8-e7e099d51dda)

RDS (Relational Database Service): When you create a database, it is hosted in a specific region. If you need the same database in another region, you would have to create a new one there.

### And these are the Global and Region-Scoped services of AWS!!

![ThereYouHaveItSheaWhitneyGIF (2)](https://github.com/user-attachments/assets/3f13b8d9-9dbc-4ee1-a921-8f9bc3f48ba4)
