---
page_type: sample
languages:
- javascript
- typescript
products:
- azure
description: "These code samples will show you how to manage Network using Azure SDK for Javascript/Typescript."
urlFragment: network
---

# Getting started - Managing Network using Azure Javascript/Typescript SDK

These code samples will show you how to manage Network using Azure SDK for Javascript/Typescript.

## Features

This project framework provides examples for the following services:

### Network
* Using the Azure SDK for Javascript/Typescript - Network Manamgement Library [@azure/arm-network](https://www.npmjs.com/package/@azure/arm-network) for the [Virtual Network API](https://docs.microsoft.com/en-us/rest/api/virtual-network/), [Virtual WAN API](https://docs.microsoft.com/en-us/rest/api/virtualwan/), [Network Wather API](https://docs.microsoft.com/en-us/rest/api/network-watcher/), [Network Gateway API](https://docs.microsoft.com/en-us/rest/api/network-gateway/), [Firewall API](https://docs.microsoft.com/en-us/rest/api/firewall/), [ExpressRoute API](https://docs.microsoft.com/en-us/rest/api/expressroute/)


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
    cd azure-samples-js-management/samples/network
    npm i -g typescript
    npm install
    ```

## Demo

A demo app is included to show how to use the project.

To run the complete demo, you need to call the methods you want to test in main method. 

    ```
    async function main() {
        client = new NetworkManagementClient(credential, subscriptionId);
        await virtualNetworks_beginCreateOrUpdateAndWait();
    }
    ```

execute below command on terminal

    ```
    tsc network_base_example.ts (it will create a same name js file)
    node network_base_example.js
    ```

## Resources

- https://github.com/Azure/azure-sdk-for-js