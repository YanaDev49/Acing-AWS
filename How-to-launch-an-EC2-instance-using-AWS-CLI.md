# Exploring the AWS CLI 🚀

𝗛𝗲𝗹𝗹𝗼 𝗘𝘃𝗲𝗿𝘆𝗼𝗻𝗲 𝗮𝗻𝗱 𝘄𝗲𝗹𝗰𝗼𝗺𝗲 𝘁𝗼 𝘁𝗵𝗶𝘀 𝗥𝗘𝗔𝗗𝗠𝗘, 𝘄𝗵𝗲𝗿𝗲 𝗶 𝘀𝗵𝗼𝘄 𝘆𝗼𝘂 𝗵𝗼𝘄 𝘁𝗼 𝗹𝗮𝘂𝗻𝗰𝗵 𝗮𝗻 𝗘𝗖𝟮 𝗶𝗻𝘀𝘁𝗮𝗻𝗰𝗲 𝗳𝗿𝗼𝗺 𝘁𝗵𝗲 𝗔𝗪𝗦 𝗰𝗼𝗺𝗺𝗮𝗻𝗱 𝗟𝗶𝗻𝗲 𝗶𝗻𝘁𝗲𝗿𝗳𝗮𝗰𝗲!!😄👋

𝘄𝗲 𝗵𝗮𝘃𝗲 𝗯𝗲𝗲𝗻 𝗲𝘅𝗽𝗹𝗼𝗿𝗶𝗻𝗴 𝗮𝗻𝗱 𝘂𝗻𝗱𝗲𝗿𝘀𝘁𝗮𝗻𝗱𝗶𝗻𝗴 𝘁𝗵𝗲 𝘀𝘁𝗿𝘂𝗰𝘁𝘂𝗿𝗲 𝗼𝗳 𝗔𝗺𝗮𝘇𝗼𝗻 𝗪𝗲𝗯 𝗦𝗲𝗿𝘃𝗶𝗰𝗲𝘀 𝗳𝗼𝗿 𝘀𝗼𝗺𝗲 𝘁𝗶𝗺𝗲 𝗻𝗼𝘄, 𝗮𝗻𝗱 𝗼𝗻𝗲 𝗼𝗳 𝘁𝗵𝗲 𝗺𝗼𝘀𝘁 𝗶𝗻𝘁𝗲𝗿𝗲𝘀𝘁𝗶𝗻𝗴 𝗳𝗲𝗮𝘁𝘂𝗿𝗲𝘀 𝗶 𝗳𝗼𝘂𝗻𝗱 𝘄𝗮𝘀 𝘁𝗵𝗲 𝗔𝗪𝗦 𝗖𝗟𝗜. 

𝗦𝗼 𝗶 𝗱𝗲𝗰𝗶𝗱𝗲𝗱 𝘁𝗼 𝗴𝗲𝘁 𝘀𝗼𝗺𝗲 𝗵𝗮𝗻𝗱𝘀 𝗼𝗻 𝗲𝘅𝗽𝗲𝗿𝗶𝗲𝗻𝗰𝗲 𝘂𝘀𝗶𝗻𝗴 𝗶𝘁 𝘄𝗵𝗶𝗰𝗵 𝗶𝗹𝗹 𝗯𝗲 𝘀𝗵𝗼𝘄𝗶𝗻𝗴 𝘆𝗼𝘂 𝘁𝗼𝗱𝗮𝘆! 🚀

