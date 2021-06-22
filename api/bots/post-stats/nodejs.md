---
description: 'How to post stats using Node.js or JavaScript
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

Simple package to easily post stats to [dbots.ml](https://dbots.ml). 

### NodeJS

```javascript
const dbots = require("discord.dbl");
const dbl = new dbots("API-TOKEN-HERE", client, { autoPost: 900001 });

client.on("ready", async () => {
  dbl.postStats(); => Note: You can only use this package for discord.js use
  // console.log("Server count posted")
  
});
```


