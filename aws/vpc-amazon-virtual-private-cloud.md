## Virtual Private Cloud

#### Virtual Private Cloud Overview
* __Logically isolated network__ in the AWS cloud:  simplify it and think of a VPC as the first/biggest/master/primary subnet. Use it to create smaller subnet, deploy resources/instances and configure env and everything.

* __Control of network architecture__: divide VPC into smaller subnet for different purposes such as IP Address/DMZ/Web/DB

* __Enhanced security__: have access to security group for recourses, have access to NACLs(network access control list) to be able to filter down and control what's coming in/going out (SSH/HTTP/HTTPS/UDP and etc..)