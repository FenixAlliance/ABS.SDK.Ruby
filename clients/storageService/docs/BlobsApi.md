# OpenapiClient::BlobsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_blob_async**](BlobsApi.md#get_blob_async) | **GET** /api/v2/StorageService/Blobs/Single |  |
| [**get_blobs_async**](BlobsApi.md#get_blobs_async) | **GET** /api/v2/StorageService/Blobs |  |


## get_blob_async

> <BlobEnvelope> get_blob_async(opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlobsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  file_path: 'file_path_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.get_blob_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlobsApi->get_blob_async: #{e}"
end
```

#### Using the get_blob_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlobEnvelope>, Integer, Hash)> get_blob_async_with_http_info(opts)

```ruby
begin
  
  data, status_code, headers = api_instance.get_blob_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlobEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlobsApi->get_blob_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **file_path** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BlobEnvelope**](BlobEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## get_blobs_async

> <BlobEnvelope> get_blobs_async(opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlobsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  folder_path: 'folder_path_example', # String | 
  browse_filter: 'browse_filter_example', # String | 
  file_prefix: 'file_prefix_example', # String | 
  recurse: true, # Boolean | 
  max_results: 56, # Integer | 
  include_attributes: true, # Boolean | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.get_blobs_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlobsApi->get_blobs_async: #{e}"
end
```

#### Using the get_blobs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlobEnvelope>, Integer, Hash)> get_blobs_async_with_http_info(opts)

```ruby
begin
  
  data, status_code, headers = api_instance.get_blobs_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlobEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlobsApi->get_blobs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **folder_path** | **String** |  | [optional] |
| **browse_filter** | **String** |  | [optional] |
| **file_prefix** | **String** |  | [optional] |
| **recurse** | **Boolean** |  | [optional] |
| **max_results** | **Integer** |  | [optional] |
| **include_attributes** | **Boolean** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BlobEnvelope**](BlobEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png

