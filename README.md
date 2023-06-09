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

- Whenever a new video is uploaded in netflix it uses s3 for storing of data, next s3 bucket triggers lambda function because it is serverless, also we will create IAM user.
- Later using lambda they trigger SNS and sends email notification to all the subscribers.
- Lets upload an image into S3 then we will trigger lambda and SNS after that we will send notification.
- Entire configuration we will create using lambda function. 

### Steps:

- Goto terminal and clone the Github code and configure AWS.
- ![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/67f435cd-58e6-4915-8dd4-4ee18298ba14)
- ![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/ba19a755-6586-4104-a77f-bf812cdf9526)
- ![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/eab02006-fae0-4baa-a5f1-138306d91099)

- After that go inside folders and execute shell script.
- ![image](https://github.com/Anusha2710/s3-event-triggering/assets/47424821/7f50e412-11d9-4db3-aff7-d8b6465da113)

