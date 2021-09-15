# AWS Control Tower Integration

We are happy to announce our AWS Control Tower integration. We worked with the Control Tower team to support the automatic enrollment of AWS accounts created by cloudtamer.io.

Control Tower is a free AWS service that offers great features out of the box, like SCP and Config guardrails on all accounts. It also provides a landing zone where all your AWS accounts can send CloudTrail logs and notifications for Config rules. You can read more about Control Tower here: [What is Control Tower?](https://docs.aws.amazon.com/controltower/latest/userguide/what-is-control-tower.html)

The integration is deployed via a CloudFormation template in your AWS management account. The template sets up a Lambda function that performs the enrollment and a CloudWatch Event Rule that triggers the Lambda when a new AWS account is created from Organizations.

This repository contains the CloudFormation templates to support the intergration between cloudtamer.io and AWS Control Tower.

The Support Center article is available [here](https://cloudtamer.zendesk.com/hc/en-us/articles/360043394512-AWS-Control-Tower-Integration).

The AWS blog article on the integration is available [here](https://aws.amazon.com/blogs/awsmarketplace/seamlessly-uphold-security-and-budgeting-posture-with-cloudtamer-io-and-aws-control-tower/).
