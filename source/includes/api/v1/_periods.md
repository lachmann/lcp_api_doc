<h1 id="api-title-periods">Periods</h1>

## Get all Periods
`GET /api/v1/periods`

<a id="opIdgetApiV1Periods"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/periods',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1periods-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all periods|None|

## Get a Period
`GET /api/v1/periods/{id}`

<a id="opIdgetApiV1PeriodsId"></a>

> Code samples

```ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://www.levantineceramics.org/api/v1/periods/{id}',
  params: {
  }

p JSON.parse(result)

```

<h3 id="getapiv1periodsid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer(int32)|true|none|

<h3 id="getapiv1periodsid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return a period|None|
