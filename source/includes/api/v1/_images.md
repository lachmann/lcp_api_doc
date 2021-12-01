<h1 id="api-title-images">images</h1>

Operations about images

## getApiV1ImagesId

<a id="opIdgetApiV1ImagesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/images/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/images/{id}`

Return a Image

<h3 id="getapiv1imagesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1imagesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a Image|None|

## getApiV1Images

<a id="opIdgetApiV1Images"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/images',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/images`

Return all Images

<h3 id="getapiv1images-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all Images|None|
