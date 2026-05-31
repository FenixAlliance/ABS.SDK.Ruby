# OpenapiClient::ItemRefundPoliciesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_item_refund_policies_async**](ItemRefundPoliciesApi.md#count_item_refund_policies_async) | **GET** /api/v2/CatalogService/ItemRefundPolicies/Count | Count item refund policies |
| [**get_item_refund_policies_async**](ItemRefundPoliciesApi.md#get_item_refund_policies_async) | **GET** /api/v2/CatalogService/ItemRefundPolicies | Get item refund policies |
| [**get_item_refund_policy_by_id_async**](ItemRefundPoliciesApi.md#get_item_refund_policy_by_id_async) | **GET** /api/v2/CatalogService/ItemRefundPolicies/{itemRefundPolicyId} | Get item refund policy by ID |
| [**relate_item_to_refund_policy_async**](ItemRefundPoliciesApi.md#relate_item_to_refund_policy_async) | **POST** /api/v2/CatalogService/ItemRefundPolicies | Relate item to refund policy |
| [**remove_refund_policy_from_item_async**](ItemRefundPoliciesApi.md#remove_refund_policy_from_item_async) | **DELETE** /api/v2/CatalogService/ItemRefundPolicies/{itemRefundPolicyId} | Remove refund policy from item |


## count_item_refund_policies_async

> <Int32Envelope> count_item_refund_policies_async(opts)

Count item refund policies

Counts all refund policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRefundPoliciesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count item refund policies
  result = api_instance.count_item_refund_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->count_item_refund_policies_async: #{e}"
end
```

#### Using the count_item_refund_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_item_refund_policies_async_with_http_info(opts)

```ruby
begin
  # Count item refund policies
  data, status_code, headers = api_instance.count_item_refund_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->count_item_refund_policies_async_with_http_info: #{e}"
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


## get_item_refund_policies_async

> <ItemRefundPolicyDtoListEnvelope> get_item_refund_policies_async(opts)

Get item refund policies

Retrieves all refund policies for a specific item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRefundPoliciesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item refund policies
  result = api_instance.get_item_refund_policies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->get_item_refund_policies_async: #{e}"
end
```

#### Using the get_item_refund_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRefundPolicyDtoListEnvelope>, Integer, Hash)> get_item_refund_policies_async_with_http_info(opts)

```ruby
begin
  # Get item refund policies
  data, status_code, headers = api_instance.get_item_refund_policies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRefundPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->get_item_refund_policies_async_with_http_info: #{e}"
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

[**ItemRefundPolicyDtoListEnvelope**](ItemRefundPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_refund_policy_by_id_async

> <ItemRefundPolicyDtoEnvelope> get_item_refund_policy_by_id_async(item_refund_policy_id, opts)

Get item refund policy by ID

Retrieves a specific refund policy for an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRefundPoliciesApi.new
item_refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item refund policy by ID
  result = api_instance.get_item_refund_policy_by_id_async(item_refund_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->get_item_refund_policy_by_id_async: #{e}"
end
```

#### Using the get_item_refund_policy_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRefundPolicyDtoEnvelope>, Integer, Hash)> get_item_refund_policy_by_id_async_with_http_info(item_refund_policy_id, opts)

```ruby
begin
  # Get item refund policy by ID
  data, status_code, headers = api_instance.get_item_refund_policy_by_id_async_with_http_info(item_refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRefundPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->get_item_refund_policy_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_refund_policy_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **item_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRefundPolicyDtoEnvelope**](ItemRefundPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_item_to_refund_policy_async

> relate_item_to_refund_policy_async(tenant_id, item_id, refund_policy_id, opts)

Relate item to refund policy

Relates an item to an existing refund policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRefundPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate item to refund policy
  api_instance.relate_item_to_refund_policy_async(tenant_id, item_id, refund_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->relate_item_to_refund_policy_async: #{e}"
end
```

#### Using the relate_item_to_refund_policy_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> relate_item_to_refund_policy_async_with_http_info(tenant_id, item_id, refund_policy_id, opts)

```ruby
begin
  # Relate item to refund policy
  data, status_code, headers = api_instance.relate_item_to_refund_policy_async_with_http_info(tenant_id, item_id, refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->relate_item_to_refund_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **refund_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_refund_policy_from_item_async

> remove_refund_policy_from_item_async(tenant_id, item_id, item_refund_policy_id, opts)

Remove refund policy from item

Removes a refund policy from an item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRefundPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove refund policy from item
  api_instance.remove_refund_policy_from_item_async(tenant_id, item_id, item_refund_policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->remove_refund_policy_from_item_async: #{e}"
end
```

#### Using the remove_refund_policy_from_item_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> remove_refund_policy_from_item_async_with_http_info(tenant_id, item_id, item_refund_policy_id, opts)

```ruby
begin
  # Remove refund policy from item
  data, status_code, headers = api_instance.remove_refund_policy_from_item_async_with_http_info(tenant_id, item_id, item_refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRefundPoliciesApi->remove_refund_policy_from_item_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_refund_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

