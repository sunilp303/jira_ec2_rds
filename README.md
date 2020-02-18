**This Cloud Formation Template will create an EC2 Instance & RDS Instance along with its security groups, User Data Ansible Script will help in installing and configuring JIRA**


---

## AWS Setup

1. Export both AWS Access Key and Secret Key. example: export AWS_ACCESS_KEY_ID="AAAAAAAAAAA"; export AWS_SECRET_ACCESS_KEY="XXXX"
2. Update the parameters inside the ec2_rds.json file.
3. Updated values which are used inside default needs to passed through an argument "-e key=value"
	 Reference link for the defaults: https://bitbucket.org/sunil_pothireddy/jira-ansible/src/master/roles/jira/defaults/main.yml
4. ``` aws cloudformation create-stack --stack-name jirastack --template-body file://ec2_rds.json --parameters ParameterKey=KeyName,ParameterValue=KEYNAME ```
5. ``` aws cloudformation delete-stack --stack-name jirastack ```
---
