# OpenapiClient::IPLookupsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**delete_system_ip_lookup**](IPLookupsApi.md#delete_system_ip_lookup) | **DELETE** /api/v2/SystemService/IPLookups/{ipLookupId} | Delete a system IP lookup |
| [**get_system_ip_lookup_by_id**](IPLookupsApi.md#get_system_ip_lookup_by_id) | **GET** /api/v2/SystemService/IPLookups/{ipLookupId} | Retrieve a single system IP lookup by its ID |
| [**get_system_ip_lookups**](IPLookupsApi.md#get_system_ip_lookups) | **GET** /api/v2/SystemService/IPLookups | Retrieve a list of system IP lookups |
| [**get_system_ip_lookups_count**](IPLookupsApi.md#get_system_ip_lookups_count) | **GET** /api/v2/SystemService/IPLookups/Count | Get the count of system IP lookups |


## delete_system_ip_lookup

> <EmptyEnvelope> delete_system_ip_lookup(ip_lookup_id, opts)

Delete a system IP lookup

Delete a system IP lookup by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IPLookupsApi.new
ip_lookup_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a system IP lookup
  result = api_instance.delete_system_ip_lookup(ip_lookup_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IPLookupsApi->delete_system_ip_lookup: #{e}"
end
```

#### Using the delete_system_ip_lookup_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_system_ip_lookup_with_http_info(ip_lookup_id, opts)

```ruby
begin
  # Delete a system IP lookup
  data, status_code, headers = api_instance.delete_system_ip_lookup_with_http_info(ip_lookup_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IPLookupsApi->delete_system_ip_lookup_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **ip_lookup_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_ip_lookup_by_id

> <IPLookupDtoEnvelope> get_system_ip_lookup_by_id(ip_lookup_id, opts)

Retrieve a single system IP lookup by its ID

Retrieve a single system IP lookup by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IPLookupsApi.new
ip_lookup_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single system IP lookup by its ID
  result = api_instance.get_system_ip_lookup_by_id(ip_lookup_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IPLookupsApi->get_system_ip_lookup_by_id: #{e}"
end
```

#### Using the get_system_ip_lookup_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<IPLookupDtoEnvelope>, Integer, Hash)> get_system_ip_lookup_by_id_with_http_info(ip_lookup_id, opts)

```ruby
begin
  # Retrieve a single system IP lookup by its ID
  data, status_code, headers = api_instance.get_system_ip_lookup_by_id_with_http_info(ip_lookup_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <IPLookupDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IPLookupsApi->get_system_ip_lookup_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **ip_lookup_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**IPLookupDtoEnvelope**](IPLookupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_ip_lookups

> <IPLookupDtoListEnvelope> get_system_ip_lookups(opts)

Retrieve a list of system IP lookups

Retrieve a list of all IP lookups in the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IPLookupsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of system IP lookups
  result = api_instance.get_system_ip_lookups(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IPLookupsApi->get_system_ip_lookups: #{e}"
end
```

#### Using the get_system_ip_lookups_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<IPLookupDtoListEnvelope>, Integer, Hash)> get_system_ip_lookups_with_http_info(opts)

```ruby
begin
  # Retrieve a list of system IP lookups
  data, status_code, headers = api_instance.get_system_ip_lookups_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <IPLookupDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IPLookupsApi->get_system_ip_lookups_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**IPLookupDtoListEnvelope**](IPLookupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_ip_lookups_count

> <Int32Envelope> get_system_ip_lookups_count(opts)

Get the count of system IP lookups

Get the count of all IP lookups in the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IPLookupsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of system IP lookups
  result = api_instance.get_system_ip_lookups_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IPLookupsApi->get_system_ip_lookups_count: #{e}"
end
```

#### Using the get_system_ip_lookups_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_system_ip_lookups_count_with_http_info(opts)

```ruby
begin
  # Get the count of system IP lookups
  data, status_code, headers = api_instance.get_system_ip_lookups_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IPLookupsApi->get_system_ip_lookups_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

