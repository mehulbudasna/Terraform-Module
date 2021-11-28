## EC2
### In EC2 module we are creating EC2 services 

### Instance
- Instance will be in private subnet
- We are using **amazon linux**,latest ami we are use [data source](https://github.com/mehulbudasna/Terraform-Module/blob/8c0e4c04ef154db2ebf1645e6f27e34c5cffd09b/ec2/main.tf#L1)
- We are using **aws_launch_configuration** for creating ec2 instance 
- To change instance type change [here](https://github.com/mehulbudasna/Terraform-Module/blob/8c0e4c04ef154db2ebf1645e6f27e34c5cffd09b/ec2/variable.tf#L9)

## Loadbalancer
- We are creating loadbalancerr in public subnet using terraform resource [aws_lb](https://github.com/mehulbudasna/Terraform-Module/blob/8c0e4c04ef154db2ebf1645e6f27e34c5cffd09b/ec2/main.tf#L62) 
 and attaching targate group to loadbalancer using terraform resource [aws_lb_target_group](https://github.com/mehulbudasna/Terraform-Module/blob/8c0e4c04ef154db2ebf1645e6f27e34c5cffd09b/ec2/main.tf#L77)
## Autoscaling 

-  We are createing autoscaling using terraform resouce  [aws_autoscaling_group](https://github.com/mehulbudasna/Terraform-Module/blob/8c0e4c04ef154db2ebf1645e6f27e34c5cffd09b/ec2/main.tf#L102) 
- For attaching our autoscaling group to application load balancer attachment we are using terraform resource [aws_autoscaling_attachment](https://github.com/mehulbudasna/Terraform-Module/blob/8c0e4c04ef154db2ebf1645e6f27e34c5cffd09b/ec2/autoscalling.tf#L29)

## Volume
- Secondery volume attached using terrafrom resource is [aws_launch_configuration](https://github.com/mehulbudasna/Terraform-Module/blob/8c0e4c04ef154db2ebf1645e6f27e34c5cffd09b/ec2/autoscalling.tf#L18) and mounting to instance with [user_data](https://github.com/mehulbudasna/Terraform-Module/blob/8c0e4c04ef154db2ebf1645e6f27e34c5cffd09b/ec2/autoscalling.tf#L14) script
