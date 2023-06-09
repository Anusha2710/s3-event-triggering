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

- Goto terminal and clone the Github code and configure AWS.
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/67f435cd-58e6-4915-8dd4-4ee18298ba14)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/ba19a755-6586-4104-a77f-bf812cdf9526)
- I'm using ubuntu EC2 server here,
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/fddf5929-de6c-42dc-bb7e-f65a2f505039)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/e7c2c241-18de-49bd-9e57-8bc9576b5c64)

- After that go inside folders and goto shell scripting do some changes like aws region, bucket name, email address.
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/7f50e412-11d9-4db3-aff7-d8b6465da113)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/78761489-ec0b-49ed-9dab-eb19297612c4)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/837e024a-39ff-48a3-9074-b931ae61b09b)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/4b4e7852-8f76-4b53-a303-8e22ef4ebc84)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/95b6c8ef-30c0-468d-ad72-7d05958858e3)

- Before executing script lets install some packages here,
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/9dccd179-8b0c-4f51-a435-7bb3e2df1e33)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/e30ad820-29d3-41e2-97d2-7e94e5c5934f)

- Lets execute the shell script now.
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/f6987fa1-4532-4857-adda-4a59a3c7d014)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/be89105e-73cd-4d86-be41-f720d7dd006c)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/106de765-737e-4e69-887d-634fd6b718e7)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/2e5a4034-f33c-474d-8654-78925a2a8e8a)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/a6367d3c-d62a-4828-b76e-c612bb7f4719)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/ffde3858-4745-4e00-9637-e0f37f5da545)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/9bfc6c9b-be4f-4d90-ae44-4c334ca5105e)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/731eec9f-c96e-4863-a08d-2a1388f3da8a)
![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/58be84b6-309e-4530-82cb-60a18e7d47d0)


