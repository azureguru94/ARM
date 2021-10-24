# App_Insights_Alerts 

This template deploys 6 alerts for application insights as following :

> high server memory usage

> server exceptions (dynamic threeshold)

> dependency call failures (dynamic threeshold)

> failed requests increasing (dynamic threeshold)

> increasing http requests rate (dynamic threeshold)

> average server response time more than 30 second

you can use powershell or template deployment from azure portal 

Template Parameters :
---------------------

> appinsights_id : you have to locate your app insights id which should be in the following format 

/subscriptions/"subscription id"/resourceGroups/"resource group name"/providers/microsoft.insights/components/"application insights name "

> actiongroup_id : you have to locate your action group id which should be in the following format 

/subscriptions/"subscription id"/resourceGroups/"resource group name"/providers/microsoft.insights/actiongroups/"action group name"

> custom_domain : your website name "ex:azureguru.tech" to be be able to identify whcih mail alert you're recieveing if you have multiple applications and it will also be appended 

at the beginning of the alert name.
