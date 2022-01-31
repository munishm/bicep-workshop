# Challenge 2: Complete Stack

Congratulations on creating your first Bicep template in [Challenge 1](./Challenge1.md). Now you have basic understanding of how Bicep works and how do you deploy your Bicep templates. Let us now work on a new template for a full stack application.

## Challenge

"ChocoFaco" development team is moving from Virtual machines to managed services on Azure. Their new application needs to run on a windows App service which also requires some dependecies to run. You are given a task to do the following:

1. Create a new Windows App service & share the app service URL with the development team.
2. The Application also requires a Cosmos DB to persist the data.
3. The Application stores files into Blob storage account.
4. The Application also uses a SignalR service to messaging game play with kids.

> All these service connections should be available in the Azure App service app settings so these services be used by the application code.

You should make sure the code is modularized so this can be maintained later. Learn more about [Bicep modules](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/modules)

Learn about the Bicep best practices from [here](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/best-practices)

Things to keep in mind while developing & deploying the template:

- There should be proper description of the parametes and variables
- Make sure the Parent Child relationship is maintained
- Define the Output parameters correctly
- Secrets should not be defined in the output variables
- Proper use of decorators in Bicep template
- Uniqueness of resource names
- Linting of your bicep template
- What-IF analysis to check the correct changes to the resources
- Ways to troubleshoot deployment errors

### References

- [Bicep best Practices](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/best-practices)
- [Sharing variables across Bicep Files](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/patterns-shared-variable-file)
- [Naming conventions & generation pattern](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/patterns-name-generation)
- [Secret management Scenarios](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/scenarios-secrets)
- [Troubleshooting errors](https://docs.microsoft.com/en-us/azure/azure-resource-manager/troubleshooting/quickstart-troubleshoot-bicep-deployment?tabs=azure-cli)