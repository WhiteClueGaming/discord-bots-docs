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

# Set-up

Got to your bots edit page and add it there!
```js
https://<project>.<domain>/vote
```

# Example

## using package

```js
const discord = require("discord.js")
const client = new discord.Client()
const dbots = require("discord.dbl");
const dbl = new dbots("API-TOKEN-HERE", client, { autoPost: 900001 });

client.on('ready', async () => {
  dbl.Webhook() //No need to put any thing in this brackets!
})
dbl.on("voted", voter => {
  console.log(`A user with ID: ${voter} has voted me!`) //Now only you can get users ID!
})

client.login("BOT-LOGIN-TOKEN")
```

## using express.js

```js
const express = require("express")

const app = express()

app.use(express.json())


app.post("/vote", (req, res) => {
  
const voter = req.body

if (req.header('Authorization') != "your auth key you made on site") {
    return res.status("401").end();

  }

voter.id = voter.voter

console.log(voter)

//Reward code

res.status(200).end()

})

app.listen(9000) 
```


