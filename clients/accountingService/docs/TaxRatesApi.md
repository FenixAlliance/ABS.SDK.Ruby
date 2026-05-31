# OpenapiClient::TaxRatesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tax_rate**](TaxRatesApi.md#create_tax_rate) | **POST** /api/v2/AccountingService/TaxRates | Create a tax rate |
| [**delete_tax_rate**](TaxRatesApi.md#delete_tax_rate) | **DELETE** /api/v2/AccountingService/TaxRates/{id} | Delete a tax rate |
| [**get_tax_rate**](TaxRatesApi.md#get_tax_rate) | **GET** /api/v2/AccountingService/TaxRates/{id} | Get tax rate by ID |
| [**get_tax_rates**](TaxRatesApi.md#get_tax_rates) | **GET** /api/v2/AccountingService/TaxRates | Get all tax rates for a tenant |
| [**get_tax_rates_count**](TaxRatesApi.md#get_tax_rates_count) | **GET** /api/v2/AccountingService/TaxRates/Count | Get tax rates count |
| [**update_tax_rate**](TaxRatesApi.md#update_tax_rate) | **PUT** /api/v2/AccountingService/TaxRates/{id} | Update a tax rate |


## create_tax_rate

> <EmptyEnvelope> create_tax_rate(tenant_id, opts)

Create a tax rate

Creates a new tax rate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxRatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_rate_create_dto: OpenapiClient::TaxRateCreateDto.new # TaxRateCreateDto | 
}

begin
  # Create a tax rate
  result = api_instance.create_tax_rate(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->create_tax_rate: #{e}"
end
```

#### Using the create_tax_rate_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tax_rate_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a tax rate
  data, status_code, headers = api_instance.create_tax_rate_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->create_tax_rate_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_rate_create_dto** | [**TaxRateCreateDto**](TaxRateCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tax_rate

> <EmptyEnvelope> delete_tax_rate(tenant_id, id, opts)

Delete a tax rate

Deletes a tax rate identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxRatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tax rate
  result = api_instance.delete_tax_rate(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->delete_tax_rate: #{e}"
end
```

#### Using the delete_tax_rate_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tax_rate_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a tax rate
  data, status_code, headers = api_instance.delete_tax_rate_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->delete_tax_rate_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tax_rate

> <TaxRateDtoEnvelope> get_tax_rate(tenant_id, id, opts)

Get tax rate by ID

Retrieves a specific tax rate by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxRatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get tax rate by ID
  result = api_instance.get_tax_rate(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->get_tax_rate: #{e}"
end
```

#### Using the get_tax_rate_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaxRateDtoEnvelope>, Integer, Hash)> get_tax_rate_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get tax rate by ID
  data, status_code, headers = api_instance.get_tax_rate_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaxRateDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->get_tax_rate_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TaxRateDtoEnvelope**](TaxRateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tax_rates

> <TaxRateDtoListEnvelope> get_tax_rates(tenant_id, opts)

Get all tax rates for a tenant

Retrieves all tax rates for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxRatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all tax rates for a tenant
  result = api_instance.get_tax_rates(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->get_tax_rates: #{e}"
end
```

#### Using the get_tax_rates_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TaxRateDtoListEnvelope>, Integer, Hash)> get_tax_rates_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all tax rates for a tenant
  data, status_code, headers = api_instance.get_tax_rates_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TaxRateDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->get_tax_rates_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TaxRateDtoListEnvelope**](TaxRateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tax_rates_count

> <Int32Envelope> get_tax_rates_count(tenant_id, opts)

Get tax rates count

Returns the count of tax rates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxRatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get tax rates count
  result = api_instance.get_tax_rates_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->get_tax_rates_count: #{e}"
end
```

#### Using the get_tax_rates_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tax_rates_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get tax rates count
  data, status_code, headers = api_instance.get_tax_rates_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->get_tax_rates_count_with_http_info: #{e}"
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


## update_tax_rate

> <EmptyEnvelope> update_tax_rate(tenant_id, id, opts)

Update a tax rate

Updates an existing tax rate identified by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TaxRatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tax_rate_update_dto: OpenapiClient::TaxRateUpdateDto.new # TaxRateUpdateDto | 
}

begin
  # Update a tax rate
  result = api_instance.update_tax_rate(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->update_tax_rate: #{e}"
end
```

#### Using the update_tax_rate_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tax_rate_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a tax rate
  data, status_code, headers = api_instance.update_tax_rate_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TaxRatesApi->update_tax_rate_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tax_rate_update_dto** | [**TaxRateUpdateDto**](TaxRateUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

