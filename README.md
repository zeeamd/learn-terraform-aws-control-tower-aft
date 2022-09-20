# Learn Terraform - Use Control Tower Account Factory for Terraform

This is a companion repository for the [Provision and Manage Accounts with
Control Tower Account Factory for Terraform
tutorial](https://learn.hashicorp.com/tutorials/terraform/aws-control-tower-aft)
tutorial on HashiCorp Learn.

This repository contains configuration for the AWS Account Factory for
Terraform module. The module creates a pipeline of AWS services that allow you
to create and customize AWS Control Tower accounts through Terraform
configuration. 

- touch .gitignore
- git config core.excludesFile ~/.gitignore

- Use root/Master account creds to run this automation
- The test run was taken with creds that had access to Master/AFT/Audit/Log acc
- The vpc settings in Master should have internet-accessible subnet set as allow to provision lambda having internet access with nat

The cli versions used
- Python 3.10.4
- aws-cli/2.7.33
- Terraform v1.2.9

- Under developer tools (AFT acc) -> settings -> connections -> install apps for 4 repos forked from Hashicorp post successful deployment (manual)
- Add AWSAFTExecution Role to service catalogue portfolio in Master acc post successful deployment (manual)
- If an OU is created manually register it with AWS Control Tower
