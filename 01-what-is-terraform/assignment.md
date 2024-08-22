---
slug: what-is-terraform
id: h8v6qkc5q7n9
type: challenge
title: What IsTerraform?
difficulty: basic
timelimit: 600
---
🗂️ Tabs
======
For this track you have multiple tabs in the left window. The **Editor** tab that is currently displayed is Visual Studio Code.
Beside it is the is the **Terminal** tab, where you can run CLI commands.

Alternately, you can run CLI commands using the terminal built into VSCode by pressing `CTRL+SHIFT+~`

Benefits of using Terraform
===

- Supports multiple providers such as AWS, Azure, GCP
- Easy to change configuration
- Easily portable to any other provider
- Supports Client only architecture, so no need for additional configuration management on a server


# Terraform Core concepts
===

Below are the core concepts/terminologies used in Terraform:

- **Variables**: Also used as input-variables, it is key-value pair used by Terraform modules to allow customization.
- **Provider**: It is a plugin to interact with APIs of service and access its related resources.
- **Module**: It is a folder with Terraform templates where all the configurations are defined
- **State**: It consists of cached information about the infrastructure managed by Terraform and the related configurations.
- **Resources**: It refers to a block of one or more infrastructure objects (compute instances, virtual networks, etc.), which are used in configuring and managing the infrastructure.
- **Data Source**: It is implemented by providers to return information on external objects to terraform.
- **Output Values**: These are return values of a terraform module that can be used by other configurations.
- **Plan**: It is one of the stages where it determines what needs to be created, updated, or destroyed to move from real/current state of the infrastructure to the desired state.
- **Apply**: It is one of the stages where it applies the changes real/current state of the infrastructure in order to move to the desired state.
