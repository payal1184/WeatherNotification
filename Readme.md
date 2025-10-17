# AWS Weather Alerts

A serverless AWS project that fetches real-time weather data using OpenWeatherMap API and sends alerts via AWS SNS.

---

## 🚀 Features
- ✅ Fetches real-time weather updates
- ✅ Sends SMS/Email alerts via AWS SNS
- ✅ Serverless and cost-effective using AWS Lambda
- ✅ Scheduled execution using EventBridge Scheduler

---

## 🛠 Tech Stack & AWS Services Used
- **AWS Lambda** - Executes Python script to fetch weather data
- **Amazon SNS** - Sends notifications to subscribed email/phone
- **Amazon EventBridge Scheduler** - Triggers Lambda function at scheduled times
- **Amazon CloudWatch Logs** - Monitors Lambda execution
- **OpenWeatherMap API** - Provides real-time weather data

---

## 📸 Screenshots

### 1️⃣ OpenWeatherMap API Key
![API Key Screenshot](screenshots/api_key.png)  
*API key was created to fetch weather data.*

### 2️⃣ AWS SNS Topic
![SNS Topic](screenshots/sns_topic.png)  
*SNS topic created to send notifications via email.*

### 3️⃣ Lambda Function
![Lambda Function](screenshots/lambda_function.png)  
*Lambda function fetches weather and publishes message to SNS.*

### 4️⃣ CloudWatch Logs
![CloudWatch Logs](screenshots/cloudwatch_log.png)  
*CloudWatch shows execution of Lambda function.*

### 5️⃣ EventBridge Schedule
![EventBridge Schedule](screenshots/eventbridge_schedule.png)  
*EventBridge Scheduler triggers Lambda daily at 8 AM IST.*

---

## ⚡ How to Run This Project
1. Get an OpenWeatherMap API Key from [OpenWeatherMap](https://home.openweathermap.org/api_keys).  
2. Create an SNS topic and subscribe your email/phone.  
3. Deploy the Lambda Function in AWS Lambda.  
4. Schedule the Lambda function using EventBridge Scheduler.  
5. Check your email for daily weather notifications!
