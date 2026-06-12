# OpenapiClient::Assembly

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **defined_types** | [**Array&lt;TypeInfo&gt;**](TypeInfo.md) |  | [optional][readonly] |
| **exported_types** | [**Array&lt;Type&gt;**](Type.md) |  | [optional][readonly] |
| **code_base** | **String** |  | [optional][readonly] |
| **entry_point** | [**MethodInfo**](MethodInfo.md) |  | [optional] |
| **full_name** | **String** |  | [optional][readonly] |
| **image_runtime_version** | **String** |  | [optional][readonly] |
| **is_dynamic** | **Boolean** |  | [optional][readonly] |
| **location** | **String** |  | [optional][readonly] |
| **reflection_only** | **Boolean** |  | [optional][readonly] |
| **is_collectible** | **Boolean** |  | [optional][readonly] |
| **is_fully_trusted** | **Boolean** |  | [optional][readonly] |
| **custom_attributes** | [**Array&lt;CustomAttributeData&gt;**](CustomAttributeData.md) |  | [optional][readonly] |
| **escaped_code_base** | **String** |  | [optional][readonly] |
| **manifest_module** | [**ModelModule**](ModelModule.md) |  | [optional] |
| **modules** | [**Array&lt;ModelModule&gt;**](ModelModule.md) |  | [optional][readonly] |
| **global_assembly_cache** | **Boolean** |  | [optional][readonly] |
| **host_context** | **Integer** |  | [optional][readonly] |
| **security_rule_set** | **String** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Assembly.new(
  defined_types: null,
  exported_types: null,
  code_base: null,
  entry_point: null,
  full_name: null,
  image_runtime_version: null,
  is_dynamic: null,
  location: null,
  reflection_only: null,
  is_collectible: null,
  is_fully_trusted: null,
  custom_attributes: null,
  escaped_code_base: null,
  manifest_module: null,
  modules: null,
  global_assembly_cache: null,
  host_context: null,
  security_rule_set: null
)
```

