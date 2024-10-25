# Push_WebApp_DynamoDB
This project helps in pushing data from web application to DynamoDB table using Lambda function, API Gateway, Amplify.
This project builds a basic web application using AWS services, including a front-end and back-end with API and database interactivity.

# Overview:
The application architecture consists of the following components:
1. Front-end: HTML/CSS/JavaScript, hosted on AWS Amplify
2. API Gateway: Manages API requests (AWS API Gateway)
3. Lambda: Python based Serverless function for backend logic (AWS Lambda)
4. DynamoDB: NoSQL database for data storage (AWS DynamoDB)

# Technical Flow:
1. User interacts with the web interface hosted on AWS Amplify.
2. JavaScript in the front-end makes an API call to the API Gateway when the submit button is clicked.
3. API Gateway triggers the associated Lambda function.
4. Lambda function processes the input and writes data to the DynamoDB table.
5. The response is sent back through API Gateway to the front-end.
6. Front-end displays the result to the user whether it was successfull or not.
   
# Steps to Create:
1. Create Web App: Design the front-end using HTML, CSS, and JavaScript. Host the static website on AWS Amplify by uploading a compressed ZIP file containing the HTML.
2. Building Serverless Function: Create a Lambda function using Python 3.8 in AWS Lambda. Implement logic to process user input and write to DynamoDB.
3. Link Serverless Function to Web App using API Gateway: Create a REST API using AWS API Gateway. Define HTTP methods (POST). Integrate the API with the Lambda function. Enable the CORS. Deploy the API.
4. Create Data Table: Set up a DynamoDB table with "ID" as the partition key.
5. Interactivity to Web APP: Add IAM policy to Lambda execution role for DynamoDB access.

# Working:
1. User opens the web application hosted on AWS Amplify.
2. User enters data into the form fields (First Name and Last Name).
3. Upon clicking the "Submit" button, the JavaScript callAPI function is triggered.
4. The function makes a POST request to the API Gateway endpoint.
5. API Gateway invokes the Lambda function.
6. Lambda function processes the input and writes the data to DynamoDB.
7. The response is sent back through the API to the front-end.
8. An alert displays the result to the user.
   
# Sample Testing Images:
![Screenshot 2024-10-24 at 12 35 30 PM](https://github.com/user-attachments/assets/0cb81a38-0423-49ce-a59c-76960e91fd19)
![Screenshot 2024-10-24 at 12 36 16 PM](https://github.com/user-attachments/assets/d3604ef5-0625-47d0-8046-9d80e9982ac2)
