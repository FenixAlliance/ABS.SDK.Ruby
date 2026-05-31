# OpenapiClient::ReturnPoliciesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_return_policy_async**](ReturnPoliciesApi.md#create_return_policy_async) | **POST** /api/v2/SupportService/ReturnPolicies | Create a new return policy |
| [**delete_return_policy_async**](ReturnPoliciesApi.md#delete_return_policy_async) | **DELETE** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Delete a return policy |
| [**get_return_policies_async**](ReturnPoliciesApi.md#get_return_policies_async) | **GET** /api/v2/SupportService/ReturnPolicies | Retrieve a list of return policies |
| [**get_return_policies_count_async**](ReturnPoliciesApi.md#get_return_policies_count_async) | **GET** /api/v2/SupportService/ReturnPolicies/Count | Get the count of return policies |
| [**get_return_policy_async**](ReturnPoliciesApi.md#get_return_policy_async) | **GET** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Retrieve a return policy by ID |
| [**update_return_policy_async**](ReturnPoliciesApi.md#update_return_policy_async) | **PUT** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Update a return policy |


## create_return_policy_async

> <EmptyEnvelope> create_return_policy_async(tenant_id, opts)

Create a new return policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_return_policy_create_dto: OpenapiClient::ItemReturnPolicyCreateDto.new({title: 'title_example'}) # ItemReturnPolicyCreateDto | 
}

begin
  # Create a new return policy
  result = api_instance.create_return_policy_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->create_return_policy_async: #{e}"
end
```

#### Using the create_return_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_return_policy_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new return policy
  data, status_code, headers = api_instance.create_return_policy_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->create_return_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_return_policy_create_dto** | [**ItemReturnPolicyCreateDto**](ItemReturnPolicyCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_return_policy_async

> <EmptyEnvelope> delete_return_policy_async(tenant_id, return_policy_id, opts)

Delete a return policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a return policy
  result = api_instance.delete_return_policy_async(tenant_id, return_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->delete_return_policy_async: #{e}"
end
```

#### Using the delete_return_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_return_policy_async_with_http_info(tenant_id, return_policy_id, opts)

```ruby
begin
  # Delete a return policy
  data, status_code, headers = api_instance.delete_return_policy_async_with_http_info(tenant_id, return_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->delete_return_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **return_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_return_policies_async

> <ItemReturnPolicyDtoListEnvelope> get_return_policies_async(tenant_id, opts)

Retrieve a list of return policies

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of return policies
  result = api_instance.get_return_policies_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->get_return_policies_async: #{e}"
end
```

#### Using the get_return_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReturnPolicyDtoListEnvelope>, Integer, Hash)> get_return_policies_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of return policies
  data, status_code, headers = api_instance.get_return_policies_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReturnPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->get_return_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReturnPolicyDtoListEnvelope**](ItemReturnPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_return_policies_count_async

> <Int32Envelope> get_return_policies_count_async(tenant_id, opts)

Get the count of return policies

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of return policies
  result = api_instance.get_return_policies_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->get_return_policies_count_async: #{e}"
end
```

#### Using the get_return_policies_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_return_policies_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of return policies
  data, status_code, headers = api_instance.get_return_policies_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->get_return_policies_count_async_with_http_info: #{e}"
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


## get_return_policy_async

> <ItemReturnPolicyDtoEnvelope> get_return_policy_async(tenant_id, return_policy_id, opts)

Retrieve a return policy by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a return policy by ID
  result = api_instance.get_return_policy_async(tenant_id, return_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->get_return_policy_async: #{e}"
end
```

#### Using the get_return_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReturnPolicyDtoEnvelope>, Integer, Hash)> get_return_policy_async_with_http_info(tenant_id, return_policy_id, opts)

```ruby
begin
  # Retrieve a return policy by ID
  data, status_code, headers = api_instance.get_return_policy_async_with_http_info(tenant_id, return_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReturnPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->get_return_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **return_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReturnPolicyDtoEnvelope**](ItemReturnPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_return_policy_async

> <EmptyEnvelope> update_return_policy_async(tenant_id, return_policy_id, opts)

Update a return policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReturnPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_return_policy_update_dto: OpenapiClient::ItemReturnPolicyUpdateDto.new # ItemReturnPolicyUpdateDto | 
}

begin
  # Update a return policy
  result = api_instance.update_return_policy_async(tenant_id, return_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->update_return_policy_async: #{e}"
end
```

#### Using the update_return_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_return_policy_async_with_http_info(tenant_id, return_policy_id, opts)

```ruby
begin
  # Update a return policy
  data, status_code, headers = api_instance.update_return_policy_async_with_http_info(tenant_id, return_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReturnPoliciesApi->update_return_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **return_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_return_policy_update_dto** | [**ItemReturnPolicyUpdateDto**](ItemReturnPolicyUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

