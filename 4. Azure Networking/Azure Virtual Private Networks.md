A VPN uses an encrypted tunnel within another network. Used to connect two or more trusted private networks to one another over an untrusted network (like public internet). 
Traffic is encrypted while travelling. 
Enables network security.

**VPN Gateways** -

A type of Virtual network Gateway. Azure VPN Gateways instances are deployed in a dedicated subnet of the VNet and enable the following - 

- Connect on-premises datacenters to virtual networks through a site-to-site connection.
- Connect individual devices to virtual networks through a point-to-site connection.
- Connect virtual networks to other virtual networks through a network-to-network connection.
![[Pasted image 20260924234610.png]]


You can deploy only one VPN Gateway in each virtual network. 
You can use one gateway to connect to multiple locations, which includes other VNets or on-prem datacenters.

2 VPN gateway types - policy based and route based.
This needs to be specified when setting up gateway.
Regardless of type, method of authentication is a preshared key.

- Policy-based VPN gateways specify statically the IP address of packets that should be encrypted through each tunnel. This type of device evaluates every data packet against those sets of IP addresses to choose the tunnel through which that packet is sent.
- In route-based gateways, IPSec tunnels are modeled as a network interface or virtual tunnel interface. IP routing (either static routes or dynamic routing protocols) decides which one of these tunnel interfaces to use when sending each packet. Route-based VPNs are the preferred connection method for on-premises devices. They're more resilient to topology changes such as the creation of new subnets.

Use a route-based VPN gateway if you need any of the following types of connectivity:

- Connections between virtual networks
- Point-to-site connections
- Multisite connections
- Coexistence with an Azure ExpressRoute gateway

**Ways to maximize the resiliency of VPN Gateway** -

Active/Standby

By default, VPN Gateways are deployed as 2 instances. Active/Standby. When something disrupts the active instance, the standby instance starts working automatically. Connections are only interrupted for few seconds during planned maintenance, and 90 seconds are unplanned disruptions.

Active/Active

Using BGP routing protocol, you can deploy gateways in active/active config. You assign a unique public IP to each instance. 
Create separate tunnels from the on-prem devices to each IP.

ExpressRoute Failover

Configure a VPN Gateway as a secure failover for ExpressRoute connections. 

Zone Redundant Gateways 

For regions that support availability zones, VPN gateways and ExpressRoute gateways can be deployed in zone-redundant config. This protects from zone level failures. These gateways require different SKUs and use Standard public IP addresses instead of Basic public IP addresses