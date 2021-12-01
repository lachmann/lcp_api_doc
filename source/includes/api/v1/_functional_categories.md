<h1 id="api-title-functional_categories">Functional Categories</h1>

Operations about functional_categories

## getApiV1FunctionalCategoriesId

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

## getApiV1FunctionalCategories

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

`GET /api/v1/functional_categories`

Return all Functional categories

<h3 id="getapiv1functionalcategories-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all Functional categories|None|
