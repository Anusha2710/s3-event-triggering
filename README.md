# AWS S3 Event Triggering

You can also watch the entire implementation using the below YouTube video

https://youtu.be/qLZ-s7wvK7w

**NOTE**: REPLACE YOUR AWS ACCOUNT ID IN THE LAMBDA FUNCTION CODE.

AWS S3 Event triggering is a very popular project used by top companies in the Industry.

Here are some examples of top companies that use S3 event triggering:

**Netflix**: Netflix use S3 event triggering to automatically process video files uploaded to Amazon S3, enabling seamless content ingestion and processing.

**Airbnb**: This lodging and homestays aggregator use S3 event triggering to automatically process and analyze data stored in Amazon S3, such as guest reviews and booking information.

**Expedia**: They use S3 event triggering to automatically process and analyze data stored in Amazon S3, such as travel bookings, user profiles, and pricing information, to power their personalized travel recommendations and search features.


![Screenshot 2023-04-14 at 7 06 46 PM](https://user-images.githubusercontent.com/43399466/232058778-a7299e9b-9892-471c-a05d-14d773b5b333.png)

- Whenever a new video is uploaded in netflix it uses s3 for storing of data, next s3 bucket triggers lambda function because it is serverless, also it will create new IAM role.
- Later using lambda they trigger SNS and sends email notification to all the subscribers.
- Lets upload an image into S3 then we will trigger lambda and SNS after that we will send notification.
- Entire configuration we will create using lambda function. 

### Steps:

- Goto terminal and clone the Github code and enter into the folders

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/67f435cd-58e6-4915-8dd4-4ee18298ba14)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/88716a20-519f-4f50-a9a7-4aa3ea54c5be)

- I'm using ubuntu EC2 server here to configure AWS lets install some packages

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/fddf5929-de6c-42dc-bb7e-f65a2f505039)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/e7c2c241-18de-49bd-9e57-8bc9576b5c64)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/7f50e412-11d9-4db3-aff7-d8b6465da113)

- Goto shell scripting do some changes like aws region, bucket name, email address.
- 
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/78761489-ec0b-49ed-9dab-eb19297612c4)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/837e024a-39ff-48a3-9074-b931ae61b09b)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/4b4e7852-8f76-4b53-a303-8e22ef4ebc84)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/95b6c8ef-30c0-468d-ad72-7d05958858e3)

- Before executing script lets install some packages here,

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/9dccd179-8b0c-4f51-a435-7bb3e2df1e33)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/e30ad820-29d3-41e2-97d2-7e94e5c5934f)

- Lets execute the shell script now.

- AWS region, s3 bucket name, lambda function name, role name, email address has been set.

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/31a09d8e-9e88-48a9-8d84-bc4399fe28e4)

- IAM role has been created

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/fa84f018-5c6e-46ef-8c25-6fb068d1cd9b)

- Lets chek IAM in AWS Console

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/7c152fb2-41ae-47e4-a8e0-30035490ea9a)

- Permissions has been given inside IAM role

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/ac1d3afd-0aff-427f-b21e-4060dec44560)

- Lets check inside s3-lambda-sns role

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/8175a48a-f488-4471-9771-8d129f837a8f)

- S3 bucket has been created

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/5ad5b100-75ca-4358-90f6-53326349f3ab)

- Lets check in s3 bucket in AWS console

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/0f0a99ef-66ab-4aeb-a86d-bb2dc545f084)

- Event notification has been set in S3 bucket ppermisssions

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/2312ad08-4676-4f03-bf7f-0e078da4a169)

- Lambda function has been created

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/3e803053-dc6c-4fe2-ba0a-e638667ed154)

- Lets check lambda function in AWS console

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/0f97fb04-22b9-4494-b05c-43e7dfd80a32)

- Python Source code inside lambda function

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/0101661c-2451-405e-b872-4094cf1e47b7)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/95135cff-0a21-48d4-b43a-d1fb7b13e7da)

- SNS notification has been sent

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/35409fe6-4ffb-4c7c-a51a-903958f8668f)

- Lets check SNS notificaion inside AWS console

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/f3992286-8df0-4a89-a317-3f1fb1eb35ee)

- Lets go to mailId and confirm subscription

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/2b635b1a-01b8-4428-8d63-e7be02df9e56)

- We will get a popup message conforming the subscription

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/df271373-d1f1-4b30-96e9-0d64ee34af5a)

- Lets go to SNS subscriptions and check, it is confirmed

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/c3054a01-6e64-4de2-b6c8-9fa54b062ea6)

- Now, lets upload a file image and check whether we get notification to mail or not.

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/b9bad0f9-521c-40a1-b8fd-90246ef22311)

- Upload of image is succeeded

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/9526df32-14cb-40d0-bf88-1648972df667)

- Lets execute shell script again and check the mail

![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/0ef58b02-24a0-4a01-a41f-15a133d9c78a)


