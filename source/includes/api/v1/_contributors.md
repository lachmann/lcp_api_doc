<h1 id="api-title-contributors">Contributors</h1>

Operations about contributors

## getApiV1ContributorsId

<a id="opIdgetApiV1ContributorsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/contributors/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/contributors/{id}`

Return a Contributor

<h3 id="getapiv1contributorsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1contributorsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a Contributor|None|

## getApiV1Contributors

<a id="opIdgetApiV1Contributors"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/contributors',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/contributors`

Return all Contributors

<h3 id="getapiv1contributors-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all Contributors|None|
