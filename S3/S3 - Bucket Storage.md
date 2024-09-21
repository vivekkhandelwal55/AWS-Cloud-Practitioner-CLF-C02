
 - there is no directory concept in S3 bucket(UI may confuse you)
 - there are keys through which data can be accessed
	 - s3://my-bucket/file.txt
	 - s3://my-bucket/image/cat.png
	- Max Object Size is 5TB, if you are uploading file greater than 5GB, then you should use `multi-part upload`
- There can be versioning ID, if versioning ID is enabled 
## S3 Security

### User Based Policies

-  **IAM Policies** - User with the proper IAM Access to view S3

### Resource Based Policies

  **Bucket Policy** - bucket wise access from the s3 console - allow cross account
  **Object Access Control List** - An **object ACL** is an access control list specifically for an individual S3 object
  **Bucket Access Control List** - A **bucket ACL** is an access control list that defines who can access the bucket itself and what actions they can perform (like listing objects in the bucket).


##### Key Difference: **Bucket Policy vs ACL**

- **Bucket Policy:** More flexible, supports conditions, written in JSON, and applies to both the bucket and objects.
- **ACL:** More basic, doesn’t support conditions, applies directly to individual objects or buckets


> Generally S3 Bucket Policy contains Principal Field, using this you can differentiate from IAM Json Policy which does not contain Principal Field 


##### Usage of S3 Bucket Policy
 - When you want to provide the cross AWS account access
 - When you want to from objects to be encrypted at upload
 - When you want to give public access to bucket

> • For Protecting Company Data Leak, AWS provide one more layer for blocking Public Access
> • This can be set at the account level

