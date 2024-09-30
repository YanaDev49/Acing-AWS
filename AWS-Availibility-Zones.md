# What Are AWS Availibility Zones? 

![image](https://github.com/user-attachments/assets/8c2754ce-923a-4205-ace4-a4c63b278bd4)

### One of the key features that makes AWS extremely reliable and highly available are Availability zones.

![image](https://github.com/user-attachments/assets/429e2e09-6151-4c0d-842d-8124711fdbcc)

- Availibility Zones are essential isolated data centres within an AWS region that help ensure high availibility and fault tolerance for your apllications.

![image](https://github.com/user-attachments/assets/c183ab83-55b4-474e-945e-4b4420861606)

- Each AWS region consists of multiple Availibility Zones, and each AZ is a seperate physical location with its own independent infrastructure, such as power, cooling, and networking. This ensures that even if one AZ has an issue the others can still function.

![image](https://github.com/user-attachments/assets/2cd99a3f-9d40-4550-ab42-24ed440d2f42)

- Since AZ's are isolated from one another, they provide fault tolerance. If one AZ goes down due to an outrage or natrual disaster, the others in the same region remain unaffected, so your applications can keep running smoothly.

![image](https://github.com/user-attachments/assets/4ae79dde-5efe-4817-a353-bbb670472797)
 
- AWS typically has at least two or more AZ's in each region for example 'us-east-1a', 'us-east-1b', 'us-east-1c'. This allows you to distribute your resorces across multiplr AZ's within the same region to achieve high availibility.

![image](https://github.com/user-attachments/assets/e4bf6b6e-8b5a-4386-8119-c9a9fd1b5489)

- Despite being physically seperate, AZ's within the same region are connected by low-latency, high-speed networking. This allows your apllications to replicate data or communicate between AZ's quickly without much delay.

  
  
- To ensure your apllications are resilient, it is recommend to deploy your workloads across multiple AZ's. This way, even if one AZ fails, your apllication can continue running on another AZ.
