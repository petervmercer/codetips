# Installation

## link to download AWS CLI

https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html#install-tool-bundled

## Configuration

First set up IAM user for CLI Administration and save the access key and secret

### Setting up the configuration file

```shell script
$ aws configure
  AWS Access Key ID: <the Access key ID from the csv>
  AWS Secret Access Key: <the Secret access key from the csv>
  Default region name: <your AWS region such as eu-west-1>
  Default output format: <optional>
```

### Creating a specific profile

```shell script
$ aws configure --profile dev
```

