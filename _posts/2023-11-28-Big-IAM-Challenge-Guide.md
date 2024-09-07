---
title: "Big IAM Challenge Guide"
---
## About

The Big IAM Challenge is a cloud security Capture-The-Flag (CTF) learning exercise designed to teach players how to use Identity and Access Management (IAM) in Amazon Web Services, then discover and exploit misconfigurations in IAM policies.

The challenge doesn't require you to create an AWS account or spin up your own resources, since everything is self-contained within the website.

The challenge has 6 sections, each focused on a particular service and with its own flag to find.

1. S3 Bucket (Get/List operations)
2. SQS (Send/Receive messages)
3. SNS
4. S3, but more stringent
5. Cognito
6. Final Stage

## Getting Started

### Helpful Links

[About The Big IAM Challenge](https://www.wiz.io/blog/the-big-iam-challenge)

[Go to The Big IAM Challenge](https://bigiamchallenge.com/challenge/1)

[AWS CLI Command Reference](https://docs.aws.amazon.com/cli/latest/reference/s3/ls.html)

### AWS Commands

To get started with the challenge, let's break down the first command they give you.

    aws sts get-caller-identity

The AWS Command Line Interface (CLI) is a tool used to manage AWS resources from a terminal/command prompt. It is called by the ```aws``` argument.

Security Token Service (STS) is a web service that enables you to request and manage temporary, limited-privilege credentials for AWS resources. The ```sts``` argument directs the AWS CLI to interact with this service.

```get-caller-identity``` allows you to retrieve the User ID, account number, and Amazon Resource Name (ARN) of the access credentials used to run this command.

Altogether, ```aws sts get-caller-identity``` operates similarly to a Linux ```whoami```. 

### First Steps

The first challenge presents a public S3 bucket allowing **GetObject** and **ListBucket** actions. We can see this by clicking the "View IAM Policy" button.

We can go to the AWS CLI documentation to search for commands related to the actions listed in the policy.

You can use the above link or manually search "aws cli s3" to find the commands.

To list the contents of a bucket in S3, use the command ```aws s3 ls s3://bucket-url``` 

Note that the ```aws s3 ls``` and the Bash```ls``` commands have their own unique syntax and arguments, and you will need to reference the AWS CLI documentation for more guidance.

Remember to submit the whole flag, including the {} brackets and wiz: tag.

## Further Help

1st Challenge Hint: The shell provided is read-only. To copy the contents of the bucket to the command line, use the ```-``` operator.

2nd Challenge Hint: The format for a SQS URL is: 
```
https://sqs.region-name.amazonaws.com/account-number/resource-name
```

3rd Challenge Hint: You will need an HTTP Request Catcher to complete this challenge. 

4th Challenge Hint: The option needed to solve this challenge is a part of the S3 CLI library.

