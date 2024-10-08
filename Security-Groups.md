# What Are Security Groups? 🤔

Security Groups  control who can and can’t come in (or out) of your virtual machine. You set up rules that say which traffic (like from the internet or other servers) is allowed to talk to your instance and which is blocked.

![image](https://github.com/user-attachments/assets/8441dbd3-1160-4334-bc9d-9edb30e80b53)

## Inbound Rules

- These decide what kind of traffic can come into your EC2 instance. For example, if you want people to access a website hosted on your server, you’d allow incoming traffic on port 80 (HTTP) or 443 (HTTPS). If you don’t want anyone accessing certain things, you can block those ports.

## Outbound Rules 

- These control what traffic can go out from your instance. For example, if your EC2 instance needs to connect to another service (like a database), you set up an outbound rule to allow that.

## Default Behavior 

- By default, Security Groups block everything. Nothing can get in or out unless you specifically allow it with a rule. So, it’s like starting with a locked door, and then you open specific windows and doors for the right people.

## Stateful

- Security Groups remember things! If you allow incoming traffic, the return traffic is automatically allowed out. So, if someone connects to your server, their response is allowed back without needing another rule.


#### In summary, Security Groups are just a way to control the "traffic" in and out of your EC2 instance, making sure only the right people can access it and keeping unwanted visitors out.

### And there you have it everyone!!

![ThereYouHaveItSheaWhitneyGIF (2)](https://github.com/user-attachments/assets/5c4b0d6e-e50e-4478-9606-41f95169e418)
