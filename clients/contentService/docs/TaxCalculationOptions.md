# OpenapiClient::TaxCalculationOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable_taxes** | **Boolean** |  | [optional] |
| **round_taxes_at_subtotal_level** | **Boolean** |  | [optional] |
| **display_price_suffix** | **String** |  | [optional] |
| **display_price_prefix** | **String** |  | [optional] |
| **standard_rates** | **Array&lt;String&gt;** |  | [optional] |
| **zero_rate_rates** | **Array&lt;String&gt;** |  | [optional] |
| **reduced_rate_rates** | **Array&lt;String&gt;** |  | [optional] |
| **additional_tax_classes** | **Hash&lt;String, Array&lt;String&gt;&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TaxCalculationOptions.new(
  enable_taxes: null,
  round_taxes_at_subtotal_level: null,
  display_price_suffix: null,
  display_price_prefix: null,
  standard_rates: null,
  zero_rate_rates: null,
  reduced_rate_rates: null,
  additional_tax_classes: null
)
```

