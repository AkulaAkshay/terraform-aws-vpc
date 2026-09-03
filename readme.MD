# Terraform AWS vpc 

This module creates the following resources

* VPC
* IGW
* public subnets in us-east-1a and us-east-1b AZ
* private subnets in us-east-1a and us-east-1b AZ
* database subnets in us-east-1a and us-east-1b AZ
* Public Route table
* Private Route table
* Database Route table
* EIP for NAT
* NAT gateway in public subnet 1a AZ
* IGW route is added to public route table
* NAT gateway route to private and database route tables
* Route table association with subnets
* VPC to default VPC peering
* Public route table to default VPC route
* Default VPC main route table to created VPC route


### INPUTS

* vpc_cidr - (Required). User must supply the CIDR for VPC
* project_name - (Required). User must supply the project name.
* environment - (Required). User must supply the environment name....
