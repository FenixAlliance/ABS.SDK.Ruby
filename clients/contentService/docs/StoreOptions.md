# OpenapiClient::StoreOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable** | **Boolean** |  | [optional] |
| **name** | **String** |  | [optional] |
| **logo** | **String** |  | [optional] |
| **footer_logo** | **String** |  | [optional] |
| **tagline** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **address_line1** | **String** |  | [optional] |
| **address_line2** | **String** |  | [optional] |
| **city_id** | **String** |  | [optional] |
| **state_id** | **String** |  | [optional] |
| **country_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **postal_code** | **String** |  | [optional] |
| **number_of_decimals** | **Integer** |  | [optional] |
| **decimal_separator** | **String** |  | [optional] |
| **sell_to_all_countries** | **Boolean** |  | [optional] |
| **cart_options** | [**CartOptions**](CartOptions.md) |  | [optional] |
| **email_options** | [**EmailOptions**](EmailOptions.md) |  | [optional] |
| **coupons_options** | [**CouponsOptions**](CouponsOptions.md) |  | [optional] |
| **payment_options** | [**PaymentOptions**](PaymentOptions.md) |  | [optional] |
| **product_options** | **Object** |  | [optional] |
| **reviews_options** | [**ReviewsOptions**](ReviewsOptions.md) |  | [optional] |
| **advanced_options** | [**AdvancedOptions**](AdvancedOptions.md) |  | [optional] |
| **services_options** | [**ServicesOptions**](ServicesOptions.md) |  | [optional] |
| **inventory_options** | [**InventoryOptions**](InventoryOptions.md) |  | [optional] |
| **integration_options** | [**IntegrationOptions**](IntegrationOptions.md) |  | [optional] |
| **measurement_options** | [**MeasurementOptions**](MeasurementOptions.md) |  | [optional] |
| **downloadables_options** | [**DownloadablesOptions**](DownloadablesOptions.md) |  | [optional] |
| **subscriptions_options** | [**SubscriptionsOptions**](SubscriptionsOptions.md) |  | [optional] |
| **tax_calculation_options** | [**TaxCalculationOptions**](TaxCalculationOptions.md) |  | [optional] |
| **recommendation_options** | [**RecommendationOptions**](RecommendationOptions.md) |  | [optional] |
| **price_calculation_options** | [**PriceCalculationOptions**](PriceCalculationOptions.md) |  | [optional] |
| **identity_and_privacy_options** | [**IdentityAndPrivacyOptions**](IdentityAndPrivacyOptions.md) |  | [optional] |
| **included_selling_locations** | **Array&lt;String&gt;** |  | [optional] |
| **excluded_selling_locations** | **Array&lt;String&gt;** |  | [optional] |
| **included_shipping_locations** | **Array&lt;String&gt;** |  | [optional] |
| **excluded_shipping_locations** | **Array&lt;String&gt;** |  | [optional] |
| **currency_position** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::StoreOptions.new(
  enable: null,
  name: null,
  logo: null,
  footer_logo: null,
  tagline: null,
  description: null,
  address_line1: null,
  address_line2: null,
  city_id: null,
  state_id: null,
  country_id: null,
  currency_id: null,
  postal_code: null,
  number_of_decimals: null,
  decimal_separator: null,
  sell_to_all_countries: null,
  cart_options: null,
  email_options: null,
  coupons_options: null,
  payment_options: null,
  product_options: null,
  reviews_options: null,
  advanced_options: null,
  services_options: null,
  inventory_options: null,
  integration_options: null,
  measurement_options: null,
  downloadables_options: null,
  subscriptions_options: null,
  tax_calculation_options: null,
  recommendation_options: null,
  price_calculation_options: null,
  identity_and_privacy_options: null,
  included_selling_locations: null,
  excluded_selling_locations: null,
  included_shipping_locations: null,
  excluded_shipping_locations: null,
  currency_position: null
)
```

