This is for brand new analysts to AWS. This will provide a basic overview of what's needed to complete the rest of these challenges

# Starter Challenges

- Create an ec2 Instance using the supplied VPC 
    - Create 1 Ubuntu Linux Instance in the public subnet
        - Clone the following code: {INSERT CODE HERE} 
        - Name the server "Maya's First Web Server"
    - Create 1 Red Hat Linux Instance in the private subnet
        - Name the server "Maya's First Bastion Host"

- Create a VPC named "Maya's VPC"
    - Create a public subnet called "Maya's public subnet" 
        - create a web server named "Maya's web server" 
    - Create a private subnet called  "Maya's private subnet" 
        - create an ec2 instance in this subnet called "Maya's Bastion Host" 


## Pre-Reqs
- Create a public key to authenticate to the ec2 instances
- Create a security group that allows access to the public server
- Create a security group that allows access to the bastion host
