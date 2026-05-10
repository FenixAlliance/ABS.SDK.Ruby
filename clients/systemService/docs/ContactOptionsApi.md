# OpenapiClient::ContactOptionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_system_contact_option**](ContactOptionsApi.md#create_system_contact_option) | **POST** /api/v2/SystemService/Contacts/{contactId}/Options | Create a new contact option (admin) |
| [**delete_system_contact_option**](ContactOptionsApi.md#delete_system_contact_option) | **DELETE** /api/v2/SystemService/Contacts/{contactId}/Options/{optionId} | Delete a contact option (admin) |
| [**get_system_contact_option_by_id**](ContactOptionsApi.md#get_system_contact_option_by_id) | **GET** /api/v2/SystemService/Contacts/{contactId}/Options/{optionId} | Retrieve a single contact option by its ID (admin) |
| [**get_system_contact_options**](ContactOptionsApi.md#get_system_contact_options) | **GET** /api/v2/SystemService/Contacts/{contactId}/Options | Retrieve a list of contact options (admin) |
| [**get_system_contact_options_count**](ContactOptionsApi.md#get_system_contact_options_count) | **GET** /api/v2/SystemService/Contacts/{contactId}/Options/Count | Get the count of contact options (admin) |
| [**update_system_contact_option**](ContactOptionsApi.md#update_system_contact_option) | **PUT** /api/v2/SystemService/Contacts/{contactId}/Options/{optionId} | Update a contact option (admin) |


## create_system_contact_option

> <EmptyEnvelope> create_system_contact_option(contact_id, key, opts)

Create a new contact option (admin)

Admin endpoint to create an option for any contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactOptionsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_create_dto: OpenapiClient::OptionCreateDto.new({key: 'key_example', value: 'value_example'}) # OptionCreateDto | 
}

begin
  # Create a new contact option (admin)
  result = api_instance.create_system_contact_option(contact_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->create_system_contact_option: #{e}"
end
```

#### Using the create_system_contact_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_system_contact_option_with_http_info(contact_id, key, opts)

```ruby
begin
  # Create a new contact option (admin)
  data, status_code, headers = api_instance.create_system_contact_option_with_http_info(contact_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->create_system_contact_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **key** | **String** |  |  |
| **portal_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **option_create_dto** | [**OptionCreateDto**](OptionCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_system_contact_option

> <EmptyEnvelope> delete_system_contact_option(contact_id, option_id, opts)

Delete a contact option (admin)

Admin endpoint to delete an option for any contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactOptionsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact option (admin)
  result = api_instance.delete_system_contact_option(contact_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->delete_system_contact_option: #{e}"
end
```

#### Using the delete_system_contact_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_system_contact_option_with_http_info(contact_id, option_id, opts)

```ruby
begin
  # Delete a contact option (admin)
  data, status_code, headers = api_instance.delete_system_contact_option_with_http_info(contact_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->delete_system_contact_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **option_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_contact_option_by_id

> <OptionDtoEnvelope> get_system_contact_option_by_id(contact_id, option_id, opts)

Retrieve a single contact option by its ID (admin)

Admin endpoint to retrieve a single option for any contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactOptionsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single contact option by its ID (admin)
  result = api_instance.get_system_contact_option_by_id(contact_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->get_system_contact_option_by_id: #{e}"
end
```

#### Using the get_system_contact_option_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_system_contact_option_by_id_with_http_info(contact_id, option_id, opts)

```ruby
begin
  # Retrieve a single contact option by its ID (admin)
  data, status_code, headers = api_instance.get_system_contact_option_by_id_with_http_info(contact_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->get_system_contact_option_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **option_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OptionDtoEnvelope**](OptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_contact_options

> <OptionDtoListEnvelope> get_system_contact_options(contact_id, opts)

Retrieve a list of contact options (admin)

Admin endpoint to retrieve options for any contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactOptionsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of contact options (admin)
  result = api_instance.get_system_contact_options(contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->get_system_contact_options: #{e}"
end
```

#### Using the get_system_contact_options_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoListEnvelope>, Integer, Hash)> get_system_contact_options_with_http_info(contact_id, opts)

```ruby
begin
  # Retrieve a list of contact options (admin)
  data, status_code, headers = api_instance.get_system_contact_options_with_http_info(contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->get_system_contact_options_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **portal_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OptionDtoListEnvelope**](OptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_contact_options_count

> <Int32Envelope> get_system_contact_options_count(contact_id, opts)

Get the count of contact options (admin)

Admin endpoint to get the count of options for any contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactOptionsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of contact options (admin)
  result = api_instance.get_system_contact_options_count(contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->get_system_contact_options_count: #{e}"
end
```

#### Using the get_system_contact_options_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_system_contact_options_count_with_http_info(contact_id, opts)

```ruby
begin
  # Get the count of contact options (admin)
  data, status_code, headers = api_instance.get_system_contact_options_count_with_http_info(contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->get_system_contact_options_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **portal_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_system_contact_option

> <EmptyEnvelope> update_system_contact_option(contact_id, option_id, opts)

Update a contact option (admin)

Admin endpoint to update an option for any contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactOptionsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_update_dto: OpenapiClient::OptionUpdateDto.new # OptionUpdateDto | 
}

begin
  # Update a contact option (admin)
  result = api_instance.update_system_contact_option(contact_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->update_system_contact_option: #{e}"
end
```

#### Using the update_system_contact_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_system_contact_option_with_http_info(contact_id, option_id, opts)

```ruby
begin
  # Update a contact option (admin)
  data, status_code, headers = api_instance.update_system_contact_option_with_http_info(contact_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactOptionsApi->update_system_contact_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **option_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **option_update_dto** | [**OptionUpdateDto**](OptionUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

