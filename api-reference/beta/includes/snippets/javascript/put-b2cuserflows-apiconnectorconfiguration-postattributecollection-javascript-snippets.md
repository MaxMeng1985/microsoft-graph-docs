---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    @odata.id: "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
};

let res = await client.api('/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref')
	.version('beta')
	.put(identityApiConnector);

```