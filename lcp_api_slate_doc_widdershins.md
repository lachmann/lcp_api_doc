---
title: API title v0.0.1
language_tabs:
  - ruby: Ruby
  - curl: Shell
language_clients:
  - ruby: ""
  - curl: ""
toc_footers: []
includes: []
search: true
highlight_theme: darkula
headingLevel: 2

---

<!-- Generator: Widdershins v4.0.1 -->

<h1 id="api-title">API title v0.0.1</h1>

> Scroll down for code samples, example requests and responses. Select a language for code samples from the tabs above or the mobile navigation menu.

Base URLs:

* <a href="//localhost:3000">//localhost:3000</a>

<h1 id="api-title-wares">wares</h1>

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

result = RestClient.patch '/localhost:3000/api/v1/wares/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1WaresId

<a id="opIdgetApiV1WaresId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/wares/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## postApiV1Wares

<a id="opIdpostApiV1Wares"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post '/localhost:3000/api/v1/wares',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Wares

<a id="opIdgetApiV1Wares"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/wares',
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

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-vessels">vessels</h1>

Operations about vessels

## postApiV1VesselsBulkInsert

<a id="opIdpostApiV1VesselsBulkInsert"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post '/localhost:3000/api/v1/vessels/bulk_insert',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`POST /api/v1/vessels/bulk_insert`

Bulk insert vessels

> Body parameter

```yaml
"vessels[inventory_number]":
  - string
"vessels[ware_id]":
  - string
"vessels[petrofabric_id]":
  - string
"vessels[petrofab_name]":
  - string
"vessels[petrofab_visual_desc]":
  - string
"vessels[chron]":
  - string
"vessels[period]":
  - string
"vessels[manu_tech]":
  - string
"vessels[region_tokens]":
  - string
"vessels[site_type]":
  - string
"vessels[arch_context]":
  - string
"vessels[shape_name]":
  - string
"vessels[shape_rtype]":
  - string
"vessels[site_id]":
  - string
"vessels[shape_sub_group]":
  - string
"vessels[functional_category_id]":
  - string
"vessels[height]":
  - string
"vessels[preserved_height]":
  - string
"vessels[true_height]":
  - string
"vessels[max_diameter]":
  - string
"vessels[estimated_max_diameter]":
  - string
"vessels[true_max_diameter]":
  - string
"vessels[diameter_rim]":
  - string
"vessels[estimated_diameter_rim]":
  - string
"vessels[true_diameter_rim]":
  - string
"vessels[diameter_base]":
  - string
"vessels[estimated_diameter_base]":
  - string
"vessels[true_diameter_base]":
  - string
"vessels[thickness]":
  - string
"vessels[color]":
  - string
"vessels[firing]":
  - string
"vessels[surface_treatment]":
  - string
"vessels[contributor_tokens]":
  - string
"vessels[privacy_status]":
  - string
"vessels[privacy_tokens]":
  - string
"vessels[acknowledgement]":
  - string
"vessels[shape_id]":
  - string

```

<h3 id="postapiv1vesselsbulkinsert-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|object|true|none|
|» vessels[inventory_number]|body|[string]|true|Inventory number of the vessel|
|» vessels[ware_id]|body|[string]|false|Ware of the vessel|
|» vessels[petrofabric_id]|body|[string]|false|Petrofabric of the vessel|
|» vessels[petrofab_name]|body|[string]|false|Petrofab name of the vessel|
|» vessels[petrofab_visual_desc]|body|[string]|false|Petrofab visual desc of the vessel|
|» vessels[chron]|body|[string]|false|Chron of the vessel|
|» vessels[period]|body|[string]|false|Period of the vessel|
|» vessels[manu_tech]|body|[string]|false|Manu tech of the vessel|
|» vessels[region_tokens]|body|[string]|false|Region tokens of the vessel|
|» vessels[site_type]|body|[string]|false|Site type of the vessel|
|» vessels[arch_context]|body|[string]|false|Arch context of the vessel|
|» vessels[shape_name]|body|[string]|false|Shape name of the vessel|
|» vessels[shape_rtype]|body|[string]|false|Shape rtype of the vessel|
|» vessels[site_id]|body|[string]|false|Site of the vessel|
|» vessels[shape_sub_group]|body|[string]|false|Shape sub group of the vessel|
|» vessels[functional_category_id]|body|[string]|false|Functional category of the vessel|
|» vessels[height]|body|[string]|false|Height of the vessel|
|» vessels[preserved_height]|body|[string]|false|Preserved height of the vessel|
|» vessels[true_height]|body|[string]|false|True height of the vessel|
|» vessels[max_diameter]|body|[string]|false|Max diameter of the vessel|
|» vessels[estimated_max_diameter]|body|[string]|false|Estimated max diameter of the vessel|
|» vessels[true_max_diameter]|body|[string]|false|True max diameter of the vessel|
|» vessels[diameter_rim]|body|[string]|false|Diameter rim of the vessel|
|» vessels[estimated_diameter_rim]|body|[string]|false|Estimated diameter rim of the vessel|
|» vessels[true_diameter_rim]|body|[string]|false|True diameter rim of the vessel|
|» vessels[diameter_base]|body|[string]|false|Diameter base of the vessel|
|» vessels[estimated_diameter_base]|body|[string]|false|Estimated diameter base of the vessel|
|» vessels[true_diameter_base]|body|[string]|false|True diameter base of the vessel|
|» vessels[thickness]|body|[string]|false|Thickness of the vessel|
|» vessels[color]|body|[string]|false|Color of the vessel|
|» vessels[firing]|body|[string]|false|Firing of the vessel|
|» vessels[surface_treatment]|body|[string]|false|Surface treatment of the vessel|
|» vessels[contributor_tokens]|body|[string]|false|Contributor tokens of the vessel|
|» vessels[privacy_status]|body|[string]|false|Privacy status of the vessel|
|» vessels[privacy_tokens]|body|[string]|false|Privacy tokens of the vessel|
|» vessels[acknowledgement]|body|[string]|false|Acknowledgement of the vessel|
|» vessels[shape_id]|body|[string]|false|Shape of the vessel|

