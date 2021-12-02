<h1 id="api-title-functional_categories">Functional Categories</h1>

## Get all Functional Categories
`GET /api/v1/functional_categories`

<a id="opIdgetApiV1FunctionalCategories"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/functional_categories',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1functionalcategories-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all Functional categories|None|

## Get a Functional Category
`GET /api/v1/functional_categories/{id}`

<a id="opIdgetApiV1FunctionalCategoriesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/functional_categories/{id}',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1functionalcategoriesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1functionalcategoriesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a Functional category|None|
