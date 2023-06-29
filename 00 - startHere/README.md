This is for brand new analysts to AWS. This will provide a basic overview of what's needed to complete the rest of these challenges

# Starter Challenges
## Challenge One 
**Create a public webserver that serves content to the public. Also, you will need to create a Bastion Host server to administer the web server.**
### Steps
- Create an ec2 Instance using the supplied VPC 
    - Create 1 Ubuntu Linux Instance in the public subnet
        - Name the server `Maya's Web Server`
        - Use the `mayas-keypair` that you created earlier
        - Add the ec2 instance to the public subnet provided
        - Add the `web server sg` to the ec2 instance that we created earlier
        - Clone the following code: {INSERT CODE HERE} 

    - Create 1 Red Hat Linux Instance in the private subnet
        - Name the server `Maya's Bastion Host`
        - Use the `mayas-keypair` that you created earlier
        - Add the ec2 instance to the private subnet provided
        - Add the `bastion host sg` to the ec2 instance that we created earlier

- Create a VPC named "Maya's VPC"
    - Create a public subnet called "Maya's public subnet" 
        - create a web server named "Maya's web server" 
    - Create a private subnet called  "Maya's private subnet" 
        - create an ec2 instance in this subnet called "Maya's Bastion Host" 


## Pre-Reqs
- Create a public key to authenticate to the ec2 instances
- Create a security group that allows access to the public server
- Create a security group that allows access to the bastion host

[CloudFormation Template](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?templateURL=https://aws-security-labs.s3.amazonaws.com/ec2-template.yml&stackName=starter-pack-00)
