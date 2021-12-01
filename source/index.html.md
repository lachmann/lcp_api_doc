---
title: API v1
language_tabs:
  - ruby: Ruby
  - curl: Shell
language_clients:
  - ruby: ""
  - curl: ""
toc_footers: []
includes: [
  api/v1/wares,
  api/v1/petrographics,
  api/v1/kilns,
  api/v1/shapes,
  api/v1/sites,
  api/v1/references,
  api/v1/periods,
  api/v1/period_categories,
  api/v1/images,
  api/v1/functional_categories,
  api/v1/contributors,
  api/v1/citations
]
search: true
highlight_theme: darkula
headingLevel: 2

---

<!-- Generator: Widdershins v4.0.1 -->

<h1 id="api-title">API v1</h1>

> Scroll down for code samples, example requests and responses. Select a language for code samples from the tabs above or the mobile navigation menu.

Base URLs:

* <a href="https://www.levantineceramics.org/">https://www.levantineceramics.org/</a>

<h1 id="authentitation">Introduction</h1>
_The Levantine Ceramics Project_ (LCP) is an open, interactive website focused on ceramics produced in the Levant from the Neolithic era (c. 5500 B.C.E.) through the Ottoman period (c. 1920 C.E.). Here you can submit and find information—whether long published or newly discovered—about ceramic wares, shapes, specific vessels, scientific analyses, kiln sites, and chronology. The LCP makes it simple to access, share, use, and refine data, to link scholars and to foster collaborative research. **Watch a brief video about the LCP** [here](https://www.youtube.com/watch?v=kFk_7f4B1vY).

<h1 id="authentitation">Authentication</h1>
<aside class="warning">
  Every endpoint requires authentiation
</aside>

The Levantine Ceramics Project expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: Bearer <token>`

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

result = RestClient.post 'https://www.levantineceramics.org/api/v1/vessels/bulk_insert',
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

## patchApiV1VesselsId

<a id="opIdpatchApiV1VesselsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.patch 'https://www.levantineceramics.org/api/v1/vessels/{id}',
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

## getApiV1VesselsId

<a id="opIdgetApiV1VesselsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/vessels/{id}',
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

## postApiV1Vessels

<a id="opIdpostApiV1Vessels"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/x-www-form-urlencoded'
}

result = RestClient.post 'https://www.levantineceramics.org/api/v1/vessels',
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

## getApiV1Vessels

<a id="opIdgetApiV1Vessels"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/vessels',
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
