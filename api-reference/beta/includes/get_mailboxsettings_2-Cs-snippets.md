
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
	.Request()
	.Select( e => new {
			 e.MailboxSettings 
			 })
	.GetAsync();

var automaticRepliesSetting = me.MailboxSettings.AutomaticRepliesSetting;

```