# OpenapiClient::TypeInfo

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional][readonly] |
| **custom_attributes** | [**Array&lt;CustomAttributeData&gt;**](CustomAttributeData.md) |  | [optional][readonly] |
| **is_collectible** | **Boolean** |  | [optional][readonly] |
| **metadata_token** | **Integer** |  | [optional][readonly] |
| **member_type** | **String** |  | [optional][readonly] |
| **namespace** | **String** |  | [optional][readonly] |
| **assembly_qualified_name** | **String** |  | [optional][readonly] |
| **full_name** | **String** |  | [optional][readonly] |
| **assembly** | [**Assembly**](Assembly.md) |  | [optional] |
| **_module** | [**ModelModule**](ModelModule.md) |  | [optional] |
| **is_interface** | **Boolean** |  | [optional][readonly] |
| **is_nested** | **Boolean** |  | [optional][readonly] |
| **declaring_type** | [**Type**](Type.md) |  | [optional] |
| **declaring_method** | [**MethodBase**](MethodBase.md) |  | [optional] |
| **reflected_type** | [**Type**](Type.md) |  | [optional] |
| **underlying_system_type** | [**Type**](Type.md) |  | [optional] |
| **is_type_definition** | **Boolean** |  | [optional][readonly] |
| **is_array** | **Boolean** |  | [optional][readonly] |
| **is_by_ref** | **Boolean** |  | [optional][readonly] |
| **is_pointer** | **Boolean** |  | [optional][readonly] |
| **is_constructed_generic_type** | **Boolean** |  | [optional][readonly] |
| **is_generic_parameter** | **Boolean** |  | [optional][readonly] |
| **is_generic_type_parameter** | **Boolean** |  | [optional][readonly] |
| **is_generic_method_parameter** | **Boolean** |  | [optional][readonly] |
| **is_generic_type** | **Boolean** |  | [optional][readonly] |
| **is_generic_type_definition** | **Boolean** |  | [optional][readonly] |
| **is_sz_array** | **Boolean** |  | [optional][readonly] |
| **is_variable_bound_array** | **Boolean** |  | [optional][readonly] |
| **is_by_ref_like** | **Boolean** |  | [optional][readonly] |
| **is_function_pointer** | **Boolean** |  | [optional][readonly] |
| **is_unmanaged_function_pointer** | **Boolean** |  | [optional][readonly] |
| **has_element_type** | **Boolean** |  | [optional][readonly] |
| **generic_type_arguments** | [**Array&lt;Type&gt;**](Type.md) |  | [optional][readonly] |
| **generic_parameter_position** | **Integer** |  | [optional][readonly] |
| **generic_parameter_attributes** | **String** |  | [optional][readonly] |
| **attributes** | **String** |  | [optional][readonly] |
| **is_abstract** | **Boolean** |  | [optional][readonly] |
| **is_import** | **Boolean** |  | [optional][readonly] |
| **is_sealed** | **Boolean** |  | [optional][readonly] |
| **is_special_name** | **Boolean** |  | [optional][readonly] |
| **is_class** | **Boolean** |  | [optional][readonly] |
| **is_nested_assembly** | **Boolean** |  | [optional][readonly] |
| **is_nested_fam_and_assem** | **Boolean** |  | [optional][readonly] |
| **is_nested_family** | **Boolean** |  | [optional][readonly] |
| **is_nested_fam_or_assem** | **Boolean** |  | [optional][readonly] |
| **is_nested_private** | **Boolean** |  | [optional][readonly] |
| **is_nested_public** | **Boolean** |  | [optional][readonly] |
| **is_not_public** | **Boolean** |  | [optional][readonly] |
| **is_public** | **Boolean** |  | [optional][readonly] |
| **is_auto_layout** | **Boolean** |  | [optional][readonly] |
| **is_explicit_layout** | **Boolean** |  | [optional][readonly] |
| **is_layout_sequential** | **Boolean** |  | [optional][readonly] |
| **is_ansi_class** | **Boolean** |  | [optional][readonly] |
| **is_auto_class** | **Boolean** |  | [optional][readonly] |
| **is_unicode_class** | **Boolean** |  | [optional][readonly] |
| **is_com_object** | **Boolean** |  | [optional][readonly] |
| **is_contextful** | **Boolean** |  | [optional][readonly] |
| **is_enum** | **Boolean** |  | [optional][readonly] |
| **is_marshal_by_ref** | **Boolean** |  | [optional][readonly] |
| **is_primitive** | **Boolean** |  | [optional][readonly] |
| **is_value_type** | **Boolean** |  | [optional][readonly] |
| **is_signature_type** | **Boolean** |  | [optional][readonly] |
| **is_security_critical** | **Boolean** |  | [optional][readonly] |
| **is_security_safe_critical** | **Boolean** |  | [optional][readonly] |
| **is_security_transparent** | **Boolean** |  | [optional][readonly] |
| **struct_layout_attribute** | [**StructLayoutAttribute**](StructLayoutAttribute.md) |  | [optional] |
| **type_initializer** | [**ConstructorInfo**](ConstructorInfo.md) |  | [optional] |
| **type_handle** | [**RuntimeTypeHandle**](RuntimeTypeHandle.md) |  | [optional] |
| **guid** | **String** |  | [optional][readonly] |
| **base_type** | [**Type**](Type.md) |  | [optional] |
| **is_serializable** | **Boolean** |  | [optional][readonly] |
| **contains_generic_parameters** | **Boolean** |  | [optional][readonly] |
| **is_visible** | **Boolean** |  | [optional][readonly] |
| **generic_type_parameters** | [**Array&lt;Type&gt;**](Type.md) |  | [optional][readonly] |
| **declared_constructors** | [**Array&lt;ConstructorInfo&gt;**](ConstructorInfo.md) |  | [optional][readonly] |
| **declared_events** | [**Array&lt;EventInfo&gt;**](EventInfo.md) |  | [optional][readonly] |
| **declared_fields** | [**Array&lt;FieldInfo&gt;**](FieldInfo.md) |  | [optional][readonly] |
| **declared_members** | [**Array&lt;MemberInfo&gt;**](MemberInfo.md) |  | [optional][readonly] |
| **declared_methods** | [**Array&lt;MethodInfo&gt;**](MethodInfo.md) |  | [optional][readonly] |
| **declared_nested_types** | [**Array&lt;TypeInfo&gt;**](TypeInfo.md) |  | [optional][readonly] |
| **declared_properties** | [**Array&lt;PropertyInfo&gt;**](PropertyInfo.md) |  | [optional][readonly] |
| **implemented_interfaces** | [**Array&lt;Type&gt;**](Type.md) |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TypeInfo.new(
  name: null,
  custom_attributes: null,
  is_collectible: null,
  metadata_token: null,
  member_type: null,
  namespace: null,
  assembly_qualified_name: null,
  full_name: null,
  assembly: null,
  _module: null,
  is_interface: null,
  is_nested: null,
  declaring_type: null,
  declaring_method: null,
  reflected_type: null,
  underlying_system_type: null,
  is_type_definition: null,
  is_array: null,
  is_by_ref: null,
  is_pointer: null,
  is_constructed_generic_type: null,
  is_generic_parameter: null,
  is_generic_type_parameter: null,
  is_generic_method_parameter: null,
  is_generic_type: null,
  is_generic_type_definition: null,
  is_sz_array: null,
  is_variable_bound_array: null,
  is_by_ref_like: null,
  is_function_pointer: null,
  is_unmanaged_function_pointer: null,
  has_element_type: null,
  generic_type_arguments: null,
  generic_parameter_position: null,
  generic_parameter_attributes: null,
  attributes: null,
  is_abstract: null,
  is_import: null,
  is_sealed: null,
  is_special_name: null,
  is_class: null,
  is_nested_assembly: null,
  is_nested_fam_and_assem: null,
  is_nested_family: null,
  is_nested_fam_or_assem: null,
  is_nested_private: null,
  is_nested_public: null,
  is_not_public: null,
  is_public: null,
  is_auto_layout: null,
  is_explicit_layout: null,
  is_layout_sequential: null,
  is_ansi_class: null,
  is_auto_class: null,
  is_unicode_class: null,
  is_com_object: null,
  is_contextful: null,
  is_enum: null,
  is_marshal_by_ref: null,
  is_primitive: null,
  is_value_type: null,
  is_signature_type: null,
  is_security_critical: null,
  is_security_safe_critical: null,
  is_security_transparent: null,
  struct_layout_attribute: null,
  type_initializer: null,
  type_handle: null,
  guid: null,
  base_type: null,
  is_serializable: null,
  contains_generic_parameters: null,
  is_visible: null,
  generic_type_parameters: null,
  declared_constructors: null,
  declared_events: null,
  declared_fields: null,
  declared_members: null,
  declared_methods: null,
  declared_nested_types: null,
  declared_properties: null,
  implemented_interfaces: null
)
```

