# OpenapiClient::IOpenApiDefinitionSpec

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable** | **Boolean** |  | [optional] |
| **name** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **version** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **terms_of_service** | **String** |  | [optional] |
| **open_api_endpoint** | [**IOpenApiEndpoint**](IOpenApiEndpoint.md) |  | [optional] |
| **open_api_contact** | [**IOpenApiContact**](IOpenApiContact.md) |  | [optional] |
| **license** | [**IOpenApiLicense**](IOpenApiLicense.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IOpenApiDefinitionSpec.new(
  enable: null,
  name: null,
  title: null,
  version: null,
  description: null,
  terms_of_service: null,
  open_api_endpoint: null,
  open_api_contact: null,
  license: null
)
```

