# OpenapiClient::ItemWarrantyPoliciesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_item_warranty_policies_async**](ItemWarrantyPoliciesApi.md#count_item_warranty_policies_async) | **GET** /api/v2/CatalogService/ItemWarrantyPolicies/Count | Count item warranty policies |
| [**get_item_warranty_policies_async**](ItemWarrantyPoliciesApi.md#get_item_warranty_policies_async) | **GET** /api/v2/CatalogService/ItemWarrantyPolicies | Get item warranty policies |
| [**get_item_warranty_policy_by_id_async**](ItemWarrantyPoliciesApi.md#get_item_warranty_policy_by_id_async) | **GET** /api/v2/CatalogService/ItemWarrantyPolicies/{itemWarrantyPolicyId} | Get item warranty policy by ID |
| [**relate_item_to_warranty_policy_async**](ItemWarrantyPoliciesApi.md#relate_item_to_warranty_policy_async) | **POST** /api/v2/CatalogService/ItemWarrantyPolicies | Relate item to warranty policy |
| [**remove_warranty_policy_from_item_async**](ItemWarrantyPoliciesApi.md#remove_warranty_policy_from_item_async) | **DELETE** /api/v2/CatalogService/ItemWarrantyPolicies/{itemWarrantyPolicyId} | Remove warranty policy from item |


## count_item_warranty_policies_async

> <Int32Envelope> count_item_warranty_policies_async(opts)

Count item warranty policies

Counts all warranty policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemWarrantyPoliciesApi.new
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count item warranty policies
  result = api_instance.count_item_warranty_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->count_item_warranty_policies_async: #{e}"
end
```

#### Using the count_item_warranty_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_item_warranty_policies_async_with_http_info(opts)

```ruby
begin
  # Count item warranty policies
  data, status_code, headers = api_instance.count_item_warranty_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->count_item_warranty_policies_async_with_http_info: #{e}"
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


## get_item_warranty_policies_async

> <ItemWarrantyPolicyDtoListEnvelope> get_item_warranty_policies_async(opts)

Get item warranty policies

Retrieves all warranty policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemWarrantyPoliciesApi.new
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item warranty policies
  result = api_instance.get_item_warranty_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->get_item_warranty_policies_async: #{e}"
end
```

#### Using the get_item_warranty_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemWarrantyPolicyDtoListEnvelope>, Integer, Hash)> get_item_warranty_policies_async_with_http_info(opts)

```ruby
begin
  # Get item warranty policies
  data, status_code, headers = api_instance.get_item_warranty_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemWarrantyPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->get_item_warranty_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemWarrantyPolicyDtoListEnvelope**](ItemWarrantyPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_warranty_policy_by_id_async

> <ItemWarrantyPolicyDtoEnvelope> get_item_warranty_policy_by_id_async(item_warranty_policy_id, opts)

Get item warranty policy by ID

Retrieves a specific warranty policy for an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemWarrantyPoliciesApi.new
item_warranty_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item warranty policy by ID
  result = api_instance.get_item_warranty_policy_by_id_async(item_warranty_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->get_item_warranty_policy_by_id_async: #{e}"
end
```

#### Using the get_item_warranty_policy_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemWarrantyPolicyDtoEnvelope>, Integer, Hash)> get_item_warranty_policy_by_id_async_with_http_info(item_warranty_policy_id, opts)

```ruby
begin
  # Get item warranty policy by ID
  data, status_code, headers = api_instance.get_item_warranty_policy_by_id_async_with_http_info(item_warranty_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemWarrantyPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->get_item_warranty_policy_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_warranty_policy_id** | **String** |  |  |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemWarrantyPolicyDtoEnvelope**](ItemWarrantyPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_item_to_warranty_policy_async

> relate_item_to_warranty_policy_async(tenant_id, item_id, warranty_policy_id, opts)

Relate item to warranty policy

Relates an item to an existing warranty policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemWarrantyPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate item to warranty policy
  api_instance.relate_item_to_warranty_policy_async(tenant_id, item_id, warranty_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->relate_item_to_warranty_policy_async: #{e}"
end
```

#### Using the relate_item_to_warranty_policy_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> relate_item_to_warranty_policy_async_with_http_info(tenant_id, item_id, warranty_policy_id, opts)

```ruby
begin
  # Relate item to warranty policy
  data, status_code, headers = api_instance.relate_item_to_warranty_policy_async_with_http_info(tenant_id, item_id, warranty_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->relate_item_to_warranty_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **warranty_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_warranty_policy_from_item_async

> remove_warranty_policy_from_item_async(tenant_id, item_id, item_warranty_policy_id, opts)

Remove warranty policy from item

Removes a warranty policy from an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemWarrantyPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_warranty_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove warranty policy from item
  api_instance.remove_warranty_policy_from_item_async(tenant_id, item_id, item_warranty_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->remove_warranty_policy_from_item_async: #{e}"
end
```

#### Using the remove_warranty_policy_from_item_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> remove_warranty_policy_from_item_async_with_http_info(tenant_id, item_id, item_warranty_policy_id, opts)

```ruby
begin
  # Remove warranty policy from item
  data, status_code, headers = api_instance.remove_warranty_policy_from_item_async_with_http_info(tenant_id, item_id, item_warranty_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemWarrantyPoliciesApi->remove_warranty_policy_from_item_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_warranty_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

