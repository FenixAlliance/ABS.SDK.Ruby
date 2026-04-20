# OpenapiClient::ItemTaxPoliciesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_item_tax_policies_async**](ItemTaxPoliciesApi.md#count_item_tax_policies_async) | **GET** /api/v2/CatalogService/ItemTaxPolicies/Count | Count item tax policies |
| [**get_item_tax_policies_async**](ItemTaxPoliciesApi.md#get_item_tax_policies_async) | **GET** /api/v2/CatalogService/ItemTaxPolicies | Get item tax policies |
| [**get_item_tax_policy_by_id_async**](ItemTaxPoliciesApi.md#get_item_tax_policy_by_id_async) | **GET** /api/v2/CatalogService/ItemTaxPolicies/{itemTaxPolicyId} | Get item tax policy by ID |
| [**relate_item_to_tax_policy_async**](ItemTaxPoliciesApi.md#relate_item_to_tax_policy_async) | **POST** /api/v2/CatalogService/ItemTaxPolicies | Relate item to tax policy |
| [**remove_tax_policy_from_item_async**](ItemTaxPoliciesApi.md#remove_tax_policy_from_item_async) | **DELETE** /api/v2/CatalogService/ItemTaxPolicies/{itemTaxPolicyId} | Remove tax policy from item |


## count_item_tax_policies_async

> <Int32Envelope> count_item_tax_policies_async(opts)

Count item tax policies

Counts all tax policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTaxPoliciesApi.new
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count item tax policies
  result = api_instance.count_item_tax_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->count_item_tax_policies_async: #{e}"
end
```

#### Using the count_item_tax_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_item_tax_policies_async_with_http_info(opts)

```ruby
begin
  # Count item tax policies
  data, status_code, headers = api_instance.count_item_tax_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->count_item_tax_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_tax_policies_async

> <ItemTaxPolicyDtoListEnvelope> get_item_tax_policies_async(opts)

Get item tax policies

Retrieves all tax policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTaxPoliciesApi.new
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item tax policies
  result = api_instance.get_item_tax_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->get_item_tax_policies_async: #{e}"
end
```

#### Using the get_item_tax_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTaxPolicyDtoListEnvelope>, Integer, Hash)> get_item_tax_policies_async_with_http_info(opts)

```ruby
begin
  # Get item tax policies
  data, status_code, headers = api_instance.get_item_tax_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTaxPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->get_item_tax_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTaxPolicyDtoListEnvelope**](ItemTaxPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_tax_policy_by_id_async

> <ItemTaxPolicyDtoEnvelope> get_item_tax_policy_by_id_async(item_tax_policy_id, opts)

Get item tax policy by ID

Retrieves a specific tax policy for an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTaxPoliciesApi.new
item_tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item tax policy by ID
  result = api_instance.get_item_tax_policy_by_id_async(item_tax_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->get_item_tax_policy_by_id_async: #{e}"
end
```

#### Using the get_item_tax_policy_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTaxPolicyDtoEnvelope>, Integer, Hash)> get_item_tax_policy_by_id_async_with_http_info(item_tax_policy_id, opts)

```ruby
begin
  # Get item tax policy by ID
  data, status_code, headers = api_instance.get_item_tax_policy_by_id_async_with_http_info(item_tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTaxPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->get_item_tax_policy_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_tax_policy_id** | **String** |  |  |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTaxPolicyDtoEnvelope**](ItemTaxPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_item_to_tax_policy_async

> relate_item_to_tax_policy_async(tenant_id, item_id, tax_policy_id, opts)

Relate item to tax policy

Relates an item to an existing tax policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate item to tax policy
  api_instance.relate_item_to_tax_policy_async(tenant_id, item_id, tax_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->relate_item_to_tax_policy_async: #{e}"
end
```

#### Using the relate_item_to_tax_policy_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> relate_item_to_tax_policy_async_with_http_info(tenant_id, item_id, tax_policy_id, opts)

```ruby
begin
  # Relate item to tax policy
  data, status_code, headers = api_instance.relate_item_to_tax_policy_async_with_http_info(tenant_id, item_id, tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->relate_item_to_tax_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_tax_policy_from_item_async

> remove_tax_policy_from_item_async(tenant_id, item_id, item_tax_policy_id, opts)

Remove tax policy from item

Removes a tax policy from an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTaxPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove tax policy from item
  api_instance.remove_tax_policy_from_item_async(tenant_id, item_id, item_tax_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->remove_tax_policy_from_item_async: #{e}"
end
```

#### Using the remove_tax_policy_from_item_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> remove_tax_policy_from_item_async_with_http_info(tenant_id, item_id, item_tax_policy_id, opts)

```ruby
begin
  # Remove tax policy from item
  data, status_code, headers = api_instance.remove_tax_policy_from_item_async_with_http_info(tenant_id, item_id, item_tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTaxPoliciesApi->remove_tax_policy_from_item_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

