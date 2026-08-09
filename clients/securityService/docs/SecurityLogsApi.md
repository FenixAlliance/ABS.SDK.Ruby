# OpenapiClient::SecurityLogsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_security_logs_async**](SecurityLogsApi.md#get_security_logs_async) | **GET** /api/v2/SecurityService/SecurityLogs | Get business security logs |
| [**get_security_logs_count_async**](SecurityLogsApi.md#get_security_logs_count_async) | **GET** /api/v2/SecurityService/SecurityLogs/Count | Get business security logs count |


## get_security_logs_async

> <BusinessSecurityLogDtoListEnvelope> get_security_logs_async(tenant_id, opts)

Get business security logs

Retrieves security logs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SecurityLogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  business_security_log_dto_collection_query_parameters: OpenapiClient::BusinessSecurityLogDtoCollectionQueryParameters.new # BusinessSecurityLogDtoCollectionQueryParameters | 
}

begin
  # Get business security logs
  result = api_instance.get_security_logs_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SecurityLogsApi->get_security_logs_async: #{e}"
end
```

#### Using the get_security_logs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessSecurityLogDtoListEnvelope>, Integer, Hash)> get_security_logs_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get business security logs
  data, status_code, headers = api_instance.get_security_logs_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessSecurityLogDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SecurityLogsApi->get_security_logs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **business_security_log_dto_collection_query_parameters** | [**BusinessSecurityLogDtoCollectionQueryParameters**](BusinessSecurityLogDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BusinessSecurityLogDtoListEnvelope**](BusinessSecurityLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_security_logs_count_async

> <Int32Envelope> get_security_logs_count_async(tenant_id, opts)

Get business security logs count

Retrieves the count of security logs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SecurityLogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  business_security_log_dto_collection_query_parameters: OpenapiClient::BusinessSecurityLogDtoCollectionQueryParameters.new # BusinessSecurityLogDtoCollectionQueryParameters | 
}

begin
  # Get business security logs count
  result = api_instance.get_security_logs_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SecurityLogsApi->get_security_logs_count_async: #{e}"
end
```

#### Using the get_security_logs_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_security_logs_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get business security logs count
  data, status_code, headers = api_instance.get_security_logs_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SecurityLogsApi->get_security_logs_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **business_security_log_dto_collection_query_parameters** | [**BusinessSecurityLogDtoCollectionQueryParameters**](BusinessSecurityLogDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

