# Deploy Azure Lighthouse MSP relationship with Claranet.

This template will deploy Azure Lighthouse and let Claranet manage your Azure Subscription resources.

[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fclaranet%2Fazure-lighthouse-msp%2Fmaster%2FdelegatedResourceManagement.json)

[![Deploy To Azure DEBUG](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FShr3ps%2Fazure-lighthouse-msp%2Finitial_template%2FdelegatedResourceManagement.json)

## Deploying this template

You can deploy this template directly through the Azure Portal or by using scripts.

To deploy this template using the Azure Portal, click the **Deploy to Azure** button.

To deploy this template via the command line (using [Azure PowerShell or the Azure CLI](https://azure.microsoft.com/en-us/downloads/)) you can use scripts.

```bash
az deployment create --template-file delegatedResourceManagement.json --parameters 'delegatedResourceManagement.parameters.json' -n 'LightHouse-Claranet-MSP' -l 'westeurope' --subscription xxxxx
```

```powershell
New-AzDeployment -Name "LightHouse-Claranet-MSP" -Location "West Europe" -TemplateFile "delegatedResourceManagement.json" -TemplateParameterFile "delegatedResourceManagement.parameters.json" -Verbose
```
