# OpenapiClient::FiscalAuthoritiesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_fiscal_authority**](FiscalAuthoritiesApi.md#create_fiscal_authority) | **POST** /api/v2/AccountingService/Fiscals/Authorities | Create a fiscal authority |
| [**delete_fiscal_authority**](FiscalAuthoritiesApi.md#delete_fiscal_authority) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/{authorityId} | Delete a fiscal authority |
| [**get_fiscal_authorities**](FiscalAuthoritiesApi.md#get_fiscal_authorities) | **GET** /api/v2/AccountingService/Fiscals/Authorities | Get fiscal authorities |
| [**get_fiscal_authorities_count**](FiscalAuthoritiesApi.md#get_fiscal_authorities_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/Count | Get fiscal authorities count |
| [**get_fiscal_authority**](FiscalAuthoritiesApi.md#get_fiscal_authority) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId} | Get fiscal authority by ID |
| [**update_fiscal_authority**](FiscalAuthoritiesApi.md#update_fiscal_authority) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/{authorityId} | Update a fiscal authority |


## create_fiscal_authority

> <EmptyEnvelope> create_fiscal_authority(tenant_id, opts)

Create a fiscal authority

Creates a new fiscal authority for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthoritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_authority_create_dto: OpenapiClient::FiscalAuthorityCreateDto.new # FiscalAuthorityCreateDto | 
}

begin
  # Create a fiscal authority
  result = api_instance.create_fiscal_authority(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->create_fiscal_authority: #{e}"
end
```

#### Using the create_fiscal_authority_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_fiscal_authority_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a fiscal authority
  data, status_code, headers = api_instance.create_fiscal_authority_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->create_fiscal_authority_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_authority_create_dto** | [**FiscalAuthorityCreateDto**](FiscalAuthorityCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_fiscal_authority

> <EmptyEnvelope> delete_fiscal_authority(tenant_id, authority_id, opts)

Delete a fiscal authority

Deletes a fiscal authority identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthoritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a fiscal authority
  result = api_instance.delete_fiscal_authority(tenant_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->delete_fiscal_authority: #{e}"
end
```

#### Using the delete_fiscal_authority_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_fiscal_authority_with_http_info(tenant_id, authority_id, opts)

```ruby
begin
  # Delete a fiscal authority
  data, status_code, headers = api_instance.delete_fiscal_authority_with_http_info(tenant_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->delete_fiscal_authority_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_authorities

> <FiscalAuthorityDtoListEnvelope> get_fiscal_authorities(tenant_id, opts)

Get fiscal authorities

Retrieves all fiscal authorities for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthoritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal authorities
  result = api_instance.get_fiscal_authorities(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->get_fiscal_authorities: #{e}"
end
```

#### Using the get_fiscal_authorities_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalAuthorityDtoListEnvelope>, Integer, Hash)> get_fiscal_authorities_with_http_info(tenant_id, opts)

```ruby
begin
  # Get fiscal authorities
  data, status_code, headers = api_instance.get_fiscal_authorities_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalAuthorityDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->get_fiscal_authorities_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalAuthorityDtoListEnvelope**](FiscalAuthorityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_authorities_count

> <Int32Envelope> get_fiscal_authorities_count(tenant_id, opts)

Get fiscal authorities count

Returns the total count of fiscal authorities for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthoritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal authorities count
  result = api_instance.get_fiscal_authorities_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->get_fiscal_authorities_count: #{e}"
end
```

#### Using the get_fiscal_authorities_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_fiscal_authorities_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get fiscal authorities count
  data, status_code, headers = api_instance.get_fiscal_authorities_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->get_fiscal_authorities_count_with_http_info: #{e}"
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


## get_fiscal_authority

> <FiscalAuthorityDtoEnvelope> get_fiscal_authority(tenant_id, authority_id, opts)

Get fiscal authority by ID

Retrieves a specific fiscal authority by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthoritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal authority by ID
  result = api_instance.get_fiscal_authority(tenant_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->get_fiscal_authority: #{e}"
end
```

#### Using the get_fiscal_authority_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalAuthorityDtoEnvelope>, Integer, Hash)> get_fiscal_authority_with_http_info(tenant_id, authority_id, opts)

```ruby
begin
  # Get fiscal authority by ID
  data, status_code, headers = api_instance.get_fiscal_authority_with_http_info(tenant_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalAuthorityDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->get_fiscal_authority_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalAuthorityDtoEnvelope**](FiscalAuthorityDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_fiscal_authority

> <EmptyEnvelope> update_fiscal_authority(tenant_id, authority_id, opts)

Update a fiscal authority

Updates an existing fiscal authority identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthoritiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_authority_update_dto: OpenapiClient::FiscalAuthorityUpdateDto.new # FiscalAuthorityUpdateDto | 
}

begin
  # Update a fiscal authority
  result = api_instance.update_fiscal_authority(tenant_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->update_fiscal_authority: #{e}"
end
```

#### Using the update_fiscal_authority_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_fiscal_authority_with_http_info(tenant_id, authority_id, opts)

```ruby
begin
  # Update a fiscal authority
  data, status_code, headers = api_instance.update_fiscal_authority_with_http_info(tenant_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthoritiesApi->update_fiscal_authority_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_authority_update_dto** | [**FiscalAuthorityUpdateDto**](FiscalAuthorityUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

