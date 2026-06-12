# OpenapiClient::OAuthApplicationsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_o_auth_application_async**](OAuthApplicationsApi.md#create_o_auth_application_async) | **POST** /api/v2/SecurityService/OAuthApplications | Create a new OAuth application |
| [**delete_o_auth_application_async**](OAuthApplicationsApi.md#delete_o_auth_application_async) | **DELETE** /api/v2/SecurityService/OAuthApplications/{applicationId} | Delete an OAuth application |
| [**get_o_auth_application_by_id_async**](OAuthApplicationsApi.md#get_o_auth_application_by_id_async) | **GET** /api/v2/SecurityService/OAuthApplications/{applicationId} | Get OAuth application by ID |
| [**get_o_auth_applications_async**](OAuthApplicationsApi.md#get_o_auth_applications_async) | **GET** /api/v2/SecurityService/OAuthApplications | Get all OAuth applications |
| [**get_o_auth_applications_count_async**](OAuthApplicationsApi.md#get_o_auth_applications_count_async) | **GET** /api/v2/SecurityService/OAuthApplications/Count | Get OAuth applications count |
| [**get_o_auth_authorization_by_id_async**](OAuthApplicationsApi.md#get_o_auth_authorization_by_id_async) | **GET** /api/v2/SecurityService/OAuthApplications/Authorizations/{authorizationId} | Get OAuth authorization by ID |
| [**get_o_auth_authorizations_async**](OAuthApplicationsApi.md#get_o_auth_authorizations_async) | **GET** /api/v2/SecurityService/OAuthApplications/Authorizations | Get all OAuth authorizations |
| [**get_o_auth_authorizations_count_async**](OAuthApplicationsApi.md#get_o_auth_authorizations_count_async) | **GET** /api/v2/SecurityService/OAuthApplications/Authorizations/Count | Get OAuth authorizations count |
| [**patch_o_auth_application_async**](OAuthApplicationsApi.md#patch_o_auth_application_async) | **PATCH** /api/v2/SecurityService/OAuthApplications/{applicationId} | Patch an existing OAuth application |
| [**update_o_auth_application_async**](OAuthApplicationsApi.md#update_o_auth_application_async) | **PUT** /api/v2/SecurityService/OAuthApplications/{applicationId} | Update an existing OAuth application |


## create_o_auth_application_async

> <EmptyEnvelope> create_o_auth_application_async(tenant_id, o_auth_application_create_dto, opts)

Create a new OAuth application

Creates a new OAuth application for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
o_auth_application_create_dto = OpenapiClient::OAuthApplicationCreateDto.new({display_name: 'display_name_example'}) # OAuthApplicationCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a new OAuth application
  result = api_instance.create_o_auth_application_async(tenant_id, o_auth_application_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->create_o_auth_application_async: #{e}"
end
```

#### Using the create_o_auth_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_o_auth_application_async_with_http_info(tenant_id, o_auth_application_create_dto, opts)

```ruby
begin
  # Create a new OAuth application
  data, status_code, headers = api_instance.create_o_auth_application_async_with_http_info(tenant_id, o_auth_application_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->create_o_auth_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **o_auth_application_create_dto** | [**OAuthApplicationCreateDto**](OAuthApplicationCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_o_auth_application_async

> <EmptyEnvelope> delete_o_auth_application_async(tenant_id, application_id, opts)

Delete an OAuth application

Deletes an existing OAuth application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an OAuth application
  result = api_instance.delete_o_auth_application_async(tenant_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->delete_o_auth_application_async: #{e}"
end
```

#### Using the delete_o_auth_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_o_auth_application_async_with_http_info(tenant_id, application_id, opts)

```ruby
begin
  # Delete an OAuth application
  data, status_code, headers = api_instance.delete_o_auth_application_async_with_http_info(tenant_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->delete_o_auth_application_async_with_http_info: #{e}"
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


## get_o_auth_application_by_id_async

> <OAuthApplicationDtoEnvelope> get_o_auth_application_by_id_async(tenant_id, application_id, opts)

Get OAuth application by ID

Retrieves a specific OAuth application by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get OAuth application by ID
  result = api_instance.get_o_auth_application_by_id_async(tenant_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_application_by_id_async: #{e}"
end
```

#### Using the get_o_auth_application_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OAuthApplicationDtoEnvelope>, Integer, Hash)> get_o_auth_application_by_id_async_with_http_info(tenant_id, application_id, opts)

```ruby
begin
  # Get OAuth application by ID
  data, status_code, headers = api_instance.get_o_auth_application_by_id_async_with_http_info(tenant_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OAuthApplicationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_application_by_id_async_with_http_info: #{e}"
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

[**OAuthApplicationDtoEnvelope**](OAuthApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_o_auth_applications_async

> <OAuthApplicationDtoListEnvelope> get_o_auth_applications_async(tenant_id, opts)

Get all OAuth applications

Retrieves all OAuth applications for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all OAuth applications
  result = api_instance.get_o_auth_applications_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_applications_async: #{e}"
end
```

#### Using the get_o_auth_applications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OAuthApplicationDtoListEnvelope>, Integer, Hash)> get_o_auth_applications_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all OAuth applications
  data, status_code, headers = api_instance.get_o_auth_applications_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OAuthApplicationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_applications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OAuthApplicationDtoListEnvelope**](OAuthApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_o_auth_applications_count_async

> <Int32Envelope> get_o_auth_applications_count_async(tenant_id, opts)

Get OAuth applications count

Retrieves the count of OAuth applications for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get OAuth applications count
  result = api_instance.get_o_auth_applications_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_applications_count_async: #{e}"
end
```

#### Using the get_o_auth_applications_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_o_auth_applications_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get OAuth applications count
  data, status_code, headers = api_instance.get_o_auth_applications_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_applications_count_async_with_http_info: #{e}"
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


## get_o_auth_authorization_by_id_async

> <OAuthAuthorizationDtoEnvelope> get_o_auth_authorization_by_id_async(tenant_id, authorization_id, opts)

Get OAuth authorization by ID

Retrieves a specific OAuth authorization by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authorization_id = 'authorization_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get OAuth authorization by ID
  result = api_instance.get_o_auth_authorization_by_id_async(tenant_id, authorization_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_authorization_by_id_async: #{e}"
end
```

#### Using the get_o_auth_authorization_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OAuthAuthorizationDtoEnvelope>, Integer, Hash)> get_o_auth_authorization_by_id_async_with_http_info(tenant_id, authorization_id, opts)

```ruby
begin
  # Get OAuth authorization by ID
  data, status_code, headers = api_instance.get_o_auth_authorization_by_id_async_with_http_info(tenant_id, authorization_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OAuthAuthorizationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_authorization_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **authorization_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OAuthAuthorizationDtoEnvelope**](OAuthAuthorizationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_o_auth_authorizations_async

> <OAuthAuthorizationDtoListEnvelope> get_o_auth_authorizations_async(tenant_id, opts)

Get all OAuth authorizations

Retrieves all OAuth authorizations for the specified user.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  user_id: 'user_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all OAuth authorizations
  result = api_instance.get_o_auth_authorizations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_authorizations_async: #{e}"
end
```

#### Using the get_o_auth_authorizations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OAuthAuthorizationDtoListEnvelope>, Integer, Hash)> get_o_auth_authorizations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all OAuth authorizations
  data, status_code, headers = api_instance.get_o_auth_authorizations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OAuthAuthorizationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_authorizations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **user_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OAuthAuthorizationDtoListEnvelope**](OAuthAuthorizationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_o_auth_authorizations_count_async

> <Int32Envelope> get_o_auth_authorizations_count_async(tenant_id, opts)

Get OAuth authorizations count

Retrieves the count of OAuth authorizations for the specified user.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  user_id: 'user_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get OAuth authorizations count
  result = api_instance.get_o_auth_authorizations_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_authorizations_count_async: #{e}"
end
```

#### Using the get_o_auth_authorizations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_o_auth_authorizations_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get OAuth authorizations count
  data, status_code, headers = api_instance.get_o_auth_authorizations_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->get_o_auth_authorizations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **user_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_o_auth_application_async

> <EmptyEnvelope> patch_o_auth_application_async(tenant_id, application_id, operation, opts)

Patch an existing OAuth application

Partially updates an existing OAuth application using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
operation = [OpenapiClient::Operation.new] # Array<Operation> | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Patch an existing OAuth application
  result = api_instance.patch_o_auth_application_async(tenant_id, application_id, operation, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->patch_o_auth_application_async: #{e}"
end
```

#### Using the patch_o_auth_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_o_auth_application_async_with_http_info(tenant_id, application_id, operation, opts)

```ruby
begin
  # Patch an existing OAuth application
  data, status_code, headers = api_instance.patch_o_auth_application_async_with_http_info(tenant_id, application_id, operation, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->patch_o_auth_application_async_with_http_info: #{e}"
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


## update_o_auth_application_async

> <EmptyEnvelope> update_o_auth_application_async(tenant_id, application_id, o_auth_application_update_dto, opts)

Update an existing OAuth application

Updates an existing OAuth application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
o_auth_application_update_dto = OpenapiClient::OAuthApplicationUpdateDto.new # OAuthApplicationUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update an existing OAuth application
  result = api_instance.update_o_auth_application_async(tenant_id, application_id, o_auth_application_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->update_o_auth_application_async: #{e}"
end
```

#### Using the update_o_auth_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_o_auth_application_async_with_http_info(tenant_id, application_id, o_auth_application_update_dto, opts)

```ruby
begin
  # Update an existing OAuth application
  data, status_code, headers = api_instance.update_o_auth_application_async_with_http_info(tenant_id, application_id, o_auth_application_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApplicationsApi->update_o_auth_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **o_auth_application_update_dto** | [**OAuthApplicationUpdateDto**](OAuthApplicationUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

