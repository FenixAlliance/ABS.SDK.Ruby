# OpenapiClient::PoliciesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_refund_policy_async**](PoliciesApi.md#create_refund_policy_async) | **POST** /api/v2/SupportService/RefundPolicies | Create a new refund policy |
| [**create_return_policy_async**](PoliciesApi.md#create_return_policy_async) | **POST** /api/v2/SupportService/ReturnPolicies | Create a new return policy |
| [**create_warranty_policy_async**](PoliciesApi.md#create_warranty_policy_async) | **POST** /api/v2/SupportService/WarrantyPolicies | Create a new warranty policy |
| [**delete_refund_policy_async**](PoliciesApi.md#delete_refund_policy_async) | **DELETE** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Delete a refund policy |
| [**delete_return_policy_async**](PoliciesApi.md#delete_return_policy_async) | **DELETE** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Delete a return policy |
| [**delete_warranty_policy_async**](PoliciesApi.md#delete_warranty_policy_async) | **DELETE** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Delete a warranty policy |
| [**get_refund_policies_async**](PoliciesApi.md#get_refund_policies_async) | **GET** /api/v2/SupportService/RefundPolicies | Retrieve a list of refund policies |
| [**get_refund_policies_count_async**](PoliciesApi.md#get_refund_policies_count_async) | **GET** /api/v2/SupportService/RefundPolicies/Count | Get the count of refund policies |
| [**get_refund_policy_async**](PoliciesApi.md#get_refund_policy_async) | **GET** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Retrieve a refund policy by ID |
| [**get_return_policies_async**](PoliciesApi.md#get_return_policies_async) | **GET** /api/v2/SupportService/ReturnPolicies | Retrieve a list of return policies |
| [**get_return_policies_count_async**](PoliciesApi.md#get_return_policies_count_async) | **GET** /api/v2/SupportService/ReturnPolicies/Count | Get the count of return policies |
| [**get_return_policy_async**](PoliciesApi.md#get_return_policy_async) | **GET** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Retrieve a return policy by ID |
| [**get_warranty_policies_async**](PoliciesApi.md#get_warranty_policies_async) | **GET** /api/v2/SupportService/WarrantyPolicies | Retrieve a list of warranty policies |
| [**get_warranty_policies_count_async**](PoliciesApi.md#get_warranty_policies_count_async) | **GET** /api/v2/SupportService/WarrantyPolicies/Count | Get the count of warranty policies |
| [**get_warranty_policy_async**](PoliciesApi.md#get_warranty_policy_async) | **GET** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Retrieve a warranty policy by ID |
| [**update_refund_policy_async**](PoliciesApi.md#update_refund_policy_async) | **PUT** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Update a refund policy |
| [**update_return_policy_async**](PoliciesApi.md#update_return_policy_async) | **PUT** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Update a return policy |
| [**update_warranty_policy_async**](PoliciesApi.md#update_warranty_policy_async) | **PUT** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Update a warranty policy |


## create_refund_policy_async

> <EmptyEnvelope> create_refund_policy_async(tenant_id, opts)

Create a new refund policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->create_refund_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->create_refund_policy_async_with_http_info: #{e}"
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


## create_return_policy_async

> <EmptyEnvelope> create_return_policy_async(tenant_id, opts)

Create a new return policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->create_return_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->create_return_policy_async_with_http_info: #{e}"
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


## create_warranty_policy_async

> <EmptyEnvelope> create_warranty_policy_async(tenant_id, opts)

Create a new warranty policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->create_warranty_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->create_warranty_policy_async_with_http_info: #{e}"
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


## delete_refund_policy_async

> <EmptyEnvelope> delete_refund_policy_async(tenant_id, refund_policy_id, opts)

Delete a refund policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->delete_refund_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->delete_refund_policy_async_with_http_info: #{e}"
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


## delete_return_policy_async

> <EmptyEnvelope> delete_return_policy_async(tenant_id, return_policy_id, opts)

Delete a return policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->delete_return_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->delete_return_policy_async_with_http_info: #{e}"
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


## delete_warranty_policy_async

> <EmptyEnvelope> delete_warranty_policy_async(tenant_id, warranty_policy_id, opts)

Delete a warranty policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->delete_warranty_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->delete_warranty_policy_async_with_http_info: #{e}"
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


## get_refund_policies_async

> <ItemRefundPolicyDtoListEnvelope> get_refund_policies_async(tenant_id, opts)

Retrieve a list of refund policies

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->get_refund_policies_async: #{e}"
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
  puts "Error when calling PoliciesApi->get_refund_policies_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->get_refund_policies_count_async: #{e}"
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
  puts "Error when calling PoliciesApi->get_refund_policies_count_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->get_refund_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->get_refund_policy_async_with_http_info: #{e}"
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


## get_return_policies_async

> <ItemReturnPolicyDtoListEnvelope> get_return_policies_async(tenant_id, opts)

Retrieve a list of return policies

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->get_return_policies_async: #{e}"
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
  puts "Error when calling PoliciesApi->get_return_policies_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->get_return_policies_count_async: #{e}"
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
  puts "Error when calling PoliciesApi->get_return_policies_count_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->get_return_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->get_return_policy_async_with_http_info: #{e}"
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


## get_warranty_policies_async

> <ItemWarrantyPolicyDtoListEnvelope> get_warranty_policies_async(tenant_id, opts)

Retrieve a list of warranty policies

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->get_warranty_policies_async: #{e}"
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
  puts "Error when calling PoliciesApi->get_warranty_policies_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->get_warranty_policies_count_async: #{e}"
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
  puts "Error when calling PoliciesApi->get_warranty_policies_count_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->get_warranty_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->get_warranty_policy_async_with_http_info: #{e}"
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


## update_refund_policy_async

> <EmptyEnvelope> update_refund_policy_async(tenant_id, refund_policy_id, opts)

Update a refund policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->update_refund_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->update_refund_policy_async_with_http_info: #{e}"
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


## update_return_policy_async

> <EmptyEnvelope> update_return_policy_async(tenant_id, return_policy_id, opts)

Update a return policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->update_return_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->update_return_policy_async_with_http_info: #{e}"
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


## update_warranty_policy_async

> <EmptyEnvelope> update_warranty_policy_async(tenant_id, warranty_policy_id, opts)

Update a warranty policy

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PoliciesApi.new
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
  puts "Error when calling PoliciesApi->update_warranty_policy_async: #{e}"
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
  puts "Error when calling PoliciesApi->update_warranty_policy_async_with_http_info: #{e}"
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

