# OpenapiClient::OptionsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_system_option**](OptionsApi.md#create_system_option) | **POST** /api/v2/SystemService/Options | Create a new system option |
| [**delete_system_option**](OptionsApi.md#delete_system_option) | **DELETE** /api/v2/SystemService/Options/{optionId} | Delete a system option |
| [**get_system_option_by_id**](OptionsApi.md#get_system_option_by_id) | **GET** /api/v2/SystemService/Options/{optionId} | Retrieve a single system option by its ID |
| [**get_system_option_by_key**](OptionsApi.md#get_system_option_by_key) | **GET** /api/v2/SystemService/Options/Key/{key} | Retrieve a single system option by its key |
| [**get_system_options**](OptionsApi.md#get_system_options) | **GET** /api/v2/SystemService/Options | Retrieve a list of system options |
| [**get_system_options_count**](OptionsApi.md#get_system_options_count) | **GET** /api/v2/SystemService/Options/Count | Get the count of system options |
| [**update_system_option**](OptionsApi.md#update_system_option) | **PUT** /api/v2/SystemService/Options/{optionId} | Update a system option |
| [**upsert_system_option**](OptionsApi.md#upsert_system_option) | **PUT** /api/v2/SystemService/Options/Upsert/{key} | Create or update a system option by key |


## create_system_option

> <EmptyEnvelope> create_system_option(key, opts)

Create a new system option

Create a new system option

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
  # Create a new system option
  result = api_instance.create_system_option(key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->create_system_option: #{e}"
end
```

#### Using the create_system_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_system_option_with_http_info(key, opts)

```ruby
begin
  # Create a new system option
  data, status_code, headers = api_instance.create_system_option_with_http_info(key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->create_system_option_with_http_info: #{e}"
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


## delete_system_option

> <EmptyEnvelope> delete_system_option(option_id, opts)

Delete a system option

Delete a system option

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
  # Delete a system option
  result = api_instance.delete_system_option(option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->delete_system_option: #{e}"
end
```

#### Using the delete_system_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_system_option_with_http_info(option_id, opts)

```ruby
begin
  # Delete a system option
  data, status_code, headers = api_instance.delete_system_option_with_http_info(option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->delete_system_option_with_http_info: #{e}"
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


## get_system_option_by_id

> <OptionDtoEnvelope> get_system_option_by_id(option_id, opts)

Retrieve a single system option by its ID

Retrieve a single system option by its ID

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
  # Retrieve a single system option by its ID
  result = api_instance.get_system_option_by_id(option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_system_option_by_id: #{e}"
end
```

#### Using the get_system_option_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_system_option_by_id_with_http_info(option_id, opts)

```ruby
begin
  # Retrieve a single system option by its ID
  data, status_code, headers = api_instance.get_system_option_by_id_with_http_info(option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_system_option_by_id_with_http_info: #{e}"
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


## get_system_option_by_key

> <OptionDtoEnvelope> get_system_option_by_key(portal_id, key, opts)

Retrieve a single system option by its key

Retrieve a single system option by its key

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single system option by its key
  result = api_instance.get_system_option_by_key(portal_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_system_option_by_key: #{e}"
end
```

#### Using the get_system_option_by_key_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_system_option_by_key_with_http_info(portal_id, key, opts)

```ruby
begin
  # Retrieve a single system option by its key
  data, status_code, headers = api_instance.get_system_option_by_key_with_http_info(portal_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_system_option_by_key_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **portal_id** | **String** |  |  |
| **key** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OptionDtoEnvelope**](OptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_options

> <OptionDtoListEnvelope> get_system_options(portal_id, opts)

Retrieve a list of system options

Retrieve a list of system options for a portal

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of system options
  result = api_instance.get_system_options(portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_system_options: #{e}"
end
```

#### Using the get_system_options_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoListEnvelope>, Integer, Hash)> get_system_options_with_http_info(portal_id, opts)

```ruby
begin
  # Retrieve a list of system options
  data, status_code, headers = api_instance.get_system_options_with_http_info(portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_system_options_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **portal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OptionDtoListEnvelope**](OptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_options_count

> <Int32Envelope> get_system_options_count(portal_id, opts)

Get the count of system options

Get the count of system options for a portal

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of system options
  result = api_instance.get_system_options_count(portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_system_options_count: #{e}"
end
```

#### Using the get_system_options_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_system_options_count_with_http_info(portal_id, opts)

```ruby
begin
  # Get the count of system options
  data, status_code, headers = api_instance.get_system_options_count_with_http_info(portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_system_options_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **portal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_system_option

> <EmptyEnvelope> update_system_option(option_id, opts)

Update a system option

Update a system option

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
  # Update a system option
  result = api_instance.update_system_option(option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->update_system_option: #{e}"
end
```

#### Using the update_system_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_system_option_with_http_info(option_id, opts)

```ruby
begin
  # Update a system option
  data, status_code, headers = api_instance.update_system_option_with_http_info(option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->update_system_option_with_http_info: #{e}"
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


## upsert_system_option

> <EmptyEnvelope> upsert_system_option(key, opts)

Create or update a system option by key

Create or update a system option by key

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
  # Create or update a system option by key
  result = api_instance.upsert_system_option(key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->upsert_system_option: #{e}"
end
```

#### Using the upsert_system_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> upsert_system_option_with_http_info(key, opts)

```ruby
begin
  # Create or update a system option by key
  data, status_code, headers = api_instance.upsert_system_option_with_http_info(key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->upsert_system_option_with_http_info: #{e}"
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

