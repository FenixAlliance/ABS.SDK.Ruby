# OpenapiClient::SuiteModule

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable** | **Boolean** |  | [optional] |
| **marked_for_deletion** | **Boolean** |  | [optional] |
| **active** | **Boolean** |  | [optional][readonly] |
| **order** | **Integer** |  | [optional] |
| **id** | **String** |  | [optional] |
| **name** | **String** |  | [optional] |
| **full_name** | **String** |  | [optional][readonly] |
| **description** | **String** |  | [optional] |
| **type** | **String** |  | [optional] |
| **category** | **String** |  | [optional] |
| **configuration** | **String** |  | [optional] |
| **author** | **String** |  | [optional] |
| **author_url** | **String** |  | [optional] |
| **license** | **String** |  | [optional] |
| **require_license_acceptance** | **Boolean** |  | [optional] |
| **repository** | **String** |  | [optional] |
| **icon** | **String** |  | [optional] |
| **image** | **String** |  | [optional] |
| **nu_spec_path** | **String** |  | [optional] |
| **manifest** | **String** |  | [optional] |
| **logo** | **String** |  | [optional] |
| **website** | **String** |  | [optional] |
| **documentation** | **String** |  | [optional] |
| **url** | **String** |  | [optional] |
| **path** | **String** |  | [optional] |
| **open_api_definition_spec** | [**IOpenApiDefinitionSpec**](IOpenApiDefinitionSpec.md) |  | [optional] |
| **swagger_specs** | [**Array&lt;IOpenApiDefinitionSpec&gt;**](IOpenApiDefinitionSpec.md) |  | [optional] |
| **assembly_paths** | **Array&lt;String&gt;** |  | [optional] |
| **required_permissions** | **Array&lt;String&gt;** |  | [optional][readonly] |
| **version** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SuiteModule.new(
  enable: null,
  marked_for_deletion: null,
  active: null,
  order: null,
  id: null,
  name: null,
  full_name: null,
  description: null,
  type: null,
  category: null,
  configuration: null,
  author: null,
  author_url: null,
  license: null,
  require_license_acceptance: null,
  repository: null,
  icon: null,
  image: null,
  nu_spec_path: null,
  manifest: null,
  logo: null,
  website: null,
  documentation: null,
  url: null,
  path: null,
  open_api_definition_spec: null,
  swagger_specs: null,
  assembly_paths: null,
  required_permissions: null,
  version: null
)
```

