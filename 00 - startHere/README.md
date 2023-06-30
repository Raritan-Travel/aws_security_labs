This is for brand new analysts to AWS. This will provide a basic overview of what's needed to complete the rest of these challenges

# Starter Challenges
## Challenge One 
**Create a webserver that serves content to the public.**

## Pre-Reqs
- Create a public key to authenticate to the ec2 instances - name the key `mayas-keypair`. Save the keypair.
- Create a security group that allows access to the public server. Name the security group: `web server sg`
  - Create a rule that only allows ssh access from the `my-ip`
  - Create a rule that allows http/https from everywhere
- Click the CloudFormation template below to provision the infrastructure required.

[CloudFormation Template](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?templateURL=https://aws-security-labs.s3.amazonaws.com/ec2_start.yaml&stackName=starter-pack-00)
