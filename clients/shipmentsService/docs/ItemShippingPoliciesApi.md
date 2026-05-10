# OpenapiClient::ItemShippingPoliciesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_shipping_policy_async**](ItemShippingPoliciesApi.md#create_item_shipping_policy_async) | **POST** /api/v2/ShipmentsService/ItemShippingPolicies | Create an item shipping policy |
| [**delete_item_shipping_policy_async**](ItemShippingPoliciesApi.md#delete_item_shipping_policy_async) | **DELETE** /api/v2/ShipmentsService/ItemShippingPolicies/{policyId} | Delete an item shipping policy |
| [**get_item_shipping_policies_async**](ItemShippingPoliciesApi.md#get_item_shipping_policies_async) | **GET** /api/v2/ShipmentsService/ItemShippingPolicies | Get all item shipping policies |
| [**get_item_shipping_policies_count_async**](ItemShippingPoliciesApi.md#get_item_shipping_policies_count_async) | **GET** /api/v2/ShipmentsService/ItemShippingPolicies/Count | Get item shipping policies count |
| [**get_item_shipping_policy_by_id_async**](ItemShippingPoliciesApi.md#get_item_shipping_policy_by_id_async) | **GET** /api/v2/ShipmentsService/ItemShippingPolicies/{policyId} | Get item shipping policy by ID |
| [**update_item_shipping_policy_async**](ItemShippingPoliciesApi.md#update_item_shipping_policy_async) | **PUT** /api/v2/ShipmentsService/ItemShippingPolicies/{policyId} | Update an item shipping policy |


## create_item_shipping_policy_async

> create_item_shipping_policy_async(tenant_id, opts)

Create an item shipping policy

Creates a new item shipping policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_shipping_policy_create_dto: OpenapiClient::ItemShippingPolicyCreateDto.new({title: 'title_example', type: 'type_example', code: 'code_example', currency_id: 'currency_id_example', shipping_courier_id: 'shipping_courier_id_example'}) # ItemShippingPolicyCreateDto | 
}

begin
  # Create an item shipping policy
  api_instance.create_item_shipping_policy_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->create_item_shipping_policy_async: #{e}"
end
```

#### Using the create_item_shipping_policy_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_item_shipping_policy_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an item shipping policy
  data, status_code, headers = api_instance.create_item_shipping_policy_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->create_item_shipping_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_shipping_policy_create_dto** | [**ItemShippingPolicyCreateDto**](ItemShippingPolicyCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_shipping_policy_async

> delete_item_shipping_policy_async(tenant_id, policy_id, opts)

Delete an item shipping policy

Deletes an item shipping policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item shipping policy
  api_instance.delete_item_shipping_policy_async(tenant_id, policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->delete_item_shipping_policy_async: #{e}"
end
```

#### Using the delete_item_shipping_policy_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_shipping_policy_async_with_http_info(tenant_id, policy_id, opts)

```ruby
begin
  # Delete an item shipping policy
  data, status_code, headers = api_instance.delete_item_shipping_policy_async_with_http_info(tenant_id, policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->delete_item_shipping_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_shipping_policies_async

> <ItemShippingPolicyDtoListEnvelope> get_item_shipping_policies_async(tenant_id, opts)

Get all item shipping policies

Retrieves all item shipping policies for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item shipping policies
  result = api_instance.get_item_shipping_policies_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->get_item_shipping_policies_async: #{e}"
end
```

#### Using the get_item_shipping_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemShippingPolicyDtoListEnvelope>, Integer, Hash)> get_item_shipping_policies_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all item shipping policies
  data, status_code, headers = api_instance.get_item_shipping_policies_async_with_http_info(tenant_id, opts)
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
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemShippingPolicyDtoListEnvelope**](ItemShippingPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_shipping_policies_count_async

> <Int32Envelope> get_item_shipping_policies_count_async(tenant_id, opts)

Get item shipping policies count

Returns the count of item shipping policies.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item shipping policies count
  result = api_instance.get_item_shipping_policies_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->get_item_shipping_policies_count_async: #{e}"
end
```

#### Using the get_item_shipping_policies_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_shipping_policies_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get item shipping policies count
  data, status_code, headers = api_instance.get_item_shipping_policies_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->get_item_shipping_policies_count_async_with_http_info: #{e}"
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


## get_item_shipping_policy_by_id_async

> <ItemShippingPolicyDtoEnvelope> get_item_shipping_policy_by_id_async(tenant_id, policy_id, opts)

Get item shipping policy by ID

Retrieves a specific item shipping policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item shipping policy by ID
  result = api_instance.get_item_shipping_policy_by_id_async(tenant_id, policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->get_item_shipping_policy_by_id_async: #{e}"
end
```

#### Using the get_item_shipping_policy_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemShippingPolicyDtoEnvelope>, Integer, Hash)> get_item_shipping_policy_by_id_async_with_http_info(tenant_id, policy_id, opts)

```ruby
begin
  # Get item shipping policy by ID
  data, status_code, headers = api_instance.get_item_shipping_policy_by_id_async_with_http_info(tenant_id, policy_id, opts)
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
| **tenant_id** | **String** |  |  |
| **policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemShippingPolicyDtoEnvelope**](ItemShippingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_item_shipping_policy_async

> update_item_shipping_policy_async(tenant_id, policy_id, opts)

Update an item shipping policy

Updates an existing item shipping policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemShippingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_shipping_policy_update_dto: OpenapiClient::ItemShippingPolicyUpdateDto.new({title: 'title_example', type: 'type_example', code: 'code_example', currency_id: 'currency_id_example', shipping_courier_id: 'shipping_courier_id_example'}) # ItemShippingPolicyUpdateDto | 
}

begin
  # Update an item shipping policy
  api_instance.update_item_shipping_policy_async(tenant_id, policy_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->update_item_shipping_policy_async: #{e}"
end
```

#### Using the update_item_shipping_policy_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_item_shipping_policy_async_with_http_info(tenant_id, policy_id, opts)

```ruby
begin
  # Update an item shipping policy
  data, status_code, headers = api_instance.update_item_shipping_policy_async_with_http_info(tenant_id, policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemShippingPoliciesApi->update_item_shipping_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_shipping_policy_update_dto** | [**ItemShippingPolicyUpdateDto**](ItemShippingPolicyUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

