<h1 id="api-title-kilns">kilns</h1>

Operations about kilns

## patchApiV1KilnsId

<a id="opIdpatchApiV1KilnsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.patch 'https://www.levantineceramics.org/api/v1/kilns/{id}',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`PATCH /api/v1/kilns/{id}`

Update a kiln

> Body parameter

```yaml
location: string
chron: string
site_id: string
old_region_id: string
name: string
privacy_status: string
misc_box: string
period: string
start_year: string
end_year: string
workshop_location: string
acknowledgement: string
contributor_tokens: string
privacy_tokens: string
region_tokens: string
ware_tokens: string
save_version: string

```

<h3 id="patchapiv1kilnsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|
|body|body|object|false|none|
|» location|body|string|false|Location of the kiln|
|» chron|body|string|false|Chron of the kiln|
|» site_id|body|string|false|Site of the kiln|
|» old_region_id|body|string|false|Old region of the kiln|
|» name|body|string|false|Name of the kiln|
|» privacy_status|body|string|false|Privacy status of the kiln|
|» misc_box|body|string|false|Misc box of the kiln|
|» period|body|string|false|Period of the kiln|
|» start_year|body|string|false|Start year of the kiln|
|» end_year|body|string|false|End year of the kiln|
|» workshop_location|body|string|false|Workshop location of the kiln|
|» acknowledgement|body|string|false|Acknowledgement of the kiln|
|» contributor_tokens|body|string|false|Contributor tokens of the kiln|
|» privacy_tokens|body|string|false|Privacy tokens of the kiln|
|» region_tokens|body|string|false|Region tokens of the kiln|
|» ware_tokens|body|string|false|Ware tokens of the kiln|
|» save_version|body|string|false|Save version of the kiln|

<h3 id="patchapiv1kilnsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Update a kiln|None|

## getApiV1KilnsId

<a id="opIdgetApiV1KilnsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/kilns/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/kilns/{id}`

Return a kiln

<h3 id="getapiv1kilnsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|string|true|ID of the kiln|

<h3 id="getapiv1kilnsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a kiln|None|

## postApiV1Kilns

<a id="opIdpostApiV1Kilns"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post 'https://www.levantineceramics.org/api/v1/kilns',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`POST /api/v1/kilns`

Create a kiln

> Body parameter

```yaml
name: string
location: string
chron: string
site_id: string
old_region_id: string
privacy_status: string
misc_box: string
period: string
start_year: string
end_year: string
workshop_location: string
acknowledgement: string
contributor_tokens: string
privacy_tokens: string
region_tokens: string
ware_tokens: string
save_version: string

```

<h3 id="postapiv1kilns-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|object|true|none|
|» name|body|string|true|Name of the kiln|
|» location|body|string|false|Location of the kiln|
|» chron|body|string|false|Chron of the kiln|
|» site_id|body|string|false|Site of the kiln|
|» old_region_id|body|string|false|Old region of the kiln|
|» privacy_status|body|string|false|Privacy status of the kiln|
|» misc_box|body|string|false|Misc box of the kiln|
|» period|body|string|false|Period of the kiln|
|» start_year|body|string|false|Start year of the kiln|
|» end_year|body|string|false|End year of the kiln|
|» workshop_location|body|string|false|Workshop location of the kiln|
|» acknowledgement|body|string|false|Acknowledgement of the kiln|
|» contributor_tokens|body|string|false|Contributor tokens of the kiln|
|» privacy_tokens|body|string|false|Privacy tokens of the kiln|
|» region_tokens|body|string|false|Region tokens of the kiln|
|» ware_tokens|body|string|false|Ware tokens of the kiln|
|» save_version|body|string|false|Save version of the kiln|

<h3 id="postapiv1kilns-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Create a kiln|None|

## getApiV1Kilns

<a id="opIdgetApiV1Kilns"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/kilns',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/kilns`

Return all kilns

<h3 id="getapiv1kilns-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all kilns|None|
