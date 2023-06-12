NULL_PROVIDER

SOURCE -  Terraform Registry. 

This kind of provider has a special task - triggering another proccess without creating any resource ot a process. And not only the providers can be null in terraform and the cloud environment. More information about null_providers can be found in the official documentation, and Terraform Registry. 

REQUIREMENTS:

Terraform installed localy;
AWS account or subscription in another cloud provider;

FILES IN THE REPO
1. main.tf
2. variables.tf
3. outputs.tf
4. README.md
5. .gitignore 

TESTING
Commands for testing the null_provider block:
    terraform init
    terraform validate
    terraform plan
    terraform apply
    terraform destroy
