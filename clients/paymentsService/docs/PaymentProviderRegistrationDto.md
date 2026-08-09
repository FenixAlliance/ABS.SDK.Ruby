# OpenapiClient::PaymentProviderRegistrationDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **created_at_utc** | **Time** |  | [optional] |
| **last_modified_utc** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **provider_code** | **String** |  | [optional] |
| **credential_set_reference** | **String** |  | [optional] |
| **has_credential** | **Boolean** |  | [optional] |
| **credential_mode** | **String** |  | [optional] |
| **external_account_id** | **String** |  | [optional] |
| **enabled_capabilities** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaymentProviderRegistrationDto.new(
  id: null,
  created_at_utc: null,
  last_modified_utc: null,
  tenant_id: null,
  enrollment_id: null,
  provider_code: null,
  credential_set_reference: null,
  has_credential: null,
  credential_mode: null,
  external_account_id: null,
  enabled_capabilities: null,
  status: null
)
```

