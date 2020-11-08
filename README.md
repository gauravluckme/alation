# Alation DevOps HomeWork Assignment steps for executing the template

--> The soultion will retuen the below:-

Curl of Load Balancer will  return a “Hello World” and the instance identifier id that is being served by one of the web servers.
Removal of either one web servers should automatically fail over to the other server. 

--> The template will create the following resources in the AWS:-
1. VPC
2. Subnets
3. EC2 Instances
4. Application Load Balancer
5. Target Groups

--> Below are the required steps for running the template:-
1. First create a key-pair in AWS account, as it will be required as parameter in the template.
2. Pass the key-pair name created in the Step 1.
Ex. aws cloudformation create-stack --stack-name alation-assignment-solution --template-body file://template_alation.yml --parameters SSHKeyName=KeyPairName
