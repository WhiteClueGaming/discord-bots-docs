---
description: 'How to post stats using Node.js (JavaScript)
---

# Node.js

## Install the Package

Install the package using NPM:

```
$ npm i discord.dbl
```

{% hint style="info" %}
 Make sure to install the latest version for the latest updates and also have discord.js package.
{% endhint %}

Simple package to easily post stats to [discordz](https://discordz.gg). 

### Direct

**With Body**

```
require("node-fetch")(`https://api.discordz.gg/bot/:botID/stats`, {
        method: 'POST',
        headers: { 
          'Content-Type': 'application/json', 
          'Authorization': "Auth Token"
        },
        body: JSON.stringify({"server_count": 0, "shard_count": 0, "user_count": 0 })
    })
```

### NodeJS

```javascript
const dbots = require("discord.dbl");
const dbl = new dbots("API-TOKEN-HERE", client, { autoPost: 900001 });

client.on("ready", async () => {
  dbl.postStats(); => Note: You can only use this package for discord.js use
  // console.log("Server count posted")
  
});
```


