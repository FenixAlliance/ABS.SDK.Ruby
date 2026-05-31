# OpenapiClient::EmailsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**admin_preview_basic_email_template**](EmailsApi.md#admin_preview_basic_email_template) | **POST** /api/v2/SystemService/Emails/Preview | Preview a rendered basic email template. |
| [**admin_send_basic_email**](EmailsApi.md#admin_send_basic_email) | **POST** /api/v2/SystemService/Emails/SendBasic | Send a basic transactional email to recipients. |


## admin_preview_basic_email_template

> admin_preview_basic_email_template(opts)

Preview a rendered basic email template.

This action is only available for global administrators (business_owner role).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  object_email_dispatch_request: OpenapiClient::ObjectEmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # ObjectEmailDispatchRequest | 
}

begin
  # Preview a rendered basic email template.
  api_instance.admin_preview_basic_email_template(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailsApi->admin_preview_basic_email_template: #{e}"
end
```

#### Using the admin_preview_basic_email_template_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> admin_preview_basic_email_template_with_http_info(opts)

```ruby
begin
  # Preview a rendered basic email template.
  data, status_code, headers = api_instance.admin_preview_basic_email_template_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailsApi->admin_preview_basic_email_template_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **object_email_dispatch_request** | [**ObjectEmailDispatchRequest**](ObjectEmailDispatchRequest.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined


## admin_send_basic_email

> <Envelope> admin_send_basic_email(opts)

Send a basic transactional email to recipients.

This action is only available for global administrators (business_owner role).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  object_email_dispatch_request: OpenapiClient::ObjectEmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # ObjectEmailDispatchRequest | 
}

begin
  # Send a basic transactional email to recipients.
  result = api_instance.admin_send_basic_email(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailsApi->admin_send_basic_email: #{e}"
end
```

#### Using the admin_send_basic_email_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> admin_send_basic_email_with_http_info(opts)

```ruby
begin
  # Send a basic transactional email to recipients.
  data, status_code, headers = api_instance.admin_send_basic_email_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailsApi->admin_send_basic_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **object_email_dispatch_request** | [**ObjectEmailDispatchRequest**](ObjectEmailDispatchRequest.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

