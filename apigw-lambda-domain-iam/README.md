# What Does This Template Summon?

This template is a CloudFormation script that conjures up an API Gateway, a Lambda function, and an IAM role to secure the function.

Check out the full article on [Medium - Configurable CloudFormation Template - API Gateway, custom domain, Lambda Integration](https://medium.com/@saurabhkumar_4718/automate-api-gateway-lambda-iam-role-creation-using-cloudformation-templates-7b3b3b3b3b3b).

## API Gateway as the Front Gate:
The face of your operations, it’s a custom domain API Gateway, easily configurable to represent your unique digital presence in the cloud.

## Lambda, the Magic Worker:
Behind this gateway lies the real wizardry. Ready to execute your business logic without the need to manage servers.
The code that empowers this function rests securely in an existing S3 bucket, summoned as needed.

## The Invisible Cloak of Security:
The template weaves an IAM role automatically, granting your Lambda function the precise permissions needed to perform its duties securely and efficiently.

# Prerequisites:
Before diving into the configuration steps, ensure you have the following:

- An AWS account with administrative access.
- Your own domain name, configured with Route 53 or a third-party DNS provider.
    ######     The template will create a custom domain for the API Gateway.
- A signed ACM certificate (us-east)
- S3 bucket to hold the lambda code.
- Code repository file uploaded to the mentioned S3 bucket.
- A basic understanding of AWS Lambda functions and API Gateway configurations.
  
## Lets Get Down To Business, How to deploy the template:
1. Set up the prerequisites. 
2. Modify the Parameters at the top of the yaml. 
3. Deploy the stack using aws console or aws cli.