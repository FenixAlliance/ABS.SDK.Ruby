# OpenapiClient::SocialFeedsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_feed_post_async**](SocialFeedsApi.md#create_feed_post_async) | **POST** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts | Create a social feed post |
| [**delete_feed_post_async**](SocialFeedsApi.md#delete_feed_post_async) | **DELETE** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts/{feedPostId} | Delete a social feed post |
| [**get_feed_notifications**](SocialFeedsApi.md#get_feed_notifications) | **GET** /api/v2/SocialService/SocialFeeds | Get social feeds |
| [**get_feed_post_async**](SocialFeedsApi.md#get_feed_post_async) | **GET** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts/{feedPostId} | Get social feed post by ID |
| [**get_feed_posts_async**](SocialFeedsApi.md#get_feed_posts_async) | **GET** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts | Get social feed posts |
| [**get_feed_posts_count_async**](SocialFeedsApi.md#get_feed_posts_count_async) | **GET** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts/Count | Count social feed posts |
| [**get_notification_async**](SocialFeedsApi.md#get_notification_async) | **GET** /api/v2/SocialService/SocialFeeds/{socialFeedId} | Get social feed by ID |
| [**get_notifications_count_async**](SocialFeedsApi.md#get_notifications_count_async) | **GET** /api/v2/SocialService/SocialFeeds/Count | Count social feeds |
| [**patch_feed_post_async**](SocialFeedsApi.md#patch_feed_post_async) | **PATCH** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts/{feedPostId} | Patch a social feed post |
| [**update_feed_post_async**](SocialFeedsApi.md#update_feed_post_async) | **PUT** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts/{feedPostId} | Update a social feed post |


## create_feed_post_async

> <SocialFeedPostDtoEnvelope> create_feed_post_async(social_profile_id, social_feed_id, opts)

Create a social feed post

Creates a new post in a specific social feed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_feed_post_create_dto: OpenapiClient::SocialFeedPostCreateDto.new # SocialFeedPostCreateDto | 
}

begin
  # Create a social feed post
  result = api_instance.create_feed_post_async(social_profile_id, social_feed_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->create_feed_post_async: #{e}"
end
```

#### Using the create_feed_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialFeedPostDtoEnvelope>, Integer, Hash)> create_feed_post_async_with_http_info(social_profile_id, social_feed_id, opts)

```ruby
begin
  # Create a social feed post
  data, status_code, headers = api_instance.create_feed_post_async_with_http_info(social_profile_id, social_feed_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialFeedPostDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->create_feed_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_feed_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_feed_post_create_dto** | [**SocialFeedPostCreateDto**](SocialFeedPostCreateDto.md) |  | [optional] |

### Return type

[**SocialFeedPostDtoEnvelope**](SocialFeedPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_feed_post_async

> <EmptyEnvelope> delete_feed_post_async(social_profile_id, social_feed_id, feed_post_id, opts)

Delete a social feed post

Deletes a post from a specific social feed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
feed_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a social feed post
  result = api_instance.delete_feed_post_async(social_profile_id, social_feed_id, feed_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->delete_feed_post_async: #{e}"
end
```

#### Using the delete_feed_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_feed_post_async_with_http_info(social_profile_id, social_feed_id, feed_post_id, opts)

```ruby
begin
  # Delete a social feed post
  data, status_code, headers = api_instance.delete_feed_post_async_with_http_info(social_profile_id, social_feed_id, feed_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->delete_feed_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_feed_id** | **String** |  |  |
| **feed_post_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_feed_notifications

> <SocialFeedDtoListEnvelope> get_feed_notifications(social_profile_id, opts)

Get social feeds

Retrieves a list of social feeds for the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social feeds
  result = api_instance.get_feed_notifications(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_feed_notifications: #{e}"
end
```

#### Using the get_feed_notifications_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialFeedDtoListEnvelope>, Integer, Hash)> get_feed_notifications_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get social feeds
  data, status_code, headers = api_instance.get_feed_notifications_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialFeedDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_feed_notifications_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialFeedDtoListEnvelope**](SocialFeedDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_feed_post_async

> <SocialFeedPostDtoEnvelope> get_feed_post_async(social_profile_id, social_feed_id, feed_post_id, opts)

Get social feed post by ID

Retrieves a specific post from a social feed by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
feed_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social feed post by ID
  result = api_instance.get_feed_post_async(social_profile_id, social_feed_id, feed_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_feed_post_async: #{e}"
end
```

#### Using the get_feed_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialFeedPostDtoEnvelope>, Integer, Hash)> get_feed_post_async_with_http_info(social_profile_id, social_feed_id, feed_post_id, opts)

```ruby
begin
  # Get social feed post by ID
  data, status_code, headers = api_instance.get_feed_post_async_with_http_info(social_profile_id, social_feed_id, feed_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialFeedPostDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_feed_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_feed_id** | **String** |  |  |
| **feed_post_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialFeedPostDtoEnvelope**](SocialFeedPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_feed_posts_async

> <SocialFeedPostDtoListEnvelope> get_feed_posts_async(social_profile_id, social_feed_id, opts)

Get social feed posts

Retrieves a list of posts for a specific social feed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social feed posts
  result = api_instance.get_feed_posts_async(social_profile_id, social_feed_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_feed_posts_async: #{e}"
end
```

#### Using the get_feed_posts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialFeedPostDtoListEnvelope>, Integer, Hash)> get_feed_posts_async_with_http_info(social_profile_id, social_feed_id, opts)

```ruby
begin
  # Get social feed posts
  data, status_code, headers = api_instance.get_feed_posts_async_with_http_info(social_profile_id, social_feed_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialFeedPostDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_feed_posts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_feed_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialFeedPostDtoListEnvelope**](SocialFeedPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_feed_posts_count_async

> <Int32Envelope> get_feed_posts_count_async(social_profile_id, social_feed_id, opts)

Count social feed posts

Returns the count of posts for a specific social feed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count social feed posts
  result = api_instance.get_feed_posts_count_async(social_profile_id, social_feed_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_feed_posts_count_async: #{e}"
end
```

#### Using the get_feed_posts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_feed_posts_count_async_with_http_info(social_profile_id, social_feed_id, opts)

```ruby
begin
  # Count social feed posts
  data, status_code, headers = api_instance.get_feed_posts_count_async_with_http_info(social_profile_id, social_feed_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_feed_posts_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_feed_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_notification_async

> <SocialFeedDtoEnvelope> get_notification_async(social_profile_id, social_feed_id, opts)

Get social feed by ID

Retrieves a specific social feed by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social feed by ID
  result = api_instance.get_notification_async(social_profile_id, social_feed_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_notification_async: #{e}"
end
```

#### Using the get_notification_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialFeedDtoEnvelope>, Integer, Hash)> get_notification_async_with_http_info(social_profile_id, social_feed_id, opts)

```ruby
begin
  # Get social feed by ID
  data, status_code, headers = api_instance.get_notification_async_with_http_info(social_profile_id, social_feed_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialFeedDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_notification_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_feed_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialFeedDtoEnvelope**](SocialFeedDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_notifications_count_async

> <Int32Envelope> get_notifications_count_async(social_profile_id, opts)

Count social feeds

Returns the count of social feeds for the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count social feeds
  result = api_instance.get_notifications_count_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_notifications_count_async: #{e}"
end
```

#### Using the get_notifications_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_notifications_count_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Count social feeds
  data, status_code, headers = api_instance.get_notifications_count_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->get_notifications_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_feed_post_async

> <EmptyEnvelope> patch_feed_post_async(social_profile_id, social_feed_id, feed_post_id, opts)

Patch a social feed post

Partially updates an existing post in a specific social feed using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
feed_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a social feed post
  result = api_instance.patch_feed_post_async(social_profile_id, social_feed_id, feed_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->patch_feed_post_async: #{e}"
end
```

#### Using the patch_feed_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_feed_post_async_with_http_info(social_profile_id, social_feed_id, feed_post_id, opts)

```ruby
begin
  # Patch a social feed post
  data, status_code, headers = api_instance.patch_feed_post_async_with_http_info(social_profile_id, social_feed_id, feed_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->patch_feed_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_feed_id** | **String** |  |  |
| **feed_post_id** | **String** |  |  |
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


## update_feed_post_async

> <SocialFeedPostDtoEnvelope> update_feed_post_async(social_profile_id, social_feed_id, feed_post_id, opts)

Update a social feed post

Updates an existing post in a specific social feed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialFeedsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
feed_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_feed_post_update_dto: OpenapiClient::SocialFeedPostUpdateDto.new # SocialFeedPostUpdateDto | 
}

begin
  # Update a social feed post
  result = api_instance.update_feed_post_async(social_profile_id, social_feed_id, feed_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->update_feed_post_async: #{e}"
end
```

#### Using the update_feed_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialFeedPostDtoEnvelope>, Integer, Hash)> update_feed_post_async_with_http_info(social_profile_id, social_feed_id, feed_post_id, opts)

```ruby
begin
  # Update a social feed post
  data, status_code, headers = api_instance.update_feed_post_async_with_http_info(social_profile_id, social_feed_id, feed_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialFeedPostDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialFeedsApi->update_feed_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_feed_id** | **String** |  |  |
| **feed_post_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_feed_post_update_dto** | [**SocialFeedPostUpdateDto**](SocialFeedPostUpdateDto.md) |  | [optional] |

### Return type

[**SocialFeedPostDtoEnvelope**](SocialFeedPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

