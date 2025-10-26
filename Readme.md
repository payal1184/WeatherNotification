# AWS Weather Alerts

A serverless AWS project that fetches real-time weather data using OpenWeatherMap API and sends alerts via AWS SNS.

---

## 🚀 Features
- ✅ Fetches real-time weather updates using OpenWeatherMap API
- ✅ Sends SMS/Email alerts via AWS SNS
- ✅ Serverless and cost-effective using AWS Lambda
- ✅ Scheduled execution using EventBridge Scheduler
- ✅ Monitors execution and logs using Amazon CloudWatch
- ✅ IAM roles & policies secure AWS resources
- ✅ Easy to customize city and notification preferences

---

## 🔧 Technologies & Services
- **AWS Lambda** - Executes Python script to fetch weather data  
- **Amazon SNS** - Sends notifications to subscribed email/phone  
- **Amazon EventBridge Scheduler** - Triggers Lambda function at scheduled times  
- **Amazon CloudWatch Logs** - Monitors Lambda execution  
- **IAM Roles & Policies** - Grants Lambda permissions to publish to SNS  
- **OpenWeatherMap API** - Provides real-time weather data  

---

## 🚀 Project Setup & Configuration

Here’s a visual walkthrough of how this AWS Weather Notification project was built and configured.


## 🧩 Step 1: OpenWeatherMap API
Created an API key from OpenWeatherMap to fetch real-time weather data.
The API key allows the Lambda function to access current weather data.

![OpenWeatherMap API Screenshot](image/7d217b1f-d2f5-4267-82d2-5e9b7846814b.png)

---

## 🖥️ Step 2: AWS Lambda Function

Created a Lambda function to process weather data and send alerts.  

![Lambda Function Screenshot](image/Screenshot%20(149).png)

displays the Lambda function code editor, where the Python script fetches live weather data using OpenWeatherMap API and publishes notifications through Amazon SNS.

![Lambda Function Screenshot](image/Screenshot%20(157).png)
---


## 🔐 Step 3: IAM Roles & Policies
  
The IAM role allows the Lambda function to securely publish messages to SNS.  

![IAM Roles Screenshot](image/Screenshot%20(155).png)

Attached roles and policies to give Lambda the required permissions.   
These permissions enable the Lambda function to send notifications securely and reliably.  

![IAM Roles Screenshot](image/Screenshot%20(159).png)

## ☁️ Step 4: Amazon SNS Topic

Created an SNS topic to send weather notifications.
This topic acts as a communication channel for notifications.

![SNS Topic Screenshot](image/Screenshot%20(170).png)

Email subscription is confirmed to receive weather alerts.
Ensures that all notifications are successfully delivered to the user.

![SNS Topic Screenshot](image/Screenshot%20(171).png) 

---

## 📅 Step 5: Amazon EventBridge Scheduler
Scheduled a rule to trigger the Lambda function at regular intervals.  
Configured an EventBridge Scheduler to trigger the Lambda function at regular intervals.
This ensures that the weather data is fetched and alerts are sent automatically without manual execution.
The schedule runs the function reliably at the defined time interval.

![EventBridge Scheduler Screenshot](image/Screenshot%20(163).png)

![EventBridge Scheduler Screenshot](image/Screenshot%20(172).png)

---

## 📖 Step 6: Amazon CloudWatch Logs

Integrated Amazon CloudWatch Logs to monitor and verify Lambda function executions.
Created a dedicated CloudWatch Log Group to store Lambda execution logs.

![CloudWatch Logs Screenshot](image/Screenshot%20(166).png)

Log streams capture detailed information about API responses, notifications, and errors.
![CloudWatch Logs Screenshot](image/Screenshot%20(167).png)

Displays detailed log events from each Lambda execution, including API responses and SNS confirmations.  
Useful for debugging issues and verifying successful alert delivery.
![CloudWatch Logs Screenshot](image/Screenshot%20(169).png)

---

## 💻 Step 7: Testing & Notification

Tested the Lambda function to verify:  

1. Weather data fetched successfully  
2. Alerts sent via SNS to subscribed email  

![Email Notification Screenshot](images/email_notification.png)

---