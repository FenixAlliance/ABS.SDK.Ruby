# OpenapiClient::SeoOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **keywords** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **logo** | **String** |  | [optional] |
| **social_image** | **String** |  | [optional] |
| **title_suffix** | **String** |  | [optional] |
| **bing_verification_code** | **String** |  | [optional] |
| **google_verification_code** | **String** |  | [optional] |
| **pinterest_verification_code** | **String** |  | [optional] |
| **creator** | [**Creator**](Creator.md) |  | [optional] |
| **organization** | [**Organization**](Organization.md) |  | [optional] |
| **same_as** | **Array&lt;String&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SeoOptions.new(
  keywords: null,
  description: null,
  logo: null,
  social_image: null,
  title_suffix: null,
  bing_verification_code: null,
  google_verification_code: null,
  pinterest_verification_code: null,
  creator: null,
  organization: null,
  same_as: null
)
```

