# Application Insights Demo

Build and deploy a website that uses Application Insights for observability purposes.

```bash

# Wire-up the variables needed
TENANT_ID=<<YOUR_TENANT_ID>>
SUBSCRIPTION_ID=<<YOUR_SUBSCRIPTION_ID>>
ENVIRONMENT_NAME=<<YOUR_ENVIRONMENT_NAME>>
LOCATION=<<YOUR_AZURE_REGION>>

# Or...

source .env

# Login and execute the commands from the AZD CLI
azd auth login --tenant-id $TENANT_ID

azd env new $ENVIRONMENT_NAME --subscription $SUBSCRIPTION_ID --location $LOCATION

azd provision

azd deploy

```