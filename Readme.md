# AWS Weather Alerts

A serverless AWS project that fetches real-time weather data using OpenWeatherMap API and sends alerts via AWS SNS.

---

## 🚀 Features
- ✅ Fetches real-time weather updates
- ✅ Sends SMS/Email alerts via AWS SNS
- ✅ Serverless and cost-effective using AWS Lambda
- ✅ Scheduled execution using EventBridge Scheduler

---

## 🔧 Technologies & Services
- ✅ Fetches real-time weather updates using OpenWeatherMap API
- ✅ Sends SMS/Email alerts via AWS SNS
- ✅ Serverless and cost-effective using AWS Lambda
- ✅ Scheduled execution using EventBridge Scheduler
- ✅ Monitors execution and logs using Amazon CloudWatch
- ✅ IAM roles & policies secure AWS resources
- ✅ Easy to customize city and notification preferences


---


### 1️⃣ OpenWeatherMap API Key
![API Key Screenshot]()  
*API key was created to fetch weather data.*

### 2️⃣ AWS SNS Topic
![SNS Topic]()  
*SNS topic created to send notifications via email.*

### 3️⃣ Lambda Function
![Lambda Function])  
*Lambda function fetches weather and publishes message to SNS.*

### 4️⃣ CloudWatch Logs
![CloudWatch Logs]()  
*CloudWatch shows execution of Lambda function.*

### 5️⃣ EventBridge Schedule
![EventBridge Schedule]()  
*EventBridge Scheduler triggers Lambda daily at 8 AM IST.*

---

## ⚡ How to Run This Project
1. Get an OpenWeatherMap API Key from [OpenWeatherMap](https://home.openweathermap.org/api_keys).  
2. Create an SNS topic and subscribe your email/phone.  
3. Deploy the Lambda Function in AWS Lambda.  
4. Schedule the Lambda function using EventBridge Scheduler.  
5. Check your email for daily weather notifications!
