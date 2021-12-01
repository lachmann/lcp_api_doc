<h1 id="api-title-petrographics">petrographics</h1>

Operations about petrographics

## postApiV1PetrographicsBulkInsert

<a id="opIdpostApiV1PetrographicsBulkInsert"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post 'https://www.levantineceramics.org/api/v1/petrographics/bulk_insert',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`POST /api/v1/petrographics/bulk_insert`

Bulk insert petrographics

> Body parameter

```yaml
"petrographics[item_id]":
  - string
"petrographics[thin_section_number]":
  - string
"petrographics[geological_features]":
  - string
"petrographics[soil_type]":
  - string
"petrographics[desc]":
  - string
"petrographics[matrix_type]":
  - string
"petrographics[matrix_amt]":
  - string
"petrographics[inclusion_type]":
  - string
"petrographics[inclusion_amt]":
  - string
"petrographics[voids_shape]":
  - string
"petrographics[voids_amt]":
  - string
"petrographics[ware_id]":
  - string
"petrographics[privacy_status]":
  - string
"petrographics[petrofabric_id]":
  - string
"petrographics[ware_visual_desc]":
  - string
"petrographics[petrofab_visual_desc]":
  - string
"petrographics[local_petrographic_group]":
  - string
"petrographics[vessel_id]":
  - string
"petrographics[vessel_site_id]":
  - string
"petrographics[vessel_chron]":
  - string
"petrographics[vessel_period]":
  - string
"petrographics[vessel_shape_name]":
  - string
"petrographics[vessel_functional_category_id]":
  - string
"petrographics[skip_callbacks]":
  - string
"petrographics[vessel_ware_id]":
  - string
"petrographics[vessel_petrofabric_id]":
  - string
"petrographics[acknowledgement]":
  - string

```

<h3 id="postapiv1petrographicsbulkinsert-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|object|true|none|
|» petrographics[item_id]|body|[string]|true|Item of the petrographic|
|» petrographics[thin_section_number]|body|[string]|true|Thin section number of the petrographic|
|» petrographics[geological_features]|body|[string]|false|Geological features of the petrographic|
|» petrographics[soil_type]|body|[string]|false|Soil type of the petrographic|
|» petrographics[desc]|body|[string]|false|Desc of the petrographic|
|» petrographics[matrix_type]|body|[string]|false|Matrix type of the petrographic|
|» petrographics[matrix_amt]|body|[string]|false|Matrix amt of the petrographic|
|» petrographics[inclusion_type]|body|[string]|false|Inclusion type of the petrographic|
|» petrographics[inclusion_amt]|body|[string]|false|Inclusion amt of the petrographic|
|» petrographics[voids_shape]|body|[string]|false|Voids shape of the petrographic|
|» petrographics[voids_amt]|body|[string]|false|Voids amt of the petrographic|
|» petrographics[ware_id]|body|[string]|false|Ware of the petrographic|
|» petrographics[privacy_status]|body|[string]|false|Privacy status of the petrographic|
|» petrographics[petrofabric_id]|body|[string]|false|Petrofabric of the petrographic|
|» petrographics[ware_visual_desc]|body|[string]|false|Ware visual desc of the petrographic|
|» petrographics[petrofab_visual_desc]|body|[string]|false|Petrofab visual desc of the petrographic|
|» petrographics[local_petrographic_group]|body|[string]|false|Local petrographic group of the petrographic|
|» petrographics[vessel_id]|body|[string]|false|Vessel of the petrographic|
|» petrographics[vessel_site_id]|body|[string]|false|Vessel site of the petrographic|
|» petrographics[vessel_chron]|body|[string]|false|Vessel chron of the petrographic|
|» petrographics[vessel_period]|body|[string]|false|Vessel period of the petrographic|
|» petrographics[vessel_shape_name]|body|[string]|false|Vessel shape name of the petrographic|
|» petrographics[vessel_functional_category_id]|body|[string]|false|Vessel functional category of the petrographic|
|» petrographics[skip_callbacks]|body|[string]|false|Skip callbacks of the petrographic|
|» petrographics[vessel_ware_id]|body|[string]|false|Vessel ware of the petrographic|
|» petrographics[vessel_petrofabric_id]|body|[string]|false|Vessel petrofabric of the petrographic|
|» petrographics[acknowledgement]|body|[string]|false|Acknowledgement of the petrographic|

<h3 id="postapiv1petrographicsbulkinsert-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Bulk insert petrographics|None|

## patchApiV1PetrographicsId

<a id="opIdpatchApiV1PetrographicsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.patch 'https://www.levantineceramics.org/api/v1/petrographics/{id}',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`PATCH /api/v1/petrographics/{id}`

Update a petrographic

> Body parameter

```yaml
geological_features: string
soil_type: string
desc: string
matrix_type: string
matrix_amt: string
inclusion_type: string
inclusion_amt: string
voids_shape: string
voids_amt: string
item_id: string
ware_id: string
privacy_status: string
thin_section_number: string
petrofabric_id: string
ware_visual_desc: string
petrofab_visual_desc: string
local_petrographic_group: string
vessel_id: string
vessel_site_id: string
vessel_chron: string
vessel_period: string
vessel_shape_name: string
vessel_functional_category_id: string
skip_callbacks: string
vessel_ware_id: string
vessel_petrofabric_id: string
acknowledgement: string

```