<h3 id="postapiv1vesselsbulkinsert-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Bulk insert vessels|None|

<aside class="success">
This operation does not require authentication
</aside>

## patchApiV1VesselsId

<a id="opIdpatchApiV1VesselsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.patch '/localhost:3000/api/v1/vessels/{id}',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`PATCH /api/v1/vessels/{id}`

Update a vessel

> Body parameter

```yaml
ware_id: string
petrofabric_id: string
petrofab_name: string
petrofab_visual_desc: string
chron: string
period: string
manu_tech:
  - string
inventory_number: string
region_tokens: string
site_type: string
arch_context: string
shape_name: string
shape_rtype: string
site_id: string
shape_sub_group: string
functional_category_id: string
height: string
preserved_height: string
true_height: string
max_diameter: string
estimated_max_diameter: string
true_max_diameter: string
diameter_rim: string
estimated_diameter_rim: string
true_diameter_rim: string
diameter_base: string
estimated_diameter_base: string
true_diameter_base: string
thickness: string
color: string
firing: string
surface_treatment: string
contributor_tokens: string
privacy_status: string
privacy_tokens: string
acknowledgement: string
shape_id: string

```

<h3 id="patchapiv1vesselsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|
|body|body|object|false|none|
|» ware_id|body|string|false|Ware of the vessel|
|» petrofabric_id|body|string|false|Petrofabric of the vessel|
|» petrofab_name|body|string|false|Petrofab name of the vessel|
|» petrofab_visual_desc|body|string|false|Petrofab visual desc of the vessel|
|» chron|body|string|false|Chron of the vessel|
|» period|body|string|false|Period of the vessel|
|» manu_tech|body|[string]|false|Manu tech of the vessel|
|» inventory_number|body|string|false|Inventory number of the vessel|
|» region_tokens|body|string|false|Region tokens of the vessel|
|» site_type|body|string|false|Site type of the vessel|
|» arch_context|body|string|false|Arch context of the vessel|
|» shape_name|body|string|false|Shape name of the vessel|
|» shape_rtype|body|string|false|Shape rtype of the vessel|
|» site_id|body|string|false|Site of the vessel|
|» shape_sub_group|body|string|false|Shape sub group of the vessel|
|» functional_category_id|body|string|false|Functional category of the vessel|
|» height|body|string|false|Height of the vessel|
|» preserved_height|body|string|false|Preserved height of the vessel|
|» true_height|body|string|false|True height of the vessel|
|» max_diameter|body|string|false|Max diameter of the vessel|
|» estimated_max_diameter|body|string|false|Estimated max diameter of the vessel|
|» true_max_diameter|body|string|false|True max diameter of the vessel|
|» diameter_rim|body|string|false|Diameter rim of the vessel|
|» estimated_diameter_rim|body|string|false|Estimated diameter rim of the vessel|
|» true_diameter_rim|body|string|false|True diameter rim of the vessel|
|» diameter_base|body|string|false|Diameter base of the vessel|
|» estimated_diameter_base|body|string|false|Estimated diameter base of the vessel|
|» true_diameter_base|body|string|false|True diameter base of the vessel|
|» thickness|body|string|false|Thickness of the vessel|
|» color|body|string|false|Color of the vessel|
|» firing|body|string|false|Firing of the vessel|
|» surface_treatment|body|string|false|Surface treatment of the vessel|
|» contributor_tokens|body|string|false|Contributor tokens of the vessel|
|» privacy_status|body|string|false|Privacy status of the vessel|
|» privacy_tokens|body|string|false|Privacy tokens of the vessel|
|» acknowledgement|body|string|false|Acknowledgement of the vessel|
|» shape_id|body|string|false|Shape of the vessel|

<h3 id="patchapiv1vesselsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Update a vessel|None|

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1VesselsId

<a id="opIdgetApiV1VesselsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/vessels/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/vessels/{id}`

Return a vessel

<h3 id="getapiv1vesselsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|string|true|ID of the vessel|

<h3 id="getapiv1vesselsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a vessel|None|

<aside class="success">
This operation does not require authentication
</aside>

## postApiV1Vessels

<a id="opIdpostApiV1Vessels"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post '/localhost:3000/api/v1/vessels',
  params: {
  }, headers: headers

p JSON.parse(result)

```

`POST /api/v1/vessels`

Create a vessel

> Body parameter

```yaml
inventory_number: string
ware_id: string
petrofabric_id: string
petrofab_name: string
petrofab_visual_desc: string
chron: string
period: string
manu_tech:
  - string
region_tokens: string
site_type: string
arch_context: string
shape_name: string
shape_rtype: string
site_id: string
shape_sub_group: string
functional_category_id: string
height: string
preserved_height: string
true_height: string
max_diameter: string
estimated_max_diameter: string
true_max_diameter: string
diameter_rim: string
estimated_diameter_rim: string
true_diameter_rim: string
diameter_base: string
estimated_diameter_base: string
true_diameter_base: string
thickness: string
color: string
firing: string
surface_treatment: string
contributor_tokens: string
privacy_status: string
privacy_tokens: string
acknowledgement: string
shape_id: string

```

<h3 id="postapiv1vessels-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|object|true|none|
|» inventory_number|body|string|true|Inventory number of the vessel|
|» ware_id|body|string|false|Ware of the vessel|
|» petrofabric_id|body|string|false|Petrofabric of the vessel|
|» petrofab_name|body|string|false|Petrofab name of the vessel|
|» petrofab_visual_desc|body|string|false|Petrofab visual desc of the vessel|
|» chron|body|string|false|Chron of the vessel|
|» period|body|string|false|Period of the vessel|
|» manu_tech|body|[string]|false|Manu tech of the vessel|
|» region_tokens|body|string|false|Region tokens of the vessel|
|» site_type|body|string|false|Site type of the vessel|
|» arch_context|body|string|false|Arch context of the vessel|
|» shape_name|body|string|false|Shape name of the vessel|
|» shape_rtype|body|string|false|Shape rtype of the vessel|
|» site_id|body|string|false|Site of the vessel|
|» shape_sub_group|body|string|false|Shape sub group of the vessel|
|» functional_category_id|body|string|false|Functional category of the vessel|
|» height|body|string|false|Height of the vessel|
|» preserved_height|body|string|false|Preserved height of the vessel|
|» true_height|body|string|false|True height of the vessel|
|» max_diameter|body|string|false|Max diameter of the vessel|
|» estimated_max_diameter|body|string|false|Estimated max diameter of the vessel|
|» true_max_diameter|body|string|false|True max diameter of the vessel|
|» diameter_rim|body|string|false|Diameter rim of the vessel|
|» estimated_diameter_rim|body|string|false|Estimated diameter rim of the vessel|
|» true_diameter_rim|body|string|false|True diameter rim of the vessel|
|» diameter_base|body|string|false|Diameter base of the vessel|
|» estimated_diameter_base|body|string|false|Estimated diameter base of the vessel|
|» true_diameter_base|body|string|false|True diameter base of the vessel|
|» thickness|body|string|false|Thickness of the vessel|
|» color|body|string|false|Color of the vessel|
|» firing|body|string|false|Firing of the vessel|
|» surface_treatment|body|string|false|Surface treatment of the vessel|
|» contributor_tokens|body|string|false|Contributor tokens of the vessel|
|» privacy_status|body|string|false|Privacy status of the vessel|
|» privacy_tokens|body|string|false|Privacy tokens of the vessel|
|» acknowledgement|body|string|false|Acknowledgement of the vessel|
|» shape_id|body|string|false|Shape of the vessel|

<h3 id="postapiv1vessels-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Create a vessel|None|

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Vessels

<a id="opIdgetApiV1Vessels"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/vessels',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/vessels`

Return all vessels

<h3 id="getapiv1vessels-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all vessels|None|

<aside class="success">
This operation does not require authentication
</aside>

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

result = RestClient.post '/localhost:3000/api/v1/petrographics/bulk_insert',
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

<aside class="success">
This operation does not require authentication
</aside>

## patchApiV1PetrographicsId

<a id="opIdpatchApiV1PetrographicsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.patch '/localhost:3000/api/v1/petrographics/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1PetrographicsId

<a id="opIdgetApiV1PetrographicsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/petrographics/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## postApiV1Petrographics

<a id="opIdpostApiV1Petrographics"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post '/localhost:3000/api/v1/petrographics',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Petrographics

<a id="opIdgetApiV1Petrographics"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/petrographics',
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

<aside class="success">
This operation does not require authentication
</aside>

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

result = RestClient.patch '/localhost:3000/api/v1/kilns/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1KilnsId

<a id="opIdgetApiV1KilnsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/kilns/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## postApiV1Kilns

<a id="opIdpostApiV1Kilns"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post '/localhost:3000/api/v1/kilns',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Kilns

<a id="opIdgetApiV1Kilns"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/kilns',
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

<aside class="success">
This operation does not require authentication
</aside>

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

result = RestClient.patch '/localhost:3000/api/v1/petrofabrics/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1PetrofabricsId

<a id="opIdgetApiV1PetrofabricsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/petrofabrics/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## postApiV1Petrofabrics

<a id="opIdpostApiV1Petrofabrics"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post '/localhost:3000/api/v1/petrofabrics',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Petrofabrics

<a id="opIdgetApiV1Petrofabrics"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/petrofabrics',
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

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-shapes">shapes</h1>

Operations about shapes

## getApiV1ShapesId

<a id="opIdgetApiV1ShapesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/shapes/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Shapes

<a id="opIdgetApiV1Shapes"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/shapes',
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

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-sites">sites</h1>

Operations about sites

## getApiV1SitesId

<a id="opIdgetApiV1SitesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/sites/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/sites/{id}`

Return a site

<h3 id="getapiv1sitesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1sitesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a site|None|

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Sites

<a id="opIdgetApiV1Sites"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/sites',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/sites`

Return all sites

<h3 id="getapiv1sites-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all sites|None|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-references">references</h1>

Operations about references

## getApiV1ReferencesId

<a id="opIdgetApiV1ReferencesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/references/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/references/{id}`

Return a reference

<h3 id="getapiv1referencesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1referencesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a reference|None|

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1References

<a id="opIdgetApiV1References"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/references',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/references`

Return all references

<h3 id="getapiv1references-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all references|None|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-periods">periods</h1>

Operations about periods

## getApiV1PeriodsId

<a id="opIdgetApiV1PeriodsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/periods/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/periods/{id}`

Return a period

<h3 id="getapiv1periodsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1periodsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a period|None|

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Periods

<a id="opIdgetApiV1Periods"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/periods',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/periods`

Return all periods

<h3 id="getapiv1periods-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all periods|None|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-period_categories">period_categories</h1>

Operations about period_categories

## getApiV1PeriodCategoriesId

<a id="opIdgetApiV1PeriodCategoriesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/period_categories/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/period_categories/{id}`

Return a Period category

<h3 id="getapiv1periodcategoriesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1periodcategoriesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a Period category|None|

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1PeriodCategories

<a id="opIdgetApiV1PeriodCategories"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/period_categories',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/period_categories`

Return all Period categories

<h3 id="getapiv1periodcategories-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all Period categories|None|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-images">images</h1>

Operations about images

## getApiV1ImagesId

<a id="opIdgetApiV1ImagesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/images/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Images

<a id="opIdgetApiV1Images"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/images',
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

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-functional_categories">functional_categories</h1>

Operations about functional_categories

## getApiV1FunctionalCategoriesId

<a id="opIdgetApiV1FunctionalCategoriesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/functional_categories/{id}',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/functional_categories/{id}`

Return a Functional category

<h3 id="getapiv1functionalcategoriesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1functionalcategoriesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a Functional category|None|

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1FunctionalCategories

<a id="opIdgetApiV1FunctionalCategories"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/functional_categories',
  params: {
  }

p JSON.parse(result)

```

`GET /api/v1/functional_categories`

Return all Functional categories

<h3 id="getapiv1functionalcategories-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all Functional categories|None|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-contributors">contributors</h1>

Operations about contributors

## getApiV1ContributorsId

<a id="opIdgetApiV1ContributorsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/contributors/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Contributors

<a id="opIdgetApiV1Contributors"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/contributors',
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

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-title-citations">citations</h1>

Operations about citations

## getApiV1CitationsId

<a id="opIdgetApiV1CitationsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/citations/{id}',
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

<aside class="success">
This operation does not require authentication
</aside>

## getApiV1Citations

<a id="opIdgetApiV1Citations"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get '/localhost:3000/api/v1/citations',
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

<aside class="success">
This operation does not require authentication
</aside>

