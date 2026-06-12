# OpenapiClient::CancellationToken

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **is_cancellation_requested** | **Boolean** |  | [optional][readonly] |
| **can_be_canceled** | **Boolean** |  | [optional][readonly] |
| **wait_handle** | [**WaitHandle**](WaitHandle.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CancellationToken.new(
  is_cancellation_requested: null,
  can_be_canceled: null,
  wait_handle: null
)
```