<h3 id="patchapiv1petrographicsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|
|body|body|object|false|none|
|» geological_features|body|string|false|Geological features of the petrographic|
|» soil_type|body|string|false|Soil type of the petrographic|
|» desc|body|string|false|Desc of the petrographic|
|» matrix_type|body|string|false|Matrix type of the petrographic|
|» matrix_amt|body|string|false|Matrix amt of the petrographic|
|» inclusion_type|body|string|false|Inclusion type of the petrographic|
|» inclusion_amt|body|string|false|Inclusion amt of the petrographic|
|» voids_shape|body|string|false|Voids shape of the petrographic|
|» voids_amt|body|string|false|Voids amt of the petrographic|
|» item_id|body|string|false|Item of the petrographic|
|» ware_id|body|string|false|Ware of the petrographic|
|» privacy_status|body|string|false|Privacy status of the petrographic|
|» thin_section_number|body|string|false|Thin section number of the petrographic|
|» petrofabric_id|body|string|false|Petrofabric of the petrographic|
|» ware_visual_desc|body|string|false|Ware visual desc of the petrographic|
|» petrofab_visual_desc|body|string|false|Petrofab visual desc of the petrographic|
|» local_petrographic_group|body|string|false|Local petrographic group of the petrographic|
|» vessel_id|body|string|false|Vessel of the petrographic|
|» vessel_site_id|body|string|false|Vessel site of the petrographic|
|» vessel_chron|body|string|false|Vessel chron of the petrographic|
|» vessel_period|body|string|false|Vessel period of the petrographic|
|» vessel_shape_name|body|string|false|Vessel shape name of the petrographic|
|» vessel_functional_category_id|body|string|false|Vessel functional category of the petrographic|
|» skip_callbacks|body|string|false|Skip callbacks of the petrographic|
|» vessel_ware_id|body|string|false|Vessel ware of the petrographic|
|» vessel_petrofabric_id|body|string|false|Vessel petrofabric of the petrographic|
|» acknowledgement|body|string|false|Acknowledgement of the petrographic|

<h3 id="patchapiv1petrographicsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Update a petrographic|None|

## getApiV1PetrographicsId

<a id="opIdgetApiV1PetrographicsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/petrographics/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/petrographics/{id}`

Return a petrographic

<h3 id="getapiv1petrographicsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|string|true|ID of the petrographic|

<h3 id="getapiv1petrographicsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a petrographic|None|

## postApiV1Petrographics

<a id="opIdpostApiV1Petrographics"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post 'https://www.levantineceramics.org/api/v1/petrographics',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`POST /api/v1/petrographics`

Create a petrographic

> Body parameter

```yaml
item_id: string
thin_section_number: string
geological_features: string
soil_type: string
desc: string
matrix_type: string
matrix_amt: string
inclusion_type: string
inclusion_amt: string
voids_shape: string
voids_amt: string
ware_id: string
privacy_status: string
petrofabric_id: string
ware_visual_desc: string
petrofab_visual_desc: string
local_petrographic_group: string
vessel_id: string
vessel_site_id: string
vessel_chron: string
vessel_period: string
vessel_shape_name: string
vessel_functional_category_id: string
skip_callbacks: string
vessel_ware_id: string
vessel_petrofabric_id: string
acknowledgement: string

```

<h3 id="postapiv1petrographics-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|object|true|none|
|» item_id|body|string|true|Item of the petrographic|
|» thin_section_number|body|string|true|Thin section number of the petrographic|
|» geological_features|body|string|false|Geological features of the petrographic|
|» soil_type|body|string|false|Soil type of the petrographic|
|» desc|body|string|false|Desc of the petrographic|
|» matrix_type|body|string|false|Matrix type of the petrographic|
|» matrix_amt|body|string|false|Matrix amt of the petrographic|
|» inclusion_type|body|string|false|Inclusion type of the petrographic|
|» inclusion_amt|body|string|false|Inclusion amt of the petrographic|
|» voids_shape|body|string|false|Voids shape of the petrographic|
|» voids_amt|body|string|false|Voids amt of the petrographic|
|» ware_id|body|string|false|Ware of the petrographic|
|» privacy_status|body|string|false|Privacy status of the petrographic|
|» petrofabric_id|body|string|false|Petrofabric of the petrographic|
|» ware_visual_desc|body|string|false|Ware visual desc of the petrographic|
|» petrofab_visual_desc|body|string|false|Petrofab visual desc of the petrographic|
|» local_petrographic_group|body|string|false|Local petrographic group of the petrographic|
|» vessel_id|body|string|false|Vessel of the petrographic|
|» vessel_site_id|body|string|false|Vessel site of the petrographic|
|» vessel_chron|body|string|false|Vessel chron of the petrographic|
|» vessel_period|body|string|false|Vessel period of the petrographic|
|» vessel_shape_name|body|string|false|Vessel shape name of the petrographic|
|» vessel_functional_category_id|body|string|false|Vessel functional category of the petrographic|
|» skip_callbacks|body|string|false|Skip callbacks of the petrographic|
|» vessel_ware_id|body|string|false|Vessel ware of the petrographic|
|» vessel_petrofabric_id|body|string|false|Vessel petrofabric of the petrographic|
|» acknowledgement|body|string|false|Acknowledgement of the petrographic|

<h3 id="postapiv1petrographics-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Create a petrographic|None|

## getApiV1Petrographics

<a id="opIdgetApiV1Petrographics"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/petrographics',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/petrographics`

Return all petrographics

<h3 id="getapiv1petrographics-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all petrographics|None|
