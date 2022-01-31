# Challenge 1: First template

You are a new engineer in a chocolate factory named "ChocoFaco" which has recenlty moved their operations to Microsoft Azure. ChocoFaco have found a new chocolate recepie which is an instant hit among children and is a direct compition to "Willy Wonka chocolate" a competitor of "ChocoFaco". The business executives are bullish on the future sales and the office of CTO is ready to experiment with Azure resouces and is looking to automate the resorce provisiong so teams can be agile as much as possible. "ChocoFaco" has a good relationship with Microsoft and they are ready to invest their resources on Microsoft Azure, the current engineering team is not very happy with JSON templates and looking for a better solution and Microsoft Azure team has proposed to use Microsoft Bicep. You are asked to learn Bicep, implement and share it across "ChocoFaco".

## Pre-work: ARM Templates

To understand better how Bicep outshines the ARM JSON, you need to understand what is ARM JSON. You can learn more about ARM JSON from this [link](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/syntax).

Let us take a look at ARM JSON, Create a new Virual machine resource either from Azure Portal or use Azure CLI/Powershell.
Download the ARM template on your machine and save it so we can use it later for the comparison.

## Creating your first Bicep template

ChocoFaco team is going to run a new service on a virtual machine and the team lead has asked you to provision a new VM for the team using Bicep.

1. Use Visual studio code to write your bicep templates.
2. Check if the Bicep extension is installed.
3. Create a new resource group where the VM can be provisioned. [Reference link](https://docs.microsoft.com/en-us/cli/azure/group?view=azure-cli-latest#az-group-create) to create resoruce group
4. The Virutal machine name should be unique in the resource group.

## Time for deployment

You are ready with the Bicep template and wants to deploy the VM on Azure. Before you do that, Make sure you have set the subscription correctly on Azure CLI.

[Reference](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/deploy-cli) to deploy bicep template

## Modifications & Redeployment

Let's change the VM type and re-deploy the template. How do you make sure the changes are correct before you actually deploy. For that, you can use "what-if" analysis as discussed below.

### WHAT-IF

Your Bicep template is ready and you can't wait to deploy the template but you are not sure if it will do what it is supposed to do. You can use Azure CLI what-if command which lets you dry run the command.  Now Run the command on your machine band check the modifications by yourself.

[Reference](https://docs.microsoft.com/en-us/cli/azure/deployment/group?view=azure-cli-latest#az-deployment-group-what-if) to what-if command.

## Compiling to ARM template
In the first step, you have saved the ARM JSON template. Open the template in VS code and compare it with Bicep template. This is how easy Bicep helps to write declarative code without the complications of writing JSON.

Bicep also helps to convert the Bicep templates to JSON templates in case you want to. You can convert to JSON template using the `Build` command.

Try converting your bicep template to the JSON template.

Congratulations on completing your first Bicep challenge. Let's now move to writing some more templates.

[Click here](./Challenge2.md) to go to next Challenge 2.
