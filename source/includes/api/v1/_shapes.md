
<h1 id="api-title-shapes">shapes</h1>

Operations about shapes

## getApiV1ShapesId

<a id="opIdgetApiV1ShapesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/shapes/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/shapes/{id}`

Return a shape

<h3 id="getapiv1shapesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1shapesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a shape|None|

## getApiV1Shapes

<a id="opIdgetApiV1Shapes"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/shapes',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/shapes`

Return all shapes

<h3 id="getapiv1shapes-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all shapes|None|
