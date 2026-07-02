# OpenapiClient::SupplierProfilesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_supplier_profile_async**](SupplierProfilesApi.md#create_supplier_profile_async) | **POST** /api/v2/LogisticsService/SupplierProfiles | Create a supplier profile |
| [**delete_supplier_profile_async**](SupplierProfilesApi.md#delete_supplier_profile_async) | **DELETE** /api/v2/LogisticsService/SupplierProfiles/{supplierProfileId} | Delete a supplier profile |
| [**get_supplier_profile_by_id_async**](SupplierProfilesApi.md#get_supplier_profile_by_id_async) | **GET** /api/v2/LogisticsService/SupplierProfiles/{supplierProfileId} | Get supplier profile by ID |
| [**get_supplier_profiles_async**](SupplierProfilesApi.md#get_supplier_profiles_async) | **GET** /api/v2/LogisticsService/SupplierProfiles | Get all supplier profiles |
| [**get_supplier_profiles_count_async**](SupplierProfilesApi.md#get_supplier_profiles_count_async) | **GET** /api/v2/LogisticsService/SupplierProfiles/Count | Get supplier profiles count |
| [**patch_supplier_profile_async**](SupplierProfilesApi.md#patch_supplier_profile_async) | **PATCH** /api/v2/LogisticsService/SupplierProfiles/{supplierProfileId} | Patch a supplier profile |
| [**update_supplier_profile_async**](SupplierProfilesApi.md#update_supplier_profile_async) | **PUT** /api/v2/LogisticsService/SupplierProfiles/{supplierProfileId} | Update a supplier profile |


## create_supplier_profile_async

> <EmptyEnvelope> create_supplier_profile_async(tenant_id, opts)

Create a supplier profile

Creates a new supplier profile for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupplierProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  supplier_profile_create_dto: OpenapiClient::SupplierProfileCreateDto.new # SupplierProfileCreateDto | 
}

begin
  # Create a supplier profile
  result = api_instance.create_supplier_profile_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->create_supplier_profile_async: #{e}"
end
```

#### Using the create_supplier_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_supplier_profile_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a supplier profile
  data, status_code, headers = api_instance.create_supplier_profile_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->create_supplier_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **supplier_profile_create_dto** | [**SupplierProfileCreateDto**](SupplierProfileCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_supplier_profile_async

> <EmptyEnvelope> delete_supplier_profile_async(tenant_id, supplier_profile_id, opts)

Delete a supplier profile

Deletes a supplier profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupplierProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
supplier_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a supplier profile
  result = api_instance.delete_supplier_profile_async(tenant_id, supplier_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->delete_supplier_profile_async: #{e}"
end
```

#### Using the delete_supplier_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_supplier_profile_async_with_http_info(tenant_id, supplier_profile_id, opts)

```ruby
begin
  # Delete a supplier profile
  data, status_code, headers = api_instance.delete_supplier_profile_async_with_http_info(tenant_id, supplier_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->delete_supplier_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **supplier_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_supplier_profile_by_id_async

> <SupplierProfileDtoEnvelope> get_supplier_profile_by_id_async(tenant_id, supplier_profile_id, opts)

Get supplier profile by ID

Retrieves a specific supplier profile by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupplierProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
supplier_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get supplier profile by ID
  result = api_instance.get_supplier_profile_by_id_async(tenant_id, supplier_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->get_supplier_profile_by_id_async: #{e}"
end
```

#### Using the get_supplier_profile_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupplierProfileDtoEnvelope>, Integer, Hash)> get_supplier_profile_by_id_async_with_http_info(tenant_id, supplier_profile_id, opts)

```ruby
begin
  # Get supplier profile by ID
  data, status_code, headers = api_instance.get_supplier_profile_by_id_async_with_http_info(tenant_id, supplier_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupplierProfileDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->get_supplier_profile_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **supplier_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupplierProfileDtoEnvelope**](SupplierProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_supplier_profiles_async

> <SupplierProfileDtoListEnvelope> get_supplier_profiles_async(tenant_id, opts)

Get all supplier profiles

Retrieves all supplier profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupplierProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all supplier profiles
  result = api_instance.get_supplier_profiles_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->get_supplier_profiles_async: #{e}"
end
```

#### Using the get_supplier_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupplierProfileDtoListEnvelope>, Integer, Hash)> get_supplier_profiles_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all supplier profiles
  data, status_code, headers = api_instance.get_supplier_profiles_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupplierProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->get_supplier_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupplierProfileDtoListEnvelope**](SupplierProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_supplier_profiles_count_async

> <Int32Envelope> get_supplier_profiles_count_async(tenant_id, opts)

Get supplier profiles count

Returns the count of supplier profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupplierProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get supplier profiles count
  result = api_instance.get_supplier_profiles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->get_supplier_profiles_count_async: #{e}"
end
```

#### Using the get_supplier_profiles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_supplier_profiles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get supplier profiles count
  data, status_code, headers = api_instance.get_supplier_profiles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->get_supplier_profiles_count_async_with_http_info: #{e}"
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


## patch_supplier_profile_async

> <EmptyEnvelope> patch_supplier_profile_async(tenant_id, supplier_profile_id, opts)

Patch a supplier profile

Applies a JSON Patch document to a supplier profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupplierProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
supplier_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a supplier profile
  result = api_instance.patch_supplier_profile_async(tenant_id, supplier_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->patch_supplier_profile_async: #{e}"
end
```

#### Using the patch_supplier_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_supplier_profile_async_with_http_info(tenant_id, supplier_profile_id, opts)

```ruby
begin
  # Patch a supplier profile
  data, status_code, headers = api_instance.patch_supplier_profile_async_with_http_info(tenant_id, supplier_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->patch_supplier_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **supplier_profile_id** | **String** |  |  |
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


## update_supplier_profile_async

> <EmptyEnvelope> update_supplier_profile_async(tenant_id, supplier_profile_id, opts)

Update a supplier profile

Updates an existing supplier profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupplierProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
supplier_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  supplier_profile_update_dto: OpenapiClient::SupplierProfileUpdateDto.new # SupplierProfileUpdateDto | 
}

begin
  # Update a supplier profile
  result = api_instance.update_supplier_profile_async(tenant_id, supplier_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->update_supplier_profile_async: #{e}"
end
```

#### Using the update_supplier_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_supplier_profile_async_with_http_info(tenant_id, supplier_profile_id, opts)

```ruby
begin
  # Update a supplier profile
  data, status_code, headers = api_instance.update_supplier_profile_async_with_http_info(tenant_id, supplier_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupplierProfilesApi->update_supplier_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **supplier_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **supplier_profile_update_dto** | [**SupplierProfileUpdateDto**](SupplierProfileUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

