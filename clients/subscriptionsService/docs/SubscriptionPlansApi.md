# OpenapiClient::SubscriptionPlansApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_subscription_plan_async**](SubscriptionPlansApi.md#create_subscription_plan_async) | **POST** /api/v2/SubscriptionsService/SubscriptionPlans | Create a subscription plan |
| [**delete_subscription_plan_async**](SubscriptionPlansApi.md#delete_subscription_plan_async) | **DELETE** /api/v2/SubscriptionsService/SubscriptionPlans/{planId} | Delete a subscription plan |
| [**get_subscription_plan_by_id_async**](SubscriptionPlansApi.md#get_subscription_plan_by_id_async) | **GET** /api/v2/SubscriptionsService/SubscriptionPlans/{planId} | Get a subscription plan by ID |
| [**get_subscription_plans_async**](SubscriptionPlansApi.md#get_subscription_plans_async) | **GET** /api/v2/SubscriptionsService/SubscriptionPlans | Get all subscription plans |
| [**get_subscription_plans_count_async**](SubscriptionPlansApi.md#get_subscription_plans_count_async) | **GET** /api/v2/SubscriptionsService/SubscriptionPlans/Count | Get subscription plans count |
| [**patch_subscription_plan_async**](SubscriptionPlansApi.md#patch_subscription_plan_async) | **PATCH** /api/v2/SubscriptionsService/SubscriptionPlans/{planId} | Patch a subscription plan |
| [**update_subscription_plan_async**](SubscriptionPlansApi.md#update_subscription_plan_async) | **PUT** /api/v2/SubscriptionsService/SubscriptionPlans/{planId} | Update a subscription plan |


## create_subscription_plan_async

> <Envelope> create_subscription_plan_async(tenant_id, opts)

Create a subscription plan

Creates a new subscription plan for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  subscription_plan_create_dto: OpenapiClient::SubscriptionPlanCreateDto.new # SubscriptionPlanCreateDto | 
}

begin
  # Create a subscription plan
  result = api_instance.create_subscription_plan_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->create_subscription_plan_async: #{e}"
end
```

#### Using the create_subscription_plan_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> create_subscription_plan_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a subscription plan
  data, status_code, headers = api_instance.create_subscription_plan_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->create_subscription_plan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **subscription_plan_create_dto** | [**SubscriptionPlanCreateDto**](SubscriptionPlanCreateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_subscription_plan_async

> <Envelope> delete_subscription_plan_async(tenant_id, plan_id, opts)

Delete a subscription plan

Deletes a subscription plan by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
plan_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a subscription plan
  result = api_instance.delete_subscription_plan_async(tenant_id, plan_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->delete_subscription_plan_async: #{e}"
end
```

#### Using the delete_subscription_plan_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> delete_subscription_plan_async_with_http_info(tenant_id, plan_id, opts)

```ruby
begin
  # Delete a subscription plan
  data, status_code, headers = api_instance.delete_subscription_plan_async_with_http_info(tenant_id, plan_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->delete_subscription_plan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **plan_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_subscription_plan_by_id_async

> <SubscriptionPlanDtoEnvelope> get_subscription_plan_by_id_async(tenant_id, plan_id, opts)

Get a subscription plan by ID

Retrieves a subscription plan by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
plan_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a subscription plan by ID
  result = api_instance.get_subscription_plan_by_id_async(tenant_id, plan_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->get_subscription_plan_by_id_async: #{e}"
end
```

#### Using the get_subscription_plan_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SubscriptionPlanDtoEnvelope>, Integer, Hash)> get_subscription_plan_by_id_async_with_http_info(tenant_id, plan_id, opts)

```ruby
begin
  # Get a subscription plan by ID
  data, status_code, headers = api_instance.get_subscription_plan_by_id_async_with_http_info(tenant_id, plan_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SubscriptionPlanDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->get_subscription_plan_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **plan_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SubscriptionPlanDtoEnvelope**](SubscriptionPlanDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_subscription_plans_async

> <SubscriptionPlanDtoIReadOnlyListEnvelope> get_subscription_plans_async(tenant_id, opts)

Get all subscription plans

Retrieves all subscription plans for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  subscription_dto_collection_query_parameters: OpenapiClient::SubscriptionDtoCollectionQueryParameters.new # SubscriptionDtoCollectionQueryParameters | 
}

begin
  # Get all subscription plans
  result = api_instance.get_subscription_plans_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->get_subscription_plans_async: #{e}"
end
```

#### Using the get_subscription_plans_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SubscriptionPlanDtoIReadOnlyListEnvelope>, Integer, Hash)> get_subscription_plans_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all subscription plans
  data, status_code, headers = api_instance.get_subscription_plans_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SubscriptionPlanDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->get_subscription_plans_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **subscription_dto_collection_query_parameters** | [**SubscriptionDtoCollectionQueryParameters**](SubscriptionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SubscriptionPlanDtoIReadOnlyListEnvelope**](SubscriptionPlanDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_subscription_plans_count_async

> <Int32Envelope> get_subscription_plans_count_async(tenant_id, opts)

Get subscription plans count

Returns the count of subscription plans for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  subscription_dto_collection_query_parameters: OpenapiClient::SubscriptionDtoCollectionQueryParameters.new # SubscriptionDtoCollectionQueryParameters | 
}

begin
  # Get subscription plans count
  result = api_instance.get_subscription_plans_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->get_subscription_plans_count_async: #{e}"
end
```

#### Using the get_subscription_plans_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_subscription_plans_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get subscription plans count
  data, status_code, headers = api_instance.get_subscription_plans_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->get_subscription_plans_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **subscription_dto_collection_query_parameters** | [**SubscriptionDtoCollectionQueryParameters**](SubscriptionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_subscription_plan_async

> <EmptyEnvelope> patch_subscription_plan_async(tenant_id, plan_id, opts)

Patch a subscription plan

Patch a subscription plan

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
plan_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a subscription plan
  result = api_instance.patch_subscription_plan_async(tenant_id, plan_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->patch_subscription_plan_async: #{e}"
end
```

#### Using the patch_subscription_plan_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_subscription_plan_async_with_http_info(tenant_id, plan_id, opts)

```ruby
begin
  # Patch a subscription plan
  data, status_code, headers = api_instance.patch_subscription_plan_async_with_http_info(tenant_id, plan_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->patch_subscription_plan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **plan_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_subscription_plan_async

> <Envelope> update_subscription_plan_async(tenant_id, plan_id, opts)

Update a subscription plan

Updates an existing subscription plan.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
plan_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  subscription_plan_update_dto: OpenapiClient::SubscriptionPlanUpdateDto.new # SubscriptionPlanUpdateDto | 
}

begin
  # Update a subscription plan
  result = api_instance.update_subscription_plan_async(tenant_id, plan_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->update_subscription_plan_async: #{e}"
end
```

#### Using the update_subscription_plan_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> update_subscription_plan_async_with_http_info(tenant_id, plan_id, opts)

```ruby
begin
  # Update a subscription plan
  data, status_code, headers = api_instance.update_subscription_plan_async_with_http_info(tenant_id, plan_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionPlansApi->update_subscription_plan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **plan_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **subscription_plan_update_dto** | [**SubscriptionPlanUpdateDto**](SubscriptionPlanUpdateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

