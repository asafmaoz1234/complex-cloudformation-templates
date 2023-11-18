# AWS Lambda with Java 17
**java17-eventbridge-sqs.yaml**

## Overview

This CloudFormation template deploys an AWS Lambda function written in Java 17 and uses a jar file from S3. 
The Lambda function can be triggered by either an EventBridge event or an SQS message.<br> 
This README provides instructions on deploying and using the template.

## Prerequisites

Before deploying this template, ensure you have the following prerequisites:
- An AWS account with the necessary permissions to create Lambda functions, IAM roles, and event resources.
- An S3 bucket with the code base jar uploaded.
- SQS queue set up.
- EventBridge (formally cloudwatch) scheduled event.

## Template Details

### Resources Created

- **Lambda Function**:
    - Function Name: MyJavaLambdaFunction (Replace with your preferred Lambda function name)
    - Runtime: Java 17
    - Handler: com.example.MyHandler::handleRequest (Replace with your Lambda function handler)
    - Execution Role: IAM role with necessary permissions.
    - Code Source: JAR file stored in an S3 bucket.

- **IAM Role**:
    - Assume Role Policy: Allows Lambda service to assume the role.
    - Execution Policy: Grants permissions for Lambda function to interact with logs, SQS, and EventBridge (adjust resource ARNs as needed).

- **Lambda Event Source Mapping (SQS)**:
    - Binds the Lambda function to an SQS queue for message triggering.

- **Lambda Permission for EventBridge**:
    - Grants EventBridge the permission to invoke the Lambda function.

## Deployment

Follow these steps to deploy the CloudFormation stack:

1. Clone this repository to your local machine.

2. Navigate to the directory containing this CloudFormation template.

3. Deploy the stack using AWS CLI:
   ```shell
   aws cloudformation create-stack --stack-name MyJavaLambdaStack --template-body file://my-java-lambda-template.yaml --capabilities CAPABILITY_IAM
    ```