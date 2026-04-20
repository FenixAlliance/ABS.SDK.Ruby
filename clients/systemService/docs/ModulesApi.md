# OpenapiClient::ModulesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_all_modules**](ModulesApi.md#get_all_modules) | **GET** /api/v2/StudioService/Modules | Get all modules available on this suite server instance. |
| [**get_available_modules**](ModulesApi.md#get_available_modules) | **GET** /api/v2/StudioService/Modules/Data | Get all modules available to a tenant user. |


## get_all_modules

> <StudioModuleListEnvelope> get_all_modules(tenant_id, opts)

Get all modules available on this suite server instance.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ModulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all modules available on this suite server instance.
  result = api_instance.get_all_modules(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ModulesApi->get_all_modules: #{e}"
end
```

#### Using the get_all_modules_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StudioModuleListEnvelope>, Integer, Hash)> get_all_modules_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all modules available on this suite server instance.
  data, status_code, headers = api_instance.get_all_modules_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StudioModuleListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ModulesApi->get_all_modules_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**StudioModuleListEnvelope**](StudioModuleListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_available_modules

> <ModuleListEnvelope> get_available_modules(opts)

Get all modules available to a tenant user.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ModulesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all modules available to a tenant user.
  result = api_instance.get_available_modules(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ModulesApi->get_available_modules: #{e}"
end
```

#### Using the get_available_modules_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ModuleListEnvelope>, Integer, Hash)> get_available_modules_with_http_info(opts)

```ruby
begin
  # Get all modules available to a tenant user.
  data, status_code, headers = api_instance.get_available_modules_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ModuleListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ModulesApi->get_available_modules_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ModuleListEnvelope**](ModuleListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

