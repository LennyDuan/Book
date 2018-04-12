## VPC NAT Bottlenecks

#### NAT Instances bottlenecks
![](/assets/NAT Bottlenecks.png)

#### Sulution:
* Scale up: 
    * Increase instance size.
    * Choose instance that supports enhanced networking
* Scale out:
    * Add NAT intances/subnets and migrate workloads
    ###### One NAT instance - One subnet

Use __NAT Gateway__ instead: An AWS as-a-service
