# OpenapiClient::ActivityRecordsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_activity_records_count_async**](ActivityRecordsApi.md#get_activity_records_count_async) | **GET** /api/v2/ActivitiesService/ActivityRecords/Count | Count activity records |


## get_activity_records_count_async

> <Int32Envelope> get_activity_records_count_async(tenant_id, opts)

Count activity records

Returns the tenant-wide count of activity records across all feeds owned by the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityRecordsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count activity records
  result = api_instance.get_activity_records_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityRecordsApi->get_activity_records_count_async: #{e}"
end
```

#### Using the get_activity_records_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_activity_records_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count activity records
  data, status_code, headers = api_instance.get_activity_records_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityRecordsApi->get_activity_records_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

