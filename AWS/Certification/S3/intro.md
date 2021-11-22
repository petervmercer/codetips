#Intro to S3

s3 provides secure, drable, highly scalable object storage

- Used for files, images, web pages

- Unlimited storage

- Max size 5TB

- stored in Buckets

- S3 bucket must have a universal nameSpace
```text
https://bucket-name.s3.Region.amazonaws.com/key-name
```
S3 stores objects as key - value

example max.jpg is the key and the value is the image data.  There is also a version ID and metadata (Content type, and any extra data);

The S3 is spread across regions

## Availiability
99.95% - 99.99%
## Designed for Durability
99.999999999 (11 9's)

## Tiered Storage

## Lifecycle Management
- allows deletetion
- movement of objects to cheaper storage

## Versioning

## Secure your data
- server-Side Encryption
- Access Control Lists (ACLs) - Which AWS accounts or groups are granted access and the type of access.  You can attach s# ACLs to individual objects within a bucket.
- Bucket policies
    - What actions are alloweed or denied



