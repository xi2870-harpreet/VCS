---
slug: terraform-workflow
id: izrnaf0mfbz5
type: challenge
title: Terraform workflow
difficulty: basic
timelimit: 600
---
Terraform workflow:
===

**1.** `terraform version` : This command displays the current version of Terraform and all installed plugins.

**2.** `terraform init`
- This command initializes a working directory containing Terraform configuration files.
- This is the first command that should be run after writing a new Terraform configuration or cloning an existing one from version control.
- It is safe to run this command multiple times.
- Once it is done you will get message like : `Terraform has been successfully initialized!`
- You may now begin working with Terraform.  All Terraform commands
should now work.

**Note:**  If you ever set or change modules or backend configuration for Terraform,
rerun this command to reinitialize your working directory. If you forget, other
commands will detect it and remind you to do so if necessary.

**3.** `terraform validate` : This command validates the configuration files in a directory, referring only to the configuration and not accessing any remote services such as remote state, provider APIs, etc.

**4.** `terraform plan`
- This command will create the execution graph for creating and provisioning the infrastructure.
- Once you run this command, `Terraform State` will be refreshed and then will be used to calculate this plan
- After this, an execution plan will be generated and displayed.

**5.** `terraform apply`
- The apply stage will execute the configuration file.
- It will ask: "Do you want to perform these actions?"
- Once you type: Yes, it will execute configuration files.
- Note: There is no undo. Only 'yes' will be accepted to confirm.
- Once configuration file executes successfully, you will get message like: "Apply Complete".

**6.** `terraform apply -auto-approve` : This command is used to explicitly tell to skip approval to apply plan. This is mostly useful in automation CI/CD pipelines.

**7.** `terraform destroy`
- Finally, if you want to delete the infrastructure, you need to run the destroy command.
- Once you run this command, it will ask: "Do you really want to destroy all resources?"
- If you type: "yes", Terraform will destroy all your managed infrastructure
- Note: There is no undo. Only 'yes' will be accepted to confirm.
- Once terraform destroy executes successfully, you will get message like: "Destroy Complete".

**8.** `terraform destroy -auto-approve` : This command is used to explicitly tell to skip approval to destroy the plan. This is mostly useful in automation CI/CD pipelines.

**9.** `terraform state` : This command inspect or modify the state of Terraform-managed resources.

**10.** `terraform output` : This command let you share data between Terraform configurations, and with other tools and automation. Outputs are also the only way to share data from a child module to your configuration's root module. Output Values are like return values for a Terraform module

**11.** `terraform providers` : This command shows information about the provider requirements of the configuration in the current working directory, helps to understand where each requirement was detected from.

**12.** `terraform fmt` : This command is used to rewrite Terraform configuration files to a canonical format and style. This command applies a subset of the Terraform language style conventions, along with other minor adjustments for readability.

**13.** `terraform workspace` : This command is used to manage workspaces.


State Files
===
- Terraform store state about your managed infrastructure and configuration which is used to map real world resources to your configuration, keep track of metadata, and to improve performance for large infrastructures.
- This state is stored by default in a local file named `terraform.tfstate`
- This state file is  used to determine which changes to make to your infrastructure.
- Prior to any operation, Terraform does a refresh to update the state with the real infrastructure.

CLI Command - Version
===
Check the current version of Terraform

```
terraform -version
```
