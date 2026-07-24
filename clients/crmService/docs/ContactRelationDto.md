# OpenapiClient::ContactRelationDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **contact_name** | **String** |  | [optional] |
| **related_contact_id** | **String** |  | [optional] |
| **related_contact_name** | **String** |  | [optional] |
| **contact_relation_type_id** | **String** |  | [optional] |
| **contact_relation_type_name** | **String** |  | [optional] |
| **qualified_name** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ContactRelationDto.new(
  id: null,
  timestamp: null,
  contact_id: null,
  contact_name: null,
  related_contact_id: null,
  related_contact_name: null,
  contact_relation_type_id: null,
  contact_relation_type_name: null,
  qualified_name: null,
  tenant_id: null
)
```

