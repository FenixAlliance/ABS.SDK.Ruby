# OpenapiClient::IndustriesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_industry**](IndustriesApi.md#create_tenant_industry) | **POST** /api/v2/TenantsService/Industries | Create a new tenant industry |
| [**delete_tenant_industry**](IndustriesApi.md#delete_tenant_industry) | **DELETE** /api/v2/TenantsService/Industries/{tenantIndustryId} | Delete a tenant industry |
| [**get_tenant_industries**](IndustriesApi.md#get_tenant_industries) | **GET** /api/v2/TenantsService/Industries | Retrieve a list of tenant industries |
| [**get_tenant_industries_count**](IndustriesApi.md#get_tenant_industries_count) | **GET** /api/v2/TenantsService/Industries/Count | Get the count of tenant industries |
| [**get_tenant_industry_by_id**](IndustriesApi.md#get_tenant_industry_by_id) | **GET** /api/v2/TenantsService/Industries/{tenantIndustryId} | Retrieve a single tenant industry by its ID |
| [**update_tenant_industry**](IndustriesApi.md#update_tenant_industry) | **PUT** /api/v2/TenantsService/Industries/{tenantIndustryId} | Update a tenant industry |


## create_tenant_industry

> <EmptyEnvelope> create_tenant_industry(tenant_id, opts)

Create a new tenant industry

Create a new tenant industry

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IndustriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_industry_create_dto: OpenapiClient::TenantIndustryCreateDto.new # TenantIndustryCreateDto | 
}

begin
  # Create a new tenant industry
  result = api_instance.create_tenant_industry(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->create_tenant_industry: #{e}"
end
```

#### Using the create_tenant_industry_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_industry_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant industry
  data, status_code, headers = api_instance.create_tenant_industry_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->create_tenant_industry_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_industry_create_dto** | [**TenantIndustryCreateDto**](TenantIndustryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_industry

> <EmptyEnvelope> delete_tenant_industry(tenant_id, tenant_industry_id, opts)

Delete a tenant industry

Delete a tenant industry

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IndustriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_industry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant industry
  result = api_instance.delete_tenant_industry(tenant_id, tenant_industry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->delete_tenant_industry: #{e}"
end
```

#### Using the delete_tenant_industry_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_industry_with_http_info(tenant_id, tenant_industry_id, opts)

```ruby
begin
  # Delete a tenant industry
  data, status_code, headers = api_instance.delete_tenant_industry_with_http_info(tenant_id, tenant_industry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->delete_tenant_industry_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_industry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_industries

> <TenantIndustryDtoListEnvelope> get_tenant_industries(tenant_id, opts)

Retrieve a list of tenant industries

Retrieve a list of tenant industries

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IndustriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant industries
  result = api_instance.get_tenant_industries(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->get_tenant_industries: #{e}"
end
```

#### Using the get_tenant_industries_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantIndustryDtoListEnvelope>, Integer, Hash)> get_tenant_industries_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant industries
  data, status_code, headers = api_instance.get_tenant_industries_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantIndustryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->get_tenant_industries_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantIndustryDtoListEnvelope**](TenantIndustryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_industries_count

> <Int32Envelope> get_tenant_industries_count(tenant_id, opts)

Get the count of tenant industries

Get the count of tenant industries

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IndustriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant industries
  result = api_instance.get_tenant_industries_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->get_tenant_industries_count: #{e}"
end
```

#### Using the get_tenant_industries_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_industries_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant industries
  data, status_code, headers = api_instance.get_tenant_industries_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->get_tenant_industries_count_with_http_info: #{e}"
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


## get_tenant_industry_by_id

> <TenantIndustryDtoEnvelope> get_tenant_industry_by_id(tenant_id, tenant_industry_id, opts)

Retrieve a single tenant industry by its ID

Retrieve a single tenant industry by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IndustriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_industry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant industry by its ID
  result = api_instance.get_tenant_industry_by_id(tenant_id, tenant_industry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->get_tenant_industry_by_id: #{e}"
end
```

#### Using the get_tenant_industry_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantIndustryDtoEnvelope>, Integer, Hash)> get_tenant_industry_by_id_with_http_info(tenant_id, tenant_industry_id, opts)

```ruby
begin
  # Retrieve a single tenant industry by its ID
  data, status_code, headers = api_instance.get_tenant_industry_by_id_with_http_info(tenant_id, tenant_industry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantIndustryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->get_tenant_industry_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_industry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantIndustryDtoEnvelope**](TenantIndustryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_tenant_industry

> <EmptyEnvelope> update_tenant_industry(tenant_id, tenant_industry_id, opts)

Update a tenant industry

Update a tenant industry

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IndustriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_industry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_industry_update_dto: OpenapiClient::TenantIndustryUpdateDto.new # TenantIndustryUpdateDto | 
}

begin
  # Update a tenant industry
  result = api_instance.update_tenant_industry(tenant_id, tenant_industry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->update_tenant_industry: #{e}"
end
```

#### Using the update_tenant_industry_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_industry_with_http_info(tenant_id, tenant_industry_id, opts)

```ruby
begin
  # Update a tenant industry
  data, status_code, headers = api_instance.update_tenant_industry_with_http_info(tenant_id, tenant_industry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling IndustriesApi->update_tenant_industry_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_industry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_industry_update_dto** | [**TenantIndustryUpdateDto**](TenantIndustryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

