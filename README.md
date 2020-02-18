**This Cloud Formation Template will create an EC2 Instance & RDS Instance along with its security groups, User Data Ansible Script will help in installing and configuring JIRA**


---

## AWS Setup

You’ll start by editing this README file to learn how to edit a file in Bitbucket.

1. Export both AWS Access Key and Secret Key. example: export AWS_ACCESS_KEY_ID="AAAAAAAAAAA"; export AWS_SECRET_ACCESS_KEY="XXXX"
2. Update the parameters inside the ec2_rds.json file.
3. aws cloudformation create-stack --stack-name jirastack --template-body file://ec2_rds.json
4. aws cloudformation delete-stack --stack-name jirastack
---