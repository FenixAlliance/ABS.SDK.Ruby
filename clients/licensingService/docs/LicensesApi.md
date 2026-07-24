# OpenapiClient::LicensesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_license_async**](LicensesApi.md#create_license_async) | **POST** /api/v2/LicensingService/Licenses | Create a new license |
| [**delete_license_async**](LicensesApi.md#delete_license_async) | **DELETE** /api/v2/LicensingService/Licenses/{licenseId} | Delete a license |
| [**get_license_by_id_async**](LicensesApi.md#get_license_by_id_async) | **GET** /api/v2/LicensingService/Licenses/{licenseId} | Get license by ID |
| [**get_licenses_async**](LicensesApi.md#get_licenses_async) | **GET** /api/v2/LicensingService/Licenses | Get licenses |
| [**get_licenses_count_async**](LicensesApi.md#get_licenses_count_async) | **GET** /api/v2/LicensingService/Licenses/Count | Get licenses count |
| [**update_license_async**](LicensesApi.md#update_license_async) | **PUT** /api/v2/LicensingService/Licenses/{licenseId} | Update a license |


## create_license_async

> create_license_async(tenant_id, opts)

Create a new license

Creates a new license instance for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_create_dto: OpenapiClient::LicenseCreateDto.new({title: 'title_example'}) # LicenseCreateDto | 
}

begin
  # Create a new license
  api_instance.create_license_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->create_license_async: #{e}"
end
```

#### Using the create_license_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_license_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new license
  data, status_code, headers = api_instance.create_license_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->create_license_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_create_dto** | [**LicenseCreateDto**](LicenseCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_license_async

> delete_license_async(tenant_id, license_id, opts)

Delete a license

Deletes a license instance for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
license_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a license
  api_instance.delete_license_async(tenant_id, license_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->delete_license_async: #{e}"
end
```

#### Using the delete_license_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_license_async_with_http_info(tenant_id, license_id, opts)

```ruby
begin
  # Delete a license
  data, status_code, headers = api_instance.delete_license_async_with_http_info(tenant_id, license_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->delete_license_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **license_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_license_by_id_async

> <LicenseDto> get_license_by_id_async(tenant_id, license_id, opts)

Get license by ID

Retrieves a specific license instance by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
license_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get license by ID
  result = api_instance.get_license_by_id_async(tenant_id, license_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->get_license_by_id_async: #{e}"
end
```

#### Using the get_license_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseDto>, Integer, Hash)> get_license_by_id_async_with_http_info(tenant_id, license_id, opts)

```ruby
begin
  # Get license by ID
  data, status_code, headers = api_instance.get_license_by_id_async_with_http_info(tenant_id, license_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->get_license_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **license_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LicenseDto**](LicenseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_licenses_async

> <LicenseDtoListEnvelope> get_licenses_async(tenant_id, opts)

Get licenses

Retrieves the license instances owned by the specified tenant, filtered via OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get licenses
  result = api_instance.get_licenses_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->get_licenses_async: #{e}"
end
```

#### Using the get_licenses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseDtoListEnvelope>, Integer, Hash)> get_licenses_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get licenses
  data, status_code, headers = api_instance.get_licenses_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->get_licenses_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LicenseDtoListEnvelope**](LicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_licenses_count_async

> <Int32Envelope> get_licenses_count_async(tenant_id, opts)

Get licenses count

Returns the count of license instances owned by the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get licenses count
  result = api_instance.get_licenses_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->get_licenses_count_async: #{e}"
end
```

#### Using the get_licenses_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_licenses_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get licenses count
  data, status_code, headers = api_instance.get_licenses_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->get_licenses_count_async_with_http_info: #{e}"
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


## update_license_async

> update_license_async(tenant_id, license_id, opts)

Update a license

Updates an existing license instance for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicensesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
license_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_update_dto: OpenapiClient::LicenseUpdateDto.new # LicenseUpdateDto | 
}

begin
  # Update a license
  api_instance.update_license_async(tenant_id, license_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->update_license_async: #{e}"
end
```

#### Using the update_license_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_license_async_with_http_info(tenant_id, license_id, opts)

```ruby
begin
  # Update a license
  data, status_code, headers = api_instance.update_license_async_with_http_info(tenant_id, license_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicensesApi->update_license_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **license_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_update_dto** | [**LicenseUpdateDto**](LicenseUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

