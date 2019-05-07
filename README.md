# ![LOGO](logo.png) Azure ML Web Services Management Client **flow**ground Connector

## Description

A generated **flow**ground connector for the Azure ML Web Services Management Client API (version 2017-01-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/machinelearning-webservices/2017-01-01/swagger.json<br/>
Generated at: 2019-05-07T17:38:19+03:00

## API Description

These APIs allow end users to operate on Azure Machine Learning Web Services resources. They support the following operations:<ul><li>Create or update a web service</li><li>Get a web service</li><li>Patch a web service</li><li>Delete a web service</li><li>Get All Web Services in a Resource Group </li><li>Get All Web Services in a Subscription</li><li>Get Web Services Keys</li></ul>

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all the available REST API operations.

#### Input Parameters
* `api-version` - _required_ - The version of the Microsoft.MachineLearning resource provider API to use.

### Gets the web services in the specified subscription.

*Tags:* `WebServices`

#### Input Parameters
* `$skiptoken` - _optional_ - Continuation token for pagination.
* `api-version` - _required_ - The version of the Microsoft.MachineLearning resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.

### Gets the web services in the specified resource group.

*Tags:* `WebServices`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group in which the web service is located.
* `$skiptoken` - _optional_ - Continuation token for pagination.
* `api-version` - _required_ - The version of the Microsoft.MachineLearning resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.

### Deletes the specified web service.

*Tags:* `WebServices`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group in which the web service is located.
* `webServiceName` - _required_ - The name of the web service.
* `api-version` - _required_ - The version of the Microsoft.MachineLearning resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.

### Gets the Web Service Definition as specified by a subscription, resource group, and name. Note that the storage credentials and web service keys are not returned by this call. To get the web service access keys, call List Keys.

*Tags:* `WebServices`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group in which the web service is located.
* `webServiceName` - _required_ - The name of the web service.
* `region` - _optional_ - The region for which encrypted credential parameters are valid.
* `api-version` - _required_ - The version of the Microsoft.MachineLearning resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.

### Modifies an existing web service resource. The PATCH API call is an asynchronous operation. To determine whether it has completed successfully, you must perform a Get operation.

*Tags:* `WebServices`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group in which the web service is located.
* `webServiceName` - _required_ - The name of the web service.
* `api-version` - _required_ - The version of the Microsoft.MachineLearning resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.

### Create or update a web service. This call will overwrite an existing web service. Note that there is no warning or confirmation. This is a nonrecoverable operation. If your intent is to create a new web service, call the Get operation first to verify that it does not exist.

*Tags:* `WebServices`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group in which the web service is located.
* `webServiceName` - _required_ - The name of the web service.
* `api-version` - _required_ - The version of the Microsoft.MachineLearning resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.

### Creates an encrypted credentials parameter blob for the specified region. To get the web service from a region other than the region in which it has been created, you must first call Create Regional Web Services Properties to create a copy of the encrypted credential parameter blob in that region. You only need to do this before the first time that you get the web service in the new region.

*Tags:* `WebServices`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group in which the web service is located.
* `webServiceName` - _required_ - The name of the web service.
* `region` - _required_ - The region for which encrypted credential parameters are created.
* `api-version` - _required_ - The version of the Microsoft.MachineLearning resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.

### Gets the access keys for the specified web service.

*Tags:* `WebServices`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group in which the web service is located.
* `webServiceName` - _required_ - The name of the web service.
* `api-version` - _required_ - The version of the Microsoft.MachineLearning resource provider API to use.
* `subscriptionId` - _required_ - The Azure subscription ID.

## License

**flow**ground :- Telekom iPaaS / azure-com-machinelearning-webservices-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
