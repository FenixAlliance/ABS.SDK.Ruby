# OpenapiClient::ISwaggerSpec

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable** | **Boolean** |  | [optional] |
| **name** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **version** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **terms_of_service** | **String** |  | [optional] |
| **swagger_endpoint** | [**ISwaggerEndpoint**](ISwaggerEndpoint.md) |  | [optional] |
| **open_api_contact** | [**ISwaggerContact**](ISwaggerContact.md) |  | [optional] |
| **license** | [**ISwaggerLicense**](ISwaggerLicense.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ISwaggerSpec.new(
  enable: null,
  name: null,
  title: null,
  version: null,
  description: null,
  terms_of_service: null,
  swagger_endpoint: null,
  open_api_contact: null,
  license: null
)
```

