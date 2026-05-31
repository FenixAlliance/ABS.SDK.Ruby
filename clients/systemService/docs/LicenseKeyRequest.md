# OpenapiClient::LicenseKeyRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **order_id** | **String** |  | [optional] |
| **payment_id** | **String** |  | [optional] |
| **invoice_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **entitlement_id** | **String** |  | [optional] |
| **seats** | **Integer** |  | [optional] |
| **license_type** | **String** |  | [optional] |
| **expiration_date** | **Time** |  | [optional] |
| **features** | [**Array&lt;LicenseFeature&gt;**](LicenseFeature.md) |  | [optional] |
| **additional_attributes** | [**Array&lt;AdditionalAttribute&gt;**](AdditionalAttribute.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::LicenseKeyRequest.new(
  user_id: null,
  tenant_id: null,
  order_id: null,
  payment_id: null,
  invoice_id: null,
  enrollment_id: null,
  entitlement_id: null,
  seats: null,
  license_type: null,
  expiration_date: null,
  features: null,
  additional_attributes: null
)
```

