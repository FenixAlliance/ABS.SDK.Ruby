# OpenapiClient::FiscalRegimeDtoListEnvelope

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **is_success** | **Boolean** |  | [optional][readonly] |
| **error_message** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional][readonly] |
| **http_status** | **Integer** |  | [optional] |
| **error_code** | **String** |  | [optional] |
| **validation_details** | **Hash&lt;String, Array&lt;String&gt;&gt;** |  | [optional] |
| **activity_id** | **String** |  | [optional][readonly] |
| **result** | [**Array&lt;FiscalRegimeDto&gt;**](FiscalRegimeDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::FiscalRegimeDtoListEnvelope.new(
  is_success: null,
  error_message: null,
  correlation_id: null,
  timestamp: null,
  http_status: null,
  error_code: null,
  validation_details: null,
  activity_id: null,
  result: null
)
```

