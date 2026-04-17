# OpenapiClient::CostCentreCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **name** | **String** |  | [optional] |
| **disabled** | **Boolean** |  | [optional] |
| **description** | **String** |  | [optional] |
| **cost_centre_type** | **String** |  | [optional] |
| **cost_centres_group_id** | **String** |  | [optional] |
| **parent_cost_centre_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CostCentreCreateDto.new(
  id: null,
  timestamp: null,
  name: null,
  disabled: null,
  description: null,
  cost_centre_type: null,
  cost_centres_group_id: null,
  parent_cost_centre_id: null
)
```

