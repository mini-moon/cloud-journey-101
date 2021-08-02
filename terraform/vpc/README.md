### What 
This is a module to deploy below resources into target AWS account.
- 1 VPC 
- 1 private subnet
- 1 public subnet 
- 1 NAT in public subnet 
- 1 IGW attached to VPC

### Requirements
- AWSCLI been set up and logged in to your account, validate with:
  `aws iam list-account-aliases`
- Terraform version 14.9 been installed, validate with:
  `terraform -version`

### How to use 
In folder `terraform/vpc`, try out below commands:
- To init terraform: `terraform init`
- To check the resources will be created: `terraform plan` 
- To apply the deployment: `terraform apply`
- To list out the created resources: `terraform state list`
- To destroy terraform managed resources: `terraform destroy`

### Note
In this sample we used a local tfstate, which is for demo purposes only, for any production workload, you should ALWAYS use a remote state file instead.
Great reference at: https://www.mitrais.com/news-updates/infrastructure-as-code-using-terraform-creating-an-aws-virtual-private-cloud/
