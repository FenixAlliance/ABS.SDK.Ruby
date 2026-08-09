# OpenapiClient::PostingExecutionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_posting_executions_async**](PostingExecutionsApi.md#count_posting_executions_async) | **GET** /api/v2/AccountingService/PostingExecutions/Count | Count posting executions |
| [**get_posting_executions_async**](PostingExecutionsApi.md#get_posting_executions_async) | **GET** /api/v2/AccountingService/PostingExecutions | List posting executions |


## count_posting_executions_async

> <Int32Envelope> count_posting_executions_async(tenant_id, opts)

Count posting executions

Returns the count of the tenant's posting-inbox executions under the same OData shaping as the list read (e.g. $filter=Status eq 'Rejected' to count rejected intents). Requires journals_read.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PostingExecutionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  posting_execution_dto_collection_query_parameters: OpenapiClient::PostingExecutionDtoCollectionQueryParameters.new # PostingExecutionDtoCollectionQueryParameters | 
}

begin
  # Count posting executions
  result = api_instance.count_posting_executions_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PostingExecutionsApi->count_posting_executions_async: #{e}"
end
```

#### Using the count_posting_executions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_posting_executions_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count posting executions
  data, status_code, headers = api_instance.count_posting_executions_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PostingExecutionsApi->count_posting_executions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **posting_execution_dto_collection_query_parameters** | [**PostingExecutionDtoCollectionQueryParameters**](PostingExecutionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_posting_executions_async

> <PostingExecutionDtoIReadOnlyListEnvelope> get_posting_executions_async(tenant_id, opts)

List posting executions

Lists the tenant's posting-inbox executions (the durable evidence of every posting intent). Use OData to scope to a state — e.g. $filter=Status eq 'Rejected' for rejected intents, or Status eq 'PendingMapping'/'PendingPeriod'/'PendingRate' for the retryable pending set — and to page/order. Requires journals_read.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PostingExecutionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  posting_execution_dto_collection_query_parameters: OpenapiClient::PostingExecutionDtoCollectionQueryParameters.new # PostingExecutionDtoCollectionQueryParameters | 
}

begin
  # List posting executions
  result = api_instance.get_posting_executions_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PostingExecutionsApi->get_posting_executions_async: #{e}"
end
```

#### Using the get_posting_executions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PostingExecutionDtoIReadOnlyListEnvelope>, Integer, Hash)> get_posting_executions_async_with_http_info(tenant_id, opts)

```ruby
begin
  # List posting executions
  data, status_code, headers = api_instance.get_posting_executions_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PostingExecutionDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PostingExecutionsApi->get_posting_executions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **posting_execution_dto_collection_query_parameters** | [**PostingExecutionDtoCollectionQueryParameters**](PostingExecutionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**PostingExecutionDtoIReadOnlyListEnvelope**](PostingExecutionDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

