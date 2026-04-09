# OpenapiClient::TransactionDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **description** | **String** |  | [optional] |
| **price** | **Float** |  | [optional] |
| **quantity** | **Float** |  | [optional] |
| **external_description** | **String** |  | [optional] |
| **basis_quantity** | **Float** |  | [optional] |
| **basis_amount** | **Float** |  | [optional] |
| **percent** | **Float** |  | [optional] |
| **unit_group_id** | **String** |  | [optional] |
| **unit_id** | **String** |  | [optional] |
| **transaction_category_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TransactionDto.new(
  id: null,
  timestamp: null,
  description: null,
  price: null,
  quantity: null,
  external_description: null,
  basis_quantity: null,
  basis_amount: null,
  percent: null,
  unit_group_id: null,
  unit_id: null,
  transaction_category_id: null,
  currency_id: null,
  tenant_id: null,
  enrollment_id: null
)
```

