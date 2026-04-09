# OpenapiClient::AssetValueAmendDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **Object** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **business_id** | **Object** |  | [optional] |
| **business_profile_record_id** | **Object** |  | [optional] |
| **asset_id** | **Object** |  | [optional] |
| **asset_name** | **String** |  | [optional] |
| **previous_value** | **Float** |  | [optional] |
| **new_value** | **Float** |  | [optional] |
| **amendment_amount** | **Float** |  | [optional] |
| **reason** | **String** |  | [optional] |
| **amendment_date** | **Time** |  | [optional] |
| **approved_by** | **String** |  | [optional] |
| **approval_date** | **Time** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AssetValueAmendDto.new(
  id: null,
  timestamp: null,
  business_id: null,
  business_profile_record_id: null,
  asset_id: null,
  asset_name: null,
  previous_value: null,
  new_value: null,
  amendment_amount: null,
  reason: null,
  amendment_date: null,
  approved_by: null,
  approval_date: null
)
```

