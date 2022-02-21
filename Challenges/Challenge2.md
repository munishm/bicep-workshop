# Challenge 2: Complete Stack

Congratulations on creating your first Bicep template in [Challenge 1](./Challenge1.md). By now you should have some basic understanding of how Bicep works and how to deploy Bicep templates. Let us now work on creating a template for a full-stack application.

## Challenge

The "ChocoFaco" development team is moving from Virtual machines to managed services on Azure. Their new application needs to run on a App service which also requires some dependencies to run. You have been requested to provision the following resources:

1. An App service
2. Cosmos DB SQL API, is required for data persistence
3. Storage account with a blob container

After the resources are provisioned, you are requested to output the URL of the App service.

Learn about the Bicep best practices from [here](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/best-practices)

Few of the considerations to take care of when developing and deploying the Bicep template:

- Proper description of the parameters and variables
- Parent-Child relationship
- Define the Output parameters correctly
- Use of decorators
- Uniqueness of resources
- Linting of your bicep template
- What-IF analysis to check the correctness of deployment
- Troubleshooting deployment errors

### References

- [Bicep best Practices](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/best-practices)
- [Sharing variables across Bicep Files](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/patterns-shared-variable-file)
- [Naming conventions & generation pattern](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/patterns-name-generation)
- [Troubleshooting errors](https://docs.microsoft.com/en-us/azure/azure-resource-manager/troubleshooting/quickstart-troubleshoot-bicep-deployment?tabs=azure-cli)