# OpenapiClient::BlogPostCommentCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **message** | **String** |  |  |
| **owner_social_profile_id** | **String** |  | [optional] |
| **social_post_id** | **String** |  | [optional] |
| **parent_comment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BlogPostCommentCreateDto.new(
  id: null,
  timestamp: null,
  message: null,
  owner_social_profile_id: null,
  social_post_id: null,
  parent_comment_id: null
)
```

