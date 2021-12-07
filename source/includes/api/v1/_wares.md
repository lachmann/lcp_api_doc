<h1 id="api-title-wares">Wares</h1>

## List all wares
`GET /api/v1/wares`

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

> Code samples

```shell
curl "localhost:3000/api/v1/wares?page=1&per_page=5" \
  -H "Authorization: Bearer <token>"
```

<h3 id="getapiv1wares-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all wares|None|

## Get a ware
`GET /api/v1/wares/{id}`

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

```shell
curl "localhost:3000/api/v1/wares/:id" \
  -H "Authorization: Bearer <token>"
```

<h3 id="getapiv1waresid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|string|true|ID of the ware|

<h3 id="getapiv1waresid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a ware|None|

## Create a ware
`POST /api/v1/wares`

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

```shell
curl -X POST "localhost:3000/api/v1/wares" \
  -H "Authorization: Bearer <token>" \
  -H "Content-Type: application/json" \
  -d '{ "name": "A mistery ware", "alternative_name": "Alternative name", "definition": "Magical", "desc": "Name", "chron_range": "Once upon a time", "period": "", "privacy_status": 1,"acknowledgement": "Found by X", "save_version": false }'
```

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
save_version: boolean

```

<h3 id="postapiv1wares-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|name|body|string|true|Name of the ware|
|alternative_name|body|string|false|Alternative name of the ware|
|definition|body|string|false|Definition of the ware|
|desc|body|string|false|Desc of the ware|
|chron_range|body|string|false|Chron range of the ware|
|period|body|string|false|Period of the ware|
|privacy_status|body|string|false|Privacy status of the ware|
|acknowledgement|body|string|false|Acknowledgement of the ware|
|save_version|body|boolean|false|Save version of the ware|

<h3 id="postapiv1wares-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Create a ware|None|

## Update a ware
`PATCH /api/v1/wares/{id}`

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
```shell
curl -X PATCH "localhost:3000/api/v1/wares/:id" \
  -H "Authorization: Bearer <token>" \
  -H "Content-Type: application/json" \
  -d '{ "name": "New name", "alternative_name": "New Alternative name", "definition": "Magical", "desc": "Name", "chron_range": "Once upon a time", "period": "", "privacy_status": 1,"acknowledgement": "Found by X", "save_version": false }'
```

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
|name|body|string|false|Name of the ware|
|alternative_name|body|string|false|Alternative name of the ware|
|definition|body|string|false|Definition of the ware|
|desc|body|string|false|Desc of the ware|
|chron_range|body|string|false|Chron range of the ware|
|period|body|string|false|Period of the ware|
|privacy_status|body|string|false|Privacy status of the ware|
|acknowledgement|body|string|false|Acknowledgement of the ware|
|save_version|body|boolean|false|Save version of the ware|

<h3 id="patchapiv1waresid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Update a ware|None|
