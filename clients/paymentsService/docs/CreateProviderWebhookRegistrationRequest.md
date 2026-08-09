# OpenapiClient::CreateProviderWebhookRegistrationRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **provider_code** | **String** |  | [optional] |
| **external_account_id** | **String** |  | [optional] |
| **webhook_signing_secret** | **String** |  | [optional] |
| **credential_mode** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CreateProviderWebhookRegistrationRequest.new(
  provider_code: null,
  external_account_id: null,
  webhook_signing_secret: null,
  credential_mode: null
)
```

