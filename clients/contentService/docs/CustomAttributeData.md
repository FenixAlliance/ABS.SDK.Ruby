# OpenapiClient::CustomAttributeData

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **attribute_type** | [**Type**](Type.md) |  | [optional] |
| **constructor** | [**ConstructorInfo**](ConstructorInfo.md) |  | [optional] |
| **constructor_arguments** | [**Array&lt;CustomAttributeTypedArgument&gt;**](CustomAttributeTypedArgument.md) |  | [optional][readonly] |
| **named_arguments** | [**Array&lt;CustomAttributeNamedArgument&gt;**](CustomAttributeNamedArgument.md) |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CustomAttributeData.new(
  attribute_type: null,
  constructor: null,
  constructor_arguments: null,
  named_arguments: null
)
```

