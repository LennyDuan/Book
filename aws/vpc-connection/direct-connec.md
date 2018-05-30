## AWS Direct Connect

#### Benefits
1. Predictable bandwidth
2. Predictable performance/consistent network experience
3. 1 Gbps or 10 Gbps, multiple port
4. Less than 1GBps thourgh AWS Partner Network(APN)
5. Support for VLAN Trunking (802.1Q)
6. Direct Connect can be partitioned Into Multiple virtual interfaces(VIFS)
![](/assets/Direct Connect Benefit.png)

#### Diagram
Depending on how far your corporate data center is from nearest AWS region or from the nearest AWS Edge router, that will determine the speed that you're going to get to AWS. The closer you are to an Edge router or to a region, the better performance, lower latency. ![](/assets/AWS DC Diagram.png)

#####Colo will/can have direct connect with AWS
![](/assets/AWS DC Diagram 2.png)

##### P.S. Default direct connect doest not come with, it is not redundant.

Direct Connect: Now, AWS best practive will dictate that you have redundancy with AWS that you need 2 ports on two seperate routers on AWS side and do the same thing on your corporate Datacenter side as well.