<h1 id="api-title-sites">Sites</h1>

## List all Sites
`GET /api/v1/sites`

<a id="opIdgetApiV1Sites"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/sites',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1sites-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all sites|None|

## Get a Site
`GET /api/v1/sites/{id}`

<a id="opIdgetApiV1SitesId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/sites/{id}',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1sitesid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1sitesid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a site|None|
