# OpenapiClient::GigsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_gig_async**](GigsApi.md#create_gig_async) | **POST** /api/v2/HrmsService/Gigs | Create a gig |
| [**delete_gig_async**](GigsApi.md#delete_gig_async) | **DELETE** /api/v2/HrmsService/Gigs/{gigId} | Delete a gig |
| [**get_gig_by_id_async**](GigsApi.md#get_gig_by_id_async) | **GET** /api/v2/HrmsService/Gigs/{gigId} | Get gig by ID |
| [**get_gigs_async**](GigsApi.md#get_gigs_async) | **GET** /api/v2/HrmsService/Gigs | Get gigs |
| [**get_gigs_count_async**](GigsApi.md#get_gigs_count_async) | **GET** /api/v2/HrmsService/Gigs/Count | Count gigs |
| [**update_gig_async**](GigsApi.md#update_gig_async) | **PUT** /api/v2/HrmsService/Gigs/{gigId} | Update a gig |


## create_gig_async

> <EmptyEnvelope> create_gig_async(tenant_id, opts)

Create a gig

Creates a new gig for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  gig_create_dto: OpenapiClient::GigCreateDto.new # GigCreateDto | 
}

begin
  # Create a gig
  result = api_instance.create_gig_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->create_gig_async: #{e}"
end
```

#### Using the create_gig_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_gig_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a gig
  data, status_code, headers = api_instance.create_gig_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->create_gig_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **gig_create_dto** | [**GigCreateDto**](GigCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_gig_async

> <EmptyEnvelope> delete_gig_async(tenant_id, gig_id, opts)

Delete a gig

Deletes a gig for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
gig_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a gig
  result = api_instance.delete_gig_async(tenant_id, gig_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->delete_gig_async: #{e}"
end
```

#### Using the delete_gig_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_gig_async_with_http_info(tenant_id, gig_id, opts)

```ruby
begin
  # Delete a gig
  data, status_code, headers = api_instance.delete_gig_async_with_http_info(tenant_id, gig_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->delete_gig_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **gig_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_gig_by_id_async

> <GigDtoEnvelope> get_gig_by_id_async(tenant_id, gig_id, opts)

Get gig by ID

Retrieves a specific gig by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
gig_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get gig by ID
  result = api_instance.get_gig_by_id_async(tenant_id, gig_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->get_gig_by_id_async: #{e}"
end
```

#### Using the get_gig_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GigDtoEnvelope>, Integer, Hash)> get_gig_by_id_async_with_http_info(tenant_id, gig_id, opts)

```ruby
begin
  # Get gig by ID
  data, status_code, headers = api_instance.get_gig_by_id_async_with_http_info(tenant_id, gig_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GigDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->get_gig_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **gig_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**GigDtoEnvelope**](GigDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_gigs_async

> <GigDtoListEnvelope> get_gigs_async(tenant_id, opts)

Get gigs

Retrieves gigs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get gigs
  result = api_instance.get_gigs_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->get_gigs_async: #{e}"
end
```

#### Using the get_gigs_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GigDtoListEnvelope>, Integer, Hash)> get_gigs_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get gigs
  data, status_code, headers = api_instance.get_gigs_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GigDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->get_gigs_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**GigDtoListEnvelope**](GigDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_gigs_count_async

> <Int32Envelope> get_gigs_count_async(tenant_id, opts)

Count gigs

Counts gigs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count gigs
  result = api_instance.get_gigs_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->get_gigs_count_async: #{e}"
end
```

#### Using the get_gigs_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_gigs_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count gigs
  data, status_code, headers = api_instance.get_gigs_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->get_gigs_count_async_with_http_info: #{e}"
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


## update_gig_async

> <EmptyEnvelope> update_gig_async(tenant_id, gig_id, opts)

Update a gig

Updates an existing gig for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::GigsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
gig_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  gig_update_dto: OpenapiClient::GigUpdateDto.new # GigUpdateDto | 
}

begin
  # Update a gig
  result = api_instance.update_gig_async(tenant_id, gig_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->update_gig_async: #{e}"
end
```

#### Using the update_gig_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_gig_async_with_http_info(tenant_id, gig_id, opts)

```ruby
begin
  # Update a gig
  data, status_code, headers = api_instance.update_gig_async_with_http_info(tenant_id, gig_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling GigsApi->update_gig_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **gig_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **gig_update_dto** | [**GigUpdateDto**](GigUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

