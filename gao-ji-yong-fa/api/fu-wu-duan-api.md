---
description: '通过网络请求与 PAGENOTE 服务器进行数据交互。服务器地址：https://api.pagenote.cn'
---

# 服务端 API

{% api-method method="get" host="/api/signin" path="" %}
{% api-method-summary %}
 登录
{% endapi-method-summary %}

{% api-method-description %}
 根据用户名、密码换取身份凭证
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-form-data-parameters %}
{% api-method-parameter name="username" type="string" required=true %}
 用户名
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=true %}
 密码
{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

