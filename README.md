# WildRydes - End-to-End Serverless Web Application Using 7 Services (Tutorial)
This repository contains a tutorial for building a serverless application on AWS using the WildRydes example. The tutorial provides step-by-step guidance to create a backend system for the WildRydes application using various AWS services, such as Lambda, API Gateway, DynamoDB, and others. This repository aims to help developers, particularly those new to serverless architecture, understand key AWS services and learn how to integrate them into a complete serverless application.

Table of Contents
Introduction
Prerequisites
Architecture Overview
Setup Instructions
Step 1: Create a Lambda Function
Step 2: Set Up DynamoDB
Step 3: Configure API Gateway
Step 4: Connect API Gateway to Lambda
Step 5: Test the Application
Error Handling and Troubleshooting
Contributing
License
Introduction
This tutorial guides you through the process of building a serverless backend for a WildRydes application on AWS. You will learn how to create a Lambda function, set up DynamoDB to store data, and use API Gateway to handle HTTP requests. By the end of the tutorial, you will have a basic serverless backend application that processes and stores ride requests.

## Prerequisites
Before starting, ensure you have the following:
An AWS account
AWS CLI installed and configured
Basic knowledge of JavaScript and AWS services like Lambda, API Gateway, and DynamoDB
A text editor/notepad app
An ArcGIS account (made at www.arcgis.com)

Architecture Overview
The serverless architecture for this application involves:
![CodeCommit 40](https://github.com/najmamusa/WildRydesAWS/assets/110435863/fb9627fd-91fc-418f-b0b8-9c5d9811c259)

Lambda Functions: Responsible for executing backend code.
DynamoDB: Serves as a NoSQL database to store application data.
API Gateway: Acts as the HTTP endpoint to trigger Lambda functions and manage RESTful interactions.
Cognito: (Optional) Used for authentication and authorization of users.
Setup Instructions
Here’s how to set up the application:

Step 1: Create a Lambda Function
Navigate to the AWS Lambda console.
Create a new function with your desired runtime (e.g., Node.js).
Implement the logic for handling ride requests and storing data in DynamoDB.
Step 2: Set Up DynamoDB
Go to the DynamoDB console and create a new table to store ride information.
Define the primary key and set any other necessary attributes.
Step 3: Configure API Gateway
Open the API Gateway console and create a new REST API.
Define your endpoints and HTTP methods.
Set up an integration with your Lambda function.
Step 4: Connect API Gateway to Lambda
Configure API Gateway to trigger your Lambda function based on HTTP requests.
Implement CORS (Cross-Origin Resource Sharing) if the frontend application is hosted separately.
Step 5: Test the Application
Deploy the API Gateway and test your endpoints.
Simulate requests to ensure your Lambda function and DynamoDB integration are working correctly.
Error Handling and Troubleshooting
Outline common errors and solutions, such as permissions issues, incorrect resource names, and common deployment mistakes.
Provide tips for debugging Lambda functions and monitoring API Gateway logs.
