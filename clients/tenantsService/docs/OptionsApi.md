# OpenapiClient::OptionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_option**](OptionsApi.md#create_tenant_option) | **POST** /api/v2/TenantsService/Options | Create a new tenant option |
| [**delete_tenant_option**](OptionsApi.md#delete_tenant_option) | **DELETE** /api/v2/TenantsService/Options/{optionId} | Delete a tenant option |
| [**get_tenant_option_by_id**](OptionsApi.md#get_tenant_option_by_id) | **GET** /api/v2/TenantsService/Options/{optionId} | Retrieve a single tenant option by its ID |
| [**get_tenant_option_by_key**](OptionsApi.md#get_tenant_option_by_key) | **GET** /api/v2/TenantsService/Options/Key/{key} | Retrieve a single tenant option by its key |
| [**get_tenant_options**](OptionsApi.md#get_tenant_options) | **GET** /api/v2/TenantsService/Options | Retrieve a list of tenant options |
| [**get_tenant_options_count**](OptionsApi.md#get_tenant_options_count) | **GET** /api/v2/TenantsService/Options/Count | Get the count of tenant options |
| [**patch_tenant_option**](OptionsApi.md#patch_tenant_option) | **PATCH** /api/v2/TenantsService/Options/{optionId} | Patch a tenant option |
| [**update_tenant_option**](OptionsApi.md#update_tenant_option) | **PUT** /api/v2/TenantsService/Options/{optionId} | Update a tenant option |
| [**upsert_tenant_option**](OptionsApi.md#upsert_tenant_option) | **PUT** /api/v2/TenantsService/Options/Upsert/{key} | Create or update a tenant option by key |


## create_tenant_option

> <EmptyEnvelope> create_tenant_option(tenant_id, key, opts)

Create a new tenant option

Create a new tenant option

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_create_dto: OpenapiClient::OptionCreateDto.new({key: 'key_example', value: 'value_example'}) # OptionCreateDto | 
}

begin
  # Create a new tenant option
  result = api_instance.create_tenant_option(tenant_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->create_tenant_option: #{e}"
end
```

#### Using the create_tenant_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_option_with_http_info(tenant_id, key, opts)

```ruby
begin
  # Create a new tenant option
  data, status_code, headers = api_instance.create_tenant_option_with_http_info(tenant_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->create_tenant_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## delete_tenant_option

> <EmptyEnvelope> delete_tenant_option(tenant_id, option_id, opts)

Delete a tenant option

Delete a tenant option

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant option
  result = api_instance.delete_tenant_option(tenant_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->delete_tenant_option: #{e}"
end
```

#### Using the delete_tenant_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_option_with_http_info(tenant_id, option_id, opts)

```ruby
begin
  # Delete a tenant option
  data, status_code, headers = api_instance.delete_tenant_option_with_http_info(tenant_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->delete_tenant_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_tenant_option_by_id

> <OptionDtoEnvelope> get_tenant_option_by_id(tenant_id, option_id, opts)

Retrieve a single tenant option by its ID

Retrieve a single tenant option by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant option by its ID
  result = api_instance.get_tenant_option_by_id(tenant_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_tenant_option_by_id: #{e}"
end
```

#### Using the get_tenant_option_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_tenant_option_by_id_with_http_info(tenant_id, option_id, opts)

```ruby
begin
  # Retrieve a single tenant option by its ID
  data, status_code, headers = api_instance.get_tenant_option_by_id_with_http_info(tenant_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_tenant_option_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_tenant_option_by_key

> <OptionDtoEnvelope> get_tenant_option_by_key(tenant_id, key, opts)

Retrieve a single tenant option by its key

Retrieve a single tenant option by its key

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant option by its key
  result = api_instance.get_tenant_option_by_key(tenant_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_tenant_option_by_key: #{e}"
end
```

#### Using the get_tenant_option_by_key_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoEnvelope>, Integer, Hash)> get_tenant_option_by_key_with_http_info(tenant_id, key, opts)

```ruby
begin
  # Retrieve a single tenant option by its key
  data, status_code, headers = api_instance.get_tenant_option_by_key_with_http_info(tenant_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_tenant_option_by_key_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_tenant_options

> <OptionDtoListEnvelope> get_tenant_options(tenant_id, opts)

Retrieve a list of tenant options

Retrieve a list of tenant options

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant options
  result = api_instance.get_tenant_options(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_tenant_options: #{e}"
end
```

#### Using the get_tenant_options_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OptionDtoListEnvelope>, Integer, Hash)> get_tenant_options_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant options
  data, status_code, headers = api_instance.get_tenant_options_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OptionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_tenant_options_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_tenant_options_count

> <Int32Envelope> get_tenant_options_count(tenant_id, opts)

Get the count of tenant options

Get the count of tenant options

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant options
  result = api_instance.get_tenant_options_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_tenant_options_count: #{e}"
end
```

#### Using the get_tenant_options_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_options_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant options
  data, status_code, headers = api_instance.get_tenant_options_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->get_tenant_options_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## patch_tenant_option

> <EmptyEnvelope> patch_tenant_option(tenant_id, option_id, opts)

Patch a tenant option

Patch a tenant option

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a tenant option
  result = api_instance.patch_tenant_option(tenant_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->patch_tenant_option: #{e}"
end
```

#### Using the patch_tenant_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_tenant_option_with_http_info(tenant_id, option_id, opts)

```ruby
begin
  # Patch a tenant option
  data, status_code, headers = api_instance.patch_tenant_option_with_http_info(tenant_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->patch_tenant_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## update_tenant_option

> <EmptyEnvelope> update_tenant_option(tenant_id, option_id, opts)

Update a tenant option

Update a tenant option

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_update_dto: OpenapiClient::OptionUpdateDto.new # OptionUpdateDto | 
}

begin
  # Update a tenant option
  result = api_instance.update_tenant_option(tenant_id, option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->update_tenant_option: #{e}"
end
```

#### Using the update_tenant_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_option_with_http_info(tenant_id, option_id, opts)

```ruby
begin
  # Update a tenant option
  data, status_code, headers = api_instance.update_tenant_option_with_http_info(tenant_id, option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->update_tenant_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## upsert_tenant_option

> <EmptyEnvelope> upsert_tenant_option(tenant_id, key, opts)

Create or update a tenant option by key

Create or update a tenant option by key

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  portal_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  option_update_dto: OpenapiClient::OptionUpdateDto.new # OptionUpdateDto | 
}

begin
  # Create or update a tenant option by key
  result = api_instance.upsert_tenant_option(tenant_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->upsert_tenant_option: #{e}"
end
```

#### Using the upsert_tenant_option_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> upsert_tenant_option_with_http_info(tenant_id, key, opts)

```ruby
begin
  # Create or update a tenant option by key
  data, status_code, headers = api_instance.upsert_tenant_option_with_http_info(tenant_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OptionsApi->upsert_tenant_option_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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

