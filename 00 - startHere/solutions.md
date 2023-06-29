## Challenge 1
- Create an ec2 Instance using the supplied VPC 
    - Create 1 Ubuntu Linux Instance in the public subnet
        - Name the server `Maya's Web Server`
        - Use the `mayas-keypair` that you created earlier
        - Add the ec2 instance to the public subnet provided
        - Add the `web server sg` to the ec2 instance that we created earlier
        - SSH into the ec2 instance via powershell or unix cli
        - Run the commands listed below
        - Clone the following code: https://github.com/Raritan-Travel/aws_security_labs.git

    - Create 1 Red Hat Linux Instance in the private subnet
        - Name the server `Maya's Bastion Host`
        - Use the `mayas-keypair` that you created earlier
        - Add the ec2 instance to the private subnet provided
        - Add the `bastion host sg` to the ec2 instance that we created earlier
     
    ### Commands
    ```## web server script

    ## installs web server
    > sudo apt install apache2 -y 
    
    ## clones repo for web server
    > git clone https://github.com/Raritan-Travel/aws_security_labs.git
    > git checkout "startHere"
    
    ## moves into the home directory
    > cd $HOME
    > cd aws_security_labs/00 - startHere/webServerFiles
    
    ## copies files into the http directory
    > sudo cp webServerFiles/* /var/www/html
    
    ## start webserver and enables auto-restart
    > sudo systemctl start apache2 
    > sudo systemctl enable apache2```
