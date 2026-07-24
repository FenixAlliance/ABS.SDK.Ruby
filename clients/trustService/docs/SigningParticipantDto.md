# OpenapiClient::SigningParticipantDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **signing_request_id** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **contact_name** | **String** |  | [optional] |
| **role** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **routing_order** | **Integer** |  | [optional] |
| **sent_at_utc** | **Time** |  | [optional] |
| **viewed_at_utc** | **Time** |  | [optional] |
| **signed_at_utc** | **Time** |  | [optional] |
| **approved_at_utc** | **Time** |  | [optional] |
| **declined_at_utc** | **Time** |  | [optional] |
| **decline_reason** | **String** |  | [optional] |
| **signature_id** | **String** |  | [optional] |
| **access_token_expires_at_utc** | **Time** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **external_reference** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SigningParticipantDto.new(
  id: null,
  tenant_id: null,
  signing_request_id: null,
  contact_id: null,
  contact_name: null,
  role: null,
  status: null,
  routing_order: null,
  sent_at_utc: null,
  viewed_at_utc: null,
  signed_at_utc: null,
  approved_at_utc: null,
  declined_at_utc: null,
  decline_reason: null,
  signature_id: null,
  access_token_expires_at_utc: null,
  correlation_id: null,
  external_reference: null
)
```

