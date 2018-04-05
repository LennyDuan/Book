### VPC Characteristics

* AWS __reserves 5 IP address per subnet__ (first 4 of every subnet and last 1) for management purpose such as Gateway.
* User can create 3 types of subnets - Private/Publice/VPN subnets. 
* Subnets do not span AZs, subnets only for 1 AZ
* VPC have a single region multiple AZs architecture: 1 Region -> Multi-AZ. 
* CIDR 16-28. 
* Select IP Prefix.