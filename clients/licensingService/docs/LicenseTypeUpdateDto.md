# OpenapiClient::LicenseTypeUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **allow_trials** | **Boolean** |  | [optional] |
| **is_perpetual_license** | **Boolean** |  | [optional] |
| **max_license_usages** | **Integer** |  | [optional] |
| **trial_license_relative_expiration_in_days** | **Integer** |  | [optional] |
| **standard_license_relative_expiration_in_days** | **Integer** |  | [optional] |
| **licensing_certificate_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::LicenseTypeUpdateDto.new(
  title: null,
  description: null,
  allow_trials: null,
  is_perpetual_license: null,
  max_license_usages: null,
  trial_license_relative_expiration_in_days: null,
  standard_license_relative_expiration_in_days: null,
  licensing_certificate_id: null
)
```

