# OpenapiClient::MemberInfo

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

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MemberInfo.new(
  member_type: null,
  name: null,
  declaring_type: null,
  reflected_type: null,
  _module: null,
  custom_attributes: null,
  is_collectible: null,
  metadata_token: null
)
```

