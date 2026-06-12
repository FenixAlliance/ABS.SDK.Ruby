# OpenapiClient::AssetValueAmendCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **asset_id** | **String** |  | [optional] |
| **previous_value** | **Float** |  | [optional] |
| **new_value** | **Float** |  | [optional] |
| **reason** | **String** |  | [optional] |
| **amendment_date** | **Time** |  | [optional] |
| **currency_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AssetValueAmendCreateDto.new(
  id: null,
  timestamp: null,
  asset_id: null,
  previous_value: null,
  new_value: null,
  reason: null,
  amendment_date: null,
  currency_id: null
)
```

