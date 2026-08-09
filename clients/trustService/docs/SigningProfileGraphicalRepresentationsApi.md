# OpenapiClient::SigningProfileGraphicalRepresentationsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_signing_profile_graphical_representation_async**](SigningProfileGraphicalRepresentationsApi.md#create_signing_profile_graphical_representation_async) | **POST** /api/v2/TrustService/SigningProfileGraphicalRepresentations | Create a new signature representation |
| [**delete_signing_profile_graphical_representation_async**](SigningProfileGraphicalRepresentationsApi.md#delete_signing_profile_graphical_representation_async) | **DELETE** /api/v2/TrustService/SigningProfileGraphicalRepresentations/{id} | Delete a signature representation |
| [**get_signing_profile_graphical_representation_by_id_async**](SigningProfileGraphicalRepresentationsApi.md#get_signing_profile_graphical_representation_by_id_async) | **GET** /api/v2/TrustService/SigningProfileGraphicalRepresentations/{id} | Get signature representation by ID |
| [**get_signing_profile_graphical_representations_async**](SigningProfileGraphicalRepresentationsApi.md#get_signing_profile_graphical_representations_async) | **GET** /api/v2/TrustService/SigningProfileGraphicalRepresentations | Get all signature representations |
| [**get_signing_profile_graphical_representations_count_async**](SigningProfileGraphicalRepresentationsApi.md#get_signing_profile_graphical_representations_count_async) | **GET** /api/v2/TrustService/SigningProfileGraphicalRepresentations/Count | Get signature representations count |
| [**patch_signing_profile_graphical_representation_async**](SigningProfileGraphicalRepresentationsApi.md#patch_signing_profile_graphical_representation_async) | **PATCH** /api/v2/TrustService/SigningProfileGraphicalRepresentations/{id} | Patch a signature representation |
| [**update_signing_profile_graphical_representation_async**](SigningProfileGraphicalRepresentationsApi.md#update_signing_profile_graphical_representation_async) | **PUT** /api/v2/TrustService/SigningProfileGraphicalRepresentations/{id} | Update a signature representation |


## create_signing_profile_graphical_representation_async

> create_signing_profile_graphical_representation_async(tenant_id, opts)

Create a new signature representation

Creates a new reusable signature representation for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfileGraphicalRepresentationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_profile_graphical_representation_create_dto: OpenapiClient::SigningProfileGraphicalRepresentationCreateDto.new({signing_profile_id: 'signing_profile_id_example', kind: 'Drawn'}) # SigningProfileGraphicalRepresentationCreateDto | 
}

begin
  # Create a new signature representation
  api_instance.create_signing_profile_graphical_representation_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->create_signing_profile_graphical_representation_async: #{e}"
end
```

#### Using the create_signing_profile_graphical_representation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_signing_profile_graphical_representation_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new signature representation
  data, status_code, headers = api_instance.create_signing_profile_graphical_representation_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->create_signing_profile_graphical_representation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_profile_graphical_representation_create_dto** | [**SigningProfileGraphicalRepresentationCreateDto**](SigningProfileGraphicalRepresentationCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_signing_profile_graphical_representation_async

> delete_signing_profile_graphical_representation_async(tenant_id, id, opts)

Delete a signature representation

Deletes a signature representation for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfileGraphicalRepresentationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a signature representation
  api_instance.delete_signing_profile_graphical_representation_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->delete_signing_profile_graphical_representation_async: #{e}"
end
```

#### Using the delete_signing_profile_graphical_representation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_signing_profile_graphical_representation_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a signature representation
  data, status_code, headers = api_instance.delete_signing_profile_graphical_representation_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->delete_signing_profile_graphical_representation_async_with_http_info: #{e}"
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


## get_signing_profile_graphical_representation_by_id_async

> <SigningProfileGraphicalRepresentationDto> get_signing_profile_graphical_representation_by_id_async(tenant_id, id, opts)

Get signature representation by ID

Retrieves a specific signature representation by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfileGraphicalRepresentationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signature representation by ID
  result = api_instance.get_signing_profile_graphical_representation_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->get_signing_profile_graphical_representation_by_id_async: #{e}"
end
```

#### Using the get_signing_profile_graphical_representation_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningProfileGraphicalRepresentationDto>, Integer, Hash)> get_signing_profile_graphical_representation_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get signature representation by ID
  data, status_code, headers = api_instance.get_signing_profile_graphical_representation_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningProfileGraphicalRepresentationDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->get_signing_profile_graphical_representation_by_id_async_with_http_info: #{e}"
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

[**SigningProfileGraphicalRepresentationDto**](SigningProfileGraphicalRepresentationDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signing_profile_graphical_representations_async

> <SigningProfileGraphicalRepresentationDtoListEnvelope> get_signing_profile_graphical_representations_async(tenant_id, opts)

Get all signature representations

Retrieves all reusable signature representations for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfileGraphicalRepresentationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_profile_graphical_representation_dto_collection_query_parameters: OpenapiClient::SigningProfileGraphicalRepresentationDtoCollectionQueryParameters.new # SigningProfileGraphicalRepresentationDtoCollectionQueryParameters | 
}

begin
  # Get all signature representations
  result = api_instance.get_signing_profile_graphical_representations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->get_signing_profile_graphical_representations_async: #{e}"
end
```

#### Using the get_signing_profile_graphical_representations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SigningProfileGraphicalRepresentationDtoListEnvelope>, Integer, Hash)> get_signing_profile_graphical_representations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all signature representations
  data, status_code, headers = api_instance.get_signing_profile_graphical_representations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SigningProfileGraphicalRepresentationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->get_signing_profile_graphical_representations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_profile_graphical_representation_dto_collection_query_parameters** | [**SigningProfileGraphicalRepresentationDtoCollectionQueryParameters**](SigningProfileGraphicalRepresentationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SigningProfileGraphicalRepresentationDtoListEnvelope**](SigningProfileGraphicalRepresentationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_signing_profile_graphical_representations_count_async

> <Int32Envelope> get_signing_profile_graphical_representations_count_async(tenant_id, opts)

Get signature representations count

Returns the count of signature representations for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfileGraphicalRepresentationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_profile_graphical_representation_dto_collection_query_parameters: OpenapiClient::SigningProfileGraphicalRepresentationDtoCollectionQueryParameters.new # SigningProfileGraphicalRepresentationDtoCollectionQueryParameters | 
}

begin
  # Get signature representations count
  result = api_instance.get_signing_profile_graphical_representations_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->get_signing_profile_graphical_representations_count_async: #{e}"
end
```

#### Using the get_signing_profile_graphical_representations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_signing_profile_graphical_representations_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get signature representations count
  data, status_code, headers = api_instance.get_signing_profile_graphical_representations_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->get_signing_profile_graphical_representations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_profile_graphical_representation_dto_collection_query_parameters** | [**SigningProfileGraphicalRepresentationDtoCollectionQueryParameters**](SigningProfileGraphicalRepresentationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_signing_profile_graphical_representation_async

> <EmptyEnvelope> patch_signing_profile_graphical_representation_async(tenant_id, id, opts)

Patch a signature representation

Patch a signature representation

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfileGraphicalRepresentationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a signature representation
  result = api_instance.patch_signing_profile_graphical_representation_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->patch_signing_profile_graphical_representation_async: #{e}"
end
```

#### Using the patch_signing_profile_graphical_representation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_signing_profile_graphical_representation_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a signature representation
  data, status_code, headers = api_instance.patch_signing_profile_graphical_representation_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->patch_signing_profile_graphical_representation_async_with_http_info: #{e}"
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


## update_signing_profile_graphical_representation_async

> update_signing_profile_graphical_representation_async(tenant_id, id, opts)

Update a signature representation

Updates an existing signature representation for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningProfileGraphicalRepresentationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signing_profile_graphical_representation_update_dto: OpenapiClient::SigningProfileGraphicalRepresentationUpdateDto.new # SigningProfileGraphicalRepresentationUpdateDto | 
}

begin
  # Update a signature representation
  api_instance.update_signing_profile_graphical_representation_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->update_signing_profile_graphical_representation_async: #{e}"
end
```

#### Using the update_signing_profile_graphical_representation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_signing_profile_graphical_representation_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a signature representation
  data, status_code, headers = api_instance.update_signing_profile_graphical_representation_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningProfileGraphicalRepresentationsApi->update_signing_profile_graphical_representation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signing_profile_graphical_representation_update_dto** | [**SigningProfileGraphicalRepresentationUpdateDto**](SigningProfileGraphicalRepresentationUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

