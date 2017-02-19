# DevOps Prototype on AWS 

Build the DevOps Base enviornment - IaC (Infrastructure as Code) Approach using Terraform ,Packer and serverspec utilities

AWS components: 
   VPC 
   Subnets 
   Security Groups 
   IAM Policies 
   ELB 
   Auto scaling Groups 
   
 Jenkins deployed on AWS instance as CI server 
 
Masterless Saltstack deployed -IaC

Packer and serverspec used to Validate the the Server Image Spec and build the AMI

Jenkins Pipeline:
1) Automated Jenkin pipleline to Build and test the app , copy the app build RPM's  to Yum repo and S3 Bucket.
2) Trigger the downstream job by passing the application version as parameter to build the AMI , test the image by creating the Instance.
3) Trigger second downstream job to deploy the instance and app.Attach ELB to Autoscaling group first and deploy the instance to the ELB. Deployment is triggered using Green blue approach to avoid downtime in production enviornments.
