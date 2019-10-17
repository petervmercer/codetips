# Instructions for setting up API Gateway, Lambda and DynamoDB through SAMS

## Steps

### 1. Installation and configuration

Refer to installation.md file

### 2. Create an s3 bucket to store deployed lambda code

```shell script
$ aws s3api create-bucket --bucket <you-bucket-name> --profile dev --
create-bucket-configuration LocationConstraint=<your-aws-region> --region
<your-aws-region>
```
#### Regions
https://docs.aws.amazon.com/general/latest/gr/rande.html

### 3. Setting up common variables

```shell script
#!/bin/sh
export profile="dev"
export region="<your-aws-region>"
export aws_account_id=$(aws sts get-caller-identity --query 'Account' --
profile $profile | tr -d '\"')
# export aws_account_id="<your-aws-accountid>"
export template="lambda-dynamo-data-api"
export bucket="<you-bucket-name>"
export prefix="tmp/sam"
# Lambda settings
export zip_file="lambda-function.zip"
export files="lambda_return_dynamo_records.py"
```

### 4. Permissions

Refer to permissions.md

### 5. Create roles

Refer to create roles script.


