# OpenapiClient::BusinessDomainsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_business_domain_async**](BusinessDomainsApi.md#create_business_domain_async) | **POST** /api/v2/ContentService/BusinessDomains | Register a business domain |
| [**delete_business_domain_async**](BusinessDomainsApi.md#delete_business_domain_async) | **DELETE** /api/v2/ContentService/BusinessDomains/{businessDomainId} | Delete a business domain |
| [**get_business_domain_by_id_async**](BusinessDomainsApi.md#get_business_domain_by_id_async) | **GET** /api/v2/ContentService/BusinessDomains/{businessDomainId} | Get business domain by ID |
| [**get_business_domains_async**](BusinessDomainsApi.md#get_business_domains_async) | **GET** /api/v2/ContentService/BusinessDomains | Get business domains |
| [**get_business_domains_count_async**](BusinessDomainsApi.md#get_business_domains_count_async) | **GET** /api/v2/ContentService/BusinessDomains/Count | Get business domains count |
| [**update_business_domain_async**](BusinessDomainsApi.md#update_business_domain_async) | **PUT** /api/v2/ContentService/BusinessDomains/{businessDomainId} | Update a business domain |
| [**verify_business_domain_async**](BusinessDomainsApi.md#verify_business_domain_async) | **POST** /api/v2/ContentService/BusinessDomains/{businessDomainId}/Verify | Verify a business domain |


## create_business_domain_async

> <EmptyEnvelope> create_business_domain_async(tenant_id, business_domain_create_dto, opts)

Register a business domain

Registers a new (unverified) business domain for the tenant and issues a DNS TXT verification token.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_domain_create_dto = OpenapiClient::BusinessDomainCreateDto.new({domain: 'domain_example'}) # BusinessDomainCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Register a business domain
  result = api_instance.create_business_domain_async(tenant_id, business_domain_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->create_business_domain_async: #{e}"
end
```

#### Using the create_business_domain_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_business_domain_async_with_http_info(tenant_id, business_domain_create_dto, opts)

```ruby
begin
  # Register a business domain
  data, status_code, headers = api_instance.create_business_domain_async_with_http_info(tenant_id, business_domain_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->create_business_domain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_domain_create_dto** | [**BusinessDomainCreateDto**](BusinessDomainCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_business_domain_async

> <EmptyEnvelope> delete_business_domain_async(tenant_id, business_domain_id, opts)

Delete a business domain

Removes a business domain from the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_domain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a business domain
  result = api_instance.delete_business_domain_async(tenant_id, business_domain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->delete_business_domain_async: #{e}"
end
```

#### Using the delete_business_domain_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_business_domain_async_with_http_info(tenant_id, business_domain_id, opts)

```ruby
begin
  # Delete a business domain
  data, status_code, headers = api_instance.delete_business_domain_async_with_http_info(tenant_id, business_domain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->delete_business_domain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_domain_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_domain_by_id_async

> <BusinessDomainDtoEnvelope> get_business_domain_by_id_async(tenant_id, business_domain_id, opts)

Get business domain by ID

Retrieves a specific business domain.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_domain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get business domain by ID
  result = api_instance.get_business_domain_by_id_async(tenant_id, business_domain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_business_domain_by_id_async: #{e}"
end
```

#### Using the get_business_domain_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessDomainDtoEnvelope>, Integer, Hash)> get_business_domain_by_id_async_with_http_info(tenant_id, business_domain_id, opts)

```ruby
begin
  # Get business domain by ID
  data, status_code, headers = api_instance.get_business_domain_by_id_async_with_http_info(tenant_id, business_domain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessDomainDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_business_domain_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_domain_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BusinessDomainDtoEnvelope**](BusinessDomainDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_domains_async

> <BusinessDomainDtoListEnvelope> get_business_domains_async(tenant_id, opts)

Get business domains

Retrieves business domains for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  business_domain_dto_collection_query_parameters: OpenapiClient::BusinessDomainDtoCollectionQueryParameters.new # BusinessDomainDtoCollectionQueryParameters | 
}

begin
  # Get business domains
  result = api_instance.get_business_domains_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_business_domains_async: #{e}"
end
```

#### Using the get_business_domains_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessDomainDtoListEnvelope>, Integer, Hash)> get_business_domains_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get business domains
  data, status_code, headers = api_instance.get_business_domains_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessDomainDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_business_domains_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **business_domain_dto_collection_query_parameters** | [**BusinessDomainDtoCollectionQueryParameters**](BusinessDomainDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BusinessDomainDtoListEnvelope**](BusinessDomainDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_business_domains_count_async

> <Int32Envelope> get_business_domains_count_async(tenant_id, opts)

Get business domains count

Retrieves the count of business domains for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  business_domain_dto_collection_query_parameters: OpenapiClient::BusinessDomainDtoCollectionQueryParameters.new # BusinessDomainDtoCollectionQueryParameters | 
}

begin
  # Get business domains count
  result = api_instance.get_business_domains_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_business_domains_count_async: #{e}"
end
```

#### Using the get_business_domains_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_business_domains_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get business domains count
  data, status_code, headers = api_instance.get_business_domains_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_business_domains_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **business_domain_dto_collection_query_parameters** | [**BusinessDomainDtoCollectionQueryParameters**](BusinessDomainDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_business_domain_async

> <EmptyEnvelope> update_business_domain_async(tenant_id, business_domain_id, business_domain_update_dto, opts)

Update a business domain

Updates a business domain. Changing the host re-issues the verification token and clears verification.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_domain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_domain_update_dto = OpenapiClient::BusinessDomainUpdateDto.new # BusinessDomainUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a business domain
  result = api_instance.update_business_domain_async(tenant_id, business_domain_id, business_domain_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->update_business_domain_async: #{e}"
end
```

#### Using the update_business_domain_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_business_domain_async_with_http_info(tenant_id, business_domain_id, business_domain_update_dto, opts)

```ruby
begin
  # Update a business domain
  data, status_code, headers = api_instance.update_business_domain_async_with_http_info(tenant_id, business_domain_id, business_domain_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->update_business_domain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_domain_id** | **String** |  |  |
| **business_domain_update_dto** | [**BusinessDomainUpdateDto**](BusinessDomainUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## verify_business_domain_async

> <EmptyEnvelope> verify_business_domain_async(tenant_id, business_domain_id, opts)

Verify a business domain

Checks the domain's DNS TXT records for the verification token and marks the domain verified.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_domain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Verify a business domain
  result = api_instance.verify_business_domain_async(tenant_id, business_domain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->verify_business_domain_async: #{e}"
end
```

#### Using the verify_business_domain_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> verify_business_domain_async_with_http_info(tenant_id, business_domain_id, opts)

```ruby
begin
  # Verify a business domain
  data, status_code, headers = api_instance.verify_business_domain_async_with_http_info(tenant_id, business_domain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->verify_business_domain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **business_domain_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

