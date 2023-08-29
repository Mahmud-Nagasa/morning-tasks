# Terraform project warm up

1. Imagine you need to make changes to the configuration of an existing AWS EC2 instance that's being managed by Terraform. How might you go about making those changes while minimizing disruption to your production environment? of course any instance or serveries managed by terraform should only be changed using terraform. However, regarding minimizing disruption I would create an new ec2 with the configuration of the current one adjust the load balancer to start sending request to the new instance, after that I would start applying changes on the targeted instance

2. In your own words, what is a module in Terraform?
a module is a terraform file created and published by someone that enable others to make changes and reuse it in their own infrastructure.

3. What are some advantages of using modules in your Terraform code?
by reducing the time to create every last bit by just reusing a module, breaking the infrastructure to smaller more manageable codes that can be reused across multiple projects to enable consistency 

4. What are some instances that you might use an output block?
since the output block enable us to  see information about the infrastructure such as IDs,IPs or DNS. it is useful for sharing information with team members  and make it easy to access 

5. How can you pass arguments to a module? What steps do you need to take to add an argument?
I would first check the input variable provided by the publisher, then declare the variable and the value of the variable based on it's data type and the requirement of my infrastructure/
Edit: form the lecture I now understand that we add the arguments using a variable and vartf files tp add arguments to our module 

6. Imagine you're creating a Terraform module to deploy an AWS VPC. What are some variables you might define for this module to make it adaptable for different environments?

I would consider the following:

region
Cider range,
private and public subnets IPs,
enable or disable Igw, and NAT gw,

these are the main inputs I would focus on but of course there are a lot of inputs that can be added to the VPC module
