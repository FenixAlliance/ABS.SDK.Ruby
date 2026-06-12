# OpenapiClient::HttpContext

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **features** | [**Array&lt;TypeObjectKeyValuePair&gt;**](TypeObjectKeyValuePair.md) |  | [optional][readonly] |
| **request** | [**HttpRequest**](HttpRequest.md) |  | [optional] |
| **response** | [**HttpResponse**](HttpResponse.md) |  | [optional] |
| **connection** | [**ConnectionInfo**](ConnectionInfo.md) |  | [optional] |
| **web_sockets** | [**WebSocketManager**](WebSocketManager.md) |  | [optional] |
| **user** | [**ClaimsPrincipal**](ClaimsPrincipal.md) |  | [optional] |
| **items** | **Hash&lt;String, Object&gt;** |  | [optional] |
| **request_services** | **Object** |  | [optional] |
| **request_aborted** | [**CancellationToken**](CancellationToken.md) |  | [optional] |
| **trace_identifier** | **String** |  | [optional] |
| **session** | [**ISession**](ISession.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::HttpContext.new(
  features: null,
  request: null,
  response: null,
  connection: null,
  web_sockets: null,
  user: null,
  items: null,
  request_services: null,
  request_aborted: null,
  trace_identifier: null,
  session: null
)
```

