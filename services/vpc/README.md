## Virtual Private Cloud


All AWS services are launched on top of VPC.


|  Template 	| Availability Zones  | Public Subnet	| Private Subnet  	|  Internet Gateway 	|   NAT Gateway	|   Security Groups	|   Elastic IP	|   	
|---	|---	|-- |---	|---	|---	|---	|---	|
|   vpc-2azs	| 2|   2	|   2	|   1	|   2	|   1	|   2 	|   	
|   vpc-3azs	| 3|   3	|   3	|   1	|  3 	|   1	|   3	|   	


*Notes*
* if **NATGateways** parameter is set to **False**, NAT Gateways and Elastic IPs are not launched.
* The default **Security Group** allows all incoming traffic to ports 22, 80 and 443

## Cost

VPC is free but NAT Gateways have a monthly [cost](https://aws.amazon.com/vpc/pricing/).


*Note* AWS pricing varies by Region
