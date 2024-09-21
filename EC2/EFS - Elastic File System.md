 - it is a managed network file system which can be mounted on 100s of Ec2
 - unlike EBS which has one to one relationship, it can have one to many relationship
- it works with linux EC2 Instance and it is multi AZ
- Note: - it is highly available and 3x more expensive than EBS, pricing will be calculated on per use, no capacity planning


## EBS vs EFS
![[Pasted image 20240919103711.png]]


## EFS - IA ( EFS - Infrequent Access)

 - storage class which is optimised for files which is not accessed every day.
 - you can enable EFS and it will automatically move files which are not accessed over a period of time(which can be defined through Lifecycle Policy)
 - in usage or dev, there is no difference
 - it is cost saving, upto 92% on EFS Pricing