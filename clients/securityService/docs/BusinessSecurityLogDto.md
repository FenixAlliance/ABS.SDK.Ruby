# OpenapiClient::BusinessSecurityLogDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **type** | **String** |  | [optional] |
| **message** | **String** |  | [optional] |
| **security_event** | **String** |  | [optional] |
| **requires_attention** | **Boolean** |  | [optional] |
| **business_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BusinessSecurityLogDto.new(
  id: null,
  timestamp: null,
  type: null,
  message: null,
  security_event: null,
  requires_attention: null,
  business_id: null
)
```

