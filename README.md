# CloudFormationTemplate
Cloud formation template to host a webserver

The Networking stack works well as well as the security groups stack
The ALB stack has'nt been tested yet due to lack of the AWS Certification Manager's Certificate with the domain
(It should work), I've tried to do it with the creation of a single EC2 instance in the public subnet but it does'nt
give access due to a conflict with the Security Groups Stack wich is configured to work with an ALB

The order to create the stacks is:
1- Network
2- Security Groups
3- ALB

The Security Groups Stack require to call the Network
The ALB Stack requires to call the Network and Security Groups
