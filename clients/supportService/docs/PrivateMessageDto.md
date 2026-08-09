# OpenapiClient::PrivateMessageDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **read** | **Boolean** |  | [optional] |
| **title** | **String** |  | [optional] |
| **message** | **String** |  | [optional] |
| **conversation_id** | **String** |  | [optional] |
| **sender_social_profile_id** | **String** |  | [optional] |
| **receiver_social_profile_id** | **String** |  | [optional] |
| **sent_timestamp** | **Time** |  | [optional] |
| **read_timestamp** | **Time** |  | [optional] |
| **received_timestamp** | **Time** |  | [optional] |
| **social_profile_name** | **String** |  | [optional] |
| **social_profile_avatar_url** | **String** |  | [optional] |
| **social_profile_type** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PrivateMessageDto.new(
  id: null,
  timestamp: null,
  read: null,
  title: null,
  message: null,
  conversation_id: null,
  sender_social_profile_id: null,
  receiver_social_profile_id: null,
  sent_timestamp: null,
  read_timestamp: null,
  received_timestamp: null,
  social_profile_name: null,
  social_profile_avatar_url: null,
  social_profile_type: null
)
```

