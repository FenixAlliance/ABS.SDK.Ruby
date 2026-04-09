# OpenapiClient::PortalSettings

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable** | **Boolean** |  | [optional] |
| **portal_id** | **String** |  | [optional] |
| **scopes** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **home_page_id** | **String** |  | [optional] |
| **blog_page_id** | **String** |  | [optional] |
| **store_page_id** | **String** |  | [optional] |
| **base_endpoint** | **String** |  | [optional] |
| **store_route_prefix** | **String** |  | [optional] |
| **public_key** | **String** |  | [optional] |
| **private_key** | **String** |  | [optional] |
| **auth_token** | **String** |  | [optional] |
| **auth_token_type** | **String** |  | [optional] |
| **auth_token_expiration** | **Integer** |  | [optional] |
| **options** | [**PortalOptions**](PortalOptions.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PortalSettings.new(
  enable: null,
  portal_id: null,
  scopes: null,
  tenant_id: null,
  home_page_id: null,
  blog_page_id: null,
  store_page_id: null,
  base_endpoint: null,
  store_route_prefix: null,
  public_key: null,
  private_key: null,
  auth_token: null,
  auth_token_type: null,
  auth_token_expiration: null,
  options: null
)
```

