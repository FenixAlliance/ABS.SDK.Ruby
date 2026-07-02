# OpenapiClient::GigApplicationsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**accept_gig_application_async**](GigApplicationsApi.md#accept_gig_application_async) | **POST** /api/v2/HrmsService/GigApplications/{gigApplicationId}/Accept | Accept a gig application |
| [**create_gig_application_async**](GigApplicationsApi.md#create_gig_application_async) | **POST** /api/v2/HrmsService/GigApplications | Create a gig application |
| [**delete_gig_application_async**](GigApplicationsApi.md#delete_gig_application_async) | **DELETE** /api/v2/HrmsService/GigApplications/{gigApplicationId} | Delete a gig application |
| [**get_gig_application_by_id_async**](GigApplicationsApi.md#get_gig_application_by_id_async) | **GET** /api/v2/HrmsService/GigApplications/{gigApplicationId} | Get gig application by ID |
| [**get_gig_applications_async**](GigApplicationsApi.md#get_gig_applications_async) | **GET** /api/v2/HrmsService/GigApplications | Get gig applications |
| [**get_gig_applications_count_async**](GigApplicationsApi.md#get_gig_applications_count_async) | **GET** /api/v2/HrmsService/GigApplications/Count | Count gig applications |
| [**patch_gig_application_async**](GigApplicationsApi.md#patch_gig_application_async) | **PATCH** /api/v2/HrmsService/GigApplications/{gigApplicationId} | Patch a gig application |
| [**update_gig_application_async**](GigApplicationsApi.md#update_gig_application_async) | **PUT** /api/v2/HrmsService/GigApplications/{gigApplicationId} | Update a gig application |


## accept_gig_application_async

> <EmptyEnvelope> accept_gig_application_async(tenant_id, gig_application_id, opts)

Accept a gig application

Accepts the candidate's gig proposal, forming an engagement (raises GigApplicationAccepted). A proposal cannot be accepted twice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
gig_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Accept a gig application
  result = api_instance.accept_gig_application_async(tenant_id, gig_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->accept_gig_application_async: #{e}"
end
```

#### Using the accept_gig_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> accept_gig_application_async_with_http_info(tenant_id, gig_application_id, opts)

```ruby
begin
  # Accept a gig application
  data, status_code, headers = api_instance.accept_gig_application_async_with_http_info(tenant_id, gig_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->accept_gig_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **gig_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_gig_application_async

> <EmptyEnvelope> create_gig_application_async(tenant_id, opts)

Create a gig application

Records a candidate's proposal against one of the tenant's gigs. The targeted gig must belong to the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  gig_application_create_dto: OpenapiClient::GigApplicationCreateDto.new # GigApplicationCreateDto | 
}

begin
  # Create a gig application
  result = api_instance.create_gig_application_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->create_gig_application_async: #{e}"
end
```

#### Using the create_gig_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_gig_application_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a gig application
  data, status_code, headers = api_instance.create_gig_application_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->create_gig_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **gig_application_create_dto** | [**GigApplicationCreateDto**](GigApplicationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_gig_application_async

> <EmptyEnvelope> delete_gig_application_async(tenant_id, gig_application_id, opts)

Delete a gig application

Removes a proposal submitted against one of the tenant's gigs.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
gig_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a gig application
  result = api_instance.delete_gig_application_async(tenant_id, gig_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->delete_gig_application_async: #{e}"
end
```

#### Using the delete_gig_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_gig_application_async_with_http_info(tenant_id, gig_application_id, opts)

```ruby
begin
  # Delete a gig application
  data, status_code, headers = api_instance.delete_gig_application_async_with_http_info(tenant_id, gig_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->delete_gig_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **gig_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_gig_application_by_id_async

> <GigApplicationDtoEnvelope> get_gig_application_by_id_async(tenant_id, gig_application_id, opts)

Get gig application by ID

Retrieves a specific proposal submitted against one of the tenant's gigs.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
gig_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get gig application by ID
  result = api_instance.get_gig_application_by_id_async(tenant_id, gig_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->get_gig_application_by_id_async: #{e}"
end
```

#### Using the get_gig_application_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GigApplicationDtoEnvelope>, Integer, Hash)> get_gig_application_by_id_async_with_http_info(tenant_id, gig_application_id, opts)

```ruby
begin
  # Get gig application by ID
  data, status_code, headers = api_instance.get_gig_application_by_id_async_with_http_info(tenant_id, gig_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GigApplicationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->get_gig_application_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **gig_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**GigApplicationDtoEnvelope**](GigApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_gig_applications_async

> <GigApplicationDtoListEnvelope> get_gig_applications_async(tenant_id, opts)

Get gig applications

Retrieves proposals submitted against the tenant's gigs. Filter with `$filter=GigId eq '...'` or `JobApplicantProfileId eq '...'`.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get gig applications
  result = api_instance.get_gig_applications_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->get_gig_applications_async: #{e}"
end
```

#### Using the get_gig_applications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GigApplicationDtoListEnvelope>, Integer, Hash)> get_gig_applications_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get gig applications
  data, status_code, headers = api_instance.get_gig_applications_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GigApplicationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->get_gig_applications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**GigApplicationDtoListEnvelope**](GigApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_gig_applications_count_async

> <Int32Envelope> get_gig_applications_count_async(tenant_id, opts)

Count gig applications

Counts proposals submitted against the tenant's gigs.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count gig applications
  result = api_instance.get_gig_applications_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->get_gig_applications_count_async: #{e}"
end
```

#### Using the get_gig_applications_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_gig_applications_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count gig applications
  data, status_code, headers = api_instance.get_gig_applications_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->get_gig_applications_count_async_with_http_info: #{e}"
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


## patch_gig_application_async

> <EmptyEnvelope> patch_gig_application_async(tenant_id, gig_application_id, opts)

Patch a gig application

Partially updates an existing proposal submitted against one of the tenant's gigs.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
gig_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a gig application
  result = api_instance.patch_gig_application_async(tenant_id, gig_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->patch_gig_application_async: #{e}"
end
```

#### Using the patch_gig_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_gig_application_async_with_http_info(tenant_id, gig_application_id, opts)

```ruby
begin
  # Patch a gig application
  data, status_code, headers = api_instance.patch_gig_application_async_with_http_info(tenant_id, gig_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->patch_gig_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **gig_application_id** | **String** |  |  |
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


## update_gig_application_async

> <EmptyEnvelope> update_gig_application_async(tenant_id, gig_application_id, opts)

Update a gig application

Updates an existing proposal submitted against one of the tenant's gigs (e.g. accept it).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigApplicationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
gig_application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  gig_application_update_dto: OpenapiClient::GigApplicationUpdateDto.new # GigApplicationUpdateDto | 
}

begin
  # Update a gig application
  result = api_instance.update_gig_application_async(tenant_id, gig_application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->update_gig_application_async: #{e}"
end
```

#### Using the update_gig_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_gig_application_async_with_http_info(tenant_id, gig_application_id, opts)

```ruby
begin
  # Update a gig application
  data, status_code, headers = api_instance.update_gig_application_async_with_http_info(tenant_id, gig_application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigApplicationsApi->update_gig_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **gig_application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **gig_application_update_dto** | [**GigApplicationUpdateDto**](GigApplicationUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

