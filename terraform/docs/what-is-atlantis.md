---
id: what-is-atlantis
title: What is Atlantis?
# prettier-ignore
description: This is a simple feature, however it has had a massive effect on how teams writes Terraform. By bringing a Terraform workflow to pull requests, Atlantis help the Ops team collaborate better on Terraform enabling entire development team to write and execute Terraform safely.
---

 This is a simple feature, however it has had a massive effect on how teams writes Terraform. By bringing a Terraform workflow to pull requests, Atlantis help the Ops team collaborate better on Terraform enabling entire development team to write and execute Terraform safely.

![atlantis](./assets/atlantis.gif)

# Overview

Atlantis is an application for automating Terraform via pull requests. It is deployed as a standalone application into your infrastructure. No third-party has access to your credentials.

Atlantis is an application for automating `Terraform via pull requests`. It is deployed as a standalone application into your infrastructure. No third-party has access to your credentials.

Atlantis listens for `GitHub`, `GitLab` or `Bitbucket` `webhooks` about `Terraform pull requests. It then runs `terraform plan` and comments with the output back on the pull request.

When you want to apply, comment `atlantis apply` on the pull request and Atlantis will run terraform apply and comment back with the output.

# Why would you run Atlantis?

## Increased visibility

When everyone is executing Terraform on their own computers, it's hard to know the current state of your infrastructure:

## Is what's in main branch deployed?

Did someone forget to create a pull request for that latest change?
What was the output from that last terraform apply?
With Atlantis, everything is visible on the pull request. You can view the history of everything that was done to your infrastructure.

## Enable collaboration with everyone

You probably don't want to distribute Terraform credentials to everyone in your engineering organization, but now anyone can open up a Terraform pull request.

You can require approval before the pull request is applied so nothing happens accidentally.

## Review Terraform pull requests better

You can't fully review a Terraform change without seeing the output of terraform plan. Now that output is added to the pull request automatically.

## Standardize your workflows

Atlantis locks a directory/workspace until the pull request is merged or the lock is manually deleted. This ensures that changes are applied in the order expected.

The exact commands that Atlantis runs are configurable. You can run custom scripts to construct your ideal workflow.
