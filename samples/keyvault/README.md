---
page_type: sample
languages:
- javascript
- typescript
products:
- azure
description: "These code samples will show you how to manage KeyVault using Azure SDK for Javascript/Typescript."
urlFragment: KeyVault
---

# Getting started - Managing KeyVault using Azure Javascript/Typescript SDK

These code samples will show you how to manage KeyVault using Azure SDK for Javascript/Typescript.


### Features
* Using the Azure SDK for Javascript/Typescript - KeyVault Management Library [@azure/arm-keyvault](https://www.npmjs.com/package/@azure/arm-keyvault) for the [Azure KeyVault API](https://docs.microsoft.com/en-us/rest/api/keyvault/)


### Installation

1.  Before using the sdk package,we need [install nodejs](https://nodejs.org/en/download/) and add it into environment variables.

    reference :
    
    ```
    nodejs version: 14.16.0
    typescript version: 4.1.3
    ```

### Quickstart

1.  Clone the repository.

    ```
    git clone https://github.com/Azure-Samples/azure-samples-js-management
    ```

2.  Install the dependencies using npm.

    ```
    cd azure-samples-js-management/samples/links
    npm i -g typescript
    npm install
    ```

## Demo

A demo app is included to show how to use the project.

To run the complete demo, you need to call the methods you want to test in this main method.

    ```
    async function main() {
        client = new KeyVaultManagementClient(credential, subscriptionId);
        await vaults_beginCreateOrUpdateAndWait();
    }
    ```

execute below command on terminal

    ```
    tsc keyvault_examples.ts (it will create a same name js file)
    node keyvault_examples.js
    ```

## Resources

- https://github.com/Azure/azure-sdk-for-js