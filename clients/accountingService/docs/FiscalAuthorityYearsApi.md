# OpenapiClient::FiscalAuthorityYearsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_fiscal_year**](FiscalAuthorityYearsApi.md#create_fiscal_year) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalYears | Create a fiscal year |
| [**delete_fiscal_year**](FiscalAuthorityYearsApi.md#delete_fiscal_year) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalYears/{fiscalYearId} | Delete a fiscal year |
| [**get_fiscal_year**](FiscalAuthorityYearsApi.md#get_fiscal_year) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalYears/{fiscalYearId} | Get fiscal year by ID for an authority |
| [**get_fiscal_years**](FiscalAuthorityYearsApi.md#get_fiscal_years) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/FiscalYears | Get fiscal years for an authority |
| [**get_fiscal_years_count**](FiscalAuthorityYearsApi.md#get_fiscal_years_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalYears/Count | Get fiscal years count for an authority |
| [**patch_fiscal_authority_year_async**](FiscalAuthorityYearsApi.md#patch_fiscal_authority_year_async) | **PATCH** /api/v2/AccountingService/Fiscals/Authorities/FiscalYears/{fiscalYearId} | Patch a fiscal authority year |
| [**update_fiscal_year**](FiscalAuthorityYearsApi.md#update_fiscal_year) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalYears/{fiscalYearId} | Update a fiscal year |


## create_fiscal_year

> <EmptyEnvelope> create_fiscal_year(tenant_id, opts)

Create a fiscal year

Creates a new fiscal year associated with a fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthorityYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_year_create_dto: OpenapiClient::FiscalYearCreateDto.new({name: 'name_example', fiscal_authority_id: 'fiscal_authority_id_example'}) # FiscalYearCreateDto | 
}

begin
  # Create a fiscal year
  result = api_instance.create_fiscal_year(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->create_fiscal_year: #{e}"
end
```

#### Using the create_fiscal_year_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_fiscal_year_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a fiscal year
  data, status_code, headers = api_instance.create_fiscal_year_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->create_fiscal_year_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_year_create_dto** | [**FiscalYearCreateDto**](FiscalYearCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_fiscal_year

> <EmptyEnvelope> delete_fiscal_year(tenant_id, fiscal_year_id, opts)

Delete a fiscal year

Deletes a fiscal year identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthorityYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a fiscal year
  result = api_instance.delete_fiscal_year(tenant_id, fiscal_year_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->delete_fiscal_year: #{e}"
end
```

#### Using the delete_fiscal_year_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_fiscal_year_with_http_info(tenant_id, fiscal_year_id, opts)

```ruby
begin
  # Delete a fiscal year
  data, status_code, headers = api_instance.delete_fiscal_year_with_http_info(tenant_id, fiscal_year_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->delete_fiscal_year_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_year

> <FiscalYearDtoEnvelope> get_fiscal_year(tenant_id, fiscal_authority_id, fiscal_year_id, opts)

Get fiscal year by ID for an authority

Retrieves a specific fiscal year by its unique identifier within a fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthorityYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal year by ID for an authority
  result = api_instance.get_fiscal_year(tenant_id, fiscal_authority_id, fiscal_year_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->get_fiscal_year: #{e}"
end
```

#### Using the get_fiscal_year_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalYearDtoEnvelope>, Integer, Hash)> get_fiscal_year_with_http_info(tenant_id, fiscal_authority_id, fiscal_year_id, opts)

```ruby
begin
  # Get fiscal year by ID for an authority
  data, status_code, headers = api_instance.get_fiscal_year_with_http_info(tenant_id, fiscal_authority_id, fiscal_year_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalYearDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->get_fiscal_year_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalYearDtoEnvelope**](FiscalYearDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_years

> <FiscalYearDtoListEnvelope> get_fiscal_years(tenant_id, fiscal_authority_id, authority_id, opts)

Get fiscal years for an authority

Retrieves all fiscal years associated with the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthorityYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = 'authority_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal years for an authority
  result = api_instance.get_fiscal_years(tenant_id, fiscal_authority_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->get_fiscal_years: #{e}"
end
```

#### Using the get_fiscal_years_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalYearDtoListEnvelope>, Integer, Hash)> get_fiscal_years_with_http_info(tenant_id, fiscal_authority_id, authority_id, opts)

```ruby
begin
  # Get fiscal years for an authority
  data, status_code, headers = api_instance.get_fiscal_years_with_http_info(tenant_id, fiscal_authority_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalYearDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->get_fiscal_years_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **authority_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalYearDtoListEnvelope**](FiscalYearDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_years_count

> <Int32Envelope> get_fiscal_years_count(tenant_id, fiscal_authority_id, opts)

Get fiscal years count for an authority

Returns the total count of fiscal years for the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthorityYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal years count for an authority
  result = api_instance.get_fiscal_years_count(tenant_id, fiscal_authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->get_fiscal_years_count: #{e}"
end
```

#### Using the get_fiscal_years_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_fiscal_years_count_with_http_info(tenant_id, fiscal_authority_id, opts)

```ruby
begin
  # Get fiscal years count for an authority
  data, status_code, headers = api_instance.get_fiscal_years_count_with_http_info(tenant_id, fiscal_authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->get_fiscal_years_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## patch_fiscal_authority_year_async

> <EmptyEnvelope> patch_fiscal_authority_year_async(tenant_id, fiscal_year_id, opts)

Patch a fiscal authority year

Partially updates a fiscal authority year.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthorityYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a fiscal authority year
  result = api_instance.patch_fiscal_authority_year_async(tenant_id, fiscal_year_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->patch_fiscal_authority_year_async: #{e}"
end
```

#### Using the patch_fiscal_authority_year_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_fiscal_authority_year_async_with_http_info(tenant_id, fiscal_year_id, opts)

```ruby
begin
  # Patch a fiscal authority year
  data, status_code, headers = api_instance.patch_fiscal_authority_year_async_with_http_info(tenant_id, fiscal_year_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->patch_fiscal_authority_year_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
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


## update_fiscal_year

> <EmptyEnvelope> update_fiscal_year(tenant_id, fiscal_year_id, opts)

Update a fiscal year

Updates an existing fiscal year identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalAuthorityYearsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_year_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_year_update_dto: OpenapiClient::FiscalYearUpdateDto.new({name: 'name_example', fiscal_authority_id: 'fiscal_authority_id_example'}) # FiscalYearUpdateDto | 
}

begin
  # Update a fiscal year
  result = api_instance.update_fiscal_year(tenant_id, fiscal_year_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->update_fiscal_year: #{e}"
end
```

#### Using the update_fiscal_year_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_fiscal_year_with_http_info(tenant_id, fiscal_year_id, opts)

```ruby
begin
  # Update a fiscal year
  data, status_code, headers = api_instance.update_fiscal_year_with_http_info(tenant_id, fiscal_year_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalAuthorityYearsApi->update_fiscal_year_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_year_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_year_update_dto** | [**FiscalYearUpdateDto**](FiscalYearUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

