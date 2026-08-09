# OpenapiClient::SigningLogsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_signing_log_by_id_async**](SigningLogsApi.md#get_signing_log_by_id_async) | **GET** /api/v2/TrustService/SigningLogs/{id} | Get signing log by ID |
| [**get_signing_logs_async**](SigningLogsApi.md#get_signing_logs_async) | **GET** /api/v2/TrustService/SigningLogs | Get all signing logs |
| [**get_signing_logs_count_async**](SigningLogsApi.md#get_signing_logs_count_async) | **GET** /api/v2/TrustService/SigningLogs/Count | Get signing logs count |


## get_signing_log_by_id_async

> <SigningLogDto> get_signing_log_by_id_async(tenant_id, id, opts)

Get signing log by ID

Retrieves a specific signing log by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningLogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signing log by ID
  result = api_instance.get_signing_log_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningLogsApi->get_signing_log_by_id_async: #{e}"
end
```

#### Using the get_signing_log_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningLogDto>, Integer, Hash)> get_signing_log_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get signing log by ID
  data, status_code, headers = api_instance.get_signing_log_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningLogDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningLogsApi->get_signing_log_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SigningLogDto**](SigningLogDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signing_logs_async

> <SigningLogDtoListEnvelope> get_signing_logs_async(tenant_id, opts)

Get all signing logs

Retrieves all signing logs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningLogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_log_dto_collection_query_parameters: OpenapiClient::SigningLogDtoCollectionQueryParameters.new # SigningLogDtoCollectionQueryParameters | 
}

begin
  # Get all signing logs
  result = api_instance.get_signing_logs_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningLogsApi->get_signing_logs_async: #{e}"
end
```

#### Using the get_signing_logs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningLogDtoListEnvelope>, Integer, Hash)> get_signing_logs_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all signing logs
  data, status_code, headers = api_instance.get_signing_logs_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningLogDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningLogsApi->get_signing_logs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_log_dto_collection_query_parameters** | [**SigningLogDtoCollectionQueryParameters**](SigningLogDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SigningLogDtoListEnvelope**](SigningLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_signing_logs_count_async

> <Int32Envelope> get_signing_logs_count_async(tenant_id, opts)

Get signing logs count

Returns the count of signing logs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningLogsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_log_dto_collection_query_parameters: OpenapiClient::SigningLogDtoCollectionQueryParameters.new # SigningLogDtoCollectionQueryParameters | 
}

begin
  # Get signing logs count
  result = api_instance.get_signing_logs_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningLogsApi->get_signing_logs_count_async: #{e}"
end
```

#### Using the get_signing_logs_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_signing_logs_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get signing logs count
  data, status_code, headers = api_instance.get_signing_logs_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningLogsApi->get_signing_logs_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_log_dto_collection_query_parameters** | [**SigningLogDtoCollectionQueryParameters**](SigningLogDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

