# Terraform

1. What is infrastructure as code (IaC) and why is it important in modern IT operations? What are the advantages?

IaC is using machine readable files to configure and manage data centers instead of manually setting them, and that's basically the main reason why everyone is using it nowadays, it's faster easier efficient and more flexible, it wouldn't make sense to choose to do everything manually and disregard this method.

using IaC has many advantages such as reusability, it is possible to reuse a file over and over which will reduce time and effort increase security consistency and agility 


2. Explain the concept of "Infrastructure as Code" (IaC) and how Terraform fits into this concept.

the whole idea behind it is typing what I want in my cloud infrastructure, upload the file and everything will be set for you, no need to navigate through the console and do each step separately. Terraform is an open source declarative tool, and the best part is that it support up to 120 provider, so unlike other tools such as AWS cloudFormation that can only be used for aws services terraform can be utilised on Azure googleCloud and many others. it  also uses it's own file format which HCL 


3. What problems do modules help address, and how do they promote reusability?

form what I understand, modules are ready to use files published by others, these modules can be for anything VPCs, instances, pretty much everything. but one needs to be carful to go through what author of the module wrote to understand what the module will build and it also can be adjust it to our cloud needs form the input section
of course we can also create our own module which prompts reusability

4. Explain in your own words what the following commands achieve;

- `terraform init`

initialise a Terraform working directory and sets up the environment for Terraform to manage the infrastructure.as mentioned before terraform can be used by a hugh number of providers, what init do is checking the resource type and download the required plugins and cache them locally to know how to talk to this provider 

- `terraform plan`

plan simply checks the file and tells you what is the 'plan' or what terraform will be creating in you cloud

- `terraform apply`

 this is the next step after plan, simply execute the plan and make the infrastructure in the cloud 


- `terraform destroy`

destroy looks like a scary word, and in this case it is it simply remove the infrastructure made by terraform in the specific directory 

- `terraform fmt`
is a command used as good practice to format the configuration files which helps code readability and ensures all configuration files are formatted the same

- `terraform output`

is a useful tool, it is basically like console.log form java script that let you see the specific pieces after the creation of the infrastructure

- `terraform taint`

this command basically mark a specific resource as damaged and on the next apply terraform will replace it, there is a new command which is terraform replace


