# OpenapiClient::AsymmetricAlgorithm

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key_size** | **Integer** |  | [optional] |
| **legal_key_sizes** | [**Array&lt;KeySizes&gt;**](KeySizes.md) |  | [optional][readonly] |
| **signature_algorithm** | **String** |  | [optional][readonly] |
| **key_exchange_algorithm** | **String** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AsymmetricAlgorithm.new(
  key_size: null,
  legal_key_sizes: null,
  signature_algorithm: null,
  key_exchange_algorithm: null
)
```

