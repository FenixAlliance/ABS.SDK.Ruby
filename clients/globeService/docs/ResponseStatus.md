# OpenapiClient::ResponseStatus

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **success** | **Boolean** |  | [optional] |
| **error** | [**Error**](Error.md) |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **utc_timestamp** | **Time** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ResponseStatus.new(
  success: null,
  error: null,
  correlation_id: null,
  utc_timestamp: null
)
```

