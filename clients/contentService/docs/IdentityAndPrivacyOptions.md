# OpenapiClient::IdentityAndPrivacyOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **allow_guest_orders** | **Boolean** |  | [optional] |
| **allow_guest_cart_recognition** | **Boolean** |  | [optional] |
| **allow_remove_download_access_on_request** | **Boolean** |  | [optional] |
| **allow_remove_personal_data_from_orders_on_request** | **Boolean** |  | [optional] |
| **allow_remove_personal_data_from_subscriptions_on_request** | **Boolean** |  | [optional] |
| **store_checkout_privacy_policy_notice** | **String** |  | [optional] |
| **store_registration_privacy_policy_notice** | **String** |  | [optional] |
| **default_customer_location** | **String** |  | [optional] |
| **inactive_carts_retention_policy** | [**StoreDataRetentionPolicy**](StoreDataRetentionPolicy.md) |  | [optional] |
| **pending_orders_retention_policy** | [**StoreDataRetentionPolicy**](StoreDataRetentionPolicy.md) |  | [optional] |
| **failed_orders_retention_policy** | [**StoreDataRetentionPolicy**](StoreDataRetentionPolicy.md) |  | [optional] |
| **cancelled_orders_retention_policy** | [**StoreDataRetentionPolicy**](StoreDataRetentionPolicy.md) |  | [optional] |
| **completed_orders_retention_policy** | [**StoreDataRetentionPolicy**](StoreDataRetentionPolicy.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IdentityAndPrivacyOptions.new(
  allow_guest_orders: null,
  allow_guest_cart_recognition: null,
  allow_remove_download_access_on_request: null,
  allow_remove_personal_data_from_orders_on_request: null,
  allow_remove_personal_data_from_subscriptions_on_request: null,
  store_checkout_privacy_policy_notice: null,
  store_registration_privacy_policy_notice: null,
  default_customer_location: null,
  inactive_carts_retention_policy: null,
  pending_orders_retention_policy: null,
  failed_orders_retention_policy: null,
  cancelled_orders_retention_policy: null,
  completed_orders_retention_policy: null
)
```

