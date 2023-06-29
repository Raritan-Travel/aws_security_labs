## Challenge 1
#### Create a keypair
- name it `web-server-key-pair`
- keypair type = RSA
- key file format = .pem

#### create a security group for the bastion host: 
- vpc  =  week 00 vpc 
- name = `bastion host sg` 
- create an inbound rule 
  - type = ssh
  - source = my ip 

#### create a security group for the webserver 
- vpc = week 00 vpc
- name = `webserver sg` 
- create an inbound rule(s)
  - type = ssh
  - source = my ip 

  - type = http
  - source = everywhere

  - type = https
  - source = everywhere

#### create the webserver ec2 instance 
- name = public webserver
- os = ubuntu 
- keypair = webserverkeypair
- network settings 
  - vpc = week 00 vpc
  - subnet = public subnet
  - security group = webserver sg 
  - click launch instance 

#### log into the webserver 

- open powershell terminal, change into the directory where you downloaded the keypair
- copy the ssh command in the ec2 connect information and hit enter
- type in yes
- run the commands located below 



     
    ### Commands
    ```## web server script

        ## installs web server 
        sudo apt install apache2 -y
        sudo systemctl start apache2  

        ## clones repo for web server
        git clone https://github.com/Raritan-Travel/aws_security_labs.git
        cd aws_security_labs && git checkout "startHere"
        
        ## verify that the webserver is running by visiting the public ip 
        
        ## copies files into the http directory
        cd '/home/ubuntu/aws_security_labs/00 - startHere'
        sudo cp webServerFiles/* /var/www/html```
