# Challenge 1: First template

You are a new engineer in a chocolate factory named "ChocoFaco" which has recently moved its operations to Microsoft Azure. ChocoFaco has found a new chocolate recipe that is an instant hit among children and is a direct competition to "Milly Monka chocolate" a competitor of "ChocoFaco". The business executives are bullish on future sales and the office of CTO is ready to experiment with new technology and is looking to be agile as much as possible. "ChocoFaco" has a good relationship with Microsoft and they are ready to invest more in Microsoft Azure, the current engineering team is not happy with JSON templates and looking for a better solution; Somebody in the office has proposed to use Microsoft Bicep. You are given the task to lead the operations related to Bicep.

## Challenge
In this challenge you'll create a new Bicep template using Visual studio code, will learn how to deploy the Bicep template, and also learn how you can preview the modifications before you implement them.

## ARM JSON Templates vs Bicep Templates

To understand better how Bicep outshines the ARM JSON templates, you need to understand what is ARM JSON template is. Before Bicep, ARM templates were written in JSON to provision the Azure resources. In case you have not worked with ARM JSON templates before, we recommend reading this [link](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview).


*How is Bicep different from ARM JSON templates:*

Excerpt from Bicep documentation:
***
Bicep is more of a revision to the existing ARM template language rather than an entirely new language. While most of the syntax has been changed, the core functionality of ARM templates and the runtime remains the same. You have the same template functions, same resource declarations, etc.
***

Let's start with writing your first template.

## Writing your First Bicep template

ChocoFaco Data team requires to migrate some data and they need an Azure Data Factory managed service the Data team lead has requested you to provision a new ADF for her team. You will use this opportunity to create the resource using Bicep.

1. Use Visual studio code to write your bicep template.

    > Bicep extension makes the experience of writing bicep better. 
2. Create a **new resource group** from either Azure CLI or portal in which the ADF will be provisioned. [Link to create new resource group using CLI](https://docs.microsoft.com/en-us/cli/azure/group?view=azure-cli-latest#az-group-create).


## Deploy your template

Once you are ready with the Bicep template, You can deploy the resource using **Azure CLI**.
>  Please check if you are on the correct subscription before you deploy the resource

[How to deploy Bicep?](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/deploy-cli)

## Modificiation & Re-deployment

There are times when you need to do modifications to the resources and have to re-deploy them.

You are now requested to add a new tag to the resource as
  ```
  "Team": "ChocoFacoDT"
  ```

For adding the tag, you will do the modifications in your template using VS code & then you should be ready to re-deploy it.

 > How do you make sure the changes are correct before you deploy the template. You can use "what-if" analysis as discussed below.

### WHAT-IF

At this point, your modifications are done and you can't wait to re-deploy, how do you make sure if the change will add the *tags* only. 

> You can use Azure CLI [what-if command](https://docs.microsoft.com/en-us/cli/azure/deployment/group?view=azure-cli-latest#az-deployment-group-what-if) to check.  

## Compiling & Decompiling to ARM JSON template

Bicep can convert the Bicep templates to JSON templates & viceversa. You can convert Bicep to JSON template using the `Build` command.

Lets us now convert the recently developed bicep template into the JSON template & take a look. You'll see how easy is to convert bicep to JSON. If you have some JSON templates, you can even decompile them to Bicep templates as well. This is one way to convert the existing ARM templates to Bicep.

Steps to decompile: 
https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/decompile?tabs=azure-cli


Congratulations on completing your first Bicep challenge. Let's move to write some more detailed templates. [Click here](./Challenge2.md) to go to next Challenge.
