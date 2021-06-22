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
headers = {
  'Authorization': 'Your Authorization Bot Token you will get this in bot edit page at down!',
  'serverCount': 'Your Bot's Servers Count', //if you also have shards put shardCount: count below serverCount!
  'Content-Type': 'application/json'
}

response = requests.request("POST", "https://dbots.ml/api/bots/stats", headers=headers)
print(response.text.encode('utf8'))
```


