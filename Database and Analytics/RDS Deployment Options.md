
# RDS Deployment Options


## Read Replicas
- you create multiple replicas to only read the database
- write operations happens on the main db
- it can only create replicas upto 15db
![[Pasted image 20240921105953.png]]

## Multi AZ
 - we create a fail over database in another AZ, which will be used when main db has some problem
 - can only have 1 other AZ as failover
![[Pasted image 20240921110026.png]]

## Multi Region
- you create replicas of database in other regions as secondary database
- secondary database will be used as read only, which will reduce latency in reading
- writing will happen only on the main db
- as there is replication, you have to bear replication cost also

![[Pasted image 20240921110218.png]]
