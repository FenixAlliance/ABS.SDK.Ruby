# OpenapiClient::GoogleIntegrationOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable** | **Boolean** |  | [optional] |
| **google_maps** | [**GoogleMapsIntegrationOptions**](GoogleMapsIntegrationOptions.md) |  | [optional] |
| **google_merchant_center** | [**GoogleMerchantCenterIntegrationOptions**](GoogleMerchantCenterIntegrationOptions.md) |  | [optional] |
| **google_tag_manager** | [**GoogleTagManagerIntegrationOptions**](GoogleTagManagerIntegrationOptions.md) |  | [optional] |
| **google_recaptcha** | [**GoogleRecaptchaIntegrationOptions**](GoogleRecaptchaIntegrationOptions.md) |  | [optional] |
| **google_analytics** | [**GoogleAnalytics**](GoogleAnalytics.md) |  | [optional] |
| **google_my_business** | [**GoogleMyBusinessIntegrationOptions**](GoogleMyBusinessIntegrationOptions.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::GoogleIntegrationOptions.new(
  enable: null,
  google_maps: null,
  google_merchant_center: null,
  google_tag_manager: null,
  google_recaptcha: null,
  google_analytics: null,
  google_my_business: null
)
```

