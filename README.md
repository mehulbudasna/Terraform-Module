# Terraform-Module snippet for deploying ASG in private subnet behind ALB 

Below is the architecture to be implemented:

![mehul (1)](https://user-images.githubusercontent.com/21075788/143733148-110023d5-792d-45ed-87ea-7eda1aacc488.png)

# Prerequisites:
1. AWS account
2. IAM role with necessary permissions
3. Terraform (Version : 0.12) & AWS CLI configured on machine from which the scripts are to be run 


# Modules included are:

In script we are use two module use
- First module is network : for more understand please follow this [link](https://github.com/mehulbudasna/Terraform-Module/blob/master/network/README.md)
- Second module is ec2 : for more understand please follow this [link](https://github.com/mehulbudasna/Terraform-Module/blob/master/ec2/README.md)

# Follow Below Steps to RUN Terraform snippet

1. Create folder and Clone this repo.
2. Change required variable value
3. Initialize terraform using 
```bash
terraform init
```
4. Show changes required by the current configuration 
```bash
terraform plan
```
5. Create or update infrastructure 
```bash
terraform apply
```
Your infra is ready to use now.

6. Destroy previously-created infrastructure 
```bash
terraform destroy
```
