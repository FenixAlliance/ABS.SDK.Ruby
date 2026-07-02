# OpenapiClient::OptionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_user_option**](OptionsApi.md#create_user_option) | **POST** /api/v2/Me/Options | Create a new user option |
| [**delete_user_option**](OptionsApi.md#delete_user_option) | **DELETE** /api/v2/Me/Options/{optionId} | Delete a user option |
| [**get_user_option_by_id**](OptionsApi.md#get_user_option_by_id) | **GET** /api/v2/Me/Options/{optionId} | Retrieve a single user option by its ID |
| [**get_user_option_by_key**](OptionsApi.md#get_user_option_by_key) | **GET** /api/v2/Me/Options/Key/{key} | Retrieve a single user option by its key |
| [**get_user_options**](OptionsApi.md#get_user_options) | **GET** /api/v2/Me/Options | Retrieve a list of user options |
| [**get_user_options_count**](OptionsApi.md#get_user_options_count) | **GET** /api/v2/Me/Options/Count | Get the count of user options |
| [**patch_user_option**](OptionsApi.md#patch_user_option) | **PATCH** /api/v2/Me/Options/{optionId} | Patch a user option |
| [**update_user_option**](OptionsApi.md#update_user_option) | **PUT** /api/v2/Me/Options/{optionId} | Update a user option |
| [**upsert_user_option**](OptionsApi.md#upsert_user_option) | **PUT** /api/v2/Me/Options/Upsert/{key} | Create or update a user option by key |


## create_user_option

> <EmptyEnvelope> create_user_option(key, opts)

Create a new user option

Create a new option for the current user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_create_dto: OpenapiClient::OptionCreateDto.new({key: 'key_example', value: 'value_example'}) # OptionCreateDto | 
}

begin
  # Create a new user option
  result = api_instance.create_user_option(key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->create_user_option: #{e}"
end
```

#### Using the create_user_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_user_option_with_http_info(key, opts)

```ruby
begin
  # Create a new user option
  data, status_code, headers = api_instance.create_user_option_with_http_info(key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->create_user_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## delete_user_option

> <EmptyEnvelope> delete_user_option(option_id, opts)

Delete a user option

Delete a user option

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a user option
  result = api_instance.delete_user_option(option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->delete_user_option: #{e}"
end
```

#### Using the delete_user_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_user_option_with_http_info(option_id, opts)

```ruby
begin
  # Delete a user option
  data, status_code, headers = api_instance.delete_user_option_with_http_info(option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->delete_user_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## get_user_option_by_id

> <OptionDtoEnvelope> get_user_option_by_id(option_id, opts)

Retrieve a single user option by its ID

Retrieve a single user option by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single user option by its ID
  result = api_instance.get_user_option_by_id(option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_user_option_by_id: #{e}"
end
```

#### Using the get_user_option_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_user_option_by_id_with_http_info(option_id, opts)

```ruby
begin
  # Retrieve a single user option by its ID
  data, status_code, headers = api_instance.get_user_option_by_id_with_http_info(option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_user_option_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## get_user_option_by_key

> <OptionDtoEnvelope> get_user_option_by_key(key, opts)

Retrieve a single user option by its key

Retrieve a single user option by its key

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single user option by its key
  result = api_instance.get_user_option_by_key(key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_user_option_by_key: #{e}"
end
```

#### Using the get_user_option_by_key_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_user_option_by_key_with_http_info(key, opts)

```ruby
begin
  # Retrieve a single user option by its key
  data, status_code, headers = api_instance.get_user_option_by_key_with_http_info(key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_user_option_by_key_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key** | **String** |  |  |
| **portal_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OptionDtoEnvelope**](OptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_user_options

> <OptionDtoListEnvelope> get_user_options(opts)

Retrieve a list of user options

Retrieve a list of options for the current user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of user options
  result = api_instance.get_user_options(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_user_options: #{e}"
end
```

#### Using the get_user_options_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoListEnvelope>, Integer, Hash)> get_user_options_with_http_info(opts)

```ruby
begin
  # Retrieve a list of user options
  data, status_code, headers = api_instance.get_user_options_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_user_options_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## get_user_options_count

> <Int32Envelope> get_user_options_count(opts)

Get the count of user options

Get the count of options for the current user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of user options
  result = api_instance.get_user_options_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_user_options_count: #{e}"
end
```

#### Using the get_user_options_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_user_options_count_with_http_info(opts)

```ruby
begin
  # Get the count of user options
  data, status_code, headers = api_instance.get_user_options_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_user_options_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## patch_user_option

> <EmptyEnvelope> patch_user_option(option_id, opts)

Patch a user option

Partially updates a user option using a JSON Patch document

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a user option
  result = api_instance.patch_user_option(option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->patch_user_option: #{e}"
end
```

#### Using the patch_user_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_user_option_with_http_info(option_id, opts)

```ruby
begin
  # Patch a user option
  data, status_code, headers = api_instance.patch_user_option_with_http_info(option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->patch_user_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **option_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_user_option

> <EmptyEnvelope> update_user_option(option_id, opts)

Update a user option

Update a user option

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_update_dto: OpenapiClient::OptionUpdateDto.new # OptionUpdateDto | 
}

begin
  # Update a user option
  result = api_instance.update_user_option(option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->update_user_option: #{e}"
end
```

#### Using the update_user_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_user_option_with_http_info(option_id, opts)

```ruby
begin
  # Update a user option
  data, status_code, headers = api_instance.update_user_option_with_http_info(option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->update_user_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## upsert_user_option

> <EmptyEnvelope> upsert_user_option(key, opts)

Create or update a user option by key

Create or update a user option by key

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_update_dto: OpenapiClient::OptionUpdateDto.new # OptionUpdateDto | 
}

begin
  # Create or update a user option by key
  result = api_instance.upsert_user_option(key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->upsert_user_option: #{e}"
end
```

#### Using the upsert_user_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> upsert_user_option_with_http_info(key, opts)

```ruby
begin
  # Create or update a user option by key
  data, status_code, headers = api_instance.upsert_user_option_with_http_info(key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->upsert_user_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key** | **String** |  |  |
| **portal_id** | **String** |  | [optional] |
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

