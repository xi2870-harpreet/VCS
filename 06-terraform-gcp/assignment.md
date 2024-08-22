---
slug: terraform-gcp
id: tyztxl4qeot8
type: challenge
title: Terraform GCP
difficulty: basic
timelimit: 1000
---
👋 Introduction
===============

1. Use the terminal to create Compute instance Compute network(VPC)  by Terraform:
2. First run ```terraform init``` to initialize the working directory containing Terraform configuration files.
4. Now run ```terraform validate```  to validates the configuration files in a directory.
5. Now run ```terraform plan```  which creates an execution plan, which lets you preview the changes that Terraform plans to make to your infrastructure
6. Now run ```terraform apply``` to provision the resources

 Congratulations!! now Compute instance/Compute network(VPC) resources has been provisioned successfully.

- To check further about resources you can login on `GCP Console via GCP console tab`

- To know more about the terraform code you can click on `Editor` tab and check below files:

	1.  `main.tf` is terraform file which contains the main set of configuration for your module.
  2. `variable.tf` is terraform file which contains the variable definitions for your module.
  3.  `terraform.tfvars` is terraform file where the variables are provided/assigned a value


To complete this challenge, press **Check**.
