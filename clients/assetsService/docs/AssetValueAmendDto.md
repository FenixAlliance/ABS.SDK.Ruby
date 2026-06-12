# OpenapiClient::AssetValueAmendDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **asset_id** | **String** |  | [optional] |
| **asset_name** | **String** |  | [optional] |
| **previous_value** | **Float** |  | [optional] |
| **new_value** | **Float** |  | [optional] |
| **amendment_amount** | **Float** |  | [optional] |
| **reason** | **String** |  | [optional] |
| **amendment_date** | **Time** |  | [optional] |
| **currency_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AssetValueAmendDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  enrollment_id: null,
  asset_id: null,
  asset_name: null,
  previous_value: null,
  new_value: null,
  amendment_amount: null,
  reason: null,
  amendment_date: null,
  currency_id: null
)
```

