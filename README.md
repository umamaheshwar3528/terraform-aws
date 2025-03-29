Terraform AWS EC2 Instance Management
This Terraform project automates the provisioning and management of an AWS EC2 instance. It is designed to demonstrate the creation, modification, and destruction of an AWS EC2 instance using Terraform.

Prerequisites
Before you begin, ensure you have the following:

Terraform v1.x installed

AWS CLI configured with Administrator access

An AWS account with the necessary permissions to create and manage EC2 instances

Setup
Clone the Repository:

bash
Copy
git clone https://yourrepositoryurl.com
cd terraform-aws
Initialize Terraform:

Run terraform init to initialize the working directory containing Terraform configuration files.

bash
Copy
terraform init
Usage
Planning
Generate an execution plan for Terraform. This lets you preview the changes that Terraform plans to make to your AWS infrastructure.

bash
Copy
terraform plan
Applying Changes
Apply the changes required to reach the desired state of the configuration, or the pre-determined set of actions generated by a Terraform plan execution plan.

bash
Copy
terraform apply
You will need to confirm the action by typing yes when prompted.

Destroying Resources
You can destroy all resources managed by your Terraform configuration, which will terminate the EC2 instance and clean up any associated resources.

bash
Copy
terraform destroy
Again, you will need to confirm the action by typing yes when prompted.

Note on Destroying Resources
Destroying your Terraform-managed infrastructure is irreversible. The terraform destroy command will remove all components in the infrastructure managed by Terraform. This includes all AWS EC2 instance components like associated security groups, IP addresses, and block storage. Use this command with caution.

Contributions
Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
