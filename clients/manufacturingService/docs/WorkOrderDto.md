# OpenapiClient::WorkOrderDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **instructions** | **String** |  | [optional] |
| **taxable** | **Boolean** |  | [optional] |
| **work_location** | **String** |  | [optional] |
| **promised_start_date** | **Time** |  | [optional] |
| **promised_end_date** | **Time** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **individual_id** | **String** |  | [optional] |
| **organization_id** | **String** |  | [optional] |
| **production_plan_id** | **String** |  | [optional] |
| **work_order_type_id** | **String** |  | [optional] |
| **workstation_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WorkOrderDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  instructions: null,
  taxable: null,
  work_location: null,
  promised_start_date: null,
  promised_end_date: null,
  currency_id: null,
  individual_id: null,
  organization_id: null,
  production_plan_id: null,
  work_order_type_id: null,
  workstation_id: null,
  tenant_id: null
)
```

