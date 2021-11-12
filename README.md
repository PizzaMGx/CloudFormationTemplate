# CloudFormationTemplate
Cloud formation template to host a webserver

The Networking stack works well as well as the security groups stack and the networkACL 
The AMI ID for the private EC2 instante hosting the web server is: ami-01f5068f17cc178b9

The order to create the stacks is:
1- Network
2- Security Groups
3- ALB

The Security Groups Stack require to call the Network
The ALB Stack requires to call the Network and Security Groups

1Error:(Does'nt let me SSH to the Host EC2)
