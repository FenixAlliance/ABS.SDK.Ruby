# OpenapiClient::SupportTicketCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **support_ticket_status** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **support_ticket_type_id** | **String** |  | [optional] |
| **support_entitlement_id** | **String** |  | [optional] |
| **support_priority_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SupportTicketCreateDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  support_ticket_status: null,
  contact_id: null,
  support_ticket_type_id: null,
  support_entitlement_id: null,
  support_priority_id: null
)
```

