# OpenapiClient::PropertyInfo

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
| **property_type** | [**Type**](Type.md) |  | [optional] |
| **attributes** | **String** |  | [optional][readonly] |
| **is_special_name** | **Boolean** |  | [optional][readonly] |
| **can_read** | **Boolean** |  | [optional][readonly] |
| **can_write** | **Boolean** |  | [optional][readonly] |
| **get_method** | [**MethodInfo**](MethodInfo.md) |  | [optional] |
| **set_method** | [**MethodInfo**](MethodInfo.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PropertyInfo.new(
  name: null,
  declaring_type: null,
  reflected_type: null,
  _module: null,
  custom_attributes: null,
  is_collectible: null,
  metadata_token: null,
  member_type: null,
  property_type: null,
  attributes: null,
  is_special_name: null,
  can_read: null,
  can_write: null,
  get_method: null,
  set_method: null
)
```

