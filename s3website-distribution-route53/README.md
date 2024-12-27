
# Static Website CloudFormation Template
This CloudFormation template creates a static website hosted on Amazon S3 and served via Amazon CloudFront.<br> 
It creates an S3 bucket to store the website content, a CloudFront distribution to serve the content with caching and SSL support,
and uses a CloudFront Origin Access Identity (OAI) to restrict access to the S3 bucket.<br>
A Route 53 A record set to associate the custom domain name with the CloudFront distribution.<br>
## Resources Created
- S3 Bucket: Stores the static website content.
- CloudFront Distribution: Serves the website content with caching and SSL support.
- Route 53 Record Set: Associates the custom domain name with the CloudFront distribution.
- CloudFront Origin Access Identity (OAI): Restricts access to the S3 bucket to only CloudFront.
## Parameters
- HostedZone: The Route 53 hosted zone name, used also as the bucket name prefix.
- AcmCertificateArn: The ARN of the ACM certificate for SSL support.<br>
<b> Certificate in us-east1 region </b>
- WebsiteRootIndex: The index document for the website (default: index.html).
- WebsiteError: The error document for the website (default: error.html).
- RedirectFunctionArn: The ARN of the Lambda function for redirecting www to non www (optional).
## Usage
1. Create the Hosted Zone: Ensure you have a hosted zone created in Amazon Route 53.
2. Create the ACM Certificate: Ensure you have an ACM certificate created in the us-east-1 region.
3. Upload the Template: Upload the CloudFormation template to your AWS account.
4. Specify Parameters: Provide the required parameters such as HostedZone, AcmCertificateArn, and S3BucketForWebsiteContent.
5. Deploy the Stack: Deploy the CloudFormation stack to create the resources.