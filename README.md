# terraform-EKS
Creating a EKS cluster using Terraform

Terraform scripts to Provision AWS EKS

Steps to be followed:

1.	Create an IAM (Identity Access Management) user in AWS and add user to the user_group
•	Sign in into AWS console with your crendentials
•	IAM -> Add user -> name -> add to Group -> add tags -> ok and save.
•	After adding user ,Download new_user_credentials.csv file .
•	Go to the file location and copy the credentials
•	Open the terminal

$ cd Downloads/
$ aws configure --profile <profile name>
$ AWS Access Key ID : <paste from the csv file>
$ AWS Secret  Access Key: <paste from the csv file>
$ Default region name: us-east-1
$ Default output format: json

 

2.	Create the following Terraform Scripts:

•	provider.tf
•	vpc.tf
•	internet-gateway.tf
•	subnets.tf
•	eips.tf
•	nat-gateways,tf
•	route-tables.tf
•	route-table-association.tf
•	eks.tf
•	eks-nodegroup.tf

3.	Please find below url of my Github Repository for the Source code , where you can find all the Terraform Scripts as mentioned above.

https://github.com/akshaykumart/terraform-EKS.git

4.	Go to the Terminal :

•	$ cd Terraform                             //Location where your Terraform files are located in local
•	$ terraform version                    //validate the terraform version
•	$ aws –version                            // Validate the AWS version
•	$ terraform init                          // Initialize the terraform Environment
•	$ terraform plan
•	$ terraform apply 

 
5.	Validations:

•	Login to AWS console and check whether the following things are created or not.

 
	Validate own VPC  created as per the Terraform script as shown above
 

	Validate IGW (Internet Gate Way) created as per the Terraform script as shown above
 
	Validate Subnets created as per the Terraform script as shown above.
 

	Validate Elastic IP’s created as per the Terraform Script as shown above.
 

	Validate NAT Gateways created as per the Terraform Script as shown above. 
 
	Validate the Routing Tables as per the Terraform script as shown above.

 

	Validate the EKS Cluster as per the Terraform Script as shown above.


                    



                  

