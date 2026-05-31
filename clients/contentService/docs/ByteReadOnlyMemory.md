# OpenapiClient::ByteReadOnlyMemory

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **length** | **Integer** |  | [optional][readonly] |
| **is_empty** | **Boolean** |  | [optional][readonly] |
| **span** | [**ByteReadOnlySpan**](ByteReadOnlySpan.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ByteReadOnlyMemory.new(
  length: null,
  is_empty: null,
  span: null
)
```

