# OpenapiClient::InvoiceEnumerationRangeDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **prefix** | **String** |  | [optional] |
| **suffix** | **String** |  | [optional] |
| **identifier** | **String** |  | [optional] |
| **qualified_name** | **String** |  | [optional] |
| **current_numeration** | **Integer** |  | [optional] |
| **numeration_to** | **Integer** |  | [optional] |
| **numeration_from** | **Integer** |  | [optional] |
| **valid_from** | **Time** |  | [optional] |
| **valid_to** | **Time** |  | [optional] |
| **fiscal_authority_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **document_type** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::InvoiceEnumerationRangeDto.new(
  id: null,
  timestamp: null,
  prefix: null,
  suffix: null,
  identifier: null,
  qualified_name: null,
  current_numeration: null,
  numeration_to: null,
  numeration_from: null,
  valid_from: null,
  valid_to: null,
  fiscal_authority_id: null,
  tenant_id: null,
  enrollment_id: null,
  document_type: null
)
```

