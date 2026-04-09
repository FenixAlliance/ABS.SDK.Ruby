# OpenapiClient::InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **is_success** | **Boolean** |  | [optional][readonly] |
| **error_message** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional][readonly] |
| **activity_id** | **String** |  | [optional][readonly] |
| **result** | [**Array&lt;InvoiceLineAppliedTaxDto&gt;**](InvoiceLineAppliedTaxDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope.new(
  is_success: null,
  error_message: null,
  correlation_id: null,
  timestamp: null,
  activity_id: null,
  result: null
)
```

