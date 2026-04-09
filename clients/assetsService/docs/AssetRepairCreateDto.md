# OpenapiClient::AssetRepairCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **asset_id** | **String** |  | [optional] |
| **repair_status** | **String** |  | [optional] |
| **scheduled_date** | **Time** |  | [optional] |
| **completion_date** | **Time** |  | [optional] |
| **reported_date** | **Time** |  | [optional] |
| **estimated_cost** | **Float** |  | [optional] |
| **actual_cost** | **Float** |  | [optional] |
| **problem_description** | **String** |  | [optional] |
| **repair_description** | **String** |  | [optional] |
| **notes** | **String** |  | [optional] |
| **asset_maintenance_team_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AssetRepairCreateDto.new(
  id: null,
  timestamp: null,
  asset_id: null,
  repair_status: null,
  scheduled_date: null,
  completion_date: null,
  reported_date: null,
  estimated_cost: null,
  actual_cost: null,
  problem_description: null,
  repair_description: null,
  notes: null,
  asset_maintenance_team_id: null
)
```

