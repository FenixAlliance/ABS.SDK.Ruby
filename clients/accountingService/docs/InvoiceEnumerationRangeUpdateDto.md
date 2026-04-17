# OpenapiClient::InvoiceEnumerationRangeUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **prefix** | **String** |  | [optional] |
| **suffix** | **String** |  | [optional] |
| **identifier** | **String** |  | [optional] |
| **qualified_name** | **String** |  | [optional] |
| **current_numeration** | **Integer** |  | [optional] |
| **numeration_from** | **Integer** |  | [optional] |
| **numeration_to** | **Integer** |  | [optional] |
| **valid_from** | **Time** |  | [optional] |
| **valid_to** | **Time** |  | [optional] |
| **fiscal_authority_id** | **String** |  | [optional] |
| **document_type** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::InvoiceEnumerationRangeUpdateDto.new(
  prefix: null,
  suffix: null,
  identifier: null,
  qualified_name: null,
  current_numeration: null,
  numeration_from: null,
  numeration_to: null,
  valid_from: null,
  valid_to: null,
  fiscal_authority_id: null,
  document_type: null
)
```

