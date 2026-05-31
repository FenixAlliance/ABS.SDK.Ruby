# OpenapiClient::VoyagePortCallDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **sequence_number** | **Integer** |  | [optional] |
| **port_call_status** | **String** |  | [optional] |
| **eta** | **Time** |  | [optional] |
| **ata** | **Time** |  | [optional] |
| **etd** | **Time** |  | [optional] |
| **atd** | **Time** |  | [optional] |
| **berth_number** | **String** |  | [optional] |
| **remarks** | **String** |  | [optional] |
| **voyage_id** | **String** |  | [optional] |
| **port_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::VoyagePortCallDto.new(
  id: null,
  timestamp: null,
  sequence_number: null,
  port_call_status: null,
  eta: null,
  ata: null,
  etd: null,
  atd: null,
  berth_number: null,
  remarks: null,
  voyage_id: null,
  port_id: null,
  tenant_id: null
)
```

