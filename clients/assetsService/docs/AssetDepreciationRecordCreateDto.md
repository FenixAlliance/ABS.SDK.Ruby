# OpenapiClient::AssetDepreciationRecordCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **asset_id** | **String** |  | [optional] |
| **asset_depreciation_policy_id** | **String** |  | [optional] |
| **depreciation_amount** | **Float** |  | [optional] |
| **accumulated_depreciation** | **Float** |  | [optional] |
| **book_value** | **Float** |  | [optional] |
| **depreciation_date** | **Time** |  | [optional] |
| **year** | **Integer** |  | [optional] |
| **month** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AssetDepreciationRecordCreateDto.new(
  asset_id: null,
  asset_depreciation_policy_id: null,
  depreciation_amount: null,
  accumulated_depreciation: null,
  book_value: null,
  depreciation_date: null,
  year: null,
  month: null
)
```

