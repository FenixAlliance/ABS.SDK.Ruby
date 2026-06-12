# OpenapiClient::BatchStockItemUpdateRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_ids** | **Array&lt;String&gt;** |  | [optional] |
| **published** | **Boolean** |  | [optional] |
| **taxable** | **Boolean** |  | [optional] |
| **add_tax_policy_ids** | **Array&lt;String&gt;** |  | [optional] |
| **remove_tax_policy_ids** | **Array&lt;String&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BatchStockItemUpdateRequest.new(
  item_ids: null,
  published: null,
  taxable: null,
  add_tax_policy_ids: null,
  remove_tax_policy_ids: null
)
```

