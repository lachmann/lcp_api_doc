<h1 id="api-title-periods">periods</h1>

Operations about periods

## getApiV1PeriodsId

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

## getApiV1Periods

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

`GET /api/v1/periods`

Return all periods

<h3 id="getapiv1periods-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Return all periods|None|
