# Build-Severless-Website
Build Severless Website using Lambda- to display the results, S3- to host static website, API Gateway to invoke Lambda when website is queried

# Requirement
This sample project depends on boto3, the AWS SDK for Python, and requires Python 2.6.5+, 2.7, 3.3, 3.4, or 3.5. You can install boto3 using pip:

pip install boto3

# Project Execution
1. Launch S3 by enabling ACLs & Public Access
2. Launch a static website in S3 under properties tab
3. Launch Lambda function and write python code to display the results
4. Create a trigger under Lambda as HTTPs APIGateway
5. Enable CORS while creating APIgatway without which serverless website wont work
6. Host URL from triggers under lambda to check if the lambda is working
7. Update index file with APIGatway Endpoint
8. Upload both html files - index & error to S3 bucket
9. While uploading files enable public access to those files(otherwise you get 404 forbidden access)
10. Host the static website link to validate the results
