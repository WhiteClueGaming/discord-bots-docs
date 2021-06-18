---
description: >-
  Bot stats for bots on DBots.ml that can be used to make graphs and cool
  things.
---

# Bot Stats

{% api-method method="post" host="https://dbots.ml/api/bots/stats" path="/api/bots/stats" %}
{% api-method-summary %}
Post Bot Stats
{% endapi-method-summary %}

{% api-method-description %}
Get stats of a specific bot. Must provide bot API token.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=true %}
ID of the bot.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
API Token of the bot. 
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Returns updated bot stats.
{% endapi-method-response-example-description %}

```javascript
{ serverCount: number, shardCount: number}
```
