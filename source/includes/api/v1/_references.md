<h1 id="api-title-references">References</h1>

## List all References
`GET /api/v1/references`

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

<h3 id="getapiv1references-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all references|None|

## Get a Reference
`GET /api/v1/references/{id}`

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

<h3 id="getapiv1referencesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1referencesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a reference|None|
