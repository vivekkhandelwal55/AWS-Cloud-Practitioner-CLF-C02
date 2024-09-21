
#### Types of S3 Buckets

1. [x] S3 Standard
2. [x] S3 Storage Class - Infrequent Access
3. [x] S3 Storage Class - One Zone Infrequent Access
4. [x] S3 - Glacier Instant Retrieval
5. [x] S3 - Glacier Flexible Retrieval
6. [x] S3 - Glacier DeepArchive
7. [x] S3 - Intelligent Tiering

> **Note**: All Type of S3 Buckets have same durability which is 99.99....9(upto 11 9's)
> Availability Depends on Storage Class
##### 1. S3 Standard
 - Availability is 99.99%
 - Suitable for frequency accessed data
 - it provides low latency and high throughput
 - Sustain 2 Concurrent facility failures

##### 2. S3 Storage Class - Infrequent Access
 - Availability is 99.99%
 - Best suitable for data which has less access frequency and required instant access
 - it is obvious that is costs lower than s3 standard
 - **Use Cases** - disaster recovery and backups

##### 3. S3 Storage Class - One Zone Infrequent Access
- Availability is 99.5%
- High Durability in Single AZ, data is lost when AZ is destroyed
- **Use Cases** - Best suitable for secondary backups or the data you can recreate.

##### 4. S3 - Glacier Instant Retrieval
 - Accessing Speed is MilliSecond
 - Minimum storage duration is 90 days

##### 5. S3 - Glacier Flexible Retrieval
 - Accessing Speed is Minutes or Hours
 - Minimum Storage duration is 90 days

##### 6. S3 - Glacier Deep Archive
 - Minimum storage duration is 180 days
 - accessing speed is hours

##### 7. S3 - Intelligent Tiering

- No retrieval charges in this
- it will automatically move the file to tiers based on the last accessed

 _Frequent Access tier (automatic):_ default tier

• _Infrequent Access tier (automatic)_: objects not accessed for 30 days

• _Archive Instant Access tier (automatic):_ objects not accessed for 90 days

• _Archive Access tier (optional):_ configurable from 90 days to 700+ days

• _Deep Archive Access tier (optional):_ config. from 180 days to 700+ days
 


