# OpenapiClient::PublicKey

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **encoded_key_value** | [**AsnEncodedData**](AsnEncodedData.md) |  | [optional] |
| **encoded_parameters** | [**AsnEncodedData**](AsnEncodedData.md) |  | [optional] |
| **key** | [**AsymmetricAlgorithm**](AsymmetricAlgorithm.md) |  | [optional] |
| **oid** | [**Oid**](Oid.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PublicKey.new(
  encoded_key_value: null,
  encoded_parameters: null,
  key: null,
  oid: null
)
```

