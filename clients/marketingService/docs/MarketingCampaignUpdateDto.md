# OpenapiClient::MarketingCampaignUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional] |
| **offer** | **String** |  | [optional] |
| **active** | **Boolean** |  | [optional] |
| **proposed_start** | **Time** |  | [optional] |
| **proposed_end** | **Time** |  | [optional] |
| **actual_start** | **Time** |  | [optional] |
| **actual_end** | **Time** |  | [optional] |
| **code** | **String** |  | [optional] |
| **allocated_budget** | **Float** |  | [optional] |
| **activity_cost** | **Float** |  | [optional] |
| **misc_cost** | **Float** |  | [optional] |
| **expected_response_percent** | **Float** |  | [optional] |
| **marketing_area_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MarketingCampaignUpdateDto.new(
  name: null,
  offer: null,
  active: null,
  proposed_start: null,
  proposed_end: null,
  actual_start: null,
  actual_end: null,
  code: null,
  allocated_budget: null,
  activity_cost: null,
  misc_cost: null,
  expected_response_percent: null,
  marketing_area_id: null,
  currency_id: null
)
```

