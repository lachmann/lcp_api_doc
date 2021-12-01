<h1 id="api-title-wares">Ware</h1>

Operations about wares

## patchApiV1WaresId

<a id="opIdpatchApiV1WaresId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.patch 'https://www.levantineceramics.org/api/v1/wares/{id}',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`PATCH /api/v1/wares/{id}`

Update a ware

> Body parameter

```yaml
name: string
alternative_name: string
definition: string
desc: string
chron_range: string
period: string
privacy_status: string
acknowledgement: string
save_version: string

```

<h3 id="patchapiv1waresid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|
|body|body|object|false|none|
|» name|body|string|false|Name of the ware|
|» alternative_name|body|string|false|Alternative name of the ware|
|» definition|body|string|false|Definition of the ware|
|» desc|body|string|false|Desc of the ware|
|» chron_range|body|string|false|Chron range of the ware|
|» period|body|string|false|Period of the ware|
|» privacy_status|body|string|false|Privacy status of the ware|
|» acknowledgement|body|string|false|Acknowledgement of the ware|
|» save_version|body|string|false|Save version of the ware|

<h3 id="patchapiv1waresid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Update a ware|None|

## getApiV1WaresId

<a id="opIdgetApiV1WaresId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/wares/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/wares/{id}`

Return a ware

<h3 id="getapiv1waresid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|string|true|ID of the ware|

<h3 id="getapiv1waresid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a ware|None|

## postApiV1Wares

<a id="opIdpostApiV1Wares"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post 'https://www.levantineceramics.org/api/v1/wares',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`POST /api/v1/wares`

Create a ware

> Body parameter

```yaml
name: string
alternative_name: string
definition: string
desc: string
chron_range: string
period: string
privacy_status: string
acknowledgement: string
save_version: string

```

<h3 id="postapiv1wares-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|object|true|none|
|» name|body|string|true|Name of the ware|
|» alternative_name|body|string|false|Alternative name of the ware|
|» definition|body|string|false|Definition of the ware|
|» desc|body|string|false|Desc of the ware|
|» chron_range|body|string|false|Chron range of the ware|
|» period|body|string|false|Period of the ware|
|» privacy_status|body|string|false|Privacy status of the ware|
|» acknowledgement|body|string|false|Acknowledgement of the ware|
|» save_version|body|string|false|Save version of the ware|

<h3 id="postapiv1wares-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Create a ware|None|

## getApiV1Wares

<a id="opIdgetApiV1Wares"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/wares',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/wares`

Return all wares

<h3 id="getapiv1wares-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all wares|None|