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
Email subscription is confirmed to receive alerts.
Alerts are sent using the Email protocol.

![SNS Topic Screenshot](image/Screenshot%20(170).png)

![SNS Topic Screenshot](image/Screenshot%20(171).png) 

---

## 📅 Step 5: Amazon EventBridge Scheduler
Scheduled a rule to trigger the Lambda function at regular intervals.  

- **Service:** Amazon EventBridge (CloudWatch Event)  
- **Frequency:** Every 1 hour  
- **Target:** Lambda function  

![EventBridge Scheduler Screenshot](images/eventbridge_scheduler.png)

---

## 📖 Step 6: Amazon CloudWatch Logs
Monitored Lambda execution logs to ensure proper functioning and debug errors.  

- **Service:** Amazon CloudWatch Logs  
- **Purpose:** View function logs, track errors and notifications  

![CloudWatch Logs Screenshot](images/cloudwatch_logs.png)

---

## 💻 Step 7: Testing & Notification
Tested the Lambda function to verify:  

1. Weather data fetched correctly  
2. Alerts sent via SNS to subscribed email  

![Email Notification Screenshot](images/email_notification.png)

---