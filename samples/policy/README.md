---
page_type: sample
languages:
- javascript
- typescript
products:
- azure
description: "These code samples will show you how to manage Policy using Azure SDK for Javascript/Typescript."
urlFragment: policy
---

# Getting started - Managing Policy using Azure Javascript/Typescript SDK

These code samples will show you how to manage Policy using Azure SDK for Javascript/Typescript.

## Features

This project framework provides examples for the following services:

### Policy
* Using the Azure SDK for Javascript/Typescript - Policy Management Library [@azure/arm-policy](https://www.npmjs.com/package/@azure/arm-policy) for the [Azure Resources API](https://docs.microsoft.com/en-us/rest/api/resources/)


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
    cd azure-samples-js-management/samples/policy
    npm i -g typescript
    npm install
    ```

## Demo

A demo app is included to show how to use the project.

To run the complete demo, you need to call the methods you want to test in main method. 

    ```
    async function main() {
        policyclient = new PolicyClient(credential, subscriptionId);
        managementclient = new ManagementGroupsAPI(credential);
        await policyDefinitions_createOrUpdateAtManagementGroup();
    }
    ```

execute below command on terminal

    ```
    tsc policy_example.ts (it will create a same name js file)
    node policy_example.js
    ```

## Resources

- https://github.com/Azure/azure-sdk-for-js