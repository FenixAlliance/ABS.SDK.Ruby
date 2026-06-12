# OpenapiClient::ApplicationsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_business_application_async**](ApplicationsApi.md#create_business_application_async) | **POST** /api/v2/SecurityService/Applications | Create a new business application |
| [**delete_business_application_async**](ApplicationsApi.md#delete_business_application_async) | **DELETE** /api/v2/SecurityService/Applications/{applicationId} | Delete a business application |
| [**get_business_application_by_id_async**](ApplicationsApi.md#get_business_application_by_id_async) | **GET** /api/v2/SecurityService/Applications/{applicationId} | Get business application by ID |
| [**get_business_applications_async**](ApplicationsApi.md#get_business_applications_async) | **GET** /api/v2/SecurityService/Applications | Get all business applications |
| [**get_business_applications_count_async**](ApplicationsApi.md#get_business_applications_count_async) | **GET** /api/v2/SecurityService/Applications/Count | Get business applications count |
| [**get_permissions_by_application_async**](ApplicationsApi.md#get_permissions_by_application_async) | **GET** /api/v2/SecurityService/Applications/{applicationId}/Permissions | Get permissions by application |
| [**get_roles_by_application_async**](ApplicationsApi.md#get_roles_by_application_async) | **GET** /api/v2/SecurityService/Applications/{applicationId}/Roles | Get roles by application |
| [**patch_business_application_async**](ApplicationsApi.md#patch_business_application_async) | **PATCH** /api/v2/SecurityService/Applications/{applicationId} | Patch an existing business application |
| [**update_business_application_async**](ApplicationsApi.md#update_business_application_async) | **PUT** /api/v2/SecurityService/Applications/{applicationId} | Update an existing business application |


## create_business_application_async

> <EmptyEnvelope> create_business_application_async(tenant_id, business_application_create_dto, opts)

Create a new business application

Creates a new business application for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_application_create_dto = OpenapiClient::BusinessApplicationCreateDto.new({name: 'name_example'}) # BusinessApplicationCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a new business application
  result = api_instance.create_business_application_async(tenant_id, business_application_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->create_business_application_async: #{e}"
end
```

#### Using the create_business_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_business_application_async_with_http_info(tenant_id, business_application_create_dto, opts)

```ruby
begin
  # Create a new business application
  data, status_code, headers = api_instance.create_business_application_async_with_http_info(tenant_id, business_application_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->create_business_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_application_create_dto** | [**BusinessApplicationCreateDto**](BusinessApplicationCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_business_application_async

> <EmptyEnvelope> delete_business_application_async(tenant_id, application_id, opts)

Delete a business application

Deletes an existing business application for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a business application
  result = api_instance.delete_business_application_async(tenant_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->delete_business_application_async: #{e}"
end
```

#### Using the delete_business_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_business_application_async_with_http_info(tenant_id, application_id, opts)

```ruby
begin
  # Delete a business application
  data, status_code, headers = api_instance.delete_business_application_async_with_http_info(tenant_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->delete_business_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_application_by_id_async

> <BusinessApplicationDtoEnvelope> get_business_application_by_id_async(tenant_id, application_id, opts)

Get business application by ID

Retrieves a specific business application by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get business application by ID
  result = api_instance.get_business_application_by_id_async(tenant_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_business_application_by_id_async: #{e}"
end
```

#### Using the get_business_application_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessApplicationDtoEnvelope>, Integer, Hash)> get_business_application_by_id_async_with_http_info(tenant_id, application_id, opts)

```ruby
begin
  # Get business application by ID
  data, status_code, headers = api_instance.get_business_application_by_id_async_with_http_info(tenant_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessApplicationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_business_application_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BusinessApplicationDtoEnvelope**](BusinessApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_applications_async

> <BusinessApplicationDtoListEnvelope> get_business_applications_async(tenant_id, opts)

Get all business applications

Retrieves all business applications for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all business applications
  result = api_instance.get_business_applications_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_business_applications_async: #{e}"
end
```

#### Using the get_business_applications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessApplicationDtoListEnvelope>, Integer, Hash)> get_business_applications_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all business applications
  data, status_code, headers = api_instance.get_business_applications_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessApplicationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_business_applications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BusinessApplicationDtoListEnvelope**](BusinessApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_applications_count_async

> <Int32Envelope> get_business_applications_count_async(tenant_id, opts)

Get business applications count

Retrieves the count of business applications for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get business applications count
  result = api_instance.get_business_applications_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_business_applications_count_async: #{e}"
end
```

#### Using the get_business_applications_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_business_applications_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get business applications count
  data, status_code, headers = api_instance.get_business_applications_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_business_applications_count_async_with_http_info: #{e}"
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


## get_permissions_by_application_async

> <SecurityPermissionDtoListEnvelope> get_permissions_by_application_async(tenant_id, application_id, opts)

Get permissions by application

Retrieves all security permissions granted to a specific business application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get permissions by application
  result = api_instance.get_permissions_by_application_async(tenant_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_permissions_by_application_async: #{e}"
end
```

#### Using the get_permissions_by_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityPermissionDtoListEnvelope>, Integer, Hash)> get_permissions_by_application_async_with_http_info(tenant_id, application_id, opts)

```ruby
begin
  # Get permissions by application
  data, status_code, headers = api_instance.get_permissions_by_application_async_with_http_info(tenant_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityPermissionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_permissions_by_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SecurityPermissionDtoListEnvelope**](SecurityPermissionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_roles_by_application_async

> <SecurityRoleDtoListEnvelope> get_roles_by_application_async(tenant_id, application_id, opts)

Get roles by application

Retrieves all security roles granted to a specific business application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get roles by application
  result = api_instance.get_roles_by_application_async(tenant_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_roles_by_application_async: #{e}"
end
```

#### Using the get_roles_by_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityRoleDtoListEnvelope>, Integer, Hash)> get_roles_by_application_async_with_http_info(tenant_id, application_id, opts)

```ruby
begin
  # Get roles by application
  data, status_code, headers = api_instance.get_roles_by_application_async_with_http_info(tenant_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityRoleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_roles_by_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SecurityRoleDtoListEnvelope**](SecurityRoleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_business_application_async

> <EmptyEnvelope> patch_business_application_async(tenant_id, application_id, operation, opts)

Patch an existing business application

Partially updates an existing business application using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
operation = [OpenapiClient::Operation.new] # Array<Operation> | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Patch an existing business application
  result = api_instance.patch_business_application_async(tenant_id, application_id, operation, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->patch_business_application_async: #{e}"
end
```

#### Using the patch_business_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_business_application_async_with_http_info(tenant_id, application_id, operation, opts)

```ruby
begin
  # Patch an existing business application
  data, status_code, headers = api_instance.patch_business_application_async_with_http_info(tenant_id, application_id, operation, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->patch_business_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_business_application_async

> <EmptyEnvelope> update_business_application_async(tenant_id, application_id, business_application_update_dto, opts)

Update an existing business application

Updates an existing business application for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
business_application_update_dto = OpenapiClient::BusinessApplicationUpdateDto.new # BusinessApplicationUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update an existing business application
  result = api_instance.update_business_application_async(tenant_id, application_id, business_application_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->update_business_application_async: #{e}"
end
```

#### Using the update_business_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_business_application_async_with_http_info(tenant_id, application_id, business_application_update_dto, opts)

```ruby
begin
  # Update an existing business application
  data, status_code, headers = api_instance.update_business_application_async_with_http_info(tenant_id, application_id, business_application_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->update_business_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **business_application_update_dto** | [**BusinessApplicationUpdateDto**](BusinessApplicationUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

