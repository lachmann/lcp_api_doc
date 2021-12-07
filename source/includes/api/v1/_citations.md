
<h1 id="api-title-citations">Citations</h1>

## Get all Citations
`GET /api/v1/citations`

<a id="opIdgetApiV1Citations"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/citations',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1citations-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all Citations|None|

## Get a Citation
`GET /api/v1/citations/{id}`

<a id="opIdgetApiV1CitationsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/citations/{id}',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1citationsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1citationsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a Citation|None|