![HappyGIF (2)](https://github.com/user-attachments/assets/83fe9b48-8a10-40cf-b80e-068f5f749571)

## Step 1: Select Amazon Machine Image ID
<img width="925" alt="image" src="https://github.com/user-attachments/assets/2de42c78-0250-4404-b923-f5e8049d34c8">

Just like how we choose an AMI (Amazon Machine Image) On the console, we need to do the same when using the AWS CLI. The Only difference here is that we will be using the AMI ID to create our command to launch our instance, which is the blueprint for creating virtual machines.

- In This Example, we will be using the AMI ID of Ubuntu

![image](https://github.com/user-attachments/assets/00d4b52a-ef9d-4f81-b410-ce95e3b75207)

## Step 2: Choosing an instance type 
<img width="602" alt="image" src="https://github.com/user-attachments/assets/74da0421-87fe-4ce4-b0ad-cdf010c5110f">

Next, we need to choose an instance type and the most common one I normally use is t2.micro

![image](https://github.com/user-attachments/assets/c69e7b9b-3c55-44af-bf76-9a8a6b0dfd05)

### Why use t2.micro instance type?

- The t2.micro instance type is part of AWS free tier, which means that you can use it for free for up to 750 hours a month for the first year. This makes it ideal for learning, testing, or building small projects (So there you go haha 😄🙌)

## Step 3: Creating a key-pair
![ivx3azkn](https://github.com/user-attachments/assets/9121b9c3-726c-4c97-94ec-50a15c2a813a)

Then we need to create a key-pair! we can name it 'demo-key-pair'

![orowypyc](https://github.com/user-attachments/assets/6772b76d-11dc-4d69-be6d-5d4a9996f536)

## Step 4: configuring permissions ( Time to Chmod!! hehe 😁)

𝗐𝗁𝖾𝗇 𝖽𝗈𝗂𝗇𝗀 𝗌𝗆𝖺𝗅𝗅 𝗉𝗋𝗈𝗃𝖾𝖼𝗍𝗌 𝗅𝗂𝗄𝖾 𝖽𝖾𝗉𝗅𝗈𝗒𝗂𝗇𝗀 𝖶𝗈𝗋𝖽𝖯𝗋𝖾𝗌𝗌 𝗈𝗇 𝖤𝖢𝟤 𝗂 𝗆𝖺𝖽𝖾 𝗌𝗈 𝗆𝖺𝗇𝗒 𝖾𝗋𝗋𝗈𝗋𝗌 𝗐𝗂𝗍𝗁 𝗆𝗒 .𝗉𝖾𝗆 𝖿𝗂𝗅𝖾 𝖻𝖾𝖼𝖺𝗎𝗌𝖾 𝖨 𝖿𝖺𝗂𝗅𝖾𝖽 𝗍𝗈 𝖢𝖮𝖭𝖥𝖨𝖦𝖴𝖱𝖤 𝖳𝖧𝖤 𝖯𝖤𝖱𝖬𝖨𝖲𝖲𝖨𝖮𝖭𝖲!!

𝖠𝗅𝗐𝖺𝗒𝗌 𝗆𝖺𝗄𝖾 𝗌𝗎𝗋𝖾 𝗍𝗁𝖺𝗍 𝗒𝗈𝗎𝗋 𝗉𝖾𝗋𝗆𝗂𝗌𝗌𝗂𝗈𝗇𝗌 𝖿𝗈𝗋 𝗒𝗈𝗎𝗋 .𝗉𝖾𝗆 𝖿𝗂𝗅𝖾 𝖺𝗋𝖾 𝖼𝗈𝗇𝖿𝗂𝗀𝗎𝗋𝖾𝖽 𝖾𝗌𝗉𝖾𝖼𝗂𝖺𝗅𝗅𝗒 𝗐𝗁𝖾𝗇 𝗒𝗈𝗎 𝗂𝗇𝗍𝖾𝗇𝖽 𝗍𝗈 𝖲𝖲𝖧!!

![image](https://github.com/user-attachments/assets/c8eb17b8-a970-44f5-b386-026b75282da8)

## Step 5: Creating a security Group 

A security group is essential for your EC2 instance because it controls the traffic that can flow in and out. It acts as a virtual firewall, allowing you to specify which ports are open for access (like SSH for Linux or HTTP for a website). 

- Without one, your instance would be exposed to unwanted traffic or completely inaccessible!

### Lets create a Security group called 'web-sg' ⤵️
![image](https://github.com/user-attachments/assets/c95695ca-214b-4998-9869-836316f3d276)

## Step 6: Adding Inbound Rules!!

Inbound rules refer to the rules defined in the security group associated with that instance. These rules control the instance. These rules control the incoming traffic to your instance. ⤵️

![image](https://github.com/user-attachments/assets/8d9c5496-047e-49d0-bc7b-33de9116a0d1)
![image](https://github.com/user-attachments/assets/a9aa1cd5-67b8-4840-82aa-0da21d688768)
![image](https://github.com/user-attachments/assets/538b076a-51d8-4ab0-9c8f-0ddaa58db868)

- Here we have added the HTTP rule, HTTPS rule and SSH rule!

## Step 7: Time to choose a subnet!!

We will be choosing a subnet According to the availibility zone 'eu-west-2a'
![image](https://github.com/user-attachments/assets/e6ff1b43-419a-4103-aa0b-625160f73566)

- We are storing this in a variable ⤴️

## Step 8: Launching our instance 🎉😄🚀
