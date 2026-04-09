# OpenapiClient::InventoryOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable_stock_management** | **Boolean** |  | [optional] |
| **hide_out_of_stock_products** | **Boolean** |  | [optional] |
| **enable_low_stock_notifications** | **Boolean** |  | [optional] |
| **enable_out_of_stock_notifications** | **Boolean** |  | [optional] |
| **stock_notification_recipients** | **String** |  | [optional] |
| **hold_stock** | **Integer** |  | [optional] |
| **low_stock_threshold** | **Integer** |  | [optional] |
| **out_of_stock_threshold** | **Integer** |  | [optional] |
| **stock_display_format** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::InventoryOptions.new(
  enable_stock_management: null,
  hide_out_of_stock_products: null,
  enable_low_stock_notifications: null,
  enable_out_of_stock_notifications: null,
  stock_notification_recipients: null,
  hold_stock: null,
  low_stock_threshold: null,
  out_of_stock_threshold: null,
  stock_display_format: null
)
```

