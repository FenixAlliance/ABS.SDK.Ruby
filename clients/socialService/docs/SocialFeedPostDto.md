# OpenapiClient::SocialFeedPostDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  | [optional] |
| **message** | **String** |  | [optional] |
| **social_profile_id** | **String** |  | [optional] |
| **social_profile_name** | **String** |  | [optional] |
| **social_profile_avatar_url** | **String** |  | [optional] |
| **comments_count** | **Integer** |  | [optional] |
| **reactions_count** | **Integer** |  | [optional] |
| **social_profile_type** | **String** |  | [optional] |
| **body_html** | **String** |  | [optional] |
| **body_format** | **String** |  | [optional] |
| **background_style** | **String** |  | [optional] |
| **social_feed_id** | **String** |  | [optional] |
| **facepile** | [**Array&lt;SocialPostReactionFacepileDto&gt;**](SocialPostReactionFacepileDto.md) |  | [optional] |
| **attachments** | [**Array&lt;SocialPostAttachmentRefDto&gt;**](SocialPostAttachmentRefDto.md) |  | [optional] |
| **my_reaction** | **String** |  | [optional] |
| **my_reaction_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SocialFeedPostDto.new(
  id: null,
  timestamp: null,
  title: null,
  message: null,
  social_profile_id: null,
  social_profile_name: null,
  social_profile_avatar_url: null,
  comments_count: null,
  reactions_count: null,
  social_profile_type: null,
  body_html: null,
  body_format: null,
  background_style: null,
  social_feed_id: null,
  facepile: null,
  attachments: null,
  my_reaction: null,
  my_reaction_id: null
)
```

