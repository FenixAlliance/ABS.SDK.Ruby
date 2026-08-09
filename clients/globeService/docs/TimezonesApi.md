# OpenapiClient::TimezonesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_timezones_async**](TimezonesApi.md#count_timezones_async) | **GET** /api/v2/GlobeService/Timezones/Count | Count timezones |
| [**get_time_zone_by_id_async**](TimezonesApi.md#get_time_zone_by_id_async) | **GET** /api/v2/GlobeService/Timezones/{timeZoneId} | Get timezone by ID |
| [**get_time_zones_async**](TimezonesApi.md#get_time_zones_async) | **GET** /api/v2/GlobeService/Timezones | Get all timezones |


## count_timezones_async

> <Int32Envelope> count_timezones_async(opts)

Count timezones

Returns the total number of supported timezones, with optional OData filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimezonesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  timezone_dto_collection_query_parameters: OpenapiClient::TimezoneDtoCollectionQueryParameters.new # TimezoneDtoCollectionQueryParameters | 
}

begin
  # Count timezones
  result = api_instance.count_timezones_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimezonesApi->count_timezones_async: #{e}"
end
```

#### Using the count_timezones_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_timezones_async_with_http_info(opts)

```ruby
begin
  # Count timezones
  data, status_code, headers = api_instance.count_timezones_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimezonesApi->count_timezones_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **timezone_dto_collection_query_parameters** | [**TimezoneDtoCollectionQueryParameters**](TimezoneDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_time_zone_by_id_async

> <TimezoneDtoEnvelope> get_time_zone_by_id_async(time_zone_id, opts)

Get timezone by ID

Retrieves a single timezone by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimezonesApi.new
time_zone_id = 'time_zone_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get timezone by ID
  result = api_instance.get_time_zone_by_id_async(time_zone_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimezonesApi->get_time_zone_by_id_async: #{e}"
end
```

#### Using the get_time_zone_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TimezoneDtoEnvelope>, Integer, Hash)> get_time_zone_by_id_async_with_http_info(time_zone_id, opts)

```ruby
begin
  # Get timezone by ID
  data, status_code, headers = api_instance.get_time_zone_by_id_async_with_http_info(time_zone_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TimezoneDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimezonesApi->get_time_zone_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **time_zone_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TimezoneDtoEnvelope**](TimezoneDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_time_zones_async

> <TimezoneDtoListEnvelope> get_time_zones_async(opts)

Get all timezones

Retrieves the list of all supported timezones with optional OData pagination and filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TimezonesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  timezone_dto_collection_query_parameters: OpenapiClient::TimezoneDtoCollectionQueryParameters.new # TimezoneDtoCollectionQueryParameters | 
}

begin
  # Get all timezones
  result = api_instance.get_time_zones_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimezonesApi->get_time_zones_async: #{e}"
end
```

#### Using the get_time_zones_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TimezoneDtoListEnvelope>, Integer, Hash)> get_time_zones_async_with_http_info(opts)

```ruby
begin
  # Get all timezones
  data, status_code, headers = api_instance.get_time_zones_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TimezoneDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TimezonesApi->get_time_zones_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **timezone_dto_collection_query_parameters** | [**TimezoneDtoCollectionQueryParameters**](TimezoneDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TimezoneDtoListEnvelope**](TimezoneDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

