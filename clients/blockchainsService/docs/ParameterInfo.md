# OpenapiClient::ParameterInfo

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **attributes** | **String** |  | [optional][readonly] |
| **member** | [**MemberInfo**](MemberInfo.md) |  | [optional] |
| **name** | **String** |  | [optional][readonly] |
| **parameter_type** | [**Type**](Type.md) |  | [optional] |
| **position** | **Integer** |  | [optional][readonly] |
| **is_in** | **Boolean** |  | [optional][readonly] |
| **is_lcid** | **Boolean** |  | [optional][readonly] |
| **is_optional** | **Boolean** |  | [optional][readonly] |
| **is_out** | **Boolean** |  | [optional][readonly] |
| **is_retval** | **Boolean** |  | [optional][readonly] |
| **default_value** | **Object** |  | [optional][readonly] |
| **raw_default_value** | **Object** |  | [optional][readonly] |
| **has_default_value** | **Boolean** |  | [optional][readonly] |
| **custom_attributes** | [**Array&lt;CustomAttributeData&gt;**](CustomAttributeData.md) |  | [optional][readonly] |
| **metadata_token** | **Integer** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ParameterInfo.new(
  attributes: null,
  member: null,
  name: null,
  parameter_type: null,
  position: null,
  is_in: null,
  is_lcid: null,
  is_optional: null,
  is_out: null,
  is_retval: null,
  default_value: null,
  raw_default_value: null,
  has_default_value: null,
  custom_attributes: null,
  metadata_token: null
)
```

