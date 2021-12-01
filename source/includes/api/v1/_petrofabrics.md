<h1 id="api-title-petrofabrics">petrofabrics</h1>

Operations about petrofabrics

## patchApiV1PetrofabricsId

<a id="opIdpatchApiV1PetrofabricsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.patch 'https://www.levantineceramics.org/api/v1/petrofabrics/{id}',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`PATCH /api/v1/petrofabrics/{id}`

Update a petrofabric

> Body parameter

```yaml
name: string
desc: string
petrographic_id: string
raw_material: string
geo_form: string
privacy_status: string
ware_id: string
workshop_id: string
start_year: string
end_year: string
definition: string
acknowledgement: string
save_version: string

```

<h3 id="patchapiv1petrofabricsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|string|true|Id of the petrofabric|
|body|body|object|false|none|
|» name|body|string|false|Name of the petrofabric|
|» desc|body|string|false|Desc of the petrofabric|
|» petrographic_id|body|string|false|Petrographic of the petrofabric|
|» raw_material|body|string|false|Raw material of the petrofabric|
|» geo_form|body|string|false|Geo form of the petrofabric|
|» privacy_status|body|string|false|Privacy status of the petrofabric|
|» ware_id|body|string|false|Ware of the petrofabric|
|» workshop_id|body|string|false|Workshop of the petrofabric|
|» start_year|body|string|false|Start year of the petrofabric|
|» end_year|body|string|false|End year of the petrofabric|
|» definition|body|string|false|Definition of the petrofabric|
|» acknowledgement|body|string|false|Acknowledgement of the petrofabric|
|» save_version|body|string|false|Save version of the petrofabric|

<h3 id="patchapiv1petrofabricsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Update a petrofabric|None|

## getApiV1PetrofabricsId

<a id="opIdgetApiV1PetrofabricsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/petrofabrics/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/petrofabrics/{id}`

Return a petrofabric

<h3 id="getapiv1petrofabricsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|string|true|ID of the petrofabric|

<h3 id="getapiv1petrofabricsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a petrofabric|None|

## postApiV1Petrofabrics

<a id="opIdpostApiV1Petrofabrics"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post 'https://www.levantineceramics.org/api/v1/petrofabrics',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`POST /api/v1/petrofabrics`

Create a petrofabric

> Body parameter

```yaml
name: string
id: string
desc: string
petrographic_id: string
raw_material: string
geo_form: string
privacy_status: string
ware_id: string
workshop_id: string
start_year: string
end_year: string
definition: string
acknowledgement: string
save_version: string

```

<h3 id="postapiv1petrofabrics-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|object|true|none|
|» name|body|string|true|Name of the petrofabric|
|» id|body|string|false|Id of the petrofabric|
|» desc|body|string|false|Desc of the petrofabric|
|» petrographic_id|body|string|false|Petrographic of the petrofabric|
|» raw_material|body|string|false|Raw material of the petrofabric|
|» geo_form|body|string|false|Geo form of the petrofabric|
|» privacy_status|body|string|false|Privacy status of the petrofabric|
|» ware_id|body|string|false|Ware of the petrofabric|
|» workshop_id|body|string|false|Workshop of the petrofabric|
|» start_year|body|string|false|Start year of the petrofabric|
|» end_year|body|string|false|End year of the petrofabric|
|» definition|body|string|false|Definition of the petrofabric|
|» acknowledgement|body|string|false|Acknowledgement of the petrofabric|
|» save_version|body|string|false|Save version of the petrofabric|

<h3 id="postapiv1petrofabrics-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Create a petrofabric|None|

## getApiV1Petrofabrics

<a id="opIdgetApiV1Petrofabrics"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/petrofabrics',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/petrofabrics`

Return all petrofabrics

<h3 id="getapiv1petrofabrics-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all petrofabrics|None|
