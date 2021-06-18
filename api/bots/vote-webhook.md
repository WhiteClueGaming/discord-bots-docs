---
description: >-
  Track that who voted for your discord bot using the vote tracker!
---

# Bot Stats

Npm package: https://www.npmjs.com/package/discord.dbl

Install our npm package!

```js
npm i discord.dbl
```

# Example

```js
const express = require("express")
const app = express()

client.on("ready", async () => {
  console.log("bot online")
});

app.post("/dblwebhook", async (req,res) => {
const voter = req.header('voterID')
console.log(voter) //it will log the user ID
})

```

