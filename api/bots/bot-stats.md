---
description: >-
  Bot stats for bots on discordz that can be used to make graphs and cool
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
const dbots = require("discord.dbl");
const dbl = new dbots("API-TOKEN-HERE", client, { autoPost: 900001 });
//Note: you will get Api token on your bots edit page!

client.on("ready", async () => {
  dbl.postStats(); => Note: You can only use this package for discord.js use
  // console.log("Server count posted")
  
  let hasVote = await dbl.hasVoted("714451348212678658");
  if(hasVote === true) {
    console.log("Voted")
  } else {
    console.log("Vote please.")
  }
  
  
  let search = await dbl.search("BOT-ID")
  console.log(search)
  
});
```

