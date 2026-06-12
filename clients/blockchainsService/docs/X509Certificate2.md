# OpenapiClient::X509Certificate2

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **handle** | **Object** |  | [optional] |
| **issuer** | **String** |  | [optional][readonly] |
| **subject** | **String** |  | [optional][readonly] |
| **serial_number_bytes** | [**ByteReadOnlyMemory**](ByteReadOnlyMemory.md) |  | [optional] |
| **archived** | **Boolean** |  | [optional] |
| **extensions** | [**Array&lt;X509Extension&gt;**](X509Extension.md) |  | [optional][readonly] |
| **friendly_name** | **String** |  | [optional] |
| **has_private_key** | **Boolean** |  | [optional][readonly] |
| **private_key** | [**AsymmetricAlgorithm**](AsymmetricAlgorithm.md) |  | [optional] |
| **issuer_name** | [**X500DistinguishedName**](X500DistinguishedName.md) |  | [optional] |
| **not_after** | **Time** |  | [optional][readonly] |
| **not_before** | **Time** |  | [optional][readonly] |
| **public_key** | [**PublicKey**](PublicKey.md) |  | [optional] |
| **raw_data** | **String** |  | [optional][readonly] |
| **raw_data_memory** | [**ByteReadOnlyMemory**](ByteReadOnlyMemory.md) |  | [optional] |
| **serial_number** | **String** |  | [optional][readonly] |
| **signature_algorithm** | [**Oid**](Oid.md) |  | [optional] |
| **subject_name** | [**X500DistinguishedName**](X500DistinguishedName.md) |  | [optional] |
| **thumbprint** | **String** |  | [optional][readonly] |
| **version** | **Integer** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::X509Certificate2.new(
  handle: null,
  issuer: null,
  subject: null,
  serial_number_bytes: null,
  archived: null,
  extensions: null,
  friendly_name: null,
  has_private_key: null,
  private_key: null,
  issuer_name: null,
  not_after: null,
  not_before: null,
  public_key: null,
  raw_data: null,
  raw_data_memory: null,
  serial_number: null,
  signature_algorithm: null,
  subject_name: null,
  thumbprint: null,
  version: null
)
```

