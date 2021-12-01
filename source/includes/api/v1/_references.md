<h1 id="api-title-references">references</h1>

Operations about references

## getApiV1ReferencesId

<a id="opIdgetApiV1ReferencesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/references/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/references/{id}`

Return a reference

<h3 id="getapiv1referencesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1referencesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a reference|None|

## getApiV1References

<a id="opIdgetApiV1References"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/references',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/references`

Return all references

<h3 id="getapiv1references-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all references|None|
