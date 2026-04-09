# OpenapiClient::IntegrationsOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable** | **Boolean** |  | [optional] |
| **e_payco** | [**EPaycoIntegrationOptions**](EPaycoIntegrationOptions.md) |  | [optional] |
| **google** | [**GoogleIntegrationOptions**](GoogleIntegrationOptions.md) |  | [optional] |
| **facebook** | [**FacebookIntegrationOptions**](FacebookIntegrationOptions.md) |  | [optional] |
| **sendgrid** | [**SendgridIntegrationsOptions**](SendgridIntegrationsOptions.md) |  | [optional] |
| **free_geo_ip** | [**FreeGeoIPIntegrationOptions**](FreeGeoIPIntegrationOptions.md) |  | [optional] |
| **microsoft** | [**MicrosoftIntegrationsOptions**](MicrosoftIntegrationsOptions.md) |  | [optional] |
| **fenix_alliance** | [**FenixAllianceIntegrationsOptions**](FenixAllianceIntegrationsOptions.md) |  | [optional] |
| **open_exchange_rates** | [**OpenExchangeRatesIntegrationsOptions**](OpenExchangeRatesIntegrationsOptions.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IntegrationsOptions.new(
  enable: null,
  e_payco: null,
  google: null,
  facebook: null,
  sendgrid: null,
  free_geo_ip: null,
  microsoft: null,
  fenix_alliance: null,
  open_exchange_rates: null
)
```

