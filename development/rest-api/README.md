# REST API Overview

**This section contains the documentations for Classifai REST APIs.** 

All API access is over HTTP, and accessed from [http://localhost:{port}](http://localhost:9999). All data is send and received as JSON. 

If you have any problems or requests, do contact us through

1. [Classifai Discord Community Support](https://discord.com/invite/WsBFgNP)
2. Email _hello@classifai.ai_

## **Example** 

{% api-method method="get" host="http://localhost:{port}" path="/bndbox/projects" %}
{% api-method-summary %}
Get a list of bounding box projects
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
**- message:** integer  
          - 1 for success , 0 for failure  
**- content:** list of strings
{% endapi-method-response-example-description %}

```
{
    "message": 1,
    "content": [
        "abc",
        "def",
        "ghi"
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}







