# OpenapiClient::EventInfo

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
| **is_special_name** | **Boolean** |  | [optional][readonly] |
| **add_method** | [**MethodInfo**](MethodInfo.md) |  | [optional] |
| **remove_method** | [**MethodInfo**](MethodInfo.md) |  | [optional] |
| **raise_method** | [**MethodInfo**](MethodInfo.md) |  | [optional] |
| **is_multicast** | **Boolean** |  | [optional][readonly] |
| **event_handler_type** | [**Type**](Type.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::EventInfo.new(
  name: null,
  declaring_type: null,
  reflected_type: null,
  _module: null,
  custom_attributes: null,
  is_collectible: null,
  metadata_token: null,
  member_type: null,
  attributes: null,
  is_special_name: null,
  add_method: null,
  remove_method: null,
  raise_method: null,
  is_multicast: null,
  event_handler_type: null
)
```

