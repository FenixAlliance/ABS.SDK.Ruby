# OpenapiClient::FieldInfo

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional][readonly] |
| **declaring_type** | [**Type**](Type.md) |  | [optional] |
| **reflected_type** | [**Type**](Type.md) |  | [optional] |
| **_module** | [**ModelModule**](ModelModule.md) |  | [optional] |
| **custom_attributes** | [**Array&lt;CustomAttributeData&gt;**](CustomAttributeData.md) |  | [optional][readonly] |
| **is_collectible** | **Boolean** |  | [optional][readonly] |
| **metadata_token** | **Integer** |  | [optional][readonly] |
| **member_type** | **String** |  | [optional][readonly] |
| **attributes** | **String** |  | [optional][readonly] |
| **field_type** | [**Type**](Type.md) |  | [optional] |
| **is_init_only** | **Boolean** |  | [optional][readonly] |
| **is_literal** | **Boolean** |  | [optional][readonly] |
| **is_not_serialized** | **Boolean** |  | [optional][readonly] |
| **is_pinvoke_impl** | **Boolean** |  | [optional][readonly] |
| **is_special_name** | **Boolean** |  | [optional][readonly] |
| **is_static** | **Boolean** |  | [optional][readonly] |
| **is_assembly** | **Boolean** |  | [optional][readonly] |
| **is_family** | **Boolean** |  | [optional][readonly] |
| **is_family_and_assembly** | **Boolean** |  | [optional][readonly] |
| **is_family_or_assembly** | **Boolean** |  | [optional][readonly] |
| **is_private** | **Boolean** |  | [optional][readonly] |
| **is_public** | **Boolean** |  | [optional][readonly] |
| **is_security_critical** | **Boolean** |  | [optional][readonly] |
| **is_security_safe_critical** | **Boolean** |  | [optional][readonly] |
| **is_security_transparent** | **Boolean** |  | [optional][readonly] |
| **field_handle** | [**RuntimeFieldHandle**](RuntimeFieldHandle.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::FieldInfo.new(
  name: null,
  declaring_type: null,
  reflected_type: null,
  _module: null,
  custom_attributes: null,
  is_collectible: null,
  metadata_token: null,
  member_type: null,
  attributes: null,
  field_type: null,
  is_init_only: null,
  is_literal: null,
  is_not_serialized: null,
  is_pinvoke_impl: null,
  is_special_name: null,
  is_static: null,
  is_assembly: null,
  is_family: null,
  is_family_and_assembly: null,
  is_family_or_assembly: null,
  is_private: null,
  is_public: null,
  is_security_critical: null,
  is_security_safe_critical: null,
  is_security_transparent: null,
  field_handle: null
)
```

