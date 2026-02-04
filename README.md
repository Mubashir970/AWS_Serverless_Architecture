# Serverless Management System — AWS
Serverless Student Management System

A cloud-native serverless web application built using AWS services that allows users to add and retrieve student details through a web interface without managing any servers.

This project demonstrates real-world serverless architecture using AWS best practices such as API Gateway, Lambda, DynamoDB, and S3 Static Website Hosting.

#📌 Project Overview
The application provides a simple UI where users can:

Add student information (Student ID, Name, Class, Age)

View all stored student records in real time

All backend operations are handled by AWS managed services, ensuring scalability, security, and cost efficiency.

#🧩 Core Highlights

Fully serverless architecture

Static frontend hosted on Amazon S3

REST APIs powered by Amazon API Gateway

Business logic implemented using AWS Lambda

Data persistence using Amazon DynamoDB

CORS-enabled API for browser access

No servers, no infrastructure management

🖥️ Application Preview
🔹 Student Management UI
<img width="796" height="699" alt="student-information-details s3-website-us-east-1 amazonaws com_" src="https://github.com/user-attachments/assets/b8f8ab00-dfae-4c70-baba-8481701af9da" />

🏗️ Cloud Architecture Diagram
Serverless Architecture Overview

User Browser
     |
     v
Amazon S3 (Static Website Hosting)
     |
     v
Amazon API Gateway (GET / POST)
     |
     v
AWS Lambda Functions
     |
     v
Amazon DynamoDB

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/13e455e6-a923-4e35-9488-6a12c96fded8" />

🔄 Architecture Flow

User accesses the frontend hosted on Amazon S3

Frontend sends HTTP requests using JavaScript (AJAX)

Requests reach Amazon API Gateway

API Gateway triggers AWS Lambda

Lambda performs CRUD operations on DynamoDB

Response is returned back to the browser

🧰 Technologies Used
Frontend

HTML5

CSS3

JavaScript

jQuery (AJAX)

AWS Cloud Services

Amazon S3 – Static Website Hosting

Amazon API Gateway – REST API

AWS Lambda – Backend compute

Amazon DynamoDB – NoSQL database

IAM – Secure access control

🗄️ DynamoDB Design

Table Name: Student_Details

Attribute	Type
studentid	    String (Partition Key)
name	        String
class	        Number
age	          Number

