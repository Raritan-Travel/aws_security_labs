## Challenge 1
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
