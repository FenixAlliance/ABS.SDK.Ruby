# OpenapiClient::SocialPostCommentDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **message** | **String** |  | [optional] |
| **parent_comment_id** | **String** |  | [optional] |
| **social_profile_id** | **String** |  | [optional] |
| **social_feed_post_id** | **String** |  | [optional] |
| **social_profile_name** | **String** |  | [optional] |
| **social_profile_avatar_url** | **String** |  | [optional] |
| **social_profile_type** | **String** |  | [optional] |
| **body_html** | **String** |  | [optional] |
| **body_format** | **String** |  | [optional] |
| **reply_count** | **Integer** |  | [optional] |
| **reactions_count** | **Integer** |  | [optional] |
| **social_post_id** | **String** |  | [optional] |
| **facepile** | [**Array&lt;SocialPostReactionFacepileDto&gt;**](SocialPostReactionFacepileDto.md) |  | [optional] |
| **my_reaction** | **String** |  | [optional] |
| **my_reaction_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SocialPostCommentDto.new(
  id: null,
  timestamp: null,
  message: null,
  parent_comment_id: null,
  social_profile_id: null,
  social_feed_post_id: null,
  social_profile_name: null,
  social_profile_avatar_url: null,
  social_profile_type: null,
  body_html: null,
  body_format: null,
  reply_count: null,
  reactions_count: null,
  social_post_id: null,
  facepile: null,
  my_reaction: null,
  my_reaction_id: null
)
```

