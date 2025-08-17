# Serverless-Architecture-Cloud-Automation
Sample of serverless Architecture automation
# Assignment 4: Automatic EBS Snapshot and Cleanup Using AWS Lambda and Boto3

This project includes scripts and resources to automatically create and clean up Amazon EBS snapshots using AWS Lambda and the Boto3 Python SDK.

## Features

- **Automatic EBS Snapshot Creation**: Lambda functions are triggered to create snapshots of specified EBS volumes on a schedule.
- **Snapshot Cleanup**: Old snapshots beyond a retention period are deleted to save costs and maintain compliance.
- **Serverless Architecture**: The solution is designed to be fully serverless using AWS Lambda.

## How It Works

1. **Lambda Function for Snapshot Creation**: Automatically creates snapshots for defined EBS volumes using Boto3.
2. **Lambda Function for Cleanup**: Periodically scans for outdated snapshots and deletes them.
3. **Scheduling**: AWS CloudWatch Events (EventBridge) can be used to trigger Lambda functions at desired intervals.

## Prerequisites

- An AWS account with necessary IAM permissions for EBS and Lambda.
- Python (for local development and testing).
- The AWS CLI and Boto3 installed.

## Deployment

1. Configure your AWS credentials.
2. Deploy the Lambda functions using the AWS Console or AWS CLI.
3. Set up CloudWatch Events to trigger the functions as required.

## License

This project is for educational purposes.
