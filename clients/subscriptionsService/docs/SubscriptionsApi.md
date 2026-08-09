# OpenapiClient::SubscriptionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_subscription_async**](SubscriptionsApi.md#create_subscription_async) | **POST** /api/v2/SubscriptionsService/Subscriptions | Create a subscription |
| [**delete_subscription_async**](SubscriptionsApi.md#delete_subscription_async) | **DELETE** /api/v2/SubscriptionsService/Subscriptions/{subscriptionId} | Delete a subscription |
| [**get_subscription_by_id_async**](SubscriptionsApi.md#get_subscription_by_id_async) | **GET** /api/v2/SubscriptionsService/Subscriptions/{subscriptionId} | Get a subscription by ID |
| [**get_subscriptions_async**](SubscriptionsApi.md#get_subscriptions_async) | **GET** /api/v2/SubscriptionsService/Subscriptions | Get all subscriptions |
| [**get_subscriptions_count_async**](SubscriptionsApi.md#get_subscriptions_count_async) | **GET** /api/v2/SubscriptionsService/Subscriptions/Count | Get subscriptions count |
| [**patch_subscription_async**](SubscriptionsApi.md#patch_subscription_async) | **PATCH** /api/v2/SubscriptionsService/Subscriptions/{subscriptionId} | Patch a subscription |
| [**update_subscription_async**](SubscriptionsApi.md#update_subscription_async) | **PUT** /api/v2/SubscriptionsService/Subscriptions/{subscriptionId} | Update a subscription |


## create_subscription_async

> <Envelope> create_subscription_async(tenant_id, opts)

Create a subscription

Creates a new subscription for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  subscription_create_dto: OpenapiClient::SubscriptionCreateDto.new # SubscriptionCreateDto | 
}

begin
  # Create a subscription
  result = api_instance.create_subscription_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->create_subscription_async: #{e}"
end
```

#### Using the create_subscription_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> create_subscription_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a subscription
  data, status_code, headers = api_instance.create_subscription_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->create_subscription_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **subscription_create_dto** | [**SubscriptionCreateDto**](SubscriptionCreateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_subscription_async

> <Envelope> delete_subscription_async(tenant_id, subscription_id, opts)

Delete a subscription

Deletes a subscription by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
subscription_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a subscription
  result = api_instance.delete_subscription_async(tenant_id, subscription_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->delete_subscription_async: #{e}"
end
```

#### Using the delete_subscription_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> delete_subscription_async_with_http_info(tenant_id, subscription_id, opts)

```ruby
begin
  # Delete a subscription
  data, status_code, headers = api_instance.delete_subscription_async_with_http_info(tenant_id, subscription_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->delete_subscription_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **subscription_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_subscription_by_id_async

> <SubscriptionDtoEnvelope> get_subscription_by_id_async(tenant_id, subscription_id, opts)

Get a subscription by ID

Retrieves a subscription by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
subscription_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a subscription by ID
  result = api_instance.get_subscription_by_id_async(tenant_id, subscription_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->get_subscription_by_id_async: #{e}"
end
```

#### Using the get_subscription_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SubscriptionDtoEnvelope>, Integer, Hash)> get_subscription_by_id_async_with_http_info(tenant_id, subscription_id, opts)

```ruby
begin
  # Get a subscription by ID
  data, status_code, headers = api_instance.get_subscription_by_id_async_with_http_info(tenant_id, subscription_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SubscriptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->get_subscription_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **subscription_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SubscriptionDtoEnvelope**](SubscriptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_subscriptions_async

> <SubscriptionDtoIReadOnlyListEnvelope> get_subscriptions_async(tenant_id, opts)

Get all subscriptions

Retrieves all subscriptions for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  subscription_dto_collection_query_parameters: OpenapiClient::SubscriptionDtoCollectionQueryParameters.new # SubscriptionDtoCollectionQueryParameters | 
}

begin
  # Get all subscriptions
  result = api_instance.get_subscriptions_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->get_subscriptions_async: #{e}"
end
```

#### Using the get_subscriptions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SubscriptionDtoIReadOnlyListEnvelope>, Integer, Hash)> get_subscriptions_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all subscriptions
  data, status_code, headers = api_instance.get_subscriptions_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SubscriptionDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->get_subscriptions_async_with_http_info: #{e}"
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

[**SubscriptionDtoIReadOnlyListEnvelope**](SubscriptionDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_subscriptions_count_async

> <Int32Envelope> get_subscriptions_count_async(tenant_id, opts)

Get subscriptions count

Returns the count of subscriptions for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  subscription_dto_collection_query_parameters: OpenapiClient::SubscriptionDtoCollectionQueryParameters.new # SubscriptionDtoCollectionQueryParameters | 
}

begin
  # Get subscriptions count
  result = api_instance.get_subscriptions_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->get_subscriptions_count_async: #{e}"
end
```

#### Using the get_subscriptions_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_subscriptions_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get subscriptions count
  data, status_code, headers = api_instance.get_subscriptions_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->get_subscriptions_count_async_with_http_info: #{e}"
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


## patch_subscription_async

> <EmptyEnvelope> patch_subscription_async(tenant_id, subscription_id, opts)

Patch a subscription

Patch a subscription

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
subscription_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a subscription
  result = api_instance.patch_subscription_async(tenant_id, subscription_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->patch_subscription_async: #{e}"
end
```

#### Using the patch_subscription_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_subscription_async_with_http_info(tenant_id, subscription_id, opts)

```ruby
begin
  # Patch a subscription
  data, status_code, headers = api_instance.patch_subscription_async_with_http_info(tenant_id, subscription_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->patch_subscription_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **subscription_id** | **String** |  |  |
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


## update_subscription_async

> <Envelope> update_subscription_async(tenant_id, subscription_id, opts)

Update a subscription

Updates an existing subscription.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
subscription_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  subscription_update_dto: OpenapiClient::SubscriptionUpdateDto.new # SubscriptionUpdateDto | 
}

begin
  # Update a subscription
  result = api_instance.update_subscription_async(tenant_id, subscription_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->update_subscription_async: #{e}"
end
```

#### Using the update_subscription_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> update_subscription_async_with_http_info(tenant_id, subscription_id, opts)

```ruby
begin
  # Update a subscription
  data, status_code, headers = api_instance.update_subscription_async_with_http_info(tenant_id, subscription_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SubscriptionsApi->update_subscription_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **subscription_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **subscription_update_dto** | [**SubscriptionUpdateDto**](SubscriptionUpdateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

