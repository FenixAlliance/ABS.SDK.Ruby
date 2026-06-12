# OpenapiClient::LoyaltyProgramsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_loyalty_programs_async**](LoyaltyProgramsApi.md#count_loyalty_programs_async) | **GET** /api/v2/SalesService/LoyaltyPrograms/Count | Get loyalty programs count |
| [**create_loyalty_program_async**](LoyaltyProgramsApi.md#create_loyalty_program_async) | **POST** /api/v2/SalesService/LoyaltyPrograms | Create a loyalty program |
| [**delete_loyalty_program_async**](LoyaltyProgramsApi.md#delete_loyalty_program_async) | **DELETE** /api/v2/SalesService/LoyaltyPrograms/{loyaltyProgramId} | Delete a loyalty program |
| [**get_loyalty_program_async**](LoyaltyProgramsApi.md#get_loyalty_program_async) | **GET** /api/v2/SalesService/LoyaltyPrograms/{loyaltyProgramId} | Get loyalty program by ID |
| [**get_loyalty_programs_async**](LoyaltyProgramsApi.md#get_loyalty_programs_async) | **GET** /api/v2/SalesService/LoyaltyPrograms | Get loyalty programs |
| [**patch_loyalty_program_async**](LoyaltyProgramsApi.md#patch_loyalty_program_async) | **PATCH** /api/v2/SalesService/LoyaltyPrograms/{loyaltyProgramId} | Patch a loyalty program |
| [**update_loyalty_program_async**](LoyaltyProgramsApi.md#update_loyalty_program_async) | **PUT** /api/v2/SalesService/LoyaltyPrograms/{loyaltyProgramId} | Update a loyalty program |


## count_loyalty_programs_async

> <Int32Envelope> count_loyalty_programs_async(tenant_id)

Get loyalty programs count

Returns the total count of loyalty programs for the specified tenant with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoyaltyProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get loyalty programs count
  result = api_instance.count_loyalty_programs_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->count_loyalty_programs_async: #{e}"
end
```

#### Using the count_loyalty_programs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_loyalty_programs_async_with_http_info(tenant_id)

```ruby
begin
  # Get loyalty programs count
  data, status_code, headers = api_instance.count_loyalty_programs_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->count_loyalty_programs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_loyalty_program_async

> <EmptyEnvelope> create_loyalty_program_async(tenant_id, opts)

Create a loyalty program

Creates a new loyalty program for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoyaltyProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  loyalty_program_create_dto: OpenapiClient::LoyaltyProgramCreateDto.new({title: 'title_example'}) # LoyaltyProgramCreateDto | 
}

begin
  # Create a loyalty program
  result = api_instance.create_loyalty_program_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->create_loyalty_program_async: #{e}"
end
```

#### Using the create_loyalty_program_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_loyalty_program_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a loyalty program
  data, status_code, headers = api_instance.create_loyalty_program_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->create_loyalty_program_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loyalty_program_create_dto** | [**LoyaltyProgramCreateDto**](LoyaltyProgramCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_loyalty_program_async

> <EmptyEnvelope> delete_loyalty_program_async(tenant_id, loyalty_program_id)

Delete a loyalty program

Deletes an existing loyalty program by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoyaltyProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loyalty_program_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a loyalty program
  result = api_instance.delete_loyalty_program_async(tenant_id, loyalty_program_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->delete_loyalty_program_async: #{e}"
end
```

#### Using the delete_loyalty_program_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_loyalty_program_async_with_http_info(tenant_id, loyalty_program_id)

```ruby
begin
  # Delete a loyalty program
  data, status_code, headers = api_instance.delete_loyalty_program_async_with_http_info(tenant_id, loyalty_program_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->delete_loyalty_program_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loyalty_program_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_loyalty_program_async

> <LoyaltyProgramDtoEnvelope> get_loyalty_program_async(tenant_id, loyalty_program_id)

Get loyalty program by ID

Retrieves a single loyalty program by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoyaltyProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loyalty_program_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get loyalty program by ID
  result = api_instance.get_loyalty_program_async(tenant_id, loyalty_program_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->get_loyalty_program_async: #{e}"
end
```

#### Using the get_loyalty_program_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LoyaltyProgramDtoEnvelope>, Integer, Hash)> get_loyalty_program_async_with_http_info(tenant_id, loyalty_program_id)

```ruby
begin
  # Get loyalty program by ID
  data, status_code, headers = api_instance.get_loyalty_program_async_with_http_info(tenant_id, loyalty_program_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LoyaltyProgramDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->get_loyalty_program_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loyalty_program_id** | **String** |  |  |

### Return type

[**LoyaltyProgramDtoEnvelope**](LoyaltyProgramDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_loyalty_programs_async

> <LoyaltyProgramDtoListEnvelope> get_loyalty_programs_async(tenant_id)

Get loyalty programs

Retrieves a list of loyalty programs for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoyaltyProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get loyalty programs
  result = api_instance.get_loyalty_programs_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->get_loyalty_programs_async: #{e}"
end
```

#### Using the get_loyalty_programs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LoyaltyProgramDtoListEnvelope>, Integer, Hash)> get_loyalty_programs_async_with_http_info(tenant_id)

```ruby
begin
  # Get loyalty programs
  data, status_code, headers = api_instance.get_loyalty_programs_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LoyaltyProgramDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->get_loyalty_programs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**LoyaltyProgramDtoListEnvelope**](LoyaltyProgramDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_loyalty_program_async

> <EmptyEnvelope> patch_loyalty_program_async(tenant_id, loyalty_program_id, opts)

Patch a loyalty program

Partially updates an existing loyalty program using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoyaltyProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loyalty_program_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a loyalty program
  result = api_instance.patch_loyalty_program_async(tenant_id, loyalty_program_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->patch_loyalty_program_async: #{e}"
end
```

#### Using the patch_loyalty_program_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_loyalty_program_async_with_http_info(tenant_id, loyalty_program_id, opts)

```ruby
begin
  # Patch a loyalty program
  data, status_code, headers = api_instance.patch_loyalty_program_async_with_http_info(tenant_id, loyalty_program_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->patch_loyalty_program_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loyalty_program_id** | **String** |  |  |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_loyalty_program_async

> <EmptyEnvelope> update_loyalty_program_async(tenant_id, loyalty_program_id, opts)

Update a loyalty program

Updates an existing loyalty program by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoyaltyProgramsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loyalty_program_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  loyalty_program_update_dto: OpenapiClient::LoyaltyProgramUpdateDto.new # LoyaltyProgramUpdateDto | 
}

begin
  # Update a loyalty program
  result = api_instance.update_loyalty_program_async(tenant_id, loyalty_program_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->update_loyalty_program_async: #{e}"
end
```

#### Using the update_loyalty_program_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_loyalty_program_async_with_http_info(tenant_id, loyalty_program_id, opts)

```ruby
begin
  # Update a loyalty program
  data, status_code, headers = api_instance.update_loyalty_program_async_with_http_info(tenant_id, loyalty_program_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoyaltyProgramsApi->update_loyalty_program_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loyalty_program_id** | **String** |  |  |
| **loyalty_program_update_dto** | [**LoyaltyProgramUpdateDto**](LoyaltyProgramUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

