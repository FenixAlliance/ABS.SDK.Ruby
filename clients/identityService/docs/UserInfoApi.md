# OpenapiClient::UserInfoApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**connect_userinfo_get**](UserInfoApi.md#connect_userinfo_get) | **GET** /connect/userinfo |  |
| [**connect_userinfo_post**](UserInfoApi.md#connect_userinfo_post) | **POST** /connect/userinfo |  |


## connect_userinfo_get

> connect_userinfo_get(opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UserInfoApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  api_instance.connect_userinfo_get(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserInfoApi->connect_userinfo_get: #{e}"
end
```

#### Using the connect_userinfo_get_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> connect_userinfo_get_with_http_info(opts)

```ruby
begin
  
  data, status_code, headers = api_instance.connect_userinfo_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserInfoApi->connect_userinfo_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## connect_userinfo_post

> connect_userinfo_post(opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UserInfoApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  api_instance.connect_userinfo_post(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserInfoApi->connect_userinfo_post: #{e}"
end
```

#### Using the connect_userinfo_post_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> connect_userinfo_post_with_http_info(opts)

```ruby
begin
  
  data, status_code, headers = api_instance.connect_userinfo_post_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserInfoApi->connect_userinfo_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

