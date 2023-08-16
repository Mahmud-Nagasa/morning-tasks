# Cloud Services

Decide whether the following AWS services are Infrastructure as a service (IaaS), Platform as a service (PaaS), Software as a service (SaaS), or Serverless and give your reasoning.

EC2
this server is considered a IaaS because it is basically just a device with an operation system and a power supply, and that's it it's up to the user to do the rest which gives an absolute control over the management of the server

S3
I would say that S3 is a PaaS since as the name indicate it is simple storage server, that used to store the data in storage containers called buckets, and PaaS are servers that provide a ready to use server without considering the underlying infrastructure.

RDS
is a server that allows working with many database engines such as postgreSQl or MYSQL which means it is also a PaaS since we only concerned about the database

Lambda
it is also known as function as a server, because it only has a small code to run when it is needed that being said since it's only triggered in certain events it is a serverless  

EKS
what I understood is that EKS is a Kubernetes provided by amazon to manage or organize the dockers (containers), however, EKS has two options either using Fargate which is a serverless or EC2 which is IaaS

DynamoDB
is like rds a PaaS. However, this one is NOSql database unlike rds that support SQL queries 

ECR
is used to store manage and deploy dockers but I am not sure if it is a IaaS or a PaaS