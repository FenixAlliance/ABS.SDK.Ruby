# OpenapiClient::ItemReturnPoliciesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_item_return_policies_async**](ItemReturnPoliciesApi.md#count_item_return_policies_async) | **GET** /api/v2/CatalogService/ItemReturnPolicies/Count | Count item return policies |
| [**get_item_return_policies_async**](ItemReturnPoliciesApi.md#get_item_return_policies_async) | **GET** /api/v2/CatalogService/ItemReturnPolicies | Get item return policies |
| [**get_item_return_policy_by_id_async**](ItemReturnPoliciesApi.md#get_item_return_policy_by_id_async) | **GET** /api/v2/CatalogService/ItemReturnPolicies/{itemReturnPolicyId} | Get item return policy by ID |
| [**relate_item_to_return_policy_async**](ItemReturnPoliciesApi.md#relate_item_to_return_policy_async) | **POST** /api/v2/CatalogService/ItemReturnPolicies | Relate item to return policy |
| [**remove_return_policy_from_item_async**](ItemReturnPoliciesApi.md#remove_return_policy_from_item_async) | **DELETE** /api/v2/CatalogService/ItemReturnPolicies/{itemReturnPolicyId} | Remove return policy from item |


## count_item_return_policies_async

> <Int32Envelope> count_item_return_policies_async(opts)

Count item return policies

Counts all return policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReturnPoliciesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count item return policies
  result = api_instance.count_item_return_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->count_item_return_policies_async: #{e}"
end
```

#### Using the count_item_return_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_item_return_policies_async_with_http_info(opts)

```ruby
begin
  # Count item return policies
  data, status_code, headers = api_instance.count_item_return_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->count_item_return_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
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


## get_item_return_policies_async

> <ItemReturnPolicyDtoListEnvelope> get_item_return_policies_async(opts)

Get item return policies

Retrieves all return policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReturnPoliciesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item return policies
  result = api_instance.get_item_return_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->get_item_return_policies_async: #{e}"
end
```

#### Using the get_item_return_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReturnPolicyDtoListEnvelope>, Integer, Hash)> get_item_return_policies_async_with_http_info(opts)

```ruby
begin
  # Get item return policies
  data, status_code, headers = api_instance.get_item_return_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReturnPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->get_item_return_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReturnPolicyDtoListEnvelope**](ItemReturnPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_return_policy_by_id_async

> <ItemReturnPolicyDtoEnvelope> get_item_return_policy_by_id_async(item_return_policy_id, opts)

Get item return policy by ID

Retrieves a specific return policy for an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReturnPoliciesApi.new
item_return_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item return policy by ID
  result = api_instance.get_item_return_policy_by_id_async(item_return_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->get_item_return_policy_by_id_async: #{e}"
end
```

#### Using the get_item_return_policy_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReturnPolicyDtoEnvelope>, Integer, Hash)> get_item_return_policy_by_id_async_with_http_info(item_return_policy_id, opts)

```ruby
begin
  # Get item return policy by ID
  data, status_code, headers = api_instance.get_item_return_policy_by_id_async_with_http_info(item_return_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReturnPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->get_item_return_policy_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_return_policy_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReturnPolicyDtoEnvelope**](ItemReturnPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_item_to_return_policy_async

> relate_item_to_return_policy_async(tenant_id, item_id, return_policy_id, opts)

Relate item to return policy

Relates an item to an existing return policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReturnPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate item to return policy
  api_instance.relate_item_to_return_policy_async(tenant_id, item_id, return_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->relate_item_to_return_policy_async: #{e}"
end
```

#### Using the relate_item_to_return_policy_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> relate_item_to_return_policy_async_with_http_info(tenant_id, item_id, return_policy_id, opts)

```ruby
begin
  # Relate item to return policy
  data, status_code, headers = api_instance.relate_item_to_return_policy_async_with_http_info(tenant_id, item_id, return_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->relate_item_to_return_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **return_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_return_policy_from_item_async

> remove_return_policy_from_item_async(tenant_id, item_id, item_return_policy_id, opts)

Remove return policy from item

Removes a return policy from an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemReturnPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_return_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove return policy from item
  api_instance.remove_return_policy_from_item_async(tenant_id, item_id, item_return_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->remove_return_policy_from_item_async: #{e}"
end
```

#### Using the remove_return_policy_from_item_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> remove_return_policy_from_item_async_with_http_info(tenant_id, item_id, item_return_policy_id, opts)

```ruby
begin
  # Remove return policy from item
  data, status_code, headers = api_instance.remove_return_policy_from_item_async_with_http_info(tenant_id, item_id, item_return_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemReturnPoliciesApi->remove_return_policy_from_item_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_return_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

