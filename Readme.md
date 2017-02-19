# DevOps Prototype enviornment on AWS 

Terraform (TF), provides the ability  to write a template for an environment, perform a dry run to see what is going  to happen and whether it is expected, deploy the template, and make  adjustments where necessary without leaving the shell prompt   

  
Terraform script uses IaC (Infrastructure as a code) approach to build the infrastructure components required have the Devops enviornment.Enviornment build can be automated by using the terraform file components 


This module provides the terraform scripts  to build the base DevOps Prototype enviornment on AWS 

Components Build after runnung this script 

1) VPC 
2) Subnets 
3) Security Groups
4) Autoscaling group 
5) IAM Policiies   
6) ELB 
7) Jenkins EC2 Instance 
8) Sync with  Code commit respoitary to get Saltstack components 
 

 

