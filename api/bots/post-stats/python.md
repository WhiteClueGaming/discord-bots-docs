---
description: 'How to post stats using Python!
---

# Python

## Install the Package

Install the package named requests

{% hint style="info" %}
 Make sure to install the latest version for the latest updates and also have discord.py package.
{% endhint %}

### Python

```py
import requests
botid: int = 1234567890987654321
req = requests.post(
  f'https://api.discordz.gg/bot/{botid}/stats', 
  headers={'Content-Type':'application/json', 'Authorization': "Auth Token"},
  data={"server_count": 0, "shard_count": 0, "user_count": 0}
)
print(req.json())
```


