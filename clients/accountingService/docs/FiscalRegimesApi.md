# OpenapiClient::FiscalRegimesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_fiscal_regime**](FiscalRegimesApi.md#create_fiscal_regime) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalRegimes | Create a fiscal regime |
| [**delete_fiscal_regime**](FiscalRegimesApi.md#delete_fiscal_regime) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalRegimes/{regimeId} | Delete a fiscal regime |
| [**get_fiscal_regime**](FiscalRegimesApi.md#get_fiscal_regime) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalRegimes/{regimeId} | Get fiscal regime by ID |
| [**get_fiscal_regimes**](FiscalRegimesApi.md#get_fiscal_regimes) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/FiscalRegimes | Get fiscal regimes for an authority |
| [**get_fiscal_regimes_count**](FiscalRegimesApi.md#get_fiscal_regimes_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalRegimes/Count | Get fiscal regimes count |
| [**update_fiscal_regime**](FiscalRegimesApi.md#update_fiscal_regime) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalRegimes/{regimeId} | Update a fiscal regime |


## create_fiscal_regime

> <EmptyEnvelope> create_fiscal_regime(tenant_id, opts)

Create a fiscal regime

Creates a new fiscal regime for a fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalRegimesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_regime_create_dto: OpenapiClient::FiscalRegimeCreateDto.new # FiscalRegimeCreateDto | 
}

begin
  # Create a fiscal regime
  result = api_instance.create_fiscal_regime(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->create_fiscal_regime: #{e}"
end
```

#### Using the create_fiscal_regime_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_fiscal_regime_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a fiscal regime
  data, status_code, headers = api_instance.create_fiscal_regime_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->create_fiscal_regime_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_regime_create_dto** | [**FiscalRegimeCreateDto**](FiscalRegimeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_fiscal_regime

> <EmptyEnvelope> delete_fiscal_regime(tenant_id, regime_id, opts)

Delete a fiscal regime

Deletes a fiscal regime identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalRegimesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
regime_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a fiscal regime
  result = api_instance.delete_fiscal_regime(tenant_id, regime_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->delete_fiscal_regime: #{e}"
end
```

#### Using the delete_fiscal_regime_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_fiscal_regime_with_http_info(tenant_id, regime_id, opts)

```ruby
begin
  # Delete a fiscal regime
  data, status_code, headers = api_instance.delete_fiscal_regime_with_http_info(tenant_id, regime_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->delete_fiscal_regime_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **regime_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_regime

> <FiscalRegimeDtoEnvelope> get_fiscal_regime(tenant_id, fiscal_authority_id, regime_id, opts)

Get fiscal regime by ID

Retrieves a specific fiscal regime by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalRegimesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
regime_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal regime by ID
  result = api_instance.get_fiscal_regime(tenant_id, fiscal_authority_id, regime_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->get_fiscal_regime: #{e}"
end
```

#### Using the get_fiscal_regime_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalRegimeDtoEnvelope>, Integer, Hash)> get_fiscal_regime_with_http_info(tenant_id, fiscal_authority_id, regime_id, opts)

```ruby
begin
  # Get fiscal regime by ID
  data, status_code, headers = api_instance.get_fiscal_regime_with_http_info(tenant_id, fiscal_authority_id, regime_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalRegimeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->get_fiscal_regime_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **fiscal_authority_id** | **String** |  |  |
| **regime_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FiscalRegimeDtoEnvelope**](FiscalRegimeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_regimes

> <FiscalRegimeDtoListEnvelope> get_fiscal_regimes(fiscal_authority_id, authority_id, opts)

Get fiscal regimes for an authority

Retrieves all fiscal regimes for the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalRegimesApi.new
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
authority_id = 'authority_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal regimes for an authority
  result = api_instance.get_fiscal_regimes(fiscal_authority_id, authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->get_fiscal_regimes: #{e}"
end
```

#### Using the get_fiscal_regimes_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FiscalRegimeDtoListEnvelope>, Integer, Hash)> get_fiscal_regimes_with_http_info(fiscal_authority_id, authority_id, opts)

```ruby
begin
  # Get fiscal regimes for an authority
  data, status_code, headers = api_instance.get_fiscal_regimes_with_http_info(fiscal_authority_id, authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FiscalRegimeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->get_fiscal_regimes_with_http_info: #{e}"
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

[**FiscalRegimeDtoListEnvelope**](FiscalRegimeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_fiscal_regimes_count

> <Int32Envelope> get_fiscal_regimes_count(fiscal_authority_id, opts)

Get fiscal regimes count

Returns the total count of fiscal regimes for the specified fiscal authority.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalRegimesApi.new
fiscal_authority_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get fiscal regimes count
  result = api_instance.get_fiscal_regimes_count(fiscal_authority_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->get_fiscal_regimes_count: #{e}"
end
```

#### Using the get_fiscal_regimes_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_fiscal_regimes_count_with_http_info(fiscal_authority_id, opts)

```ruby
begin
  # Get fiscal regimes count
  data, status_code, headers = api_instance.get_fiscal_regimes_count_with_http_info(fiscal_authority_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->get_fiscal_regimes_count_with_http_info: #{e}"
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


## update_fiscal_regime

> <EmptyEnvelope> update_fiscal_regime(tenant_id, regime_id, opts)

Update a fiscal regime

Updates an existing fiscal regime identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FiscalRegimesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
regime_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  fiscal_regime_update_dto: OpenapiClient::FiscalRegimeUpdateDto.new # FiscalRegimeUpdateDto | 
}

begin
  # Update a fiscal regime
  result = api_instance.update_fiscal_regime(tenant_id, regime_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->update_fiscal_regime: #{e}"
end
```

#### Using the update_fiscal_regime_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_fiscal_regime_with_http_info(tenant_id, regime_id, opts)

```ruby
begin
  # Update a fiscal regime
  data, status_code, headers = api_instance.update_fiscal_regime_with_http_info(tenant_id, regime_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FiscalRegimesApi->update_fiscal_regime_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **regime_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **fiscal_regime_update_dto** | [**FiscalRegimeUpdateDto**](FiscalRegimeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

