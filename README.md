# Arizona Bootstrap Review Site

This repository contains the CloudFormation template to deploy the infrastructure
required to host the Arizona Digital review site over HTTPS.

## Manula Steps
- Before initial deploy, you must create a certificate in ACM in the us-east-1 region
- After deploy, you will need to add the domain record to Route53 as an alias to the cloudfront distributuin

## Teardown
- Delete everything from the S3 bucket
- Delete the CloudFormation stack
- Delete the Rout53 entries for the main domain and the ACM certificate verification domain
- Delete the certificate from ACM
