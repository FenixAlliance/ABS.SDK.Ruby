# OpenapiClient::ConnectionInfo

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **remote_ip_address** | [**IPAddress**](IPAddress.md) |  | [optional] |
| **remote_port** | **Integer** |  | [optional] |
| **local_ip_address** | [**IPAddress**](IPAddress.md) |  | [optional] |
| **local_port** | **Integer** |  | [optional] |
| **client_certificate** | [**X509Certificate2**](X509Certificate2.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ConnectionInfo.new(
  id: null,
  remote_ip_address: null,
  remote_port: null,
  local_ip_address: null,
  local_port: null,
  client_certificate: null
)
```

