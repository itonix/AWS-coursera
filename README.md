![net](https://github.com/user-attachments/assets/13b841ed-bcef-4033-af01-0c3f0c944800)


When you create a VPC, you need to choose three main things. 

    The name of your VPC.

    A Region for your VPC to live in. Each VPC spans multiple Availability Zones within the Region you choose.

    A IP range for your VPC in CIDR notation. This determines the size of your network. Each VPC can have up to four /16 IP ranges.

 When you create a subnet, you need to choose three settings.

    The VPC you want your subnet to live in, in this case VPC (10.0.0.0/16).

    The Availability Zone you want your subnet to live in, in this case AZ1.

    A CIDR block for your subnet, which must be a subset of the VPC CIDR block, in this case 10.0.0.0/24.

  ![image](https://github.com/user-attachments/assets/fc6fe835-6e55-4730-b672-6f7b958bb393)

Gateways

Internet Gateway 

To enable internet connectivity for your VPC, you need to create an internet gateway. After you create an internet gateway, you then need to attach it to your VPC.  

Virtual Private Gateway  

A virtual private gateway allows you to connect your AWS VPC to another private network. Once you create and attach a VGW to a VPC, the gateway acts as anchor on the AWS side of the connection. On the other side of the connection, you’ll need to connect a customer gateway to the other private network. A customer gateway device is a physical device or software application on your side of the connection. Once you have both gateways, you can then establish an encrypted VPN connection between the two sides. 


