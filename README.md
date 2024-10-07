This Project demonstrate how to create a VPC that you can use for servers in a production environment.

To improve resiliency, you deploy the servers in two availablity zones, by using an Auto Scaling group and an Application Load Balancer. For additonal security we deploy the servers in private subnet. The server receive request through the Load Balancer. The servers can connect to the internet using the NAT gateway.


![image](https://github.com/user-attachments/assets/a0fce6f7-69b5-47ea-b1bd-2dd00d6a74b4)




Overview
Here we create VPC having public subnets and private subnets in two Availability Zones.

Each public subnet contains a NAT gateway and a load balancer node.

The server run in the private subnets, they are launched and terminated using the Auto scaling group, and receive traffic from the load balancer.

The servers can connect to the internet by using the NAT gateway.


