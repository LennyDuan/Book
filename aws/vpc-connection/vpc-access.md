## AWS VPC Access

How do access the VPC from __outside__ of the AWS. How do connect __on-premises__ environment to AWS VPC
 
#### VPN - Virtual Private Networking & Gateways
![](/assets/vpn_gateways.png)
* __Hardware-based VPN__: where you have a hardware appliance that you are installing on-premises that you are using to connect to an endpoint on AWS VPC.
* __Direct Connect__: Dedicated Private connection that you use where, your AWS will show up as another node as your WAN, or if you're going to  though colo.
* __VPN CloudHub__: is where you have several branches offices and figure out how to give these branch offices access to VPC (on-premises data center / directly to VPC)
* __Software VPN__: Where you can stand up an instance on AWS, turn that instance into the endpoint gateway and then through software just connect to if rom your on-premises enviroment
* __IGW__: Configure on AWS VPC side, this is useful to allow instances on VPC to get access to the internet 
* __VP Gateway__: Is used when you're configuring a __hard-ware based VPN__ to connect your on-premises data center to AWS or to your VPC. This is the endpoint that you configure on your VPC
* __CG__: the representation of what you do at the customer side in order to connect through a __hardware-based VPN__ to your __VP Gateway__

#### VPN Types
* __Common VPN__: It is an encrypted connection from the user's location to that remote access server.
* __Site-to-site VPN__: using internet and an encrypted connection, it's a site-to-site connection between your corporate office and branch. But it leveraging the internet as a mechanism, as the medium of transport and as a result you are encrypting.
* __Private connection__: typically don through a private connection, this could be an MPLS, a T1, T3 and whatever it can be.

---
* [Pluralsight course link](https://app.pluralsight.com/player?course=aws-certified-solutions-architect-associate&author=elias-khnaser&name=aws-certified-solutions-architect-associate-m4&clip=3&mode=live)

