# Azure Firewall Policies

Azure Pipeline YAML Deployment workflow

This script is configured to run on an Ubuntu agent (vmImage: ubuntu-latest) and consists of two stages: Deploy_Bicep and two jobs within that stage: Checkout and Deploy. The Checkout job checks out the repository using the self option, and the Deploy job uses the AzureCLI task to deploy the Bicep template to an Azure resource group.

The 'resourceGroupName' and 'serviceConnectionName' variables are used to specify the Azure resource group name and the Azure service connection name respectively. These variables are defined in the variables section at the beginning of the script and can be adjusted as per your project's requirements.

Note: Please make sure to update the file paths for the Bicep template and parameters files in the 'az deployment group create' command to match the correct locations within your repository.