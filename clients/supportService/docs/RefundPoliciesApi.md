# OpenapiClient::RefundPoliciesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_refund_policy_async**](RefundPoliciesApi.md#create_refund_policy_async) | **POST** /api/v2/SupportService/RefundPolicies | Create a new refund policy |
| [**delete_refund_policy_async**](RefundPoliciesApi.md#delete_refund_policy_async) | **DELETE** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Delete a refund policy |
| [**get_refund_policies_async**](RefundPoliciesApi.md#get_refund_policies_async) | **GET** /api/v2/SupportService/RefundPolicies | Retrieve a list of refund policies |
| [**get_refund_policies_count_async**](RefundPoliciesApi.md#get_refund_policies_count_async) | **GET** /api/v2/SupportService/RefundPolicies/Count | Get the count of refund policies |
| [**get_refund_policy_async**](RefundPoliciesApi.md#get_refund_policy_async) | **GET** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Retrieve a refund policy by ID |
| [**patch_refund_policy_async**](RefundPoliciesApi.md#patch_refund_policy_async) | **PATCH** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Patch a refund policy |
| [**update_refund_policy_async**](RefundPoliciesApi.md#update_refund_policy_async) | **PUT** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Update a refund policy |


## create_refund_policy_async

> <EmptyEnvelope> create_refund_policy_async(tenant_id, opts)

Create a new refund policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_refund_policy_create_dto: OpenapiClient::ItemRefundPolicyCreateDto.new({title: 'title_example'}) # ItemRefundPolicyCreateDto | 
}

begin
  # Create a new refund policy
  result = api_instance.create_refund_policy_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->create_refund_policy_async: #{e}"
end
```

#### Using the create_refund_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_refund_policy_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new refund policy
  data, status_code, headers = api_instance.create_refund_policy_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->create_refund_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_refund_policy_create_dto** | [**ItemRefundPolicyCreateDto**](ItemRefundPolicyCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_refund_policy_async

> <EmptyEnvelope> delete_refund_policy_async(tenant_id, refund_policy_id, opts)

Delete a refund policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a refund policy
  result = api_instance.delete_refund_policy_async(tenant_id, refund_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->delete_refund_policy_async: #{e}"
end
```

#### Using the delete_refund_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_refund_policy_async_with_http_info(tenant_id, refund_policy_id, opts)

```ruby
begin
  # Delete a refund policy
  data, status_code, headers = api_instance.delete_refund_policy_async_with_http_info(tenant_id, refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->delete_refund_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_refund_policies_async

> <ItemRefundPolicyDtoListEnvelope> get_refund_policies_async(tenant_id, opts)

Retrieve a list of refund policies

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of refund policies
  result = api_instance.get_refund_policies_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->get_refund_policies_async: #{e}"
end
```

#### Using the get_refund_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRefundPolicyDtoListEnvelope>, Integer, Hash)> get_refund_policies_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of refund policies
  data, status_code, headers = api_instance.get_refund_policies_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRefundPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->get_refund_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRefundPolicyDtoListEnvelope**](ItemRefundPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_refund_policies_count_async

> <Int32Envelope> get_refund_policies_count_async(tenant_id, opts)

Get the count of refund policies

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of refund policies
  result = api_instance.get_refund_policies_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->get_refund_policies_count_async: #{e}"
end
```

#### Using the get_refund_policies_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_refund_policies_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of refund policies
  data, status_code, headers = api_instance.get_refund_policies_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->get_refund_policies_count_async_with_http_info: #{e}"
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


## get_refund_policy_async

> <ItemRefundPolicyDtoEnvelope> get_refund_policy_async(tenant_id, refund_policy_id, opts)

Retrieve a refund policy by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a refund policy by ID
  result = api_instance.get_refund_policy_async(tenant_id, refund_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->get_refund_policy_async: #{e}"
end
```

#### Using the get_refund_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRefundPolicyDtoEnvelope>, Integer, Hash)> get_refund_policy_async_with_http_info(tenant_id, refund_policy_id, opts)

```ruby
begin
  # Retrieve a refund policy by ID
  data, status_code, headers = api_instance.get_refund_policy_async_with_http_info(tenant_id, refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRefundPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->get_refund_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRefundPolicyDtoEnvelope**](ItemRefundPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_refund_policy_async

> <EmptyEnvelope> patch_refund_policy_async(tenant_id, refund_policy_id, opts)

Patch a refund policy

Partially updates an existing refund policy by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a refund policy
  result = api_instance.patch_refund_policy_async(tenant_id, refund_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->patch_refund_policy_async: #{e}"
end
```

#### Using the patch_refund_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_refund_policy_async_with_http_info(tenant_id, refund_policy_id, opts)

```ruby
begin
  # Patch a refund policy
  data, status_code, headers = api_instance.patch_refund_policy_async_with_http_info(tenant_id, refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->patch_refund_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_refund_policy_async

> <EmptyEnvelope> update_refund_policy_async(tenant_id, refund_policy_id, opts)

Update a refund policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RefundPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_refund_policy_update_dto: OpenapiClient::ItemRefundPolicyUpdateDto.new # ItemRefundPolicyUpdateDto | 
}

begin
  # Update a refund policy
  result = api_instance.update_refund_policy_async(tenant_id, refund_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->update_refund_policy_async: #{e}"
end
```

#### Using the update_refund_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_refund_policy_async_with_http_info(tenant_id, refund_policy_id, opts)

```ruby
begin
  # Update a refund policy
  data, status_code, headers = api_instance.update_refund_policy_async_with_http_info(tenant_id, refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RefundPoliciesApi->update_refund_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_refund_policy_update_dto** | [**ItemRefundPolicyUpdateDto**](ItemRefundPolicyUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

