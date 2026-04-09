# OpenapiClient::ObjectEmailDispatchRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **title** | **String** |  |  |
| **message** | **String** |  |  |
| **button_link** | **String** |  | [optional] |
| **button_text** | **String** |  | [optional] |
| **alert_message** | **String** |  | [optional] |
| **alert_type** | **String** |  | [optional] |
| **culture** | **String** |  |  |
| **ui_culture** | **String** |  |  |
| **recipients** | **Array&lt;String&gt;** |  |  |
| **contact_ids** | **Array&lt;String&gt;** |  | [optional] |
| **tenant_ids** | **Array&lt;String&gt;** |  | [optional] |
| **user_ids** | **Array&lt;String&gt;** |  | [optional] |
| **template_url** | **String** |  | [optional] |
| **email_template_id** | **String** |  | [optional] |
| **payload** | **Object** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ObjectEmailDispatchRequest.new(
  title: null,
  message: null,
  button_link: null,
  button_text: null,
  alert_message: null,
  alert_type: null,
  culture: null,
  ui_culture: null,
  recipients: null,
  contact_ids: null,
  tenant_ids: null,
  user_ids: null,
  template_url: null,
  email_template_id: null,
  payload: null
)
```

