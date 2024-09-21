Goal of ASG is to
 - Scale Out(Add Ec2) automatically to match the increase load
 - Scale in (remove Ec2) automatically to match the decreased load
 - we can have max and min no. of instances.
 - it can also automatically attach newly add instances to load balancer and can continuously monitor health issues
 - it is cost efficient, as we are using only the required no. of instance at point of time


## Strategies of ASG

- Manual Scaling - Update the size of ASG manually
- Dynamic Scaling
	- Simple/Step Scaling - 
		- We can use Cloud watch for tracking something like if CPU >70% for 5 minutes then add 2 Units
	- Target Tracking Scaling - 
		- i want the average of all cpu to stay around 40%
	- Scheduling Scaling - 
		- anticipate the scaling in advance like increase the min capacity to 5 on Friday nights
	- Predictive Scaling
		- it used machine learning algorithm to learn the traffic behaviour
		- it will provision new EC2 instance in advance
		- it will be helpful when you are having time based predictable traffic pattern 






> Note what is Cloud Watch