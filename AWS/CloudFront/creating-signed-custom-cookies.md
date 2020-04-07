# The steps to create signed custom cookies

## STEPS

### 1. Create s3 Bucket

### 2. Create CloudFront distribution

### 3. Create CloudFront key pairs

1. Login with root credentials
2. Under profile name select my Security credentials
3. Under CloudFront key pairs click create New Key pair
4. Download the public and private keys
5. Record the key pair 

### 4. Create KMS key

1. Open up Key Management Service (KMS)
2. Create a key (Symmetric)
3. Add correct access accounts to decrypt

### 5. Encrypt the CloudFront private key using AWS-CLI
1. Use Batch
2. navigate to directory of private key
```shell script
aws kms encrypt --key-id _REPLACE_WITH_KMS_KEY_ID --plaintext "$(cat REPLACE_WITH_PRIVATE_KEY_FILE_NAME.pem)" --query CiphertextBlob --output text
```

### 6. Open Cloudfront
1. Create a new distribution
2. Add S3 bucket and make sure there is a SSL certificate attached and it is HTTPS only
3. Add an origin identity and make sure bucket policy is updated
4. S3 should be under sub-domain
5. s3 - create a public and private area to the site using Behaviours
6. Add trusted signers (tick box)to private content and default content
7. Add api gateway as an origin
8. IMPORTANT the stage is added into the origin and therefore not used when talking to the API. Naming for API and S3 paths is therefore very important.  
It is also important to have api gateway and s3 under the same origin to allow the cookies to work

