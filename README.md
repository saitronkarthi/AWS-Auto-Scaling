# AWS-Auto-Scaling
1. Create Amazon Machine Image(AMI) on the instance you want to autoscale
2. Create Load balancer to have a common url for all the instances
3. Create Launch Configuration
4. Create Autoscalling group
5. Create scaling poliicies for scaling up(Cloud alarm -Network in >=10000), Scaling down(when CPU utilization <10%)
6. Configure Apache Jmeter test plan to simulate 100 users.
7 An instance is spun automatically when 100 users are simulated.
8.When the simulation stops there is an auto scaledown of instance when the cpu utilization reduces.
To protect an AMI from being terminated during scale down enable scale in protection on the instances in Autoscaling
