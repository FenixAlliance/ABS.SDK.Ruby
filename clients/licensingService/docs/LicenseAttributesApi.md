# OpenapiClient::LicenseAttributesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_license_attribute_async**](LicenseAttributesApi.md#create_license_attribute_async) | **POST** /api/v2/LicensingService/LicenseAttributes | Create a new license attribute |
| [**delete_license_attribute_async**](LicenseAttributesApi.md#delete_license_attribute_async) | **DELETE** /api/v2/LicensingService/LicenseAttributes/{id} | Delete a license attribute |
| [**get_license_attribute_by_id_async**](LicenseAttributesApi.md#get_license_attribute_by_id_async) | **GET** /api/v2/LicensingService/LicenseAttributes/{id} | Get license attribute by ID |
| [**get_license_attributes_async**](LicenseAttributesApi.md#get_license_attributes_async) | **GET** /api/v2/LicensingService/LicenseAttributes | Get all license attributes |
| [**get_license_attributes_count_async**](LicenseAttributesApi.md#get_license_attributes_count_async) | **GET** /api/v2/LicensingService/LicenseAttributes/Count | Get license attributes count |
| [**patch_license_attribute_async**](LicenseAttributesApi.md#patch_license_attribute_async) | **PATCH** /api/v2/LicensingService/LicenseAttributes/{id} | Patch a license attribute |
| [**update_license_attribute_async**](LicenseAttributesApi.md#update_license_attribute_async) | **PUT** /api/v2/LicensingService/LicenseAttributes/{id} | Update a license attribute |


## create_license_attribute_async

> create_license_attribute_async(tenant_id, opts)

Create a new license attribute

Creates a new license attribute for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_attribute_create_dto: OpenapiClient::LicenseAttributeCreateDto.new({name: 'name_example'}) # LicenseAttributeCreateDto | 
}

begin
  # Create a new license attribute
  api_instance.create_license_attribute_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->create_license_attribute_async: #{e}"
end
```

#### Using the create_license_attribute_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_license_attribute_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new license attribute
  data, status_code, headers = api_instance.create_license_attribute_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->create_license_attribute_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_attribute_create_dto** | [**LicenseAttributeCreateDto**](LicenseAttributeCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_license_attribute_async

> delete_license_attribute_async(tenant_id, id, opts)

Delete a license attribute

Deletes a license attribute for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a license attribute
  api_instance.delete_license_attribute_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->delete_license_attribute_async: #{e}"
end
```

#### Using the delete_license_attribute_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_license_attribute_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a license attribute
  data, status_code, headers = api_instance.delete_license_attribute_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->delete_license_attribute_async_with_http_info: #{e}"
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

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_license_attribute_by_id_async

> <LicenseAttributeDto> get_license_attribute_by_id_async(tenant_id, id, opts)

Get license attribute by ID

Retrieves a specific license attribute by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get license attribute by ID
  result = api_instance.get_license_attribute_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->get_license_attribute_by_id_async: #{e}"
end
```

#### Using the get_license_attribute_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseAttributeDto>, Integer, Hash)> get_license_attribute_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get license attribute by ID
  data, status_code, headers = api_instance.get_license_attribute_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseAttributeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->get_license_attribute_by_id_async_with_http_info: #{e}"
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

[**LicenseAttributeDto**](LicenseAttributeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_license_attributes_async

> <LicenseAttributeDtoListEnvelope> get_license_attributes_async(tenant_id, opts)

Get all license attributes

Retrieves all license attributes for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all license attributes
  result = api_instance.get_license_attributes_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->get_license_attributes_async: #{e}"
end
```

#### Using the get_license_attributes_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseAttributeDtoListEnvelope>, Integer, Hash)> get_license_attributes_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all license attributes
  data, status_code, headers = api_instance.get_license_attributes_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseAttributeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->get_license_attributes_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LicenseAttributeDtoListEnvelope**](LicenseAttributeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_license_attributes_count_async

> <Int32Envelope> get_license_attributes_count_async(tenant_id, opts)

Get license attributes count

Returns the count of license attributes for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get license attributes count
  result = api_instance.get_license_attributes_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->get_license_attributes_count_async: #{e}"
end
```

#### Using the get_license_attributes_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_license_attributes_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get license attributes count
  data, status_code, headers = api_instance.get_license_attributes_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->get_license_attributes_count_async_with_http_info: #{e}"
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


## patch_license_attribute_async

> <EmptyEnvelope> patch_license_attribute_async(tenant_id, id, opts)

Patch a license attribute

Patch a license attribute for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a license attribute
  result = api_instance.patch_license_attribute_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->patch_license_attribute_async: #{e}"
end
```

#### Using the patch_license_attribute_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_license_attribute_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a license attribute
  data, status_code, headers = api_instance.patch_license_attribute_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->patch_license_attribute_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_license_attribute_async

> update_license_attribute_async(tenant_id, id, opts)

Update a license attribute

Updates an existing license attribute for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_attribute_update_dto: OpenapiClient::LicenseAttributeUpdateDto.new # LicenseAttributeUpdateDto | 
}

begin
  # Update a license attribute
  api_instance.update_license_attribute_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->update_license_attribute_async: #{e}"
end
```

#### Using the update_license_attribute_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_license_attribute_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a license attribute
  data, status_code, headers = api_instance.update_license_attribute_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseAttributesApi->update_license_attribute_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_attribute_update_dto** | [**LicenseAttributeUpdateDto**](LicenseAttributeUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

