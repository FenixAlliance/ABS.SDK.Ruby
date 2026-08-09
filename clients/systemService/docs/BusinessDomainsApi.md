# OpenapiClient::BusinessDomainsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**delete_system_business_domain**](BusinessDomainsApi.md#delete_system_business_domain) | **DELETE** /api/v2/SystemService/BusinessDomains/{businessDomainId} | Delete a business domain |
| [**get_system_business_domain_by_id**](BusinessDomainsApi.md#get_system_business_domain_by_id) | **GET** /api/v2/SystemService/BusinessDomains/{businessDomainId} | Retrieve a business domain by its ID |
| [**get_system_business_domains**](BusinessDomainsApi.md#get_system_business_domains) | **GET** /api/v2/SystemService/BusinessDomains | Retrieve all business domains in the system |
| [**get_system_business_domains_count**](BusinessDomainsApi.md#get_system_business_domains_count) | **GET** /api/v2/SystemService/BusinessDomains/Count | Get the count of all business domains in the system |
| [**verify_system_business_domain**](BusinessDomainsApi.md#verify_system_business_domain) | **POST** /api/v2/SystemService/BusinessDomains/{businessDomainId}/Verify | Verify a business domain |


## delete_system_business_domain

> <EmptyEnvelope> delete_system_business_domain(business_domain_id, opts)

Delete a business domain

Removes any business domain from the system, regardless of owning tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
business_domain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a business domain
  result = api_instance.delete_system_business_domain(business_domain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->delete_system_business_domain: #{e}"
end
```

#### Using the delete_system_business_domain_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_system_business_domain_with_http_info(business_domain_id, opts)

```ruby
begin
  # Delete a business domain
  data, status_code, headers = api_instance.delete_system_business_domain_with_http_info(business_domain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->delete_system_business_domain_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## get_system_business_domain_by_id

> <BusinessDomainDtoEnvelope> get_system_business_domain_by_id(business_domain_id, opts)

Retrieve a business domain by its ID

Retrieve any business domain by its ID, regardless of owning tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
business_domain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a business domain by its ID
  result = api_instance.get_system_business_domain_by_id(business_domain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_system_business_domain_by_id: #{e}"
end
```

#### Using the get_system_business_domain_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessDomainDtoEnvelope>, Integer, Hash)> get_system_business_domain_by_id_with_http_info(business_domain_id, opts)

```ruby
begin
  # Retrieve a business domain by its ID
  data, status_code, headers = api_instance.get_system_business_domain_by_id_with_http_info(business_domain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessDomainDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_system_business_domain_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## get_system_business_domains

> <BusinessDomainDtoListEnvelope> get_system_business_domains(opts)

Retrieve all business domains in the system

Retrieve all registered business domains across every tenant (global administrators only).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  business_domain_dto_collection_query_parameters: OpenapiClient::BusinessDomainDtoCollectionQueryParameters.new # BusinessDomainDtoCollectionQueryParameters | 
}

begin
  # Retrieve all business domains in the system
  result = api_instance.get_system_business_domains(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_system_business_domains: #{e}"
end
```

#### Using the get_system_business_domains_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessDomainDtoListEnvelope>, Integer, Hash)> get_system_business_domains_with_http_info(opts)

```ruby
begin
  # Retrieve all business domains in the system
  data, status_code, headers = api_instance.get_system_business_domains_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessDomainDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_system_business_domains_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## get_system_business_domains_count

> <Int32Envelope> get_system_business_domains_count(opts)

Get the count of all business domains in the system

Get the count of all registered business domains across every tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  business_domain_dto_collection_query_parameters: OpenapiClient::BusinessDomainDtoCollectionQueryParameters.new # BusinessDomainDtoCollectionQueryParameters | 
}

begin
  # Get the count of all business domains in the system
  result = api_instance.get_system_business_domains_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_system_business_domains_count: #{e}"
end
```

#### Using the get_system_business_domains_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_system_business_domains_count_with_http_info(opts)

```ruby
begin
  # Get the count of all business domains in the system
  data, status_code, headers = api_instance.get_system_business_domains_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->get_system_business_domains_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## verify_system_business_domain

> <EmptyEnvelope> verify_system_business_domain(business_domain_id, opts)

Verify a business domain

Checks the domain's DNS TXT records for the verification token and marks it verified.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BusinessDomainsApi.new
business_domain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Verify a business domain
  result = api_instance.verify_system_business_domain(business_domain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->verify_system_business_domain: #{e}"
end
```

#### Using the verify_system_business_domain_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> verify_system_business_domain_with_http_info(business_domain_id, opts)

```ruby
begin
  # Verify a business domain
  data, status_code, headers = api_instance.verify_system_business_domain_with_http_info(business_domain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BusinessDomainsApi->verify_system_business_domain_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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

