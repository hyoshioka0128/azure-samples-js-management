---
page_type: sample
languages:
- javascript
- typescript
products:
- azure
description: "These code samples will show you how to manage Links using Azure SDK for Javascript/Typescript."
urlFragment: links
---

# Getting started - Managing Links using Azure Javascript/Typescript SDK

These code samples will show you how to manage Links using Azure SDK for Javascript/Typescript.

## Features

This project framework provides examples for the following services:

### Links
* Using the Azure SDK for Javascript/Typescript - Links Management Library [@azure/arm-links](https://www.npmjs.com/package/@azure/arm-links) for the [Azure Resources API](https://docs.microsoft.com/en-us/rest/api/resources/)


### Installation

1.  Before using the sdk package,we need [install nodejs](https://nodejs.org/en/download/) and add it into environment variables.

    reference version :
    
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

To run the complete demo, you need to  call the methods you want to test in main method. 

    ```
    async function main() {
        client = new ManagementLinkClient(credential, subscriptionId);
        resources_client = new ResourceManagementClient(credential,subscriptionId);
        await create_resourceId();
    }
    ```

execute below command on terminal

    ```
    tsc links_example.ts (it will create a same name js file)
    node links_example.js
    ```

## Resources

- https://github.com/Azure/azure-sdk-for-js