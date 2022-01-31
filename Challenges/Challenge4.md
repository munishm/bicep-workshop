# Challenge 4: Publishing Artifcats

In the [previous challenge](./Challenge3.md) you created the automated pipelines to provision the infrastructure for the applications.

## Challenge

This all works well for a sinle development team and you have bestowed upon with a task to share the template across the organization. Right now, there are different discussions happening across ChocoFaco to use this template or add more generic template however for now some other team wants to use your template and asked you to share the template with them. Due to obvious reasons, you doesn't want to share the repo code with them so you thought about sharing it via Private registry.

Create a new private registry and share your template using that private registry. Also, show the new team on how you can directly consume the template from the registry.

https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/private-module-registry?tabs=azure-powershell

CLI resources to publish and restore templates- https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/bicep-cli

This way you can share the modules privately, the dsicussions by the office of CTO has progressed well and now they want you to share the template across the organization so the other teams can also use these templates.

Create a template spec and publish it to Azure. You can read more about template specs [here](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/template-specs?tabs=azure-powershell)

Do the following to understand the Bicep template spec:

- Deploy the Bicep template into the template spec using CLI
- Deploy the template spec
- Do a minor change and update the template spec with a new version

### References:

- [Template Spec](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/template-specs?tabs=azure-powershell)
- [Bicep CLI Commands](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/bicep-cli)
- [Module settings in Bicep config file](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/bicep-config-modules)
