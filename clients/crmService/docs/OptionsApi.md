# OpenapiClient::OptionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_contact_option**](OptionsApi.md#create_contact_option) | **POST** /api/v2/CrmService/Contacts/{contactId}/Options | Create a new contact option |
| [**delete_contact_option**](OptionsApi.md#delete_contact_option) | **DELETE** /api/v2/CrmService/Contacts/{contactId}/Options/{optionId} | Delete a contact option |
| [**get_contact_option_by_id**](OptionsApi.md#get_contact_option_by_id) | **GET** /api/v2/CrmService/Contacts/{contactId}/Options/{optionId} | Retrieve a single contact option by its ID |
| [**get_contact_option_by_key**](OptionsApi.md#get_contact_option_by_key) | **GET** /api/v2/CrmService/Contacts/{contactId}/Options/Key/{key} | Retrieve a single contact option by its key |
| [**get_contact_options**](OptionsApi.md#get_contact_options) | **GET** /api/v2/CrmService/Contacts/{contactId}/Options | Retrieve a list of contact options |
| [**get_contact_options_count**](OptionsApi.md#get_contact_options_count) | **GET** /api/v2/CrmService/Contacts/{contactId}/Options/Count | Get the count of contact options |
| [**patch_contact_option_async**](OptionsApi.md#patch_contact_option_async) | **PATCH** /api/v2/CrmService/Contacts/{contactId}/Options/{optionId} | Patch a contact option |
| [**patch_contact_option_by_key_async**](OptionsApi.md#patch_contact_option_by_key_async) | **PATCH** /api/v2/CrmService/Contacts/{contactId}/Options/Key/{key} | Patch a contact option by key |
| [**update_contact_option**](OptionsApi.md#update_contact_option) | **PUT** /api/v2/CrmService/Contacts/{contactId}/Options/{optionId} | Update a contact option |
| [**upsert_contact_option**](OptionsApi.md#upsert_contact_option) | **PUT** /api/v2/CrmService/Contacts/{contactId}/Options/Upsert/{key} | Create or update a contact option by key |


## create_contact_option

> <EmptyEnvelope> create_contact_option(tenant_id, contact_id, key, opts)

Create a new contact option

Create a new option for a contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_create_dto: OpenapiClient::OptionCreateDto.new({key: 'key_example', value: 'value_example'}) # OptionCreateDto | 
}

begin
  # Create a new contact option
  result = api_instance.create_contact_option(tenant_id, contact_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->create_contact_option: #{e}"
end
```

#### Using the create_contact_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_contact_option_with_http_info(tenant_id, contact_id, key, opts)

```ruby
begin
  # Create a new contact option
  data, status_code, headers = api_instance.create_contact_option_with_http_info(tenant_id, contact_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->create_contact_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## delete_contact_option

> <EmptyEnvelope> delete_contact_option(tenant_id, contact_id, option_id, opts)

Delete a contact option

Delete a contact option

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact option
  result = api_instance.delete_contact_option(tenant_id, contact_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->delete_contact_option: #{e}"
end
```

#### Using the delete_contact_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_contact_option_with_http_info(tenant_id, contact_id, option_id, opts)

```ruby
begin
  # Delete a contact option
  data, status_code, headers = api_instance.delete_contact_option_with_http_info(tenant_id, contact_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->delete_contact_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_contact_option_by_id

> <OptionDtoEnvelope> get_contact_option_by_id(tenant_id, contact_id, option_id, opts)

Retrieve a single contact option by its ID

Retrieve a single contact option by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single contact option by its ID
  result = api_instance.get_contact_option_by_id(tenant_id, contact_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_contact_option_by_id: #{e}"
end
```

#### Using the get_contact_option_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_contact_option_by_id_with_http_info(tenant_id, contact_id, option_id, opts)

```ruby
begin
  # Retrieve a single contact option by its ID
  data, status_code, headers = api_instance.get_contact_option_by_id_with_http_info(tenant_id, contact_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_contact_option_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_contact_option_by_key

> <OptionDtoEnvelope> get_contact_option_by_key(tenant_id, contact_id, key, opts)

Retrieve a single contact option by its key

Retrieve a single contact option by its key

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single contact option by its key
  result = api_instance.get_contact_option_by_key(tenant_id, contact_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_contact_option_by_key: #{e}"
end
```

#### Using the get_contact_option_by_key_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_contact_option_by_key_with_http_info(tenant_id, contact_id, key, opts)

```ruby
begin
  # Retrieve a single contact option by its key
  data, status_code, headers = api_instance.get_contact_option_by_key_with_http_info(tenant_id, contact_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_contact_option_by_key_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
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


## get_contact_options

> <OptionDtoListEnvelope> get_contact_options(tenant_id, contact_id, opts)

Retrieve a list of contact options

Retrieve a list of options for a contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of contact options
  result = api_instance.get_contact_options(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_contact_options: #{e}"
end
```

#### Using the get_contact_options_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoListEnvelope>, Integer, Hash)> get_contact_options_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Retrieve a list of contact options
  data, status_code, headers = api_instance.get_contact_options_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_contact_options_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_contact_options_count

> <Int32Envelope> get_contact_options_count(tenant_id, contact_id, opts)

Get the count of contact options

Get the count of options for a contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of contact options
  result = api_instance.get_contact_options_count(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_contact_options_count: #{e}"
end
```

#### Using the get_contact_options_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_contact_options_count_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get the count of contact options
  data, status_code, headers = api_instance.get_contact_options_count_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_contact_options_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## patch_contact_option_async

> <EmptyEnvelope> patch_contact_option_async(tenant_id, contact_id, option_id, opts)

Patch a contact option

Patch a contact option

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a contact option
  result = api_instance.patch_contact_option_async(tenant_id, contact_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->patch_contact_option_async: #{e}"
end
```

#### Using the patch_contact_option_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_contact_option_async_with_http_info(tenant_id, contact_id, option_id, opts)

```ruby
begin
  # Patch a contact option
  data, status_code, headers = api_instance.patch_contact_option_async_with_http_info(tenant_id, contact_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->patch_contact_option_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
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


## patch_contact_option_by_key_async

> <EmptyEnvelope> patch_contact_option_by_key_async(tenant_id, contact_id, key, opts)

Patch a contact option by key

Patch a contact option by key

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a contact option by key
  result = api_instance.patch_contact_option_by_key_async(tenant_id, contact_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->patch_contact_option_by_key_async: #{e}"
end
```

#### Using the patch_contact_option_by_key_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_contact_option_by_key_async_with_http_info(tenant_id, contact_id, key, opts)

```ruby
begin
  # Patch a contact option by key
  data, status_code, headers = api_instance.patch_contact_option_by_key_async_with_http_info(tenant_id, contact_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->patch_contact_option_by_key_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **key** | **String** |  |  |
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


## update_contact_option

> <EmptyEnvelope> update_contact_option(tenant_id, contact_id, option_id, opts)

Update a contact option

Update a contact option

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_update_dto: OpenapiClient::OptionUpdateDto.new # OptionUpdateDto | 
}

begin
  # Update a contact option
  result = api_instance.update_contact_option(tenant_id, contact_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->update_contact_option: #{e}"
end
```

#### Using the update_contact_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_contact_option_with_http_info(tenant_id, contact_id, option_id, opts)

```ruby
begin
  # Update a contact option
  data, status_code, headers = api_instance.update_contact_option_with_http_info(tenant_id, contact_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->update_contact_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## upsert_contact_option

> <EmptyEnvelope> upsert_contact_option(tenant_id, contact_id, key, opts)

Create or update a contact option by key

Create or update a contact option by key

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_update_dto: OpenapiClient::OptionUpdateDto.new # OptionUpdateDto | 
}

begin
  # Create or update a contact option by key
  result = api_instance.upsert_contact_option(tenant_id, contact_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->upsert_contact_option: #{e}"
end
```

#### Using the upsert_contact_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> upsert_contact_option_with_http_info(tenant_id, contact_id, key, opts)

```ruby
begin
  # Create or update a contact option by key
  data, status_code, headers = api_instance.upsert_contact_option_with_http_info(tenant_id, contact_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->upsert_contact_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
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

