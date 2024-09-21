
 - Network Drive you can attach to any ec2 instance
	 - it uses network to communicate the drive and intsance, so there will be some latency
	 - it can be detached from one instance and can be attached to another easily
 - it is specific for availability zones
	 - they are bound to AZ
	 - if you want to move it, you have to take snapshot
 - at a time EBS can only connect to one instance only

### Delete on termination behaviour

Controls the EBS behaviour when an EC2 instance terminates

• By default, the root EBS volume is deleted (attribute enabled)

• By default, any other attached EBS volume is not deleted (attribute disabled)



## EBS Volume Snapshot
 - Make a backup of EBS Volume at any point of time
 - it is not necessary to de attach EBS Volume to do snapshot, but it is recommended
 - it helps copy Volume Snapshot in on AZ to another

###  EBS Volume Snapshot Archive
 - move the snapshot to archive tier as it is 75% cheaper
 - it takes 24 to 72 hours for restoring this archive

### EBS Recycle Bin
 - you can configure retain policy from recycle bin from 1 day to 1 year
 - helps to retain the accidentally deleted snapshot
