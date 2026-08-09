# OpenapiClient::SocialPostsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_social_comment_reaction_async**](SocialPostsApi.md#create_social_comment_reaction_async) | **POST** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId}/Reactions | Create a social comment reaction |
| [**create_social_post_async**](SocialPostsApi.md#create_social_post_async) | **POST** /api/v2/SocialService/SocialPosts | Create a social post |
| [**create_social_post_attachment_async**](SocialPostsApi.md#create_social_post_attachment_async) | **POST** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments | Create a social post attachment |
| [**create_social_post_comment_async**](SocialPostsApi.md#create_social_post_comment_async) | **POST** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments | Create a social post comment |
| [**create_social_post_reaction_async**](SocialPostsApi.md#create_social_post_reaction_async) | **POST** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions | Create a social post reaction |
| [**delete_social_comment_reaction_async**](SocialPostsApi.md#delete_social_comment_reaction_async) | **DELETE** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId}/Reactions/{reactionId} | Delete a social comment reaction |
| [**delete_social_post_async**](SocialPostsApi.md#delete_social_post_async) | **DELETE** /api/v2/SocialService/SocialPosts/{socialPostId} | Delete a social post |
| [**delete_social_post_attachment_async**](SocialPostsApi.md#delete_social_post_attachment_async) | **DELETE** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments/{attachmentId} | Delete a social post attachment |
| [**delete_social_post_comment_async**](SocialPostsApi.md#delete_social_post_comment_async) | **DELETE** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId} | Delete a social post comment |
| [**delete_social_post_reaction_async**](SocialPostsApi.md#delete_social_post_reaction_async) | **DELETE** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions/{reactionId} | Delete a social post reaction |
| [**get_social_comment_reaction_async**](SocialPostsApi.md#get_social_comment_reaction_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId}/Reactions/{reactionId} | Get social comment reaction by ID |
| [**get_social_comment_reactions_async**](SocialPostsApi.md#get_social_comment_reactions_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId}/Reactions | Get social comment reactions |
| [**get_social_comment_reactions_count_async**](SocialPostsApi.md#get_social_comment_reactions_count_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId}/Reactions/Count | Count social comment reactions |
| [**get_social_post_async**](SocialPostsApi.md#get_social_post_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId} | Get social post by ID |
| [**get_social_post_attachment_async**](SocialPostsApi.md#get_social_post_attachment_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments/{attachmentId} | Get social post attachment by ID |
| [**get_social_post_attachments_async**](SocialPostsApi.md#get_social_post_attachments_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments | Get social post attachments |
| [**get_social_post_attachments_count_async**](SocialPostsApi.md#get_social_post_attachments_count_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments/Count | Count social post attachments |
| [**get_social_post_comment_async**](SocialPostsApi.md#get_social_post_comment_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId} | Get social post comment by ID |
| [**get_social_post_comments_async**](SocialPostsApi.md#get_social_post_comments_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments | Get social post comments |
| [**get_social_post_comments_count_async**](SocialPostsApi.md#get_social_post_comments_count_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/Count | Count social post comments |
| [**get_social_post_reaction_async**](SocialPostsApi.md#get_social_post_reaction_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions/{reactionId} | Get social post reaction by ID |
| [**get_social_post_reactions_async**](SocialPostsApi.md#get_social_post_reactions_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions | Get social post reactions |
| [**get_social_post_reactions_count_async**](SocialPostsApi.md#get_social_post_reactions_count_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions/Count | Count social post reactions |
| [**get_social_posts_async**](SocialPostsApi.md#get_social_posts_async) | **GET** /api/v2/SocialService/SocialPosts | Get social posts |
| [**get_social_posts_count_async**](SocialPostsApi.md#get_social_posts_count_async) | **GET** /api/v2/SocialService/SocialPosts/Count | Count social posts |
| [**patch_social_post_async**](SocialPostsApi.md#patch_social_post_async) | **PATCH** /api/v2/SocialService/SocialPosts/{socialPostId} | Patch a social post |
| [**update_social_comment_reaction_async**](SocialPostsApi.md#update_social_comment_reaction_async) | **PUT** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId}/Reactions/{reactionId} | Update a social comment reaction |
| [**update_social_post_async**](SocialPostsApi.md#update_social_post_async) | **PUT** /api/v2/SocialService/SocialPosts/{socialPostId} | Update a social post |
| [**update_social_post_attachment_async**](SocialPostsApi.md#update_social_post_attachment_async) | **PUT** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments/{attachmentId} | Update a social post attachment |
| [**update_social_post_comment_async**](SocialPostsApi.md#update_social_post_comment_async) | **PUT** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId} | Update a social post comment |
| [**update_social_post_reaction_async**](SocialPostsApi.md#update_social_post_reaction_async) | **PUT** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions/{reactionId} | Update a social post reaction |
| [**upload_social_post_image_attachment_async**](SocialPostsApi.md#upload_social_post_image_attachment_async) | **POST** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments/Image | Upload a social post image attachment |


## create_social_comment_reaction_async

> <SocialCommentReactionDtoEnvelope> create_social_comment_reaction_async(social_post_id, comment_id, social_profile_id, opts)

Create a social comment reaction

Creates a new reaction on a specific social comment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_reaction_create_dto: OpenapiClient::SocialReactionCreateDto.new # SocialReactionCreateDto | 
}

begin
  # Create a social comment reaction
  result = api_instance.create_social_comment_reaction_async(social_post_id, comment_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_comment_reaction_async: #{e}"
end
```

#### Using the create_social_comment_reaction_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialCommentReactionDtoEnvelope>, Integer, Hash)> create_social_comment_reaction_async_with_http_info(social_post_id, comment_id, social_profile_id, opts)

```ruby
begin
  # Create a social comment reaction
  data, status_code, headers = api_instance.create_social_comment_reaction_async_with_http_info(social_post_id, comment_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialCommentReactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_comment_reaction_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_reaction_create_dto** | [**SocialReactionCreateDto**](SocialReactionCreateDto.md) |  | [optional] |

### Return type

[**SocialCommentReactionDtoEnvelope**](SocialCommentReactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_social_post_async

> <SocialPostDtoEnvelope> create_social_post_async(social_profile_id, opts)

Create a social post

Creates a new social post for the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_create_dto: OpenapiClient::SocialPostCreateDto.new # SocialPostCreateDto | 
}

begin
  # Create a social post
  result = api_instance.create_social_post_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_post_async: #{e}"
end
```

#### Using the create_social_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostDtoEnvelope>, Integer, Hash)> create_social_post_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Create a social post
  data, status_code, headers = api_instance.create_social_post_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_create_dto** | [**SocialPostCreateDto**](SocialPostCreateDto.md) |  | [optional] |

### Return type

[**SocialPostDtoEnvelope**](SocialPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_social_post_attachment_async

> <SocialPostAttachmentDtoEnvelope> create_social_post_attachment_async(social_post_id, social_profile_id, opts)

Create a social post attachment

Creates a new attachment for a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_attachment_create_dto: OpenapiClient::SocialPostAttachmentCreateDto.new # SocialPostAttachmentCreateDto | 
}

begin
  # Create a social post attachment
  result = api_instance.create_social_post_attachment_async(social_post_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_post_attachment_async: #{e}"
end
```

#### Using the create_social_post_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostAttachmentDtoEnvelope>, Integer, Hash)> create_social_post_attachment_async_with_http_info(social_post_id, social_profile_id, opts)

```ruby
begin
  # Create a social post attachment
  data, status_code, headers = api_instance.create_social_post_attachment_async_with_http_info(social_post_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostAttachmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_post_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_attachment_create_dto** | [**SocialPostAttachmentCreateDto**](SocialPostAttachmentCreateDto.md) |  | [optional] |

### Return type

[**SocialPostAttachmentDtoEnvelope**](SocialPostAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_social_post_comment_async

> <EmptyEnvelope> create_social_post_comment_async(social_profile_id, social_post_id, opts)

Create a social post comment

Creates a new comment on a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_comment_create_dto: OpenapiClient::SocialPostCommentCreateDto.new # SocialPostCommentCreateDto | 
}

begin
  # Create a social post comment
  result = api_instance.create_social_post_comment_async(social_profile_id, social_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_post_comment_async: #{e}"
end
```

#### Using the create_social_post_comment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_social_post_comment_async_with_http_info(social_profile_id, social_post_id, opts)

```ruby
begin
  # Create a social post comment
  data, status_code, headers = api_instance.create_social_post_comment_async_with_http_info(social_profile_id, social_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_post_comment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_comment_create_dto** | [**SocialPostCommentCreateDto**](SocialPostCommentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_social_post_reaction_async

> <SocialPostReactionDtoEnvelope> create_social_post_reaction_async(social_post_id, social_profile_id, opts)

Create a social post reaction

Creates a new reaction on a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_reaction_create_dto: OpenapiClient::SocialReactionCreateDto.new # SocialReactionCreateDto | 
}

begin
  # Create a social post reaction
  result = api_instance.create_social_post_reaction_async(social_post_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_post_reaction_async: #{e}"
end
```

#### Using the create_social_post_reaction_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostReactionDtoEnvelope>, Integer, Hash)> create_social_post_reaction_async_with_http_info(social_post_id, social_profile_id, opts)

```ruby
begin
  # Create a social post reaction
  data, status_code, headers = api_instance.create_social_post_reaction_async_with_http_info(social_post_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostReactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->create_social_post_reaction_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_reaction_create_dto** | [**SocialReactionCreateDto**](SocialReactionCreateDto.md) |  | [optional] |

### Return type

[**SocialPostReactionDtoEnvelope**](SocialPostReactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_social_comment_reaction_async

> <EmptyEnvelope> delete_social_comment_reaction_async(social_post_id, comment_id, reaction_id, social_profile_id, opts)

Delete a social comment reaction

Deletes a reaction from a specific social comment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a social comment reaction
  result = api_instance.delete_social_comment_reaction_async(social_post_id, comment_id, reaction_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_comment_reaction_async: #{e}"
end
```

#### Using the delete_social_comment_reaction_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_social_comment_reaction_async_with_http_info(social_post_id, comment_id, reaction_id, social_profile_id, opts)

```ruby
begin
  # Delete a social comment reaction
  data, status_code, headers = api_instance.delete_social_comment_reaction_async_with_http_info(social_post_id, comment_id, reaction_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_comment_reaction_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **reaction_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_social_post_async

> <EmptyEnvelope> delete_social_post_async(social_profile_id, social_post_id, opts)

Delete a social post

Deletes a social post by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a social post
  result = api_instance.delete_social_post_async(social_profile_id, social_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_post_async: #{e}"
end
```

#### Using the delete_social_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_social_post_async_with_http_info(social_profile_id, social_post_id, opts)

```ruby
begin
  # Delete a social post
  data, status_code, headers = api_instance.delete_social_post_async_with_http_info(social_profile_id, social_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_social_post_attachment_async

> <EmptyEnvelope> delete_social_post_attachment_async(social_profile_id, social_post_id, attachment_id, opts)

Delete a social post attachment

Deletes an attachment from a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a social post attachment
  result = api_instance.delete_social_post_attachment_async(social_profile_id, social_post_id, attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_post_attachment_async: #{e}"
end
```

#### Using the delete_social_post_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_social_post_attachment_async_with_http_info(social_profile_id, social_post_id, attachment_id, opts)

```ruby
begin
  # Delete a social post attachment
  data, status_code, headers = api_instance.delete_social_post_attachment_async_with_http_info(social_profile_id, social_post_id, attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_post_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_social_post_comment_async

> <EmptyEnvelope> delete_social_post_comment_async(social_profile_id, social_post_id, comment_id, opts)

Delete a social post comment

Deletes a comment from a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a social post comment
  result = api_instance.delete_social_post_comment_async(social_profile_id, social_post_id, comment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_post_comment_async: #{e}"
end
```

#### Using the delete_social_post_comment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_social_post_comment_async_with_http_info(social_profile_id, social_post_id, comment_id, opts)

```ruby
begin
  # Delete a social post comment
  data, status_code, headers = api_instance.delete_social_post_comment_async_with_http_info(social_profile_id, social_post_id, comment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_post_comment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_social_post_reaction_async

> <EmptyEnvelope> delete_social_post_reaction_async(social_profile_id, social_post_id, reaction_id, opts)

Delete a social post reaction

Deletes a reaction from a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a social post reaction
  result = api_instance.delete_social_post_reaction_async(social_profile_id, social_post_id, reaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_post_reaction_async: #{e}"
end
```

#### Using the delete_social_post_reaction_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_social_post_reaction_async_with_http_info(social_profile_id, social_post_id, reaction_id, opts)

```ruby
begin
  # Delete a social post reaction
  data, status_code, headers = api_instance.delete_social_post_reaction_async_with_http_info(social_profile_id, social_post_id, reaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->delete_social_post_reaction_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **reaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_comment_reaction_async

> <SocialCommentReactionDtoEnvelope> get_social_comment_reaction_async(social_post_id, comment_id, reaction_id, opts)

Get social comment reaction by ID

Retrieves a specific reaction from a social comment by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social comment reaction by ID
  result = api_instance.get_social_comment_reaction_async(social_post_id, comment_id, reaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_comment_reaction_async: #{e}"
end
```

#### Using the get_social_comment_reaction_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialCommentReactionDtoEnvelope>, Integer, Hash)> get_social_comment_reaction_async_with_http_info(social_post_id, comment_id, reaction_id, opts)

```ruby
begin
  # Get social comment reaction by ID
  data, status_code, headers = api_instance.get_social_comment_reaction_async_with_http_info(social_post_id, comment_id, reaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialCommentReactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_comment_reaction_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **reaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialCommentReactionDtoEnvelope**](SocialCommentReactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_comment_reactions_async

> <SocialCommentReactionDtoListEnvelope> get_social_comment_reactions_async(social_post_id, comment_id, social_profile_id, opts)

Get social comment reactions

Retrieves a list of reactions for a specific social comment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_comment_reaction_dto_collection_query_parameters: OpenapiClient::SocialCommentReactionDtoCollectionQueryParameters.new # SocialCommentReactionDtoCollectionQueryParameters | 
}

begin
  # Get social comment reactions
  result = api_instance.get_social_comment_reactions_async(social_post_id, comment_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_comment_reactions_async: #{e}"
end
```

#### Using the get_social_comment_reactions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialCommentReactionDtoListEnvelope>, Integer, Hash)> get_social_comment_reactions_async_with_http_info(social_post_id, comment_id, social_profile_id, opts)

```ruby
begin
  # Get social comment reactions
  data, status_code, headers = api_instance.get_social_comment_reactions_async_with_http_info(social_post_id, comment_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialCommentReactionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_comment_reactions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_comment_reaction_dto_collection_query_parameters** | [**SocialCommentReactionDtoCollectionQueryParameters**](SocialCommentReactionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SocialCommentReactionDtoListEnvelope**](SocialCommentReactionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_comment_reactions_count_async

> <Int32Envelope> get_social_comment_reactions_count_async(social_post_id, comment_id, social_profile_id, opts)

Count social comment reactions

Returns the count of reactions for a specific social comment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_comment_reaction_dto_collection_query_parameters: OpenapiClient::SocialCommentReactionDtoCollectionQueryParameters.new # SocialCommentReactionDtoCollectionQueryParameters | 
}

begin
  # Count social comment reactions
  result = api_instance.get_social_comment_reactions_count_async(social_post_id, comment_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_comment_reactions_count_async: #{e}"
end
```

#### Using the get_social_comment_reactions_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_social_comment_reactions_count_async_with_http_info(social_post_id, comment_id, social_profile_id, opts)

```ruby
begin
  # Count social comment reactions
  data, status_code, headers = api_instance.get_social_comment_reactions_count_async_with_http_info(social_post_id, comment_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_comment_reactions_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_comment_reaction_dto_collection_query_parameters** | [**SocialCommentReactionDtoCollectionQueryParameters**](SocialCommentReactionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_post_async

> <SocialPostDtoEnvelope> get_social_post_async(social_profile_id, social_post_id, opts)

Get social post by ID

Retrieves a specific social post by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social post by ID
  result = api_instance.get_social_post_async(social_profile_id, social_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_async: #{e}"
end
```

#### Using the get_social_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostDtoEnvelope>, Integer, Hash)> get_social_post_async_with_http_info(social_profile_id, social_post_id, opts)

```ruby
begin
  # Get social post by ID
  data, status_code, headers = api_instance.get_social_post_async_with_http_info(social_profile_id, social_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialPostDtoEnvelope**](SocialPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_post_attachment_async

> <EmptyEnvelope> get_social_post_attachment_async(social_post_id, attachment_id, opts)

Get social post attachment by ID

Retrieves a specific attachment from a social post by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social post attachment by ID
  result = api_instance.get_social_post_attachment_async(social_post_id, attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_attachment_async: #{e}"
end
```

#### Using the get_social_post_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_social_post_attachment_async_with_http_info(social_post_id, attachment_id, opts)

```ruby
begin
  # Get social post attachment by ID
  data, status_code, headers = api_instance.get_social_post_attachment_async_with_http_info(social_post_id, attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_post_attachments_async

> <SocialPostAttachmentDtoListEnvelope> get_social_post_attachments_async(social_post_id, opts)

Get social post attachments

Retrieves a list of attachments for a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_attachment_dto_collection_query_parameters: OpenapiClient::SocialPostAttachmentDtoCollectionQueryParameters.new # SocialPostAttachmentDtoCollectionQueryParameters | 
}

begin
  # Get social post attachments
  result = api_instance.get_social_post_attachments_async(social_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_attachments_async: #{e}"
end
```

#### Using the get_social_post_attachments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostAttachmentDtoListEnvelope>, Integer, Hash)> get_social_post_attachments_async_with_http_info(social_post_id, opts)

```ruby
begin
  # Get social post attachments
  data, status_code, headers = api_instance.get_social_post_attachments_async_with_http_info(social_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostAttachmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_attachments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_attachment_dto_collection_query_parameters** | [**SocialPostAttachmentDtoCollectionQueryParameters**](SocialPostAttachmentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SocialPostAttachmentDtoListEnvelope**](SocialPostAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_post_attachments_count_async

> <Int32Envelope> get_social_post_attachments_count_async(social_post_id, opts)

Count social post attachments

Returns the count of attachments for a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_attachment_dto_collection_query_parameters: OpenapiClient::SocialPostAttachmentDtoCollectionQueryParameters.new # SocialPostAttachmentDtoCollectionQueryParameters | 
}

begin
  # Count social post attachments
  result = api_instance.get_social_post_attachments_count_async(social_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_attachments_count_async: #{e}"
end
```

#### Using the get_social_post_attachments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_social_post_attachments_count_async_with_http_info(social_post_id, opts)

```ruby
begin
  # Count social post attachments
  data, status_code, headers = api_instance.get_social_post_attachments_count_async_with_http_info(social_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_attachments_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_attachment_dto_collection_query_parameters** | [**SocialPostAttachmentDtoCollectionQueryParameters**](SocialPostAttachmentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_post_comment_async

> <SocialPostCommentDtoEnvelope> get_social_post_comment_async(social_profile_id, social_post_id, comment_id, opts)

Get social post comment by ID

Retrieves a specific comment from a social post by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social post comment by ID
  result = api_instance.get_social_post_comment_async(social_profile_id, social_post_id, comment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_comment_async: #{e}"
end
```

#### Using the get_social_post_comment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostCommentDtoEnvelope>, Integer, Hash)> get_social_post_comment_async_with_http_info(social_profile_id, social_post_id, comment_id, opts)

```ruby
begin
  # Get social post comment by ID
  data, status_code, headers = api_instance.get_social_post_comment_async_with_http_info(social_profile_id, social_post_id, comment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostCommentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_comment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialPostCommentDtoEnvelope**](SocialPostCommentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_post_comments_async

> <SocialPostCommentDtoListEnvelope> get_social_post_comments_async(social_profile_id, social_post_id, opts)

Get social post comments

Retrieves a list of comments for a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  parent_comment_id: 'parent_comment_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_comment_dto_collection_query_parameters: OpenapiClient::SocialPostCommentDtoCollectionQueryParameters.new # SocialPostCommentDtoCollectionQueryParameters | 
}

begin
  # Get social post comments
  result = api_instance.get_social_post_comments_async(social_profile_id, social_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_comments_async: #{e}"
end
```

#### Using the get_social_post_comments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostCommentDtoListEnvelope>, Integer, Hash)> get_social_post_comments_async_with_http_info(social_profile_id, social_post_id, opts)

```ruby
begin
  # Get social post comments
  data, status_code, headers = api_instance.get_social_post_comments_async_with_http_info(social_profile_id, social_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostCommentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_comments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **parent_comment_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_comment_dto_collection_query_parameters** | [**SocialPostCommentDtoCollectionQueryParameters**](SocialPostCommentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SocialPostCommentDtoListEnvelope**](SocialPostCommentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_post_comments_count_async

> <Int32Envelope> get_social_post_comments_count_async(social_profile_id, social_post_id, opts)

Count social post comments

Returns the count of comments for a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  parent_comment_id: 'parent_comment_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_comment_dto_collection_query_parameters: OpenapiClient::SocialPostCommentDtoCollectionQueryParameters.new # SocialPostCommentDtoCollectionQueryParameters | 
}

begin
  # Count social post comments
  result = api_instance.get_social_post_comments_count_async(social_profile_id, social_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_comments_count_async: #{e}"
end
```

#### Using the get_social_post_comments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_social_post_comments_count_async_with_http_info(social_profile_id, social_post_id, opts)

```ruby
begin
  # Count social post comments
  data, status_code, headers = api_instance.get_social_post_comments_count_async_with_http_info(social_profile_id, social_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_comments_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **parent_comment_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_comment_dto_collection_query_parameters** | [**SocialPostCommentDtoCollectionQueryParameters**](SocialPostCommentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_post_reaction_async

> <SocialReactionDtoEnvelope> get_social_post_reaction_async(social_post_id, reaction_id, opts)

Get social post reaction by ID

Retrieves a specific reaction from a social post by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get social post reaction by ID
  result = api_instance.get_social_post_reaction_async(social_post_id, reaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_reaction_async: #{e}"
end
```

#### Using the get_social_post_reaction_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialReactionDtoEnvelope>, Integer, Hash)> get_social_post_reaction_async_with_http_info(social_post_id, reaction_id, opts)

```ruby
begin
  # Get social post reaction by ID
  data, status_code, headers = api_instance.get_social_post_reaction_async_with_http_info(social_post_id, reaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialReactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_reaction_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **reaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialReactionDtoEnvelope**](SocialReactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_social_post_reactions_async

> <SocialReactionDtoListEnvelope> get_social_post_reactions_async(social_post_id, social_profile_id, opts)

Get social post reactions

Retrieves a list of reactions for a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_reaction_dto_collection_query_parameters: OpenapiClient::SocialPostReactionDtoCollectionQueryParameters.new # SocialPostReactionDtoCollectionQueryParameters | 
}

begin
  # Get social post reactions
  result = api_instance.get_social_post_reactions_async(social_post_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_reactions_async: #{e}"
end
```

#### Using the get_social_post_reactions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialReactionDtoListEnvelope>, Integer, Hash)> get_social_post_reactions_async_with_http_info(social_post_id, social_profile_id, opts)

```ruby
begin
  # Get social post reactions
  data, status_code, headers = api_instance.get_social_post_reactions_async_with_http_info(social_post_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialReactionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_reactions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_reaction_dto_collection_query_parameters** | [**SocialPostReactionDtoCollectionQueryParameters**](SocialPostReactionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SocialReactionDtoListEnvelope**](SocialReactionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_post_reactions_count_async

> <Int32Envelope> get_social_post_reactions_count_async(social_post_id, social_profile_id, opts)

Count social post reactions

Returns the count of reactions for a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_reaction_dto_collection_query_parameters: OpenapiClient::SocialPostReactionDtoCollectionQueryParameters.new # SocialPostReactionDtoCollectionQueryParameters | 
}

begin
  # Count social post reactions
  result = api_instance.get_social_post_reactions_count_async(social_post_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_reactions_count_async: #{e}"
end
```

#### Using the get_social_post_reactions_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_social_post_reactions_count_async_with_http_info(social_post_id, social_profile_id, opts)

```ruby
begin
  # Count social post reactions
  data, status_code, headers = api_instance.get_social_post_reactions_count_async_with_http_info(social_post_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_post_reactions_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_reaction_dto_collection_query_parameters** | [**SocialPostReactionDtoCollectionQueryParameters**](SocialPostReactionDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_posts_async

> <SocialPostDtoListEnvelope> get_social_posts_async(social_profile_id, opts)

Get social posts

Retrieves a list of social posts for the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_dto_collection_query_parameters: OpenapiClient::SocialPostDtoCollectionQueryParameters.new # SocialPostDtoCollectionQueryParameters | 
}

begin
  # Get social posts
  result = api_instance.get_social_posts_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_posts_async: #{e}"
end
```

#### Using the get_social_posts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostDtoListEnvelope>, Integer, Hash)> get_social_posts_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get social posts
  data, status_code, headers = api_instance.get_social_posts_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_posts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_dto_collection_query_parameters** | [**SocialPostDtoCollectionQueryParameters**](SocialPostDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SocialPostDtoListEnvelope**](SocialPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_social_posts_count_async

> <Int32Envelope> get_social_posts_count_async(social_profile_id, opts)

Count social posts

Returns the count of social posts for the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_dto_collection_query_parameters: OpenapiClient::SocialPostDtoCollectionQueryParameters.new # SocialPostDtoCollectionQueryParameters | 
}

begin
  # Count social posts
  result = api_instance.get_social_posts_count_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_posts_count_async: #{e}"
end
```

#### Using the get_social_posts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_social_posts_count_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Count social posts
  data, status_code, headers = api_instance.get_social_posts_count_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->get_social_posts_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_dto_collection_query_parameters** | [**SocialPostDtoCollectionQueryParameters**](SocialPostDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_social_post_async

> <EmptyEnvelope> patch_social_post_async(social_profile_id, social_post_id, opts)

Patch a social post

Partially updates an existing social post by its ID using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a social post
  result = api_instance.patch_social_post_async(social_profile_id, social_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->patch_social_post_async: #{e}"
end
```

#### Using the patch_social_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_social_post_async_with_http_info(social_profile_id, social_post_id, opts)

```ruby
begin
  # Patch a social post
  data, status_code, headers = api_instance.patch_social_post_async_with_http_info(social_profile_id, social_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->patch_social_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
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


## update_social_comment_reaction_async

> <SocialCommentReactionDtoEnvelope> update_social_comment_reaction_async(social_post_id, comment_id, reaction_id, social_profile_id, opts)

Update a social comment reaction

Updates an existing reaction on a specific social comment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_reaction_update_dto: OpenapiClient::SocialReactionUpdateDto.new # SocialReactionUpdateDto | 
}

begin
  # Update a social comment reaction
  result = api_instance.update_social_comment_reaction_async(social_post_id, comment_id, reaction_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_comment_reaction_async: #{e}"
end
```

#### Using the update_social_comment_reaction_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialCommentReactionDtoEnvelope>, Integer, Hash)> update_social_comment_reaction_async_with_http_info(social_post_id, comment_id, reaction_id, social_profile_id, opts)

```ruby
begin
  # Update a social comment reaction
  data, status_code, headers = api_instance.update_social_comment_reaction_async_with_http_info(social_post_id, comment_id, reaction_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialCommentReactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_comment_reaction_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **reaction_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_reaction_update_dto** | [**SocialReactionUpdateDto**](SocialReactionUpdateDto.md) |  | [optional] |

### Return type

[**SocialCommentReactionDtoEnvelope**](SocialCommentReactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_social_post_async

> <EmptyEnvelope> update_social_post_async(social_profile_id, social_post_id, opts)

Update a social post

Updates an existing social post by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_update_dto: OpenapiClient::SocialPostUpdateDto.new # SocialPostUpdateDto | 
}

begin
  # Update a social post
  result = api_instance.update_social_post_async(social_profile_id, social_post_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_post_async: #{e}"
end
```

#### Using the update_social_post_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_social_post_async_with_http_info(social_profile_id, social_post_id, opts)

```ruby
begin
  # Update a social post
  data, status_code, headers = api_instance.update_social_post_async_with_http_info(social_profile_id, social_post_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_post_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_update_dto** | [**SocialPostUpdateDto**](SocialPostUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_social_post_attachment_async

> <EmptyEnvelope> update_social_post_attachment_async(social_profile_id, social_post_id, attachment_id, opts)

Update a social post attachment

Updates an existing attachment on a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_attachment_update_dto: OpenapiClient::SocialPostAttachmentUpdateDto.new # SocialPostAttachmentUpdateDto | 
}

begin
  # Update a social post attachment
  result = api_instance.update_social_post_attachment_async(social_profile_id, social_post_id, attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_post_attachment_async: #{e}"
end
```

#### Using the update_social_post_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_social_post_attachment_async_with_http_info(social_profile_id, social_post_id, attachment_id, opts)

```ruby
begin
  # Update a social post attachment
  data, status_code, headers = api_instance.update_social_post_attachment_async_with_http_info(social_profile_id, social_post_id, attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_post_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_attachment_update_dto** | [**SocialPostAttachmentUpdateDto**](SocialPostAttachmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_social_post_comment_async

> <EmptyEnvelope> update_social_post_comment_async(social_profile_id, social_post_id, comment_id, opts)

Update a social post comment

Updates an existing comment on a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
comment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_post_comment_update_dto: OpenapiClient::SocialPostCommentUpdateDto.new # SocialPostCommentUpdateDto | 
}

begin
  # Update a social post comment
  result = api_instance.update_social_post_comment_async(social_profile_id, social_post_id, comment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_post_comment_async: #{e}"
end
```

#### Using the update_social_post_comment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_social_post_comment_async_with_http_info(social_profile_id, social_post_id, comment_id, opts)

```ruby
begin
  # Update a social post comment
  data, status_code, headers = api_instance.update_social_post_comment_async_with_http_info(social_profile_id, social_post_id, comment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_post_comment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **comment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_post_comment_update_dto** | [**SocialPostCommentUpdateDto**](SocialPostCommentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_social_post_reaction_async

> <SocialPostReactionDtoEnvelope> update_social_post_reaction_async(social_profile_id, social_post_id, reaction_id, opts)

Update a social post reaction

Updates an existing reaction on a specific social post.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reaction_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  social_reaction_update_dto: OpenapiClient::SocialReactionUpdateDto.new # SocialReactionUpdateDto | 
}

begin
  # Update a social post reaction
  result = api_instance.update_social_post_reaction_async(social_profile_id, social_post_id, reaction_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_post_reaction_async: #{e}"
end
```

#### Using the update_social_post_reaction_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostReactionDtoEnvelope>, Integer, Hash)> update_social_post_reaction_async_with_http_info(social_profile_id, social_post_id, reaction_id, opts)

```ruby
begin
  # Update a social post reaction
  data, status_code, headers = api_instance.update_social_post_reaction_async_with_http_info(social_profile_id, social_post_id, reaction_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostReactionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->update_social_post_reaction_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **social_post_id** | **String** |  |  |
| **reaction_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **social_reaction_update_dto** | [**SocialReactionUpdateDto**](SocialReactionUpdateDto.md) |  | [optional] |

### Return type

[**SocialPostReactionDtoEnvelope**](SocialPostReactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## upload_social_post_image_attachment_async

> <SocialPostAttachmentDtoEnvelope> upload_social_post_image_attachment_async(social_post_id, social_profile_id, opts)

Upload a social post image attachment

Uploads an image and attaches it to a social post, storing the bytes through the storage spine.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SocialPostsApi.new
social_post_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload a social post image attachment
  result = api_instance.upload_social_post_image_attachment_async(social_post_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->upload_social_post_image_attachment_async: #{e}"
end
```

#### Using the upload_social_post_image_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialPostAttachmentDtoEnvelope>, Integer, Hash)> upload_social_post_image_attachment_async_with_http_info(social_post_id, social_profile_id, opts)

```ruby
begin
  # Upload a social post image attachment
  data, status_code, headers = api_instance.upload_social_post_image_attachment_async_with_http_info(social_post_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialPostAttachmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SocialPostsApi->upload_social_post_image_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_post_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |

### Return type

[**SocialPostAttachmentDtoEnvelope**](SocialPostAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml

