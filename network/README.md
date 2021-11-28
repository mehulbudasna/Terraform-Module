# NETWORK
- In this module we are createing  **VPC*, **public_subnet** and **private_subnet**
- For change the cidr block open variable.tf
- In network module we are creating 3 public and 3 private subnet in the mumbai region
- If you want to change the region than please change [here](https://github.com/mehulbudasna/Terraform-Module/blob/master/provider.tf) and change [availability zone](https://github.com/mehulbudasna/Terraform-Module/blob/master/network/variable.tf)
## How to create resource , please check this file
- [VPC](https://github.com/mehulbudasna/Terraform-Module/blob/master/network/vpc.tf)
- [Internet Gateway](https://github.com/mehulbudasna/Terraform-Module/blob/master/network/ig.tf)
- [Nat Gateway](https://github.com/mehulbudasna/Terraform-Module/blob/master/network/netig.tf)
- [Subnet](https://github.com/mehulbudasna/Terraform-Module/blob/master/network/subnet.tf)
- [route_table](https://github.com/mehulbudasna/Terraform-Module/blob/master/network/routetable.tf)
