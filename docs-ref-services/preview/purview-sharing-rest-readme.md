---
title: Azure Purview Sharing REST client library for JavaScript
keywords: Azure, javascript, SDK, API, @azure-rest/purview-sharing, purview
author: qiaozha
ms.author: qiaozha
ms.date: 03/14/2023
ms.topic: reference
ms.devlang: javascript
ms.service: purview
---
# Azure Purview Sharing REST client library for JavaScript - version 1.0.0-beta.1 


Purview Sharing Client

\*\*If you are not familiar with our REST client, please spend 5 minutes to take a look at our [REST client docs](https://github.com/Azure/azure-sdk-for-js/blob/@azure-rest/purview-sharing_1.0.0-beta.1/documentation/rest-clients.md) to use this library, the REST client provides a light-weighted & developer friendly way to call azure rest api

Key links:

- [Source code](https://github.com/Azure/azure-sdk-for-js/tree/@azure-rest/purview-sharing_1.0.0-beta.1/sdk/purview/purview-sharing-rest)
- [Package (NPM)](https://www.npmjs.com/package/@azure-rest/purview-sharing)
- [API reference documentation](/javascript/api/@azure-rest/purview-sharing?view=azure-node-preview)
- [Samples](https://github.com/Azure/azure-sdk-for-js/tree/@azure-rest/purview-sharing_1.0.0-beta.1/sdk/purview/purview-sharing-rest/samples)

## Getting started

### Currently supported environments

- LTS versions of Node.js

### Prerequisites

- You must have an [Azure subscription](https://azure.microsoft.com/free/) to use this package.

### Install the `@azure-rest/purview-sharing` package

Install the Azure Purview Sharing REST client library for JavaScript with `npm`:

```bash
npm install @azure-rest/purview-sharing
```

### Create and authenticate a `PurviewSharingClient`

To use an [Azure Active Directory (AAD) token credential](https://github.com/Azure/azure-sdk-for-js/blob/@azure-rest/purview-sharing_1.0.0-beta.1/sdk/identity/identity/samples/AzureIdentityExamples.md#authenticating-with-a-pre-fetched-access-token),
provide an instance of the desired credential type obtained from the
[@azure/identity](https://github.com/Azure/azure-sdk-for-js/tree/@azure-rest/purview-sharing_1.0.0-beta.1/sdk/identity/identity#credentials) library.

To authenticate with AAD, you must first `npm` install [`@azure/identity`](https://www.npmjs.com/package/@azure/identity)

After setup, you can choose which type of [credential](https://github.com/Azure/azure-sdk-for-js/tree/@azure-rest/purview-sharing_1.0.0-beta.1/sdk/identity/identity#credentials) from `@azure/identity` to use.
As an example, [DefaultAzureCredential](https://github.com/Azure/azure-sdk-for-js/tree/@azure-rest/purview-sharing_1.0.0-beta.1/sdk/identity/identity#defaultazurecredential)
can be used to authenticate the client.

Set the values of the client ID, tenant ID, and client secret of the AAD application as environment variables:
AZURE_CLIENT_ID, AZURE_TENANT_ID, AZURE_CLIENT_SECRET

## Troubleshooting

### Logging

Enabling logging may help uncover useful information about failures. In order to see a log of HTTP requests and responses, set the `AZURE_LOG_LEVEL` environment variable to `info`. Alternatively, logging can be enabled at runtime by calling `setLogLevel` in the `@azure/logger`:

```javascript
const { setLogLevel } = require("@azure/logger");

setLogLevel("info");
```

For more detailed instructions on how to enable logs, you can look at the [@azure/logger package docs](https://github.com/Azure/azure-sdk-for-js/tree/@azure-rest/purview-sharing_1.0.0-beta.1/sdk/core/logger).

