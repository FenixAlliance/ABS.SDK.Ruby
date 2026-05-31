# OpenapiClient::CustomAttributeNamedArgument

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **member_info** | [**MemberInfo**](MemberInfo.md) |  | [optional] |
| **typed_value** | [**CustomAttributeTypedArgument**](CustomAttributeTypedArgument.md) |  | [optional] |
| **member_name** | **String** |  | [optional][readonly] |
| **is_field** | **Boolean** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CustomAttributeNamedArgument.new(
  member_info: null,
  typed_value: null,
  member_name: null,
  is_field: null
)
```

