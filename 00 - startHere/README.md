This is for brand new analysts to AWS. This will provide a basic overview of what's needed to complete the rest of these challenges

# Starter Challenges
## Challenge One 
**Create a public webserver that serves content to the public. Also, you will need to create a Bastion Host server to administer the web server.**

## Pre-Reqs
- Create a public key to authenticate to the ec2 instances - name the key `mayas-keypair`. Save the keypair.
- Create a security group that allows access to the bastion host. Name the security group: `bastion host sg`
  - Create a rule that allows ssh from `My-IP` 
- Create a security group that allows access to the public server. Name the security group: `web server sg`
  - Create a rule that only allows ssh access from the `bastion host sg`
  - Create a rule that allows http/https from everywhere
- Click the CloudFormation template below to provision the infrastructure required.

[CloudFormation Template](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?templateURL=https://aws-security-labs.s3.amazonaws.com/ec2-template.yml&stackName=starter-pack-00)
