NULL_PROVIDER & NULL_RESOURCE

SOURCE -  Terraform Registry. 

This kind of provider has a special task - triggering another proccess without creating any resource ot a process. And not only the providers can be null in terraform and the cloud environment. More information about null_providers can be found in the official documentation, and Terraform Registry. To demonstrate what exactly this provider can do, it used another block with "null_resource" in the configuration. Mein task ot this configuration is to generate ids in the state file, but no real resources are deployed in any vendor like AWS, Azure ect. 

REQUIREMENTS:

Terraform installed localy.

FILES IN THE REPO
1. main.tf - this file contains the configuration for the resources  
4. README.md
5. .gitignore 

TESTING
Commands for testing the null_provider block:
    terraform init - after using this command the required plugins are installed.
    terraform validate - via this command we are validating that the configuration has no syntactical problems and will not produce an error.
    terraform plan - with this command terraform is making plan before applying the configuration. The plan could be stored in a file (terraform plan -out <FILE>) and could be executed latter. 
    terraform apply - this command is doing the main action - to deploy the given infrastructure anywere. In this case in the main.tf file there are no real resources to be deployed in a cloud. During the creation process terraform creates one tfstate file as a source ot truth for the deployed infrastructure. 
    terraform destroy - the command destroys everything that was deployed by the previous command. This means that the infrastructure will not be available. 
