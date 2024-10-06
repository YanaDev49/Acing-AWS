# Exploring the AWS CLI 🚀

𝗛𝗲𝗹𝗹𝗼 𝗘𝘃𝗲𝗿𝘆𝗼𝗻𝗲 𝗮𝗻𝗱 𝘄𝗲𝗹𝗰𝗼𝗺𝗲 𝘁𝗼 𝘁𝗵𝗶𝘀 𝗥𝗘𝗔𝗗𝗠𝗘, 𝘄𝗵𝗲𝗿𝗲 𝗶 𝘀𝗵𝗼𝘄 𝘆𝗼𝘂 𝗵𝗼𝘄 𝘁𝗼 𝗹𝗮𝘂𝗻𝗰𝗵 𝗮𝗻 𝗘𝗖𝟮 𝗶𝗻𝘀𝘁𝗮𝗻𝗰𝗲 𝗳𝗿𝗼𝗺 𝘁𝗵𝗲 𝗔𝗪𝗦 𝗰𝗼𝗺𝗺𝗮𝗻𝗱 𝗟𝗶𝗻𝗲 𝗶𝗻𝘁𝗲𝗿𝗳𝗮𝗰𝗲!!😄👋

𝘄𝗲 𝗵𝗮𝘃𝗲 𝗯𝗲𝗲𝗻 𝗲𝘅𝗽𝗹𝗼𝗿𝗶𝗻𝗴 𝗮𝗻𝗱 𝘂𝗻𝗱𝗲𝗿𝘀𝘁𝗮𝗻𝗱𝗶𝗻𝗴 𝘁𝗵𝗲 𝘀𝘁𝗿𝘂𝗰𝘁𝘂𝗿𝗲 𝗼𝗳 𝗔𝗺𝗮𝘇𝗼𝗻 𝗪𝗲𝗯 𝗦𝗲𝗿𝘃𝗶𝗰𝗲𝘀 𝗳𝗼𝗿 𝘀𝗼𝗺𝗲 𝘁𝗶𝗺𝗲 𝗻𝗼𝘄, 𝗮𝗻𝗱 𝗼𝗻𝗲 𝗼𝗳 𝘁𝗵𝗲 𝗺𝗼𝘀𝘁 𝗶𝗻𝘁𝗲𝗿𝗲𝘀𝘁𝗶𝗻𝗴 𝗳𝗲𝗮𝘁𝘂𝗿𝗲𝘀 𝗶 𝗳𝗼𝘂𝗻𝗱 𝘄𝗮𝘀 𝘁𝗵𝗲 𝗔𝗪𝗦 𝗖𝗟𝗜. 

𝗦𝗼 𝗶 𝗱𝗲𝗰𝗶𝗱𝗲𝗱 𝘁𝗼 𝗴𝗲𝘁 𝘀𝗼𝗺𝗲 𝗵𝗮𝗻𝗱𝘀 𝗼𝗻 𝗲𝘅𝗽𝗲𝗿𝗶𝗲𝗻𝗰𝗲 𝘂𝘀𝗶𝗻𝗴 𝗶𝘁 𝘄𝗵𝗶𝗰𝗵 𝗶𝗹𝗹 𝗯𝗲 𝘀𝗵𝗼𝘄𝗶𝗻𝗴 𝘆𝗼𝘂 𝘁𝗼𝗱𝗮𝘆! 🚀

![HappyGIF (2)](https://github.com/user-attachments/assets/83fe9b48-8a10-40cf-b80e-068f5f749571)

## Step 1: Select Amazon Machine Image ID
<img width="925" alt="image" src="https://github.com/user-attachments/assets/2de42c78-0250-4404-b923-f5e8049d34c8">

Just like how we choose an AMI (Amazon Machine Image) On the console, we need to do the same when using the AWS CLI. The Only difference here is that we will be using the AMI ID to create our command to launch our instance, which is the blueprint for creating virtual machines.

- In This Example, we will be using the AMI ID of Ubuntu

  ![image](https://github.com/user-attachments/assets/dfc3b1d9-7b5a-4cf9-a76e-098923bc9624)

## Step 2: Choosing an instance type 
<img width="602" alt="image" src="https://github.com/user-attachments/assets/74da0421-87fe-4ce4-b0ad-cdf010c5110f">

Next, we need to choose an instance type and the most common one I normally use is t2.micro

![image](https://github.com/user-attachments/assets/cd98afc4-6991-4660-ae50-ca6a398cca0d)

### Why use t2.micro instance type?

- The t2.micro instnce type is part of AWS free tier, which means that you can use it for free for up to 750 hours a month for the first year. This makes it ideal for learning, testing, or small projects (So there you go haha 😄🙌)

## Step 3: Creating a key-pair
![Screenshot 2024-10-01 001852](https://github.com/user-attachments/assets/f90e94ab-86d6-40a9-9c4e-d65e33d6d4ca)

