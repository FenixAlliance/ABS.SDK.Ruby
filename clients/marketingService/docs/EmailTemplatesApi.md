# OpenapiClient::EmailTemplatesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_email_template_async**](EmailTemplatesApi.md#create_email_template_async) | **POST** /api/v2/MarketingService/EmailTemplates | Create an email template |
| [**delete_email_template_async**](EmailTemplatesApi.md#delete_email_template_async) | **DELETE** /api/v2/MarketingService/EmailTemplates/{emailTemplateId} | Delete an email template |
| [**get_email_template_details_async**](EmailTemplatesApi.md#get_email_template_details_async) | **GET** /api/v2/MarketingService/EmailTemplates/{emailTemplateId} | Get email template by ID |
| [**get_email_templates_count_async**](EmailTemplatesApi.md#get_email_templates_count_async) | **GET** /api/v2/MarketingService/EmailTemplates/Count | Get email templates count |
| [**get_email_templates_o_data_async**](EmailTemplatesApi.md#get_email_templates_o_data_async) | **GET** /api/v2/MarketingService/EmailTemplates | Get email templates |
| [**update_email_template_async**](EmailTemplatesApi.md#update_email_template_async) | **PUT** /api/v2/MarketingService/EmailTemplates/{emailTemplateId} | Update an email template |


## create_email_template_async

> <EmptyEnvelope> create_email_template_async(tenant_id, email_template_create_dto, opts)

Create an email template

Creates a new email template for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_template_create_dto = OpenapiClient::EmailTemplateCreateDto.new({title: 'title_example'}) # EmailTemplateCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create an email template
  result = api_instance.create_email_template_async(tenant_id, email_template_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->create_email_template_async: #{e}"
end
```

#### Using the create_email_template_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_email_template_async_with_http_info(tenant_id, email_template_create_dto, opts)

```ruby
begin
  # Create an email template
  data, status_code, headers = api_instance.create_email_template_async_with_http_info(tenant_id, email_template_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->create_email_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **email_template_create_dto** | [**EmailTemplateCreateDto**](EmailTemplateCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_email_template_async

> <EmptyEnvelope> delete_email_template_async(tenant_id, email_template_id, opts)

Delete an email template

Deletes an email template by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an email template
  result = api_instance.delete_email_template_async(tenant_id, email_template_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->delete_email_template_async: #{e}"
end
```

#### Using the delete_email_template_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_email_template_async_with_http_info(tenant_id, email_template_id, opts)

```ruby
begin
  # Delete an email template
  data, status_code, headers = api_instance.delete_email_template_async_with_http_info(tenant_id, email_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->delete_email_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **email_template_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_email_template_details_async

> <EmailTemplateDtoEnvelope> get_email_template_details_async(tenant_id, email_template_id, opts)

Get email template by ID

Retrieves the details of a specific email template by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get email template by ID
  result = api_instance.get_email_template_details_async(tenant_id, email_template_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->get_email_template_details_async: #{e}"
end
```

#### Using the get_email_template_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmailTemplateDtoEnvelope>, Integer, Hash)> get_email_template_details_async_with_http_info(tenant_id, email_template_id, opts)

```ruby
begin
  # Get email template by ID
  data, status_code, headers = api_instance.get_email_template_details_async_with_http_info(tenant_id, email_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmailTemplateDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->get_email_template_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **email_template_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmailTemplateDtoEnvelope**](EmailTemplateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_email_templates_count_async

> <Int32Envelope> get_email_templates_count_async(tenant_id, opts)

Get email templates count

Returns the count of email templates for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get email templates count
  result = api_instance.get_email_templates_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->get_email_templates_count_async: #{e}"
end
```

#### Using the get_email_templates_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_email_templates_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get email templates count
  data, status_code, headers = api_instance.get_email_templates_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->get_email_templates_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_email_templates_o_data_async

> <EmailTemplateDtoListEnvelope> get_email_templates_o_data_async(tenant_id, opts)

Get email templates

Retrieves a collection of email templates for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get email templates
  result = api_instance.get_email_templates_o_data_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->get_email_templates_o_data_async: #{e}"
end
```

#### Using the get_email_templates_o_data_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmailTemplateDtoListEnvelope>, Integer, Hash)> get_email_templates_o_data_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get email templates
  data, status_code, headers = api_instance.get_email_templates_o_data_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmailTemplateDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->get_email_templates_o_data_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmailTemplateDtoListEnvelope**](EmailTemplateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_email_template_async

> <EmptyEnvelope> update_email_template_async(tenant_id, email_template_id, email_template_update_dto, opts)

Update an email template

Updates an existing email template by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmailTemplatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_template_update_dto = OpenapiClient::EmailTemplateUpdateDto.new # EmailTemplateUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update an email template
  result = api_instance.update_email_template_async(tenant_id, email_template_id, email_template_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->update_email_template_async: #{e}"
end
```

#### Using the update_email_template_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_email_template_async_with_http_info(tenant_id, email_template_id, email_template_update_dto, opts)

```ruby
begin
  # Update an email template
  data, status_code, headers = api_instance.update_email_template_async_with_http_info(tenant_id, email_template_id, email_template_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmailTemplatesApi->update_email_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **email_template_id** | **String** |  |  |
| **email_template_update_dto** | [**EmailTemplateUpdateDto**](EmailTemplateUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

