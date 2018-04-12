## VPC NAT Bottlenecks

#### NAT Instances bottlenecks
![](/assets/NAT Bottlenecks.png)

#### Sulution:
* Scale up: 
    * Increase instance size.
    * Choose instance that supports enhanced networking
* Scale out:
    * Add NAT intances/subnets and migrate workloads (E.g: one 40%, one 35% and the last one 25%.)
    
###### Notice:
* One NAT instance - One subnet
* Subnet failover to another NAT is supported


#### BUT
If possible, Use __NAT Gateway__ instead: An AWS as-a-service
