
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/settings')
	.version('beta')
	.get();

```