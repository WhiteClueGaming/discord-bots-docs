---
description: >-
  Bot stats for bots on DBots.ml that can be used to make graphs and cool
  things.
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

