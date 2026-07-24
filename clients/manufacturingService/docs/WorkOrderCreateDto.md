# OpenapiClient::WorkOrderCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **instructions** | **String** |  | [optional] |
| **production_plan_id** | **String** |  | [optional] |
| **work_order_type_id** | **String** |  | [optional] |
| **workstation_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **individual_id** | **String** |  | [optional] |
| **organization_id** | **String** |  | [optional] |
| **promised_start_date** | **Time** |  | [optional] |
| **promised_end_date** | **Time** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WorkOrderCreateDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  instructions: null,
  production_plan_id: null,
  work_order_type_id: null,
  workstation_id: null,
  currency_id: null,
  individual_id: null,
  organization_id: null,
  promised_start_date: null,
  promised_end_date: null
)
```

