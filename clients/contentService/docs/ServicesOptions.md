# OpenapiClient::ServicesOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **drip_downloadable_content** | **Boolean** |  | [optional] |
| **retry_failed_payments** | **Boolean** |  | [optional] |
| **allow0_initial_checkout** | **Boolean** |  | [optional] |
| **allow_mixed_checkout** | **Boolean** |  | [optional] |
| **synchronise_renewals** | **Boolean** |  | [optional] |
| **add_to_cart_button_text** | **String** |  | [optional] |
| **place_order_button_text** | **String** |  | [optional] |
| **new_subscriber_role** | **String** |  | [optional] |
| **inactive_subscriber_role** | **String** |  | [optional] |
| **enable_automatic_payments** | **Integer** |  | [optional] |
| **enable_manual_renewals** | **Integer** |  | [optional] |
| **display_auto_renewal_toggle** | **Integer** |  | [optional] |
| **accept_early_renewals** | **Integer** |  | [optional] |
| **customer_suspensions** | **Integer** |  | [optional] |
| **enable_subscription_switching_between_groups** | **Integer** |  | [optional] |
| **enable_subscription_switching_between_variations** | **Integer** |  | [optional] |
| **prorate_first_renewal** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ServicesOptions.new(
  drip_downloadable_content: null,
  retry_failed_payments: null,
  allow0_initial_checkout: null,
  allow_mixed_checkout: null,
  synchronise_renewals: null,
  add_to_cart_button_text: null,
  place_order_button_text: null,
  new_subscriber_role: null,
  inactive_subscriber_role: null,
  enable_automatic_payments: null,
  enable_manual_renewals: null,
  display_auto_renewal_toggle: null,
  accept_early_renewals: null,
  customer_suspensions: null,
  enable_subscription_switching_between_groups: null,
  enable_subscription_switching_between_variations: null,
  prorate_first_renewal: null
)
```

