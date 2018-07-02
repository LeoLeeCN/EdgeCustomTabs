# Edge Custom Tabs
[Using Chromium Custom Tabs](https://chromium.googlesource.com/custom-tabs-client/+/master/Using.md)should be easy. 

## Edge extra action

UI customization is done through the methods exposed by
`CustomTabsSession`.

**Example:**
```java
CustomTabsClient.newSession(customTabsCallback).edgeExtraCommand(commandName, args);
```

Now we support 7 actions ： screenshot, share, hide, close, reopen, goback, forward

1. screenshot: return a screenshot by using pending Intent
2. share: return title and url by a bundle return value
3. hide: move custom tab to background task
4. close: close custom tab
5. reopen: reopen the custom tab which hide previously
6. goback: navigation back
7. forward: navigation forward
