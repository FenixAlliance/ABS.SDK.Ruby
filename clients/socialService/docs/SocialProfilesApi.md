# OpenapiClient::SocialProfilesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_conversations_async**](SocialProfilesApi.md#count_conversations_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Conversations/Count | Count Conversations |
| [**count_followed_profiles_async**](SocialProfilesApi.md#count_followed_profiles_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Follows/Profiles/Count | Count Followed Profiles |
| [**count_follower_profiles_async**](SocialProfilesApi.md#count_follower_profiles_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Followers/Profiles/Count | Count Follower Profiles |
| [**count_followers_async**](SocialProfilesApi.md#count_followers_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Followers/Count | Count Followers |
| [**count_follows_async**](SocialProfilesApi.md#count_follows_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Follows/Count | Count Follows |
| [**count_messages_async**](SocialProfilesApi.md#count_messages_async) | **GET** /api/v2/SocialService/SocialProfiles/{conversationId}/Messages/Count | Count Messages |
| [**count_notifications_async**](SocialProfilesApi.md#count_notifications_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Notifications/Count | Count Notifications |
| [**count_social_profiles_async**](SocialProfilesApi.md#count_social_profiles_async) | **GET** /api/v2/SocialService/SocialProfiles/Count | Count Social Profiles |
| [**create_conversation_async**](SocialProfilesApi.md#create_conversation_async) | **POST** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Conversations | Create Conversation |
| [**create_message_async**](SocialProfilesApi.md#create_message_async) | **POST** /api/v2/SocialService/SocialProfiles/{conversationId}/Messages | Create Message |
| [**delete_message_async**](SocialProfilesApi.md#delete_message_async) | **DELETE** /api/v2/SocialService/SocialProfiles/{conversationId}/Messages/{messageId} | Delete Message |
| [**follow_async**](SocialProfilesApi.md#follow_async) | **POST** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Follows/{followedSocialProfileId} | Follow |
| [**follow_exists_async**](SocialProfilesApi.md#follow_exists_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Follows/{followedSocialProfileId} | Check if Follow Exists |
| [**get_conversations_async**](SocialProfilesApi.md#get_conversations_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Conversations | Get Conversations |
| [**get_followed_profiles_async**](SocialProfilesApi.md#get_followed_profiles_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Follows/Profiles | Get Followed Profiles |
| [**get_follower_profiles_async**](SocialProfilesApi.md#get_follower_profiles_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Followers/Profiles | Get Follower Profiles |
| [**get_followers_async**](SocialProfilesApi.md#get_followers_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Followers | Get Followers |
| [**get_follows_async**](SocialProfilesApi.md#get_follows_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Follows | Get Follows |
| [**get_messages_async**](SocialProfilesApi.md#get_messages_async) | **GET** /api/v2/SocialService/SocialProfiles/{conversationId}/Messages | Get Messages |
| [**get_notifications_async**](SocialProfilesApi.md#get_notifications_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Notifications | Get Notifications |
| [**get_social_profile_async**](SocialProfilesApi.md#get_social_profile_async) | **GET** /api/v2/SocialService/SocialProfiles/{socialProfileId} | Get Social Profile |
| [**get_social_profiles_async**](SocialProfilesApi.md#get_social_profiles_async) | **GET** /api/v2/SocialService/SocialProfiles | Get Social Profiles |
| [**unfollow_async**](SocialProfilesApi.md#unfollow_async) | **DELETE** /api/v2/SocialService/SocialProfiles/{socialProfileId}/Follows/{followedSocialProfileId} | Unfollow |
| [**update_message_async**](SocialProfilesApi.md#update_message_async) | **PUT** /api/v2/SocialService/SocialProfiles/{conversationId}/Messages/{messageId} | Update Message |


## count_conversations_async

> <Int32Envelope> count_conversations_async(social_profile_id, opts)

Count Conversations

Count conversations for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count Conversations
  result = api_instance.count_conversations_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_conversations_async: #{e}"
end
```

#### Using the count_conversations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_conversations_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Count Conversations
  data, status_code, headers = api_instance.count_conversations_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_conversations_async_with_http_info: #{e}"
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


## count_followed_profiles_async

> <Int32Envelope> count_followed_profiles_async(social_profile_id, opts)

Count Followed Profiles

Count followed profiles for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count Followed Profiles
  result = api_instance.count_followed_profiles_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_followed_profiles_async: #{e}"
end
```

#### Using the count_followed_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_followed_profiles_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Count Followed Profiles
  data, status_code, headers = api_instance.count_followed_profiles_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_followed_profiles_async_with_http_info: #{e}"
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


## count_follower_profiles_async

> <Int32Envelope> count_follower_profiles_async(social_profile_id, opts)

Count Follower Profiles

Count follower profiles for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count Follower Profiles
  result = api_instance.count_follower_profiles_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_follower_profiles_async: #{e}"
end
```

#### Using the count_follower_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_follower_profiles_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Count Follower Profiles
  data, status_code, headers = api_instance.count_follower_profiles_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_follower_profiles_async_with_http_info: #{e}"
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


## count_followers_async

> <Int32Envelope> count_followers_async(social_profile_id, opts)

Count Followers

Count followers for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count Followers
  result = api_instance.count_followers_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_followers_async: #{e}"
end
```

#### Using the count_followers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_followers_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Count Followers
  data, status_code, headers = api_instance.count_followers_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_followers_async_with_http_info: #{e}"
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


## count_follows_async

> <Int32Envelope> count_follows_async(social_profile_id, opts)

Count Follows

Count follows for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count Follows
  result = api_instance.count_follows_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_follows_async: #{e}"
end
```

#### Using the count_follows_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_follows_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Count Follows
  data, status_code, headers = api_instance.count_follows_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_follows_async_with_http_info: #{e}"
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


## count_messages_async

> <Int32Envelope> count_messages_async(conversation_id, opts)

Count Messages

Count messages for a conversation.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count Messages
  result = api_instance.count_messages_async(conversation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_messages_async: #{e}"
end
```

#### Using the count_messages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_messages_async_with_http_info(conversation_id, opts)

```ruby
begin
  # Count Messages
  data, status_code, headers = api_instance.count_messages_async_with_http_info(conversation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_messages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **conversation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## count_notifications_async

> <Int32Envelope> count_notifications_async(social_profile_id, opts)

Count Notifications

Count notifications for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count Notifications
  result = api_instance.count_notifications_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_notifications_async: #{e}"
end
```

#### Using the count_notifications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_notifications_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Count Notifications
  data, status_code, headers = api_instance.count_notifications_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_notifications_async_with_http_info: #{e}"
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


## count_social_profiles_async

> <Int32Envelope> count_social_profiles_async(opts)

Count Social Profiles

Count social profiles.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count Social Profiles
  result = api_instance.count_social_profiles_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_social_profiles_async: #{e}"
end
```

#### Using the count_social_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_social_profiles_async_with_http_info(opts)

```ruby
begin
  # Count Social Profiles
  data, status_code, headers = api_instance.count_social_profiles_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->count_social_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_conversation_async

> <EmptyEnvelope> create_conversation_async(social_profile_id, opts)

Create Conversation

Create a new conversation.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  conversation_create_dto: OpenapiClient::ConversationCreateDto.new # ConversationCreateDto | 
}

begin
  # Create Conversation
  result = api_instance.create_conversation_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->create_conversation_async: #{e}"
end
```

#### Using the create_conversation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_conversation_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Create Conversation
  data, status_code, headers = api_instance.create_conversation_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->create_conversation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **conversation_create_dto** | [**ConversationCreateDto**](ConversationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_message_async

> <EmptyEnvelope> create_message_async(social_profile_id, conversation_id, opts)

Create Message

Create a new message.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  private_message_create_dto: OpenapiClient::PrivateMessageCreateDto.new # PrivateMessageCreateDto | 
}

begin
  # Create Message
  result = api_instance.create_message_async(social_profile_id, conversation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->create_message_async: #{e}"
end
```

#### Using the create_message_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_message_async_with_http_info(social_profile_id, conversation_id, opts)

```ruby
begin
  # Create Message
  data, status_code, headers = api_instance.create_message_async_with_http_info(social_profile_id, conversation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->create_message_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **conversation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **private_message_create_dto** | [**PrivateMessageCreateDto**](PrivateMessageCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_message_async

> <EmptyEnvelope> delete_message_async(social_profile_id, conversation_id, message_id, opts)

Delete Message

Delete a message.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
message_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete Message
  result = api_instance.delete_message_async(social_profile_id, conversation_id, message_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->delete_message_async: #{e}"
end
```

#### Using the delete_message_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_message_async_with_http_info(social_profile_id, conversation_id, message_id, opts)

```ruby
begin
  # Delete Message
  data, status_code, headers = api_instance.delete_message_async_with_http_info(social_profile_id, conversation_id, message_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->delete_message_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **conversation_id** | **String** |  |  |
| **message_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## follow_async

> <EmptyEnvelope> follow_async(social_profile_id, followed_social_profile_id, opts)

Follow

Follow a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
followed_social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Follow
  result = api_instance.follow_async(social_profile_id, followed_social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->follow_async: #{e}"
end
```

#### Using the follow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> follow_async_with_http_info(social_profile_id, followed_social_profile_id, opts)

```ruby
begin
  # Follow
  data, status_code, headers = api_instance.follow_async_with_http_info(social_profile_id, followed_social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->follow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **followed_social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## follow_exists_async

> <BooleanEnvelope> follow_exists_async(social_profile_id, followed_social_profile_id, opts)

Check if Follow Exists

Check if a follow record exists between two social profiles.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
followed_social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Check if Follow Exists
  result = api_instance.follow_exists_async(social_profile_id, followed_social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->follow_exists_async: #{e}"
end
```

#### Using the follow_exists_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> follow_exists_async_with_http_info(social_profile_id, followed_social_profile_id, opts)

```ruby
begin
  # Check if Follow Exists
  data, status_code, headers = api_instance.follow_exists_async_with_http_info(social_profile_id, followed_social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->follow_exists_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **followed_social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_conversations_async

> <ConversationDtoListEnvelope> get_conversations_async(social_profile_id, opts)

Get Conversations

Get a list of conversations for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Conversations
  result = api_instance.get_conversations_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_conversations_async: #{e}"
end
```

#### Using the get_conversations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ConversationDtoListEnvelope>, Integer, Hash)> get_conversations_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get Conversations
  data, status_code, headers = api_instance.get_conversations_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ConversationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_conversations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ConversationDtoListEnvelope**](ConversationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_followed_profiles_async

> <SocialProfileDtoListEnvelope> get_followed_profiles_async(social_profile_id, opts)

Get Followed Profiles

Get a list of followed profiles for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Followed Profiles
  result = api_instance.get_followed_profiles_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_followed_profiles_async: #{e}"
end
```

#### Using the get_followed_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialProfileDtoListEnvelope>, Integer, Hash)> get_followed_profiles_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get Followed Profiles
  data, status_code, headers = api_instance.get_followed_profiles_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_followed_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialProfileDtoListEnvelope**](SocialProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_follower_profiles_async

> <SocialProfileDtoListEnvelope> get_follower_profiles_async(social_profile_id, opts)

Get Follower Profiles

Get a list of follower profiles for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Follower Profiles
  result = api_instance.get_follower_profiles_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_follower_profiles_async: #{e}"
end
```

#### Using the get_follower_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialProfileDtoListEnvelope>, Integer, Hash)> get_follower_profiles_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get Follower Profiles
  data, status_code, headers = api_instance.get_follower_profiles_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_follower_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialProfileDtoListEnvelope**](SocialProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_followers_async

> <FollowRecordDtoListEnvelope> get_followers_async(social_profile_id, opts)

Get Followers

Get a list of followers for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Followers
  result = api_instance.get_followers_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_followers_async: #{e}"
end
```

#### Using the get_followers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FollowRecordDtoListEnvelope>, Integer, Hash)> get_followers_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get Followers
  data, status_code, headers = api_instance.get_followers_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FollowRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_followers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FollowRecordDtoListEnvelope**](FollowRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_follows_async

> <FollowRecordDtoListEnvelope> get_follows_async(social_profile_id, opts)

Get Follows

Get a list of follows for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Follows
  result = api_instance.get_follows_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_follows_async: #{e}"
end
```

#### Using the get_follows_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FollowRecordDtoListEnvelope>, Integer, Hash)> get_follows_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get Follows
  data, status_code, headers = api_instance.get_follows_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FollowRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_follows_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FollowRecordDtoListEnvelope**](FollowRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_messages_async

> <PrivateMessageDtoListEnvelope> get_messages_async(conversation_id, opts)

Get Messages

Get a list of messages for a conversation.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Messages
  result = api_instance.get_messages_async(conversation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_messages_async: #{e}"
end
```

#### Using the get_messages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PrivateMessageDtoListEnvelope>, Integer, Hash)> get_messages_async_with_http_info(conversation_id, opts)

```ruby
begin
  # Get Messages
  data, status_code, headers = api_instance.get_messages_async_with_http_info(conversation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PrivateMessageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_messages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **conversation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PrivateMessageDtoListEnvelope**](PrivateMessageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_notifications_async

> <NotificationDtoListEnvelope> get_notifications_async(social_profile_id, opts)

Get Notifications

Get a list of notifications for a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Notifications
  result = api_instance.get_notifications_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_notifications_async: #{e}"
end
```

#### Using the get_notifications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<NotificationDtoListEnvelope>, Integer, Hash)> get_notifications_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get Notifications
  data, status_code, headers = api_instance.get_notifications_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <NotificationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_notifications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**NotificationDtoListEnvelope**](NotificationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_profile_async

> <SocialProfileDtoEnvelope> get_social_profile_async(social_profile_id, opts)

Get Social Profile

Get a social profile by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Social Profile
  result = api_instance.get_social_profile_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_social_profile_async: #{e}"
end
```

#### Using the get_social_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialProfileDtoEnvelope>, Integer, Hash)> get_social_profile_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get Social Profile
  data, status_code, headers = api_instance.get_social_profile_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialProfileDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_social_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialProfileDtoEnvelope**](SocialProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_profiles_async

> <SocialProfileDtoListEnvelope> get_social_profiles_async(opts)

Get Social Profiles

Get a list of social profiles.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Social Profiles
  result = api_instance.get_social_profiles_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_social_profiles_async: #{e}"
end
```

#### Using the get_social_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialProfileDtoListEnvelope>, Integer, Hash)> get_social_profiles_async_with_http_info(opts)

```ruby
begin
  # Get Social Profiles
  data, status_code, headers = api_instance.get_social_profiles_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->get_social_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialProfileDtoListEnvelope**](SocialProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## unfollow_async

> <EmptyEnvelope> unfollow_async(social_profile_id, followed_social_profile_id, opts)

Unfollow

Unfollow a social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
followed_social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Unfollow
  result = api_instance.unfollow_async(social_profile_id, followed_social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->unfollow_async: #{e}"
end
```

#### Using the unfollow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> unfollow_async_with_http_info(social_profile_id, followed_social_profile_id, opts)

```ruby
begin
  # Unfollow
  data, status_code, headers = api_instance.unfollow_async_with_http_info(social_profile_id, followed_social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->unfollow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **followed_social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_message_async

> <EmptyEnvelope> update_message_async(social_profile_id, conversation_id, message_id, opts)

Update Message

Update a message.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialProfilesApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
message_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  private_message_update_dto: OpenapiClient::PrivateMessageUpdateDto.new # PrivateMessageUpdateDto | 
}

begin
  # Update Message
  result = api_instance.update_message_async(social_profile_id, conversation_id, message_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->update_message_async: #{e}"
end
```

#### Using the update_message_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_message_async_with_http_info(social_profile_id, conversation_id, message_id, opts)

```ruby
begin
  # Update Message
  data, status_code, headers = api_instance.update_message_async_with_http_info(social_profile_id, conversation_id, message_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialProfilesApi->update_message_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **conversation_id** | **String** |  |  |
| **message_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **private_message_update_dto** | [**PrivateMessageUpdateDto**](PrivateMessageUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

