
<h1 id="api-title-citations">Citations</h1>

Operations about citations

## getApiV1CitationsId

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

`GET /api/v1/citations/{id}`

Return a Citation

<h3 id="getapiv1citationsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1citationsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a Citation|None|

## getApiV1Citations

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

`GET /api/v1/citations`

Return all Citations

<h3 id="getapiv1citations-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all Citations|None|

