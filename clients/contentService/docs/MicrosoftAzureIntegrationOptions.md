# OpenapiClient::MicrosoftAzureIntegrationOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable** | **Boolean** |  | [optional] |
| **azure_app_insight** | [**AzureAppInsightIntegrationOptions**](AzureAppInsightIntegrationOptions.md) |  | [optional] |
| **azure_storage** | [**AzureStorageIntegrationOptions**](AzureStorageIntegrationOptions.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MicrosoftAzureIntegrationOptions.new(
  enable: null,
  azure_app_insight: null,
  azure_storage: null
)
```

