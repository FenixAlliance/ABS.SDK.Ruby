# OpenapiClient::CreateSigningRequestDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **routing_mode** | **String** |  | [optional] |
| **expires_at_utc** | **Time** |  | [optional] |
| **message** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **external_reference** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CreateSigningRequestDto.new(
  routing_mode: null,
  expires_at_utc: null,
  message: null,
  correlation_id: null,
  external_reference: null
)
```

