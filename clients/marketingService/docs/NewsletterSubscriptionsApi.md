# OpenapiClient::NewsletterSubscriptionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_newsletter_subscription_async**](NewsletterSubscriptionsApi.md#create_newsletter_subscription_async) | **POST** /api/v2/MarketingService/NewsletterSubscriptions | Create a newsletter subscription |
| [**delete_newsletter_subscription_async**](NewsletterSubscriptionsApi.md#delete_newsletter_subscription_async) | **DELETE** /api/v2/MarketingService/NewsletterSubscriptions/{newsletterSubscriptionId} | Delete a newsletter subscription |
| [**get_newsletter_subscription_by_id_async**](NewsletterSubscriptionsApi.md#get_newsletter_subscription_by_id_async) | **GET** /api/v2/MarketingService/NewsletterSubscriptions/{newsletterSubscriptionId} | Get newsletter subscription by ID |
| [**get_newsletter_subscriptions_async**](NewsletterSubscriptionsApi.md#get_newsletter_subscriptions_async) | **GET** /api/v2/MarketingService/NewsletterSubscriptions | Get newsletter subscriptions |
| [**get_newsletter_subscriptions_count_async**](NewsletterSubscriptionsApi.md#get_newsletter_subscriptions_count_async) | **GET** /api/v2/MarketingService/NewsletterSubscriptions/Count | Get newsletter subscriptions count |
| [**update_newsletter_subscription_async**](NewsletterSubscriptionsApi.md#update_newsletter_subscription_async) | **PUT** /api/v2/MarketingService/NewsletterSubscriptions/{newsletterSubscriptionId} | Update a newsletter subscription |


## create_newsletter_subscription_async

> <EmptyEnvelope> create_newsletter_subscription_async(tenant_id, newsletter_subscription_create_dto, opts)

Create a newsletter subscription

Creates a new newsletter subscription for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewsletterSubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_subscription_create_dto = OpenapiClient::NewsletterSubscriptionCreateDto.new # NewsletterSubscriptionCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a newsletter subscription
  result = api_instance.create_newsletter_subscription_async(tenant_id, newsletter_subscription_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->create_newsletter_subscription_async: #{e}"
end
```

#### Using the create_newsletter_subscription_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_newsletter_subscription_async_with_http_info(tenant_id, newsletter_subscription_create_dto, opts)

```ruby
begin
  # Create a newsletter subscription
  data, status_code, headers = api_instance.create_newsletter_subscription_async_with_http_info(tenant_id, newsletter_subscription_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->create_newsletter_subscription_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **newsletter_subscription_create_dto** | [**NewsletterSubscriptionCreateDto**](NewsletterSubscriptionCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_newsletter_subscription_async

> <EmptyEnvelope> delete_newsletter_subscription_async(tenant_id, newsletter_subscription_id, opts)

Delete a newsletter subscription

Deletes a newsletter subscription by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewsletterSubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_subscription_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a newsletter subscription
  result = api_instance.delete_newsletter_subscription_async(tenant_id, newsletter_subscription_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->delete_newsletter_subscription_async: #{e}"
end
```

#### Using the delete_newsletter_subscription_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_newsletter_subscription_async_with_http_info(tenant_id, newsletter_subscription_id, opts)

```ruby
begin
  # Delete a newsletter subscription
  data, status_code, headers = api_instance.delete_newsletter_subscription_async_with_http_info(tenant_id, newsletter_subscription_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->delete_newsletter_subscription_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **newsletter_subscription_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_newsletter_subscription_by_id_async

> <NewsletterSubscriptionDtoEnvelope> get_newsletter_subscription_by_id_async(tenant_id, newsletter_subscription_id, opts)

Get newsletter subscription by ID

Retrieves the details of a specific newsletter subscription by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewsletterSubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_subscription_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get newsletter subscription by ID
  result = api_instance.get_newsletter_subscription_by_id_async(tenant_id, newsletter_subscription_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->get_newsletter_subscription_by_id_async: #{e}"
end
```

#### Using the get_newsletter_subscription_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<NewsletterSubscriptionDtoEnvelope>, Integer, Hash)> get_newsletter_subscription_by_id_async_with_http_info(tenant_id, newsletter_subscription_id, opts)

```ruby
begin
  # Get newsletter subscription by ID
  data, status_code, headers = api_instance.get_newsletter_subscription_by_id_async_with_http_info(tenant_id, newsletter_subscription_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <NewsletterSubscriptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->get_newsletter_subscription_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **newsletter_subscription_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**NewsletterSubscriptionDtoEnvelope**](NewsletterSubscriptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_newsletter_subscriptions_async

> <NewsletterSubscriptionDtoListEnvelope> get_newsletter_subscriptions_async(tenant_id, opts)

Get newsletter subscriptions

Retrieves a collection of newsletter subscriptions for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewsletterSubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  newsletter_subscription_dto_collection_query_parameters: OpenapiClient::NewsletterSubscriptionDtoCollectionQueryParameters.new # NewsletterSubscriptionDtoCollectionQueryParameters | 
}

begin
  # Get newsletter subscriptions
  result = api_instance.get_newsletter_subscriptions_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->get_newsletter_subscriptions_async: #{e}"
end
```

#### Using the get_newsletter_subscriptions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<NewsletterSubscriptionDtoListEnvelope>, Integer, Hash)> get_newsletter_subscriptions_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get newsletter subscriptions
  data, status_code, headers = api_instance.get_newsletter_subscriptions_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <NewsletterSubscriptionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->get_newsletter_subscriptions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **newsletter_subscription_dto_collection_query_parameters** | [**NewsletterSubscriptionDtoCollectionQueryParameters**](NewsletterSubscriptionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**NewsletterSubscriptionDtoListEnvelope**](NewsletterSubscriptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_newsletter_subscriptions_count_async

> <Int32Envelope> get_newsletter_subscriptions_count_async(tenant_id, opts)

Get newsletter subscriptions count

Returns the count of newsletter subscriptions for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewsletterSubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  newsletter_subscription_dto_collection_query_parameters: OpenapiClient::NewsletterSubscriptionDtoCollectionQueryParameters.new # NewsletterSubscriptionDtoCollectionQueryParameters | 
}

begin
  # Get newsletter subscriptions count
  result = api_instance.get_newsletter_subscriptions_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->get_newsletter_subscriptions_count_async: #{e}"
end
```

#### Using the get_newsletter_subscriptions_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_newsletter_subscriptions_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get newsletter subscriptions count
  data, status_code, headers = api_instance.get_newsletter_subscriptions_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->get_newsletter_subscriptions_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **newsletter_subscription_dto_collection_query_parameters** | [**NewsletterSubscriptionDtoCollectionQueryParameters**](NewsletterSubscriptionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_newsletter_subscription_async

> <EmptyEnvelope> update_newsletter_subscription_async(tenant_id, newsletter_subscription_id, newsletter_subscription_update_dto, opts)

Update a newsletter subscription

Updates an existing newsletter subscription by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewsletterSubscriptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_subscription_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_subscription_update_dto = OpenapiClient::NewsletterSubscriptionUpdateDto.new # NewsletterSubscriptionUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a newsletter subscription
  result = api_instance.update_newsletter_subscription_async(tenant_id, newsletter_subscription_id, newsletter_subscription_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->update_newsletter_subscription_async: #{e}"
end
```

#### Using the update_newsletter_subscription_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_newsletter_subscription_async_with_http_info(tenant_id, newsletter_subscription_id, newsletter_subscription_update_dto, opts)

```ruby
begin
  # Update a newsletter subscription
  data, status_code, headers = api_instance.update_newsletter_subscription_async_with_http_info(tenant_id, newsletter_subscription_id, newsletter_subscription_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewsletterSubscriptionsApi->update_newsletter_subscription_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **newsletter_subscription_id** | **String** |  |  |
| **newsletter_subscription_update_dto** | [**NewsletterSubscriptionUpdateDto**](NewsletterSubscriptionUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

