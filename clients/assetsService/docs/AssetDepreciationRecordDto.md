# OpenapiClient::AssetDepreciationRecordDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **Object** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **business_id** | **Object** |  | [optional] |
| **business_profile_record_id** | **Object** |  | [optional] |
| **asset_id** | **Object** |  | [optional] |
| **asset_name** | **String** |  | [optional] |
| **asset_depreciation_policy_id** | **String** |  | [optional] |
| **asset_depreciation_policy_name** | **String** |  | [optional] |
| **depreciation_amount** | **Float** |  | [optional] |
| **accumulated_depreciation** | **Float** |  | [optional] |
| **book_value** | **Float** |  | [optional] |
| **depreciation_date** | **Time** |  | [optional] |
| **year** | **Integer** |  | [optional] |
| **month** | **Integer** |  | [optional] |
| **period** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AssetDepreciationRecordDto.new(
  id: null,
  timestamp: null,
  business_id: null,
  business_profile_record_id: null,
  asset_id: null,
  asset_name: null,
  asset_depreciation_policy_id: null,
  asset_depreciation_policy_name: null,
  depreciation_amount: null,
  accumulated_depreciation: null,
  book_value: null,
  depreciation_date: null,
  year: null,
  month: null,
  period: null
)
```

