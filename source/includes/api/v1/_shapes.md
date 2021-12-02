
<h1 id="api-title-shapes">Shapes</h1>

## List all Shapes
`GET /api/v1/shapes`

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

<h3 id="getapiv1shapes-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all shapes|None|

## Get a Shape
`GET /api/v1/shapes/{id}`

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

<h3 id="getapiv1shapesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1shapesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a shape|None|
