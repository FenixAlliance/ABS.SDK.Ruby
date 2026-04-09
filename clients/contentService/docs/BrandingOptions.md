# OpenapiClient::BrandingOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **default_lang** | **String** |  | [optional] |
| **primary_color** | **String** |  | [optional] |
| **secondary_color** | **String** |  | [optional] |
| **header_logo** | [**Logo**](Logo.md) |  | [optional] |
| **footer_logo** | [**Logo**](Logo.md) |  | [optional] |
| **favicons** | [**Favicons**](Favicons.md) |  | [optional] |
| **apple_icon** | [**AppleIcons**](AppleIcons.md) |  | [optional] |
| **ms_app_tile** | [**MSAppTile**](MSAppTile.md) |  | [optional] |
| **dashboard** | [**DashboardOptions**](DashboardOptions.md) |  | [optional] |
| **studio** | [**StudioOptions**](StudioOptions.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BrandingOptions.new(
  default_lang: null,
  primary_color: null,
  secondary_color: null,
  header_logo: null,
  footer_logo: null,
  favicons: null,
  apple_icon: null,
  ms_app_tile: null,
  dashboard: null,
  studio: null
)
```

