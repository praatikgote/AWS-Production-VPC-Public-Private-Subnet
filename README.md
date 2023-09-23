# AWS-Production-VPC-Public-Private-Subnet
Designing a High-Performance AWS VPC for Production: Public and Private Subnet Integration.


Project Title: 

AWS VPC with Public-Private Subnet for Production


Aim:

To create a VPC that is secure, scalable, and resilient, and that can be used to run production workloads.


Problem Statement:

Production workloads require a high level of security, scalability, and resilience. A traditional VPC with only public subnets is not secure enough for production workloads, as it exposes the instances directly to the public internet. A VPC with only private subnets is not scalable enough, as it requires all instances to use a NAT gateway to access the internet, which can be a bottleneck.


Solution:

The proposed solution is a VPC with public and private subnets in two Availability Zones. The public subnets will contain NAT gateways and load balancers. The servers will run in the private subnets and will be launched and terminated by using an Auto Scaling group. The servers will receive requests through the load balancer and can connect to the internet by using the NAT gateway.


Benefits:

This solution provides the following benefits:
Security: The servers are protected from the public internet by being placed in private subnets.
Scalability: The Auto Scaling group can scale the number of servers up or down as needed, without introducing any bottlenecks.
Resilience: The servers are deployed in two Availability Zones, so that if one Availability Zone goes down, the servers in the other Availability Zone can continue to serve requests.

Conclusion:

This solution provides a secure, scalable, and resilient VPC that can be used to run production workloads. It is based on best practices and is recommended by AWS.


Explanation:

The VPC will have four subnets: two public subnets in two Availability Zones, and two private subnets in two Availability Zones. Each public subnet will contain a NAT gateway and a load balancer node. The servers will run in the private subnets and will be launched and terminated by using an Auto Scaling group. The servers will receive requests through the load balancer and can connect to the internet by using the NAT gateway.

The route table for the public subnets will have a route to the internet gateway. The route table for the private subnets will have a route to the NAT gateway.

The security groups for the servers will restrict inbound traffic to only the ports and protocols that are required.


Project Architecture:

![image](https://github.com/praatikgote/AWS-Production-VPC-Public-Private-Subnet/assets/74818044/6a50be67-26af-41b6-967a-81aa3168e962)



Goal:

The goal of this project is to create a VPC that is secure, scalable, and resilient, and that can be used to run production workloads.

This project is a good starting point for anyone who is new to AWS VPCs, or who wants to learn more about how to set up a VPC for production workloads.


OutPut:
![p1](https://github.com/praatikgote/AWS-Production-VPC-Public-Private-Subnet/assets/74818044/90c75556-6622-4e53-9462-41230595bf6c)

![p2](https://github.com/praatikgote/AWS-Production-VPC-Public-Private-Subnet/assets/74818044/233f9ab8-4dde-4b6f-a0e3-2e466fe004ec)

![p3](https://github.com/praatikgote/AWS-Production-VPC-Public-Private-Subnet/assets/74818044/40afba5f-f07c-457e-8168-8039042ee5c0)


connect me:
Mail: pratikgote69@gmail.com

linkedin.com: https://www.linkedin.com/in/pratik-gote-516b361b3/

github.com: https://github.com/praatikgote


