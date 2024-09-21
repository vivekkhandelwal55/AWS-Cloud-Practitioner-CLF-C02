 - As we know that EBS Volumes are network drives  due to which they are not very performant
 - but EBS Instance Store is physical storage device attached to the EC2 instance due to this it has very high I/O speed

**Note:**  EBS Instance Store loses data if they are stopped.
 - it is our responsibility to take backups and replications
 - it is not ideal for critical data, it can be used for temp data or cache data
- Risk of losing data if hardware fails

#### Point to be Keep in Mind : They have very good Read and Write Speed due to physical attachment to the instance
