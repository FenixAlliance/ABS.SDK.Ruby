# OpenapiClient::BusinessDomainsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_business_domain_by_id_async**](BusinessDomainsApi.md#get_business_domain_by_id_async) | **GET** /api/v2/ContentService/BusinessDomains/{businessDomainId} | Get business domain by ID |
| [**get_business_domains_async**](BusinessDomainsApi.md#get_business_domains_async) | **GET** /api/v2/ContentService/BusinessDomains | Get business domains |
| [**get_business_domains_count_async**](BusinessDomainsApi.md#get_business_domains_count_async) | **GET** /api/v2/ContentService/BusinessDomains/Count | Get business domains count |


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
  x_api_version: 'x_api_version_example' # String | 
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

### Return type

[**BusinessDomainDtoListEnvelope**](BusinessDomainDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
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
  x_api_version: 'x_api_version_example' # String | 
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

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

