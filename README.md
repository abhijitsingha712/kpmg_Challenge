# kpmg_Challenge

Terraform WordPress deployment
Description:
This TF script will deploy a single region highly available WordPress site with RDS, EC2 and VPC.

#Before you begin: Create SSH Key-Pairs
ssh-keygen -f -t rsa -b 2048 Two files will be created:

no suffix file - the private key
.pub suffix - the public key. This is the file you pass in tfvars

#Before running
Along with your API credentials, ensure you specify the AMI ID in your .tfvars file. A sample has been created to reference. 
Please use a cloud-ready Ubuntu Xenial image. For list of official AMI's see: https://cloud-images.ubuntu.com/locator/ec2/.

#Networks to be provisioned:
1 VPC
2 Database subnets
1 Web subnets
2 public subnets

#Resources:
1 NLB
2 web servers (or more) (Ubuntu Xenial)
1 RDS instance (MySQL 5.7)
