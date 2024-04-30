# 👨🏼‍💻 Deploying a Free Tier Python Web Application on AWS 👨🏼‍💻


## 
In this runbook, we will implement the Python app deployment with free-tier architecture on AWS. We will be using the five popular services of AWS Amplify, AWS Lambda, Amazon API Gateway, Amazon DynamoDB, AWS IAM. We'll also see how to host a serverless application in AWS Console by end to end process.

## STEP 1: Using AWS AMPLIFY:
### A) Use simple Amplify - Hosting
1. Open console, search "AWS AMPLIFY" and click Get started.
 
 ![aws-1](https://github.com/SowmyaJ2/project1/assets/161762221/8dc51507-0770-4292-8285-0a72a87dcc7e)


2. Give App name `mathpower`
3. Drag and drop the filename (use zipfile format) and click save and deploy

 ![aws-2](https://github.com/SowmyaJ2/project1/assets/161762221/40f46c80-e4ca-427c-bee4-d8a7140ae078)


4. Copy the URL and put in browser to see the result

 ![aws-3](https://github.com/SowmyaJ2/project1/assets/161762221/2f57b90e-a6b8-4a96-bf42-724f34aaad0b)


 ## STEP 2: Using AWS LAMBDA:
### A) Math Functionality using Lambda function

1. Open console, search "AWS LAMBDA" and click "Create Function".

![aws-4](https://github.com/SowmyaJ2/project1/assets/161762221/49e31c6d-444a-46cf-a1b1-f0c344676113)


2. Give Function name `mathpower`
3. Give Runtime `Python 3.12`
4. Click "Create Function"
5. Go to the Math power APP in lambda and Click "CODE" then just paste the code (PowerOfMathFunction - Lambda-ORIGINAL) 
6. Test with new event and deploy changes.

![aws-6](https://github.com/SowmyaJ2/project1/assets/161762221/37c18156-9c55-4cb1-ad99-b915555c4040)


7. Test your code and find the successful output over it.

![aws-7](https://github.com/SowmyaJ2/project1/assets/161762221/a7b27b65-e0c2-4f16-a277-ad6e2f3c97f6)


 ## STEP 3: Using AWS APIGateway:
### A) Invoke the Math Functionality using Rest API

1. Open console, search "AWS APIGateway" and click "Create API".

![image](https://github.com/SowmyaJ2/project1/assets/161762221/e41eb8e8-6ba5-47ba-917d-fd727216b507)


2. Create Resource by enter `POST`
3. Then deploy the API.

![image](https://github.com/SowmyaJ2/project1/assets/161762221/cea4a878-b242-4bae-90d3-11bcd19d8845)


 ## STEP 4: Using AMAZON DynamoDB:
### A) Store your math results using DynamoDB table

1. Open console, search "Amazon DynamoDB" and click "Create Table".
2. Give table name `mathpower`
3. Give Partition key `ID`
4. Click "Create Table"
5. Copy the Table ARN 

![image](https://github.com/SowmyaJ2/project1/assets/161762221/adf1e976-95b3-4ca6-80aa-43fb1cef62cf)


![image](https://github.com/SowmyaJ2/project1/assets/161762221/6a895f07-22fe-4f27-93ae-bf1bcf15c7b7)


 ## STEP 5: Using AWS IAM:
### A) Store your math results using DynamoDB table

1. Open console, search "Amazon IAM"
2. Give role permission.

 ## CONGRATULATIONS!! CONGRATULATIONS!!
4. After all set, paste the final code to lambda and browser it with the URL, it works!















