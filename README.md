# Daily Tag Report Email

<p align="center">
	<a href="https://join.slack.com/t/yrisgroupe/shared_invite/zt-1q51z8dmv-GC0XzUSclzBnUQ0tpKhznw"><img alt="Slack Shield" src="https://img.shields.io/badge/slack-yris-brightgreen.svg?logo=slack"></a>
	<a href="https://github.com/Yris-ops/aws-daily-tag-report-email"><img alt="Repo size" src="https://img.shields.io/github/repo-size/Yris-ops/aws-daily-tag-report-email"></a>
	<a href="https://github.com/Yris-ops/aws-daily-tag-report-email"><img alt="Stars" src="https://img.shields.io/github/stars/Yris-ops/aws-daily-tag-report-email"></a>
	<a href="https://twitter.com/cz_antoine"><img alt="Twitter" src="https://img.shields.io/twitter/follow/cz_antoine?style=social"></a>
	<a href="https://www.linkedin.com/in/antoine-cichowicz-837575b1"><img alt="Linkedin" src="https://img.shields.io/badge/-Antoine-blue?style=flat-square&logo=Linkedin&logoColor=white"></a>
<p>

![Daily Tag Report](./img/DailyTagReportArchitecture.png)

The purpose of this template is to create a set of AWS resources that generate a daily tag report and send it to a specified email address.

## Key Components

- LambdaExecutionRole: An IAM role with permissions to access EC2 and SNS services.
- DailyTagReportLambda: A Lambda function that generates the tag report.

## Parameters

- EmailAddress: The email address to receive the tag report.

## Usage

1. Open the AWS CloudFormation console.
1. Create a new stack and upload the stack.yml file.
1. Enter the desired email address in the EmailAddress parameter.
1. Click on the "Create stack" button to deploy the resources.
1. Test the DailyTagReportLambda Function and Enjoy.

## Supported Resources

- EC2
- Security Group
- Volume
- Key Pair
- Load Balancer

[Boto3 Documentation 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#client)

## Note

The AWS region is set to `us-east-1` in the template, if you want to deploy in another region you need to modify the template accordingly.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This repository is licensed under the Apache License 2.0. See the LICENSE file.