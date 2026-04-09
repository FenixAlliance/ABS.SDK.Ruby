# OpenapiClient::SecurityCertificateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **type** | **String** |  | [optional] |
| **expire_period** | **String** |  | [optional] |
| **expired** | **Boolean** |  | [optional] |
| **disabled** | **Boolean** |  | [optional] |
| **business_id** | **String** |  | [optional] |
| **csr** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SecurityCertificateDto.new(
  id: null,
  timestamp: null,
  type: null,
  expire_period: null,
  expired: null,
  disabled: null,
  business_id: null,
  csr: null
)
```

