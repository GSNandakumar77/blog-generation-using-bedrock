🚀 Excited to share my latest project: Automated Blog Generation using AWS Bedrock!

Built an end-to-end serverless pipeline leveraging AWS Bedrock’s Titan Text Express (amazon.titan-text-express-v1) model, AWS Lambda, Amazon API Gateway, and S3.

Tools & Services:
Amazon Bedrock (Titan Text Express model)

AWS Lambda (Serverless compute)

Amazon API Gateway (HTTP endpoint for Lambda)

Amazon S3 (Storage)

Python & boto3 for integration

IAM for secure, scoped permissions

Workflow stages:
User input (blog topic via API Gateway REST API)
→ Lambda function triggers
→ Invoke Bedrock model for text generation
→ Receive generated blog text (JSON)
→ Save blog text to S3 bucket
→ Confirm completion & monitor logs

Architecture diagram:
text
User
   ↓ (HTTP POST /generate-blog)
API Gateway (REST API)
   ↓
AWS Lambda (invokes Bedrock)
   ↓
Amazon Bedrock (Titan Text Express model)
   ↓
Amazon S3 (stores blogs)
Benefits:
Cost-effective, scalable, serverless architecture

Real-time content generation with SOTA language models

Secure storage & automated workflow

Simple HTTP interface via API Gateway