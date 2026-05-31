# OpenapiClient::LicensesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**api_licensing_licenses_generate_post**](LicensesApi.md#api_licensing_licenses_generate_post) | **POST** /api/Licensing/Licenses/Generate |  |
| [**api_licensing_licenses_validate_attributes_get**](LicensesApi.md#api_licensing_licenses_validate_attributes_get) | **GET** /api/Licensing/Licenses/Validate/Attributes |  |
| [**api_licensing_licenses_validate_errors_get**](LicensesApi.md#api_licensing_licenses_validate_errors_get) | **GET** /api/Licensing/Licenses/Validate/Errors |  |
| [**api_licensing_licenses_validate_get**](LicensesApi.md#api_licensing_licenses_validate_get) | **GET** /api/Licensing/Licenses/Validate |  |


## api_licensing_licenses_generate_post

> <StringEnvelope> api_licensing_licenses_generate_post(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_key_request: OpenapiClient::LicenseKeyRequest.new # LicenseKeyRequest | 
}

begin
  
  result = api_instance.api_licensing_licenses_generate_post(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->api_licensing_licenses_generate_post: #{e}"
end
```

#### Using the api_licensing_licenses_generate_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StringEnvelope>, Integer, Hash)> api_licensing_licenses_generate_post_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_licensing_licenses_generate_post_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StringEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->api_licensing_licenses_generate_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_key_request** | [**LicenseKeyRequest**](LicenseKeyRequest.md) |  | [optional] |

### Return type

[**StringEnvelope**](StringEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## api_licensing_licenses_validate_attributes_get

> <LicenseAttributesListEnvelope> api_licensing_licenses_validate_attributes_get(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_key: OpenapiClient::LicenseKey.new # LicenseKey | 
}

begin
  
  result = api_instance.api_licensing_licenses_validate_attributes_get(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->api_licensing_licenses_validate_attributes_get: #{e}"
end
```

#### Using the api_licensing_licenses_validate_attributes_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseAttributesListEnvelope>, Integer, Hash)> api_licensing_licenses_validate_attributes_get_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_licensing_licenses_validate_attributes_get_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseAttributesListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->api_licensing_licenses_validate_attributes_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_key** | [**LicenseKey**](LicenseKey.md) |  | [optional] |

### Return type

[**LicenseAttributesListEnvelope**](LicenseAttributesListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## api_licensing_licenses_validate_errors_get

> <LicenseValidationErrorListEnvelope> api_licensing_licenses_validate_errors_get(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_key: OpenapiClient::LicenseKey.new # LicenseKey | 
}

begin
  
  result = api_instance.api_licensing_licenses_validate_errors_get(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->api_licensing_licenses_validate_errors_get: #{e}"
end
```

#### Using the api_licensing_licenses_validate_errors_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseValidationErrorListEnvelope>, Integer, Hash)> api_licensing_licenses_validate_errors_get_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_licensing_licenses_validate_errors_get_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseValidationErrorListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->api_licensing_licenses_validate_errors_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_key** | [**LicenseKey**](LicenseKey.md) |  | [optional] |

### Return type

[**LicenseValidationErrorListEnvelope**](LicenseValidationErrorListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## api_licensing_licenses_validate_get

> <BooleanEnvelope> api_licensing_licenses_validate_get(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_key: OpenapiClient::LicenseKey.new # LicenseKey | 
}

begin
  
  result = api_instance.api_licensing_licenses_validate_get(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->api_licensing_licenses_validate_get: #{e}"
end
```

#### Using the api_licensing_licenses_validate_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> api_licensing_licenses_validate_get_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_licensing_licenses_validate_get_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->api_licensing_licenses_validate_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_key** | [**LicenseKey**](LicenseKey.md) |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

