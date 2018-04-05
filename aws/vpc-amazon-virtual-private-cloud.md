## Virtual Private Cloud

#### Virtual Private Cloud Overview
* __Logically isolated network__ in the AWS cloud:  simplify it and think of a VPC as the first/biggest/master/primary subnet. Use it to create smaller subnet, deploy resources/instances and configure env and everything.

* __Control of network architecture__: divide VPC into smaller subnet for different purposes such as IP Address/DMZ/Web/DB

* __Enhanced security__: have access to security group for recourses, have access to NACLs(network access control list) to be able to filter down and control what's coming in/going out (SSH/HTTP/HTTPS/UDP and etc..)

* __Internetwork with other organizations__: Use VPC peering to connect different VPC and control other VPCs.

* __Elastic IP Address__: Public IP Address.
* __Enable hybrid cloud__ (site-to-site VPN)
* __Single tenant dedicated server handware__
* __VPC is free__
* __Region Wide__
#### VPC Infrastructure / Reference Architecture
![](/assets/AWS_VPC architech.png)

---

* [Pluralsight course link](https://app.pluralsight.com/player?course=aws-certified-solutions-architect-associate&author=elias-khnaser&name=aws-certified-solutions-architect-associate-m2&clip=1&mode=live&start=7.746127&noteid=8c787a8d-f92f-46f2-a14b-dd2113da410a)

