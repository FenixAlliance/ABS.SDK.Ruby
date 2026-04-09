# OpenapiClient::Organization

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **legal_name** | **String** |  | [optional] |
| **business_name** | **String** |  | [optional] |
| **slogan** | **String** |  | [optional] |
| **homepage** | **String** |  | [optional] |
| **facebook_page_username** | **String** |  | [optional] |
| **instagram_username** | **String** |  | [optional] |
| **linked_in_username** | **String** |  | [optional] |
| **twitter_handler** | **String** |  | [optional] |
| **git_hub_username** | **String** |  | [optional] |
| **contact_points** | [**Array&lt;ContactPoint&gt;**](ContactPoint.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Organization.new(
  legal_name: null,
  business_name: null,
  slogan: null,
  homepage: null,
  facebook_page_username: null,
  instagram_username: null,
  linked_in_username: null,
  twitter_handler: null,
  git_hub_username: null,
  contact_points: null
)
```

