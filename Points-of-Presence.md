# Points of Presence (Edge Locations) In AWS!

![image](https://github.com/user-attachments/assets/d3284f64-cded-45a6-9688-60e75b552a54)

### Points of presence, also knows as Edge Locations in AWS, are data centres located around the world that help deliver content to users more quickly. They are not the same as AWS Regions or availibility zones but are part of the AWS'S global infrastructure to ensure fast content delivery.

![image](https://github.com/user-attachments/assets/66ce888b-7026-47a2-9013-231af204d8a8)

- When a user requests data for example a webpage, video or image, instead of going all the way to the original server
 (Which could be far away), AWS uses the nearest Edge Location to serve that content. This speeds things up because the data has less
 distance to travel.

![image](https://github.com/user-attachments/assets/0d7a8f10-e718-4582-a39f-2e5752111eec)

- Amazon Cloudfront, AWS's content delivery network uses these Edge location to cache or temporarily store content. So, if a user in London is trying to access your
  website hosted in the U.S, CloudFront will deliver the content from the nearest London edge Location if its already cached there.

- Since the data is closer to users, the response time is much quicker, reducing latency. This is important for services like streaming video, loading websites, or gaming, where users expect fast load times.

  ![image](https://github.com/user-attachments/assets/ce8f62c8-709c-43a6-8572-717443fc59c7)

- AWS has hundreds of Edge Locations worldwide, Meaning users can get content faster no matter where they are. The more Edge Locations, the better global perfomance.
- Aws Edge Locations also support security features, like DDoS protection and encryption, ensuring that content is not only delivered quickly but also securely


### And that is all you need to know about Edge Location in AWS!!

![ThereYouHaveItSheaWhitneyGIF](https://github.com/user-attachments/assets/bf92078e-2509-4bb7-aacd-7cd7933606da)

