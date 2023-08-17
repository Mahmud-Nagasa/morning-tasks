# NAT, routes, Internet Gateway

Answer the following questions

1. What do you think the purpose of an internet gateway is? What would we not be able to do without one?
the internet gateway simply links the subnet or the local network to the internet, without one the network will be isolated and no one including  us can have access to it

2. Thinking back to a previous session, where do you think you might be using a NAT gateway right now?
the best place to use it in a public subnet and direct the private subnet to that NAT gateway to have an indirect access to the internet through the public subnet that have a direct access to the internet through the internet gateway Igw

3. What IP addresses will be matched by the CIDR block of `0.0.0.0/0`?
All IP address matches this CIDR block
   - for bonus points, explain why?
   because all the bites are included starting from 0.0.0.0 up to 255.255.255.255
   if for example the CIDR block was 192.168.0.0/16 that the IPs that start with 192.168 will match, and if it was 192.168.0.0/24 that means the IPs that start with 192.168.0 will match. 

4. In your own words, what is the difference between a NAT gateway and an Internet Gateway? When would you want one over the other?
the NAT gateway inside a public subnet have access to the internet, hence it has a public IP address the NAT therefore forward the traffic to the instances in the private subnet. while the igw is needed when we want to connect a subnet to the internet, which in this case a public subnet.
While the public subnets connected to the igw through a route table
the private subnets are also connected to the NAT gateway through a route table 