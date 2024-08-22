---
slug: terraform-architecture
id: al49ihjkusmm
type: challenge
title: Terraform Architecture
difficulty: basic
timelimit: 600
---
Terraform Architecture
===

Terraform has two main components that make up its architecture:

- Terraform Core
- Providers

![terraform-architecture.jpg](/assets/tracks/bvsiawzhdaxu/a53d2b45ae2c1b3ade97cafe7e218a69)

# Terraform Core
===

Terraform core uses two input sources to do its job:
1. **Terraform configuration** that you, as a user, configure. ( where you define what needs to be created or provisioned).
2. **state** where terraform keeps the up-to-date state of how the current set up of the infrastructure looks like.

So, what **terraform core** does?
1. It takes the input, and it figures out the plan of what needs to be done.
2. It compares the state, what is the current state, and what is the configuration that you desire in the end result.
3. It figures out what needs to be done to get to that desired state in the configuration file.
4. It figures what needs to be created, what needs to be updated, what needs to be deleted to create and provision the infrastructure.

**Providers:**
1. The second component of the architecture are providers for specific technologies.
2. This could be cloud providers like AWS, Azure, GCP.
3. It gives you the possibility to create infrastructure on different levels.
4. Terraform has over a hundred providers for different technologies, and each provider then gives terraform user access to its resources.

**For Example:** through AWS provider, you have access to hundreds of AWS resources like EC2 instances, the AWS users, etc.

You can always get help if you're curious about command syntax:
```
terraform help
```


Summary
===

So, this is how Terraform works, and this way, it tries to help you provision and cover the complete application setup from infrastructure all the way to the application.
