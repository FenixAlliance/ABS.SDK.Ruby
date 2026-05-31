# OpenapiClient::WarrantyPoliciesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_warranty_policy_async**](WarrantyPoliciesApi.md#create_warranty_policy_async) | **POST** /api/v2/SupportService/WarrantyPolicies | Create a new warranty policy |
| [**delete_warranty_policy_async**](WarrantyPoliciesApi.md#delete_warranty_policy_async) | **DELETE** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Delete a warranty policy |
| [**get_warranty_policies_async**](WarrantyPoliciesApi.md#get_warranty_policies_async) | **GET** /api/v2/SupportService/WarrantyPolicies | Retrieve a list of warranty policies |
| [**get_warranty_policies_count_async**](WarrantyPoliciesApi.md#get_warranty_policies_count_async) | **GET** /api/v2/SupportService/WarrantyPolicies/Count | Get the count of warranty policies |
| [**get_warranty_policy_async**](WarrantyPoliciesApi.md#get_warranty_policy_async) | **GET** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Retrieve a warranty policy by ID |
| [**update_warranty_policy_async**](WarrantyPoliciesApi.md#update_warranty_policy_async) | **PUT** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Update a warranty policy |


## create_warranty_policy_async

> <EmptyEnvelope> create_warranty_policy_async(tenant_id, opts)

Create a new warranty policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_warranty_policy_create_dto: OpenapiClient::ItemWarrantyPolicyCreateDto.new({title: 'title_example'}) # ItemWarrantyPolicyCreateDto | 
}

begin
  # Create a new warranty policy
  result = api_instance.create_warranty_policy_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->create_warranty_policy_async: #{e}"
end
```

#### Using the create_warranty_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_warranty_policy_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new warranty policy
  data, status_code, headers = api_instance.create_warranty_policy_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->create_warranty_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_warranty_policy_create_dto** | [**ItemWarrantyPolicyCreateDto**](ItemWarrantyPolicyCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_warranty_policy_async

> <EmptyEnvelope> delete_warranty_policy_async(tenant_id, warranty_policy_id, opts)

Delete a warranty policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a warranty policy
  result = api_instance.delete_warranty_policy_async(tenant_id, warranty_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->delete_warranty_policy_async: #{e}"
end
```

#### Using the delete_warranty_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_warranty_policy_async_with_http_info(tenant_id, warranty_policy_id, opts)

```ruby
begin
  # Delete a warranty policy
  data, status_code, headers = api_instance.delete_warranty_policy_async_with_http_info(tenant_id, warranty_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->delete_warranty_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warranty_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warranty_policies_async

> <ItemWarrantyPolicyDtoListEnvelope> get_warranty_policies_async(tenant_id, opts)

Retrieve a list of warranty policies

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of warranty policies
  result = api_instance.get_warranty_policies_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->get_warranty_policies_async: #{e}"
end
```

#### Using the get_warranty_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemWarrantyPolicyDtoListEnvelope>, Integer, Hash)> get_warranty_policies_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of warranty policies
  data, status_code, headers = api_instance.get_warranty_policies_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemWarrantyPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->get_warranty_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemWarrantyPolicyDtoListEnvelope**](ItemWarrantyPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warranty_policies_count_async

> <Int32Envelope> get_warranty_policies_count_async(tenant_id, opts)

Get the count of warranty policies

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of warranty policies
  result = api_instance.get_warranty_policies_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->get_warranty_policies_count_async: #{e}"
end
```

#### Using the get_warranty_policies_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_warranty_policies_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of warranty policies
  data, status_code, headers = api_instance.get_warranty_policies_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->get_warranty_policies_count_async_with_http_info: #{e}"
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


## get_warranty_policy_async

> <ItemWarrantyPolicyDtoEnvelope> get_warranty_policy_async(tenant_id, warranty_policy_id, opts)

Retrieve a warranty policy by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a warranty policy by ID
  result = api_instance.get_warranty_policy_async(tenant_id, warranty_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->get_warranty_policy_async: #{e}"
end
```

#### Using the get_warranty_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemWarrantyPolicyDtoEnvelope>, Integer, Hash)> get_warranty_policy_async_with_http_info(tenant_id, warranty_policy_id, opts)

```ruby
begin
  # Retrieve a warranty policy by ID
  data, status_code, headers = api_instance.get_warranty_policy_async_with_http_info(tenant_id, warranty_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemWarrantyPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->get_warranty_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warranty_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemWarrantyPolicyDtoEnvelope**](ItemWarrantyPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_warranty_policy_async

> <EmptyEnvelope> update_warranty_policy_async(tenant_id, warranty_policy_id, opts)

Update a warranty policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarrantyPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_warranty_policy_update_dto: OpenapiClient::ItemWarrantyPolicyUpdateDto.new # ItemWarrantyPolicyUpdateDto | 
}

begin
  # Update a warranty policy
  result = api_instance.update_warranty_policy_async(tenant_id, warranty_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->update_warranty_policy_async: #{e}"
end
```

#### Using the update_warranty_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_warranty_policy_async_with_http_info(tenant_id, warranty_policy_id, opts)

```ruby
begin
  # Update a warranty policy
  data, status_code, headers = api_instance.update_warranty_policy_async_with_http_info(tenant_id, warranty_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarrantyPoliciesApi->update_warranty_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warranty_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_warranty_policy_update_dto** | [**ItemWarrantyPolicyUpdateDto**](ItemWarrantyPolicyUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

