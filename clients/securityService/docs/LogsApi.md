# OpenapiClient::LogsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_logs_async**](LogsApi.md#get_logs_async) | **GET** /api/v2/SecurityService/Logs | Get tenant logs |
| [**get_logs_count_async**](LogsApi.md#get_logs_count_async) | **GET** /api/v2/SecurityService/Logs/Count | Get tenant logs count |


## get_logs_async

> <LogDtoListEnvelope> get_logs_async(tenant_id, opts)

Get tenant logs

Retrieves logs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  log_dto_collection_query_parameters: OpenapiClient::LogDtoCollectionQueryParameters.new # LogDtoCollectionQueryParameters | 
}

begin
  # Get tenant logs
  result = api_instance.get_logs_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LogsApi->get_logs_async: #{e}"
end
```

#### Using the get_logs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LogDtoListEnvelope>, Integer, Hash)> get_logs_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get tenant logs
  data, status_code, headers = api_instance.get_logs_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LogDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LogsApi->get_logs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **log_dto_collection_query_parameters** | [**LogDtoCollectionQueryParameters**](LogDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**LogDtoListEnvelope**](LogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_logs_count_async

> <Int32Envelope> get_logs_count_async(tenant_id, opts)

Get tenant logs count

Retrieves the count of logs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  log_dto_collection_query_parameters: OpenapiClient::LogDtoCollectionQueryParameters.new # LogDtoCollectionQueryParameters | 
}

begin
  # Get tenant logs count
  result = api_instance.get_logs_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LogsApi->get_logs_count_async: #{e}"
end
```

#### Using the get_logs_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_logs_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get tenant logs count
  data, status_code, headers = api_instance.get_logs_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LogsApi->get_logs_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **log_dto_collection_query_parameters** | [**LogDtoCollectionQueryParameters**](LogDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

