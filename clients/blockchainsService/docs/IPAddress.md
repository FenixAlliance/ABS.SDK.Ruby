# OpenapiClient::IPAddress

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **address_family** | **String** |  | [optional][readonly] |
| **scope_id** | **Integer** |  | [optional] |
| **is_ipv6_multicast** | **Boolean** |  | [optional][readonly] |
| **is_ipv6_link_local** | **Boolean** |  | [optional][readonly] |
| **is_ipv6_site_local** | **Boolean** |  | [optional][readonly] |
| **is_ipv6_teredo** | **Boolean** |  | [optional][readonly] |
| **is_ipv6_unique_local** | **Boolean** |  | [optional][readonly] |
| **is_ipv4_mapped_to_ipv6** | **Boolean** |  | [optional][readonly] |
| **address** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IPAddress.new(
  address_family: null,
  scope_id: null,
  is_ipv6_multicast: null,
  is_ipv6_link_local: null,
  is_ipv6_site_local: null,
  is_ipv6_teredo: null,
  is_ipv6_unique_local: null,
  is_ipv4_mapped_to_ipv6: null,
  address: null
)
```

