# Essential Ports You Need To Know

### There are a few very important ports that you need to know!!

![image](https://github.com/user-attachments/assets/cae1d1d5-80d8-4c71-a562-c908b305b197)

| **Port Number** | **Protocol/Service**  | **Explanation**                                                                                                                                     |
|-----------------|-----------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| **Port 22**     | SSH (Secure Shell)     | Used for logging into your Linux EC2 instance remotely. This is how you securely connect to your server’s terminal from your own computer.           |
| **Port 22 (SFTP)** | SFTP (Secure File Transfer Protocol) | Same port, but for securely transferring files between your computer and the server. Think of it like a secure version of FTP.                      |
| **Port 21**     | FTP (File Transfer Protocol) | Used for transferring files, but not secure. You’d probably avoid using this unless you have to because it sends data in plain text.               |
| **Port 80**     | HTTP (Hypertext Transfer Protocol) | This is for basic web traffic—if you’re running a website that doesn’t use HTTPS, this is the port people connect to by default.                   |
| **Port 443**    | HTTPS (Hypertext Transfer Protocol Secure) | This is the secure version of HTTP. When people visit a website that has "https://" in front, it’s using this port to encrypt the traffic.        |
| **Port 53**     | DNS (Domain Name System) | This port is used for DNS queries. It translates domain names (like example.com) into IP addresses, so browsers know where to find websites.        |
| **Port 3389**   | RDP (Remote Desktop Protocol) | This one’s for logging into Windows servers remotely. If you’re using a Windows EC2 instance, you’d use this to connect and control the desktop.     |

![ThereYouHaveItSheaWhitneyGIF (2)](https://github.com/user-attachments/assets/279b8098-cddb-4705-b319-cf1e9d43d417)

