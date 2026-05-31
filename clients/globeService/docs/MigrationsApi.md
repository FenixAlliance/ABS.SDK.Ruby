# OpenapiClient::MigrationsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**api_v2_global_system_migrate_post**](MigrationsApi.md#api_v2_global_system_migrate_post) | **POST** /api/v2/Global/System/Migrate |  |


## api_v2_global_system_migrate_post

> <PaymentResponse> api_v2_global_system_migrate_post(opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MigrationsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.api_v2_global_system_migrate_post(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MigrationsApi->api_v2_global_system_migrate_post: #{e}"
end
```

#### Using the api_v2_global_system_migrate_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentResponse>, Integer, Hash)> api_v2_global_system_migrate_post_with_http_info(opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_global_system_migrate_post_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MigrationsApi->api_v2_global_system_migrate_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentResponse**](PaymentResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

