# OpenapiClient::SegmentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_segment**](SegmentsApi.md#create_tenant_segment) | **POST** /api/v2/TenantsService/Segments | Create a new tenant segment |
| [**delete_tenant_segment**](SegmentsApi.md#delete_tenant_segment) | **DELETE** /api/v2/TenantsService/Segments/{tenantSegmentId} | Delete a tenant segment |
| [**get_tenant_segment_by_id**](SegmentsApi.md#get_tenant_segment_by_id) | **GET** /api/v2/TenantsService/Segments/{tenantSegmentId} | Retrieve a single tenant segment by its ID |
| [**get_tenant_segments**](SegmentsApi.md#get_tenant_segments) | **GET** /api/v2/TenantsService/Segments | Retrieve a list of tenant segments |
| [**get_tenant_segments_count**](SegmentsApi.md#get_tenant_segments_count) | **GET** /api/v2/TenantsService/Segments/Count | Get the count of tenant segments |
| [**update_tenant_segment**](SegmentsApi.md#update_tenant_segment) | **PUT** /api/v2/TenantsService/Segments/{tenantSegmentId} | Update a tenant segment |


## create_tenant_segment

> <EmptyEnvelope> create_tenant_segment(tenant_id, opts)

Create a new tenant segment

Create a new tenant segment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SegmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_segment_create_dto: OpenapiClient::TenantSegmentCreateDto.new # TenantSegmentCreateDto | 
}

begin
  # Create a new tenant segment
  result = api_instance.create_tenant_segment(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->create_tenant_segment: #{e}"
end
```

#### Using the create_tenant_segment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_segment_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant segment
  data, status_code, headers = api_instance.create_tenant_segment_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->create_tenant_segment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_segment_create_dto** | [**TenantSegmentCreateDto**](TenantSegmentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_segment

> <EmptyEnvelope> delete_tenant_segment(tenant_id, tenant_segment_id, opts)

Delete a tenant segment

Delete a tenant segment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SegmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_segment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant segment
  result = api_instance.delete_tenant_segment(tenant_id, tenant_segment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->delete_tenant_segment: #{e}"
end
```

#### Using the delete_tenant_segment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_segment_with_http_info(tenant_id, tenant_segment_id, opts)

```ruby
begin
  # Delete a tenant segment
  data, status_code, headers = api_instance.delete_tenant_segment_with_http_info(tenant_id, tenant_segment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->delete_tenant_segment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_segment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_segment_by_id

> <TenantSegmentDtoEnvelope> get_tenant_segment_by_id(tenant_id, tenant_segment_id, opts)

Retrieve a single tenant segment by its ID

Retrieve a single tenant segment by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SegmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_segment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant segment by its ID
  result = api_instance.get_tenant_segment_by_id(tenant_id, tenant_segment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->get_tenant_segment_by_id: #{e}"
end
```

#### Using the get_tenant_segment_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantSegmentDtoEnvelope>, Integer, Hash)> get_tenant_segment_by_id_with_http_info(tenant_id, tenant_segment_id, opts)

```ruby
begin
  # Retrieve a single tenant segment by its ID
  data, status_code, headers = api_instance.get_tenant_segment_by_id_with_http_info(tenant_id, tenant_segment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantSegmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->get_tenant_segment_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_segment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantSegmentDtoEnvelope**](TenantSegmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_segments

> <TenantSegmentDtoListEnvelope> get_tenant_segments(tenant_id, opts)

Retrieve a list of tenant segments

Retrieve a list of tenant segments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SegmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant segments
  result = api_instance.get_tenant_segments(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->get_tenant_segments: #{e}"
end
```

#### Using the get_tenant_segments_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantSegmentDtoListEnvelope>, Integer, Hash)> get_tenant_segments_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant segments
  data, status_code, headers = api_instance.get_tenant_segments_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantSegmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->get_tenant_segments_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantSegmentDtoListEnvelope**](TenantSegmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_segments_count

> <Int32Envelope> get_tenant_segments_count(tenant_id, opts)

Get the count of tenant segments

Get the count of tenant segments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SegmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant segments
  result = api_instance.get_tenant_segments_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->get_tenant_segments_count: #{e}"
end
```

#### Using the get_tenant_segments_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_segments_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant segments
  data, status_code, headers = api_instance.get_tenant_segments_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->get_tenant_segments_count_with_http_info: #{e}"
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


## update_tenant_segment

> <EmptyEnvelope> update_tenant_segment(tenant_id, tenant_segment_id, opts)

Update a tenant segment

Update a tenant segment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SegmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_segment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_segment_update_dto: OpenapiClient::TenantSegmentUpdateDto.new # TenantSegmentUpdateDto | 
}

begin
  # Update a tenant segment
  result = api_instance.update_tenant_segment(tenant_id, tenant_segment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->update_tenant_segment: #{e}"
end
```

#### Using the update_tenant_segment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_segment_with_http_info(tenant_id, tenant_segment_id, opts)

```ruby
begin
  # Update a tenant segment
  data, status_code, headers = api_instance.update_tenant_segment_with_http_info(tenant_id, tenant_segment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SegmentsApi->update_tenant_segment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_segment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_segment_update_dto** | [**TenantSegmentUpdateDto**](TenantSegmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

