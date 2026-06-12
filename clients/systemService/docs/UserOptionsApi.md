# OpenapiClient::UserOptionsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_system_user_option**](UserOptionsApi.md#create_system_user_option) | **POST** /api/v2/SystemService/Users/{userId}/Options | Create a new user option (admin) |
| [**delete_system_user_option**](UserOptionsApi.md#delete_system_user_option) | **DELETE** /api/v2/SystemService/Users/{userId}/Options/{optionId} | Delete a user option (admin) |
| [**get_system_user_option_by_id**](UserOptionsApi.md#get_system_user_option_by_id) | **GET** /api/v2/SystemService/Users/{userId}/Options/{optionId} | Retrieve a single user option by its ID (admin) |
| [**get_system_user_options**](UserOptionsApi.md#get_system_user_options) | **GET** /api/v2/SystemService/Users/{userId}/Options | Retrieve a list of user options (admin) |
| [**get_system_user_options_count**](UserOptionsApi.md#get_system_user_options_count) | **GET** /api/v2/SystemService/Users/{userId}/Options/Count | Get the count of user options (admin) |
| [**patch_system_user_option**](UserOptionsApi.md#patch_system_user_option) | **PATCH** /api/v2/SystemService/Users/{userId}/Options/{optionId} | Partially update a user option (admin) |
| [**update_system_user_option**](UserOptionsApi.md#update_system_user_option) | **PUT** /api/v2/SystemService/Users/{userId}/Options/{optionId} | Update a user option (admin) |


## create_system_user_option

> <EmptyEnvelope> create_system_user_option(user_id, key, opts)

Create a new user option (admin)

Admin endpoint to create an option for any user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UserOptionsApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_create_dto: OpenapiClient::OptionCreateDto.new({key: 'key_example', value: 'value_example'}) # OptionCreateDto | 
}

begin
  # Create a new user option (admin)
  result = api_instance.create_system_user_option(user_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->create_system_user_option: #{e}"
end
```

#### Using the create_system_user_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_system_user_option_with_http_info(user_id, key, opts)

```ruby
begin
  # Create a new user option (admin)
  data, status_code, headers = api_instance.create_system_user_option_with_http_info(user_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->create_system_user_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
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


## delete_system_user_option

> <EmptyEnvelope> delete_system_user_option(user_id, option_id, opts)

Delete a user option (admin)

Admin endpoint to delete an option for any user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UserOptionsApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a user option (admin)
  result = api_instance.delete_system_user_option(user_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->delete_system_user_option: #{e}"
end
```

#### Using the delete_system_user_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_system_user_option_with_http_info(user_id, option_id, opts)

```ruby
begin
  # Delete a user option (admin)
  data, status_code, headers = api_instance.delete_system_user_option_with_http_info(user_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->delete_system_user_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
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


## get_system_user_option_by_id

> <OptionDtoEnvelope> get_system_user_option_by_id(user_id, option_id, opts)

Retrieve a single user option by its ID (admin)

Admin endpoint to retrieve a single option for any user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UserOptionsApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single user option by its ID (admin)
  result = api_instance.get_system_user_option_by_id(user_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->get_system_user_option_by_id: #{e}"
end
```

#### Using the get_system_user_option_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_system_user_option_by_id_with_http_info(user_id, option_id, opts)

```ruby
begin
  # Retrieve a single user option by its ID (admin)
  data, status_code, headers = api_instance.get_system_user_option_by_id_with_http_info(user_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->get_system_user_option_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
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


## get_system_user_options

> <OptionDtoListEnvelope> get_system_user_options(user_id, opts)

Retrieve a list of user options (admin)

Admin endpoint to retrieve options for any user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UserOptionsApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of user options (admin)
  result = api_instance.get_system_user_options(user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->get_system_user_options: #{e}"
end
```

#### Using the get_system_user_options_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoListEnvelope>, Integer, Hash)> get_system_user_options_with_http_info(user_id, opts)

```ruby
begin
  # Retrieve a list of user options (admin)
  data, status_code, headers = api_instance.get_system_user_options_with_http_info(user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->get_system_user_options_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
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


## get_system_user_options_count

> <Int32Envelope> get_system_user_options_count(user_id, opts)

Get the count of user options (admin)

Admin endpoint to get the count of options for any user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UserOptionsApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of user options (admin)
  result = api_instance.get_system_user_options_count(user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->get_system_user_options_count: #{e}"
end
```

#### Using the get_system_user_options_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_system_user_options_count_with_http_info(user_id, opts)

```ruby
begin
  # Get the count of user options (admin)
  data, status_code, headers = api_instance.get_system_user_options_count_with_http_info(user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->get_system_user_options_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
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


## patch_system_user_option

> <EmptyEnvelope> patch_system_user_option(user_id, option_id, opts)

Partially update a user option (admin)

Admin endpoint to partially update an option for any user using a JSON Patch document

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UserOptionsApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Partially update a user option (admin)
  result = api_instance.patch_system_user_option(user_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->patch_system_user_option: #{e}"
end
```

#### Using the patch_system_user_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_system_user_option_with_http_info(user_id, option_id, opts)

```ruby
begin
  # Partially update a user option (admin)
  data, status_code, headers = api_instance.patch_system_user_option_with_http_info(user_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->patch_system_user_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
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


## update_system_user_option

> <EmptyEnvelope> update_system_user_option(user_id, option_id, opts)

Update a user option (admin)

Admin endpoint to update an option for any user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UserOptionsApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_update_dto: OpenapiClient::OptionUpdateDto.new # OptionUpdateDto | 
}

begin
  # Update a user option (admin)
  result = api_instance.update_system_user_option(user_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->update_system_user_option: #{e}"
end
```

#### Using the update_system_user_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_system_user_option_with_http_info(user_id, option_id, opts)

```ruby
begin
  # Update a user option (admin)
  data, status_code, headers = api_instance.update_system_user_option_with_http_info(user_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UserOptionsApi->update_system_user_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
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

