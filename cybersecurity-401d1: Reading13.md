Mario Pugh		October 21, 2020

Intro to AWS VPC

 A VPC (virtual private cloud) is a virtual data center in the cloud. You have complete control over your virtual networking environment, including a selection of your own private IP address range, creation of subnets and configuration of route tables and network gateways. The benefit of VPC is that it helps in aspects of cloud computing like privacy, security and preventing loss of proprietary data.

The basics of a VPC
Subnets: A subnet can be thought of as dividing a large network into smaller networks. This is done because the maintenance of smaller networks is easier and it also provides security to the network from other networks.
Route Tables: A route table contains a set of rules called routes which determine where traffic has to be directed. You can have multiple route tables in a VPC.
Internet Gateways (IGW): It is a combination of hardware and software that provides your private networks with a route to the world outside. An IGW is a horizontally scaled, redundant and highly available VPC component that allows communication between instances and the internet. Only one IGW can be attached to a VPC at a time.
Network Address Translation (NAT): Since subnet is private, the IP addresses assigned to the instances cannot be used in public. NAT maps the private IP addresses to the public address on the way out and vice versa on the way in. An Elastic IP address is a static, public IPv4 address designed for dynamic cloud computing. You can associate an Elastic IP address with any instance or network interface for any VPC in your account. With an Elastic IP address, you can mask the failure of an instance by rapidly remapping the address to another instance in your VPC.
Security groups: Security groups are a set of firewall rules that controls the traffic for your instance. In Amazon Firewall the only action that can be carried out is allow. You cannot create a rule to deny. The destination is always the instance on which the service security group is running. You can have a single security group associated with multiple instances.
Customer Gateway — An Amazon VPC VPN connection links your data center (or network) to your Amazon VPC (virtual private cloud). A customer gateway is the anchor on your side of that connection. It can be a physical or software appliance.
Virtual Private Gateway — A virtual private gateway is the VPN concentrator on the Amazon side of the VPN connection. You create a virtual private gateway and attach it to the VPC from which you want to create the VPN connection.
VPN stands for ‘virtual private networking’, which is a popular internet security method which was originally designed for large organisations where employees needed to connect to a certain computer from different locations.
VPC Peering — A VPC peering connection allows you to route traffic between two VPC’s using IPv4 or IPv6 private addresses. Instances in either VPC can communicate with each other as if they are within the same network. You can create a VPC peering connection between your own VPCs, or with a VPC in another AWS account. A VPC peering connection helps you to facilitate the transfer of data.
Network Access Control Lists (NACL)— an optional layer of security for your VPC that acts as a firewall for controlling traffic in and out of one or more subnets. You might set up network ACLs with rules similar to your security groups in order to add an additional layer of security to your VPC. The default network ACL is configured to allow all traffic to flow in and out of the subnets to which it is associated.

The following are the key concepts for VPCs:
Virtual private cloud (VPC) — A virtual network dedicated to your AWS account. 
Subnet — A range of IP addresses in your VPC. 
Route table — A set of rules, called routes, that are used to determine where network traffic is directed. 
Internet gateway — A gateway that you attach to your VPC to enable communication between resources in your VPC and the internet.
VPC endpoint — Enables you to privately connect your VPC to supported AWS services and VPC endpoint services powered by PrivateLink without requiring an internet gateway, NAT device, VPN connection, or AWS Direct Connect connection. Instances in your VPC do not require public IP addresses to communicate with resources in the service. Traffic between your VPC and the other service does not leave the Amazon network. 

References:
https://medium.com/tensult/intro-to-vpc-548b69f1bd1f

https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html
