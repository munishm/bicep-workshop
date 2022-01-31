# Challenge 1: First template

You are a new engineer in a chocolate factory named "ChocoFaco" which has recenlty moved their operations to Microsoft Azure. ChocoFaco have found a new chocolate recepie which is an instant hit among children and is a direct compition to "Milly Monka chocolate" a competitor of "ChocoFaco". The business executives are bullish on the future sales and the office of CTO is ready to experiment with new technology and is looking to be agile as much as possible. "ChocoFaco" has a good relationship with Microsoft and they are ready to invest more in Microsoft Azure, the current engineering team is not happy with JSON templates and looking for a better solution; Somebody in the office has proposed to use Microsoft Bicep. You are given the task to lead the operations related to Bicep.

## Challenge
In this challenge you'll create new Bicep template using Visual studio code, will learn how to deploy the Bicep template and also lean how you can preview the modifications before you implement them.

## ARM JSON Templates vs Bicep Templates

To understand better how Bicep outshines the ARM JSON templates, you need to understand what is ARM JSON tempalte. ARM templates are writen in JSON to provision the Azure resources. In case you have not worked with ARM JSON templates before, we recommend to read this [link](You can learn more about ARM templates from this [link](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview).


How is Bicep different from ARM JSON templates:

Excerpt from Bicep documentation:
***
Bicep is more of a revision to the existing ARM template language rather than an entirely new language. While most of the syntax has been changed, the core functionality of ARM templates and the runtime remains the same. You have the same template functions, same resource declarations, etc.
***

Let's start with writing you first template.

## Writing your First Bicep template

ChocoFaco Data team requires to migrate some data and they need an Azure Data Factory managed service and the Data team lead has requested you to provision a new ADF for her team. You will use this opportunity to create the resource using Bicep.

1. Use Visual studio code to write your bicep template.
    > Bicep extension makes the experience of writing bicep better. 
2. Create a **new resource group** in which the ADF will be provisioned. [Link to create new resource group using CLI](https://docs.microsoft.com/en-us/cli/azure/group?view=azure-cli-latest#az-group-create).


## Deploy your template

Once you are ready with the Bicep template, You can deploy the resource using **Azure CLI**.
>  Check you are on correct subscription before you deploy

[How to deploy Bicep?](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/deploy-cli)

## Modificiation & Re-deployment

Resource should be provisioned & available for the team after deployment.

You are now requested to add a new tag to the resource as
  ```
  "Team": "ChocoFacoDT"
  ```

For adding the tag, you will do the modifications in your template in VS code & then You should be ready to deploy it again.

 > How do you make sure the changes are correct before you actually deploy the template. You can use "what-if" analysis as discussed below.

### WHAT-IF

Your Bicep template is ready and you can't wait to deploy the template but you are not sure if it will add the *tags* only. 

> You can use Azure CLI [what-if command](https://docs.microsoft.com/en-us/cli/azure/deployment/group?view=azure-cli-latest#az-deployment-group-what-if) to check.  

## Compiling & Decompiling to ARM JSON template

Bicep also helps to convert the Bicep templates to JSON templates & viceversa. You can convert to JSON template using the `Build` command.

Try converting your bicep template to the JSON template or take an existing JSON template from Azure to convert it into Bicep.

Steps to decompile: 
https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/decompile?tabs=azure-cli


Congratulations on completing your first Bicep challenge. Let's now move to writing some more detailed templates.

[Click here](./Challenge2.md) to go to next Challenge.
