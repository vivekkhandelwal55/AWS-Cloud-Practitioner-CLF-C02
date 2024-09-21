An ELB (Elastic Load Balancer) is a managed load balancer

	• AWS guarantees that it will be working
	
	• AWS takes care of upgrades, maintenance, high availability
	
	• AWS provides only a few configuration knobs

- It costs less to setup your own load balancer but it will be a lot more

 - effort on your end (maintenance, integrations)

4 kinds of load balancers offered by AWS:

	• Application Load Balancer (HTTP / HTTPS only) – Layer 7
	
	• Network Load Balancer (ultra-high performance, allows for TCP) – Layer 4
	
	• Gateway Load Balancer – Layer 3
	
	• Classic Load Balancer (retired in 2023) – Layer 4 & 7


## Application Load Balancer - 

- when you want to add load balancer at layer 7(Application Layer)
- it provides http routing features
- it provides static dns url
- it is comparatively slow load balancer as it dealing with http routing

## Network Load Balancer - 

 - it provides load balancing at layer 4 which is at TCP/UDP
 - it is useful in case of usage like streaming platforms, gaming servers
 - it is highly performant - millions of request per second

## Gateway Load Balancer - 
- it is used when you want to route traffic to firewall that you manage on EC2 instance
- Intrusion detection
- GENEVE Protocol on layer 3
