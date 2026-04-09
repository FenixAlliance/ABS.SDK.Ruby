# OpenapiClient::AssetTransferCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **asset_id** | **String** |  | [optional] |
| **is_root_transfer** | **Boolean** |  | [optional] |
| **serial_list** | **String** |  | [optional] |
| **quantity** | **String** |  | [optional] |
| **serial** | **String** |  | [optional] |
| **previous_asset_transfer_id** | **String** |  | [optional] |
| **source_location_id** | **String** |  | [optional] |
| **destination_location_id** | **String** |  | [optional] |
| **source_contact_id** | **String** |  | [optional] |
| **destination_contact_id** | **String** |  | [optional] |
| **source_department_id** | **String** |  | [optional] |
| **destination_department_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AssetTransferCreateDto.new(
  asset_id: null,
  is_root_transfer: null,
  serial_list: null,
  quantity: null,
  serial: null,
  previous_asset_transfer_id: null,
  source_location_id: null,
  destination_location_id: null,
  source_contact_id: null,
  destination_contact_id: null,
  source_department_id: null,
  destination_department_id: null
)
```

