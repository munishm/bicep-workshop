# Challenge 3: What about Environments

Excellent work on completing the template to provison a full application with dependencies in [challenge 2](./Challenge2.md). We should be ready to create different environments using a Bicep template.

## Challenge

"ChocoFaco" development team wants to have another environment where they can showcase the features in flight to executives. The team has asked you to create a new environment with similar type of resources but with **lower configuration** so the price quotas can be met.

You are requested to modify the existing template so the new environment can be provisioned using the same template with a conditional setting. There should be an option through which one could decide the environment type. 

The probable options should be `prod` & `non-prod`

> For the non-production environment, keep the lowest configuration possible. Keep different SKU and Storage account types for prod vs non-prod environments.

***For Non-production environment, You are requested to create the resource group too.*** 

You can use the [conditional resource deployment](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/conditional-resource-deployment) for conditions.

Bicep supports different scopes, you can read more about them [here](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/deploy-to-management-group?tabs=azure-cli)



### References:

- [Configuration Setting pattern](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/patterns-configuration-set)
- [Bicep Scope functions](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/bicep-functions-scope)
- [Management group deployments with Bicep](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/deploy-to-management-group?tabs=azure-cli)
- [Deploy Bicep template](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/deploy-github-actions?tabs=CLI)