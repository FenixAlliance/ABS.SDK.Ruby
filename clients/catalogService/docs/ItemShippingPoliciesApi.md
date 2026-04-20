# OpenapiClient::ItemShippingPoliciesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_item_shipping_policies_async**](ItemShippingPoliciesApi.md#count_item_shipping_policies_async) | **GET** /api/v2/CatalogService/ItemShippingPolicies/Count | Count item shipping policies |
| [**get_item_shipping_policies_async**](ItemShippingPoliciesApi.md#get_item_shipping_policies_async) | **GET** /api/v2/CatalogService/ItemShippingPolicies | Get item shipping policies |
| [**get_item_shipping_policy_by_id_async**](ItemShippingPoliciesApi.md#get_item_shipping_policy_by_id_async) | **GET** /api/v2/CatalogService/ItemShippingPolicies/{itemShippingPolicyId} | Get item shipping policy by ID |
| [**relate_item_to_shipping_policy_async**](ItemShippingPoliciesApi.md#relate_item_to_shipping_policy_async) | **POST** /api/v2/CatalogService/ItemShippingPolicies | Relate item to shipping policy |
| [**remove_shipping_policy_from_item_async**](ItemShippingPoliciesApi.md#remove_shipping_policy_from_item_async) | **DELETE** /api/v2/CatalogService/ItemShippingPolicies/{itemShippingPolicyId} | Remove shipping policy from item |


## count_item_shipping_policies_async

> <Int32Envelope> count_item_shipping_policies_async(opts)

Count item shipping policies

Counts all shipping policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count item shipping policies
  result = api_instance.count_item_shipping_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->count_item_shipping_policies_async: #{e}"
end
```

#### Using the count_item_shipping_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_item_shipping_policies_async_with_http_info(opts)

```ruby
begin
  # Count item shipping policies
  data, status_code, headers = api_instance.count_item_shipping_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->count_item_shipping_policies_async_with_http_info: #{e}"
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


## get_item_shipping_policies_async

> <ItemShippingPolicyDtoListEnvelope> get_item_shipping_policies_async(opts)

Get item shipping policies

Retrieves all shipping policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item shipping policies
  result = api_instance.get_item_shipping_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->get_item_shipping_policies_async: #{e}"
end
```

#### Using the get_item_shipping_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemShippingPolicyDtoListEnvelope>, Integer, Hash)> get_item_shipping_policies_async_with_http_info(opts)

```ruby
begin
  # Get item shipping policies
  data, status_code, headers = api_instance.get_item_shipping_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemShippingPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->get_item_shipping_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemShippingPolicyDtoListEnvelope**](ItemShippingPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_shipping_policy_by_id_async

> <ItemShippingPolicyDtoEnvelope> get_item_shipping_policy_by_id_async(item_shipping_policy_id, opts)

Get item shipping policy by ID

Retrieves a specific shipping policy for an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
item_shipping_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item shipping policy by ID
  result = api_instance.get_item_shipping_policy_by_id_async(item_shipping_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->get_item_shipping_policy_by_id_async: #{e}"
end
```

#### Using the get_item_shipping_policy_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemShippingPolicyDtoEnvelope>, Integer, Hash)> get_item_shipping_policy_by_id_async_with_http_info(item_shipping_policy_id, opts)

```ruby
begin
  # Get item shipping policy by ID
  data, status_code, headers = api_instance.get_item_shipping_policy_by_id_async_with_http_info(item_shipping_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemShippingPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->get_item_shipping_policy_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_shipping_policy_id** | **String** |  |  |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemShippingPolicyDtoEnvelope**](ItemShippingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_item_to_shipping_policy_async

> relate_item_to_shipping_policy_async(tenant_id, item_id, shipping_policy_id, opts)

Relate item to shipping policy

Relates an item to an existing shipping policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
shipping_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate item to shipping policy
  api_instance.relate_item_to_shipping_policy_async(tenant_id, item_id, shipping_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->relate_item_to_shipping_policy_async: #{e}"
end
```

#### Using the relate_item_to_shipping_policy_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> relate_item_to_shipping_policy_async_with_http_info(tenant_id, item_id, shipping_policy_id, opts)

```ruby
begin
  # Relate item to shipping policy
  data, status_code, headers = api_instance.relate_item_to_shipping_policy_async_with_http_info(tenant_id, item_id, shipping_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->relate_item_to_shipping_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **shipping_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_shipping_policy_from_item_async

> remove_shipping_policy_from_item_async(tenant_id, item_id, item_shipping_policy_id, opts)

Remove shipping policy from item

Removes a shipping policy from an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_shipping_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove shipping policy from item
  api_instance.remove_shipping_policy_from_item_async(tenant_id, item_id, item_shipping_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->remove_shipping_policy_from_item_async: #{e}"
end
```

#### Using the remove_shipping_policy_from_item_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> remove_shipping_policy_from_item_async_with_http_info(tenant_id, item_id, item_shipping_policy_id, opts)

```ruby
begin
  # Remove shipping policy from item
  data, status_code, headers = api_instance.remove_shipping_policy_from_item_async_with_http_info(tenant_id, item_id, item_shipping_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->remove_shipping_policy_from_item_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_shipping_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

