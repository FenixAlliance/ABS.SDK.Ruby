# OpenapiClient::SigningProfilesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_signing_profile_async**](SigningProfilesApi.md#create_signing_profile_async) | **POST** /api/v2/TrustService/SigningProfiles | Create a new signing profile |
| [**delete_signing_profile_async**](SigningProfilesApi.md#delete_signing_profile_async) | **DELETE** /api/v2/TrustService/SigningProfiles/{id} | Delete a signing profile |
| [**get_signing_profile_by_id_async**](SigningProfilesApi.md#get_signing_profile_by_id_async) | **GET** /api/v2/TrustService/SigningProfiles/{id} | Get signing profile by ID |
| [**get_signing_profiles_async**](SigningProfilesApi.md#get_signing_profiles_async) | **GET** /api/v2/TrustService/SigningProfiles | Get all signing profiles |
| [**get_signing_profiles_count_async**](SigningProfilesApi.md#get_signing_profiles_count_async) | **GET** /api/v2/TrustService/SigningProfiles/Count | Get signing profiles count |
| [**patch_signing_profile_async**](SigningProfilesApi.md#patch_signing_profile_async) | **PATCH** /api/v2/TrustService/SigningProfiles/{id} | Patch a signing profile |
| [**update_signing_profile_async**](SigningProfilesApi.md#update_signing_profile_async) | **PUT** /api/v2/TrustService/SigningProfiles/{id} | Update a signing profile |


## create_signing_profile_async

> create_signing_profile_async(tenant_id, opts)

Create a new signing profile

Creates a new signing profile for the specified tenant (supports inline contact creation).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_profile_create_dto: OpenapiClient::SigningProfileCreateDto.new # SigningProfileCreateDto | 
}

begin
  # Create a new signing profile
  api_instance.create_signing_profile_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->create_signing_profile_async: #{e}"
end
```

#### Using the create_signing_profile_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_signing_profile_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new signing profile
  data, status_code, headers = api_instance.create_signing_profile_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->create_signing_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_profile_create_dto** | [**SigningProfileCreateDto**](SigningProfileCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_signing_profile_async

> delete_signing_profile_async(tenant_id, id, opts)

Delete a signing profile

Deletes a signing profile for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a signing profile
  api_instance.delete_signing_profile_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->delete_signing_profile_async: #{e}"
end
```

#### Using the delete_signing_profile_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_signing_profile_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a signing profile
  data, status_code, headers = api_instance.delete_signing_profile_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->delete_signing_profile_async_with_http_info: #{e}"
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


## get_signing_profile_by_id_async

> <SigningProfileDto> get_signing_profile_by_id_async(tenant_id, id, opts)

Get signing profile by ID

Retrieves a specific signing profile by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signing profile by ID
  result = api_instance.get_signing_profile_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->get_signing_profile_by_id_async: #{e}"
end
```

#### Using the get_signing_profile_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningProfileDto>, Integer, Hash)> get_signing_profile_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get signing profile by ID
  data, status_code, headers = api_instance.get_signing_profile_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningProfileDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->get_signing_profile_by_id_async_with_http_info: #{e}"
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

[**SigningProfileDto**](SigningProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signing_profiles_async

> <SigningProfileDtoListEnvelope> get_signing_profiles_async(tenant_id, opts)

Get all signing profiles

Retrieves all signing profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_profile_dto_collection_query_parameters: OpenapiClient::SigningProfileDtoCollectionQueryParameters.new # SigningProfileDtoCollectionQueryParameters | 
}

begin
  # Get all signing profiles
  result = api_instance.get_signing_profiles_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->get_signing_profiles_async: #{e}"
end
```

#### Using the get_signing_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningProfileDtoListEnvelope>, Integer, Hash)> get_signing_profiles_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all signing profiles
  data, status_code, headers = api_instance.get_signing_profiles_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->get_signing_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_profile_dto_collection_query_parameters** | [**SigningProfileDtoCollectionQueryParameters**](SigningProfileDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SigningProfileDtoListEnvelope**](SigningProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_signing_profiles_count_async

> <Int32Envelope> get_signing_profiles_count_async(tenant_id, opts)

Get signing profiles count

Returns the count of signing profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_profile_dto_collection_query_parameters: OpenapiClient::SigningProfileDtoCollectionQueryParameters.new # SigningProfileDtoCollectionQueryParameters | 
}

begin
  # Get signing profiles count
  result = api_instance.get_signing_profiles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->get_signing_profiles_count_async: #{e}"
end
```

#### Using the get_signing_profiles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_signing_profiles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get signing profiles count
  data, status_code, headers = api_instance.get_signing_profiles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->get_signing_profiles_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_profile_dto_collection_query_parameters** | [**SigningProfileDtoCollectionQueryParameters**](SigningProfileDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_signing_profile_async

> <EmptyEnvelope> patch_signing_profile_async(tenant_id, id, opts)

Patch a signing profile

Patch a signing profile

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a signing profile
  result = api_instance.patch_signing_profile_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->patch_signing_profile_async: #{e}"
end
```

#### Using the patch_signing_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_signing_profile_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a signing profile
  data, status_code, headers = api_instance.patch_signing_profile_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->patch_signing_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_signing_profile_async

> update_signing_profile_async(tenant_id, id, opts)

Update a signing profile

Updates an existing signing profile for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_profile_update_dto: OpenapiClient::SigningProfileUpdateDto.new # SigningProfileUpdateDto | 
}

begin
  # Update a signing profile
  api_instance.update_signing_profile_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->update_signing_profile_async: #{e}"
end
```

#### Using the update_signing_profile_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_signing_profile_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a signing profile
  data, status_code, headers = api_instance.update_signing_profile_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfilesApi->update_signing_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_profile_update_dto** | [**SigningProfileUpdateDto**](SigningProfileUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

