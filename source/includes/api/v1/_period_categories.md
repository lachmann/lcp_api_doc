<h1 id="api-title-period_categories">Period Categories</h1>

## Get all Period Categories
`GET /api/v1/period_categories`

<a id="opIdgetApiV1PeriodCategories"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/period_categories',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1periodcategories-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all Period categories|None|

## Get a Period Category
`GET /api/v1/period_categories/{id}`

<a id="opIdgetApiV1PeriodCategoriesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/period_categories/{id}',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1periodcategoriesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1periodcategoriesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a Period category|None|
