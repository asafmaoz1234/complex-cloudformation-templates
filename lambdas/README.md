# cloudformation-templates

<h2>AWS Lambda with EventBridge and SQS Integration</h2>

**java17-eventbridge-sqs.yaml**

<p>This CloudFormation template establishes a comprehensive AWS environment for a Java 17 Lambda function, with the added capability of being triggered by either a scheduled Amazon EventBridge event or messages from an AWS SQS queue. It provides an automated, event-driven setup that is ideal for various serverless application scenarios.</p>

<h3>Key Components of the Template:</h3>
<ul>
  <li><strong>AWS Lambda Function</strong>: Runs Java 17 code, set to be triggered by EventBridge or SQS.</li>
  <li><strong>Amazon EventBridge Rule</strong>: Configured to trigger the Lambda function daily at 20:00 UTC.</li>
  <li><strong>AWS SQS Queue</strong>: A message queue that can also trigger the Lambda function.</li>
  <li><strong>Amazon S3 Bucket</strong>: Created to store the Java Lambda function's JAR file.</li>
</ul>
