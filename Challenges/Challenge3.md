# Challenge 3: What about Environments

Excellent work on completing the full application with dependencies template in [challenge 2](./Challenge2.md). Let us now work on creating different environments using a template.

## Challenge

"ChocoFaco" development team wants to have another environment where they can showcase the features in flight to the business executives. The team has asked you to create a new environment with same resources but with lower configuration so the price quotas can be met.

Do the modifications in the existing template so the new environment with the same template. There should be an option through which one could tell whether you want to provision for production or non-production environment.

For the non-production environment, keep the lowest configuration possible.
> Create different SKU and Storage account types in different environments

Is the new environment properly deployed to Azure? If yes, there is a another demand from the office of the CTO to create a new resource group from the template itself and deploy the resources inside it. This is for experimentation and learning, so store a copy of exisitng template somewhere e.g. in version control or folder.

Bicep supports different scopes, you can read more about them [here](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/deploy-to-management-group?tabs=azure-cli)

Office of CTO has finally decided that we resource groups will be created outside of Bicep templates for ChocoFaco. The team would like to automate the provisioning of infrastrcuture theough some pipelines. You are given a task to create the pipeline or Github action to provision the infrastructure.

Once the pipeline or workflow is created, provision the infrastructure for a non-prodcution environment.


### References:

- [Configuration Setting pattern](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/patterns-configuration-set)
- [Bicep Scope functions](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/bicep-functions-scope)
- [Management group deployments with Bicep](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/deploy-to-management-group?tabs=azure-cli)
- [Deploy Bicep template](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/deploy-github-actions?tabs=CLI)