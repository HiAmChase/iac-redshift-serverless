# iac-redshift-serverless

Infrastructure as Code (IaC) the Redshift Serverless with IAM Roles, Workgroup, Namespace,... and load data pipeline into it

## Getting Started

1. Create file `access_key.config` and add AWS ACCESS KEY and AWS SECRET ACCESS KEY. This file was hidden by `gitignore` because of confidentiality

```
# access_key.config
[AWS]
KEY=Your_aws_access_key
SECRET=Your_aws_secret_key
```

2. Now you can execute command in `redshift_serverless.ipynb`. You can also change variable in `warehouse.config` if you want. The step in scripts includes:
   - Create Security Group
   - Create IAM Roles
   - Create Namespace
   - Create Workgroup
   - Connect to Redshift and create table users
   - Remove all previously built services
