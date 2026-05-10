# OpenapiClient::FiscalResponsibilitiesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_fiscal_responsibility**](FiscalResponsibilitiesApi.md#create_fiscal_responsibility) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilities | Create a fiscal responsibility |
| [**delete_fiscal_responsibility**](FiscalResponsibilitiesApi.md#delete_fiscal_responsibility) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilities/{fiscalResponsibilityId} | Delete a fiscal responsibility |
| [**get_fiscal_responsibilities**](FiscalResponsibilitiesApi.md#get_fiscal_responsibilities) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/FiscalResponsibilities | Get fiscal responsibilities for an authority |
| [**get_fiscal_responsibilities_count**](FiscalResponsibilitiesApi.md#get_fiscal_responsibilities_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/Count | Get fiscal responsibilities count |
| [**get_fiscal_responsibility**](FiscalResponsibilitiesApi.md#get_fiscal_responsibility) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/{fiscalResponsibilityId} | Get fiscal responsibility by ID |
| [**update_fiscal_responsibility**](FiscalResponsibilitiesApi.md#update_fiscal_responsibility) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilities/{fiscalResponsibilityId} | Update a fiscal responsibility |


## create_fiscal_responsibility

> <EmptyEnvelope> create_fiscal_responsibility(tenant_id, opts)

Create a fiscal responsibility

Creates a new fiscal responsibility for a fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilitiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_responsibility_create_dto: OpenapiClient::FiscalResponsibilityCreateDto.new # FiscalResponsibilityCreateDto | 
}

begin
  # Create a fiscal responsibility
  result = api_instance.create_fiscal_responsibility(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->create_fiscal_responsibility: #{e}"
end
```

#### Using the create_fiscal_responsibility_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_fiscal_responsibility_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a fiscal responsibility
  data, status_code, headers = api_instance.create_fiscal_responsibility_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->create_fiscal_responsibility_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_responsibility_create_dto** | [**FiscalResponsibilityCreateDto**](FiscalResponsibilityCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_fiscal_responsibility

> <EmptyEnvelope> delete_fiscal_responsibility(tenant_id, fiscal_responsibility_id, opts)

Delete a fiscal responsibility

Deletes a fiscal responsibility identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilitiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a fiscal responsibility
  result = api_instance.delete_fiscal_responsibility(tenant_id, fiscal_responsibility_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->delete_fiscal_responsibility: #{e}"
end
```

#### Using the delete_fiscal_responsibility_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_fiscal_responsibility_with_http_info(tenant_id, fiscal_responsibility_id, opts)

```ruby
begin
  # Delete a fiscal responsibility
  data, status_code, headers = api_instance.delete_fiscal_responsibility_with_http_info(tenant_id, fiscal_responsibility_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->delete_fiscal_responsibility_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_responsibility_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_responsibilities

> <FiscalResponsibilityDtoListEnvelope> get_fiscal_responsibilities(fiscal_authority_id, authority_id, opts)

Get fiscal responsibilities for an authority

Retrieves all fiscal responsibilities for the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilitiesApi.new
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = 'authority_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal responsibilities for an authority
  result = api_instance.get_fiscal_responsibilities(fiscal_authority_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->get_fiscal_responsibilities: #{e}"
end
```

#### Using the get_fiscal_responsibilities_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalResponsibilityDtoListEnvelope>, Integer, Hash)> get_fiscal_responsibilities_with_http_info(fiscal_authority_id, authority_id, opts)

```ruby
begin
  # Get fiscal responsibilities for an authority
  data, status_code, headers = api_instance.get_fiscal_responsibilities_with_http_info(fiscal_authority_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalResponsibilityDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->get_fiscal_responsibilities_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **fiscal_authority_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalResponsibilityDtoListEnvelope**](FiscalResponsibilityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_responsibilities_count

> <Int32Envelope> get_fiscal_responsibilities_count(fiscal_authority_id, opts)

Get fiscal responsibilities count

Returns the total count of fiscal responsibilities for the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilitiesApi.new
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal responsibilities count
  result = api_instance.get_fiscal_responsibilities_count(fiscal_authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->get_fiscal_responsibilities_count: #{e}"
end
```

#### Using the get_fiscal_responsibilities_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_fiscal_responsibilities_count_with_http_info(fiscal_authority_id, opts)

```ruby
begin
  # Get fiscal responsibilities count
  data, status_code, headers = api_instance.get_fiscal_responsibilities_count_with_http_info(fiscal_authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->get_fiscal_responsibilities_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **fiscal_authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_responsibility

> <FiscalResponsibilityDtoEnvelope> get_fiscal_responsibility(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)

Get fiscal responsibility by ID

Retrieves a specific fiscal responsibility by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilitiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal responsibility by ID
  result = api_instance.get_fiscal_responsibility(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->get_fiscal_responsibility: #{e}"
end
```

#### Using the get_fiscal_responsibility_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalResponsibilityDtoEnvelope>, Integer, Hash)> get_fiscal_responsibility_with_http_info(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)

```ruby
begin
  # Get fiscal responsibility by ID
  data, status_code, headers = api_instance.get_fiscal_responsibility_with_http_info(tenant_id, fiscal_authority_id, fiscal_responsibility_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalResponsibilityDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->get_fiscal_responsibility_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **fiscal_responsibility_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalResponsibilityDtoEnvelope**](FiscalResponsibilityDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_fiscal_responsibility

> <EmptyEnvelope> update_fiscal_responsibility(tenant_id, fiscal_responsibility_id, opts)

Update a fiscal responsibility

Updates an existing fiscal responsibility identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalResponsibilitiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_responsibility_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_responsibility_update_dto: OpenapiClient::FiscalResponsibilityUpdateDto.new # FiscalResponsibilityUpdateDto | 
}

begin
  # Update a fiscal responsibility
  result = api_instance.update_fiscal_responsibility(tenant_id, fiscal_responsibility_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->update_fiscal_responsibility: #{e}"
end
```

#### Using the update_fiscal_responsibility_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_fiscal_responsibility_with_http_info(tenant_id, fiscal_responsibility_id, opts)

```ruby
begin
  # Update a fiscal responsibility
  data, status_code, headers = api_instance.update_fiscal_responsibility_with_http_info(tenant_id, fiscal_responsibility_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalResponsibilitiesApi->update_fiscal_responsibility_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_responsibility_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_responsibility_update_dto** | [**FiscalResponsibilityUpdateDto**](FiscalResponsibilityUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

