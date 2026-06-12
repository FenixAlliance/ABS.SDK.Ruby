# OpenapiClient::MethodBase

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **member_type** | **String** |  | [optional][readonly] |
| **name** | **String** |  | [optional][readonly] |
| **declaring_type** | [**Type**](Type.md) |  | [optional] |
| **reflected_type** | [**Type**](Type.md) |  | [optional] |
| **_module** | [**ModelModule**](ModelModule.md) |  | [optional] |
| **custom_attributes** | [**Array&lt;CustomAttributeData&gt;**](CustomAttributeData.md) |  | [optional][readonly] |
| **is_collectible** | **Boolean** |  | [optional][readonly] |
| **metadata_token** | **Integer** |  | [optional][readonly] |
| **attributes** | **String** |  | [optional][readonly] |
| **method_implementation_flags** | **String** |  | [optional][readonly] |
| **calling_convention** | **String** |  | [optional][readonly] |
| **is_abstract** | **Boolean** |  | [optional][readonly] |
| **is_constructor** | **Boolean** |  | [optional][readonly] |
| **is_final** | **Boolean** |  | [optional][readonly] |
| **is_hide_by_sig** | **Boolean** |  | [optional][readonly] |
| **is_special_name** | **Boolean** |  | [optional][readonly] |
| **is_static** | **Boolean** |  | [optional][readonly] |
| **is_virtual** | **Boolean** |  | [optional][readonly] |
| **is_assembly** | **Boolean** |  | [optional][readonly] |
| **is_family** | **Boolean** |  | [optional][readonly] |
| **is_family_and_assembly** | **Boolean** |  | [optional][readonly] |
| **is_family_or_assembly** | **Boolean** |  | [optional][readonly] |
| **is_private** | **Boolean** |  | [optional][readonly] |
| **is_public** | **Boolean** |  | [optional][readonly] |
| **is_constructed_generic_method** | **Boolean** |  | [optional][readonly] |
| **is_generic_method** | **Boolean** |  | [optional][readonly] |
| **is_generic_method_definition** | **Boolean** |  | [optional][readonly] |
| **contains_generic_parameters** | **Boolean** |  | [optional][readonly] |
| **method_handle** | [**RuntimeMethodHandle**](RuntimeMethodHandle.md) |  | [optional] |
| **is_security_critical** | **Boolean** |  | [optional][readonly] |
| **is_security_safe_critical** | **Boolean** |  | [optional][readonly] |
| **is_security_transparent** | **Boolean** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MethodBase.new(
  member_type: null,
  name: null,
  declaring_type: null,
  reflected_type: null,
  _module: null,
  custom_attributes: null,
  is_collectible: null,
  metadata_token: null,
  attributes: null,
  method_implementation_flags: null,
  calling_convention: null,
  is_abstract: null,
  is_constructor: null,
  is_final: null,
  is_hide_by_sig: null,
  is_special_name: null,
  is_static: null,
  is_virtual: null,
  is_assembly: null,
  is_family: null,
  is_family_and_assembly: null,
  is_family_or_assembly: null,
  is_private: null,
  is_public: null,
  is_constructed_generic_method: null,
  is_generic_method: null,
  is_generic_method_definition: null,
  contains_generic_parameters: null,
  method_handle: null,
  is_security_critical: null,
  is_security_safe_critical: null,
  is_security_transparent: null
)
```

