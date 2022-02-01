# Challenge 2a: Managing secrets

When you are managing the secrets like connection strings, You are advised to look into the Bicep best practices to understand [Secret management scenarios](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/scenarios-secrets)

## Challenge

Resources are available for the development team to publish their website however there is the small challenge of managing App settings. The App service provisioned in the [challenge 2](./Challenge2.md) doesn't have app settings consisting of the connection strings for the dependencies. 

Now you are requested to add the connection strings for both Cosmos DB and Blob Storage into the app settings of the Azure App service.  

You also need to make sure the secrets are not defined in the output variables as there are security risks associated with them.


### References
- [Secret management Scenarios](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/scenarios-secrets)