---
id: what-is-resource-group
title: What is Resource Group?
# prettier-ignore
description: A resource group is a container that holds related resources for an Azure solution. The resource group can include all the resources for the solution, or only those resources that you want to manage as a group.
---

![Azure Resource Group](./assets/azure-resource-group.png)

[Azure Resource Group](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-portal) is a container that holds related resources for an Azure solution. The resource group can include all the resources for the solution, or only those resources that you want to manage as a group.

You decide how you want to allocate resources to resource groups based on what makes the most sense for your organization. Generally, add resources that share the same lifecycle to the same resource group so you can easily deploy, update, and delete them as a group.

The resource group scope is also used throughout the Azure portal to create views that span across multiple resources. For example:

- Metrics blade provides metrics information (CPU, resources) to users.

- Deployments blade shows the history of ARM Template or Bicep deployments targeted to that Resource Group (which includes Portal deployments).

- Policy blade provides information related to the policies enforced on the resource group.

- Diagnostics settings blade provides the ability to diagnose errors or review warnings.

The resource group stores metadata about the resources. Therefore, when you specify a location for the resource group, you're specifying where that metadata is stored. For compliance reasons, you might need to ensure that your data is stored in a particular region. Note that resources inside a resource group can be of different regions.
