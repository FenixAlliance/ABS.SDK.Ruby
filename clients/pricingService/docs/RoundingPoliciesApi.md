# OpenapiClient::RoundingPoliciesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_rounding_policy_async**](RoundingPoliciesApi.md#create_rounding_policy_async) | **POST** /api/v2/PricingService/RoundingPolicies | Creates a rounding policy |
| [**delete_rounding_policy_async**](RoundingPoliciesApi.md#delete_rounding_policy_async) | **DELETE** /api/v2/PricingService/RoundingPolicies/{roundingPolicyId} | Deletes a rounding policy |
| [**get_rounding_policies_async**](RoundingPoliciesApi.md#get_rounding_policies_async) | **GET** /api/v2/PricingService/RoundingPolicies | Gets all rounding policies |
| [**get_rounding_policies_count_async**](RoundingPoliciesApi.md#get_rounding_policies_count_async) | **GET** /api/v2/PricingService/RoundingPolicies/Count | Counts rounding policies |
| [**get_rounding_policy_by_id_async**](RoundingPoliciesApi.md#get_rounding_policy_by_id_async) | **GET** /api/v2/PricingService/RoundingPolicies/{roundingPolicyId} | Gets a rounding policy by ID |
| [**patch_rounding_policy_async**](RoundingPoliciesApi.md#patch_rounding_policy_async) | **PATCH** /api/v2/PricingService/RoundingPolicies/{roundingPolicyId} | Patches a rounding policy |
| [**update_rounding_policy_async**](RoundingPoliciesApi.md#update_rounding_policy_async) | **PUT** /api/v2/PricingService/RoundingPolicies/{roundingPolicyId} | Updates a rounding policy |


## create_rounding_policy_async

> <EmptyEnvelope> create_rounding_policy_async(tenant_id, rounding_policy_create_dto, opts)

Creates a rounding policy

Creates a new rounding policy for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoundingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
rounding_policy_create_dto = OpenapiClient::RoundingPolicyCreateDto.new # RoundingPolicyCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Creates a rounding policy
  result = api_instance.create_rounding_policy_async(tenant_id, rounding_policy_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->create_rounding_policy_async: #{e}"
end
```

#### Using the create_rounding_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_rounding_policy_async_with_http_info(tenant_id, rounding_policy_create_dto, opts)

```ruby
begin
  # Creates a rounding policy
  data, status_code, headers = api_instance.create_rounding_policy_async_with_http_info(tenant_id, rounding_policy_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->create_rounding_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **rounding_policy_create_dto** | [**RoundingPolicyCreateDto**](RoundingPolicyCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_rounding_policy_async

> <EmptyEnvelope> delete_rounding_policy_async(tenant_id, rounding_policy_id, opts)

Deletes a rounding policy

Deletes the specified rounding policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoundingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
rounding_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a rounding policy
  result = api_instance.delete_rounding_policy_async(tenant_id, rounding_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->delete_rounding_policy_async: #{e}"
end
```

#### Using the delete_rounding_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_rounding_policy_async_with_http_info(tenant_id, rounding_policy_id, opts)

```ruby
begin
  # Deletes a rounding policy
  data, status_code, headers = api_instance.delete_rounding_policy_async_with_http_info(tenant_id, rounding_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->delete_rounding_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **rounding_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_rounding_policies_async

> <RoundingPolicyDtoListEnvelope> get_rounding_policies_async(tenant_id, opts)

Gets all rounding policies

Retrieves all rounding policies for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoundingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets all rounding policies
  result = api_instance.get_rounding_policies_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->get_rounding_policies_async: #{e}"
end
```

#### Using the get_rounding_policies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RoundingPolicyDtoListEnvelope>, Integer, Hash)> get_rounding_policies_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets all rounding policies
  data, status_code, headers = api_instance.get_rounding_policies_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RoundingPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->get_rounding_policies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RoundingPolicyDtoListEnvelope**](RoundingPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_rounding_policies_count_async

> <Int32Envelope> get_rounding_policies_count_async(tenant_id, opts)

Counts rounding policies

Gets the count of rounding policies for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoundingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts rounding policies
  result = api_instance.get_rounding_policies_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->get_rounding_policies_count_async: #{e}"
end
```

#### Using the get_rounding_policies_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_rounding_policies_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts rounding policies
  data, status_code, headers = api_instance.get_rounding_policies_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->get_rounding_policies_count_async_with_http_info: #{e}"
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


## get_rounding_policy_by_id_async

> <RoundingPolicyDtoEnvelope> get_rounding_policy_by_id_async(tenant_id, rounding_policy_id, opts)

Gets a rounding policy by ID

Retrieves the details of a rounding policy using its unique ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoundingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
rounding_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a rounding policy by ID
  result = api_instance.get_rounding_policy_by_id_async(tenant_id, rounding_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->get_rounding_policy_by_id_async: #{e}"
end
```

#### Using the get_rounding_policy_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RoundingPolicyDtoEnvelope>, Integer, Hash)> get_rounding_policy_by_id_async_with_http_info(tenant_id, rounding_policy_id, opts)

```ruby
begin
  # Gets a rounding policy by ID
  data, status_code, headers = api_instance.get_rounding_policy_by_id_async_with_http_info(tenant_id, rounding_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RoundingPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->get_rounding_policy_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **rounding_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RoundingPolicyDtoEnvelope**](RoundingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_rounding_policy_async

> <EmptyEnvelope> patch_rounding_policy_async(tenant_id, rounding_policy_id, opts)

Patches a rounding policy

Partially updates the specified rounding policy using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoundingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
rounding_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a rounding policy
  result = api_instance.patch_rounding_policy_async(tenant_id, rounding_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->patch_rounding_policy_async: #{e}"
end
```

#### Using the patch_rounding_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_rounding_policy_async_with_http_info(tenant_id, rounding_policy_id, opts)

```ruby
begin
  # Patches a rounding policy
  data, status_code, headers = api_instance.patch_rounding_policy_async_with_http_info(tenant_id, rounding_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->patch_rounding_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **rounding_policy_id** | **String** |  |  |
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


## update_rounding_policy_async

> <EmptyEnvelope> update_rounding_policy_async(tenant_id, rounding_policy_id, rounding_policy_update_dto, opts)

Updates a rounding policy

Updates the specified rounding policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RoundingPoliciesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
rounding_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
rounding_policy_update_dto = OpenapiClient::RoundingPolicyUpdateDto.new # RoundingPolicyUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Updates a rounding policy
  result = api_instance.update_rounding_policy_async(tenant_id, rounding_policy_id, rounding_policy_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->update_rounding_policy_async: #{e}"
end
```

#### Using the update_rounding_policy_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_rounding_policy_async_with_http_info(tenant_id, rounding_policy_id, rounding_policy_update_dto, opts)

```ruby
begin
  # Updates a rounding policy
  data, status_code, headers = api_instance.update_rounding_policy_async_with_http_info(tenant_id, rounding_policy_id, rounding_policy_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RoundingPoliciesApi->update_rounding_policy_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **rounding_policy_id** | **String** |  |  |
| **rounding_policy_update_dto** | [**RoundingPolicyUpdateDto**](RoundingPolicyUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

