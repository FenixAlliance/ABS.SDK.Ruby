# OpenapiClient::LocalizationStringsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_localization_strings_async**](LocalizationStringsApi.md#count_localization_strings_async) | **GET** /api/v2/ContentService/LocalizationStrings/Count | Count localization strings |
| [**create_localization_string_async**](LocalizationStringsApi.md#create_localization_string_async) | **POST** /api/v2/ContentService/LocalizationStrings | Create a localization string |
| [**delete_localization_string_async**](LocalizationStringsApi.md#delete_localization_string_async) | **DELETE** /api/v2/ContentService/LocalizationStrings/{localizationStringId} | Delete a localization string |
| [**get_localization_string_by_id_async**](LocalizationStringsApi.md#get_localization_string_by_id_async) | **GET** /api/v2/ContentService/LocalizationStrings/{localizationStringId} | Get localization string by ID |
| [**get_localization_strings_async**](LocalizationStringsApi.md#get_localization_strings_async) | **GET** /api/v2/ContentService/LocalizationStrings | Get localization strings |
| [**update_localization_string_async**](LocalizationStringsApi.md#update_localization_string_async) | **PUT** /api/v2/ContentService/LocalizationStrings/{localizationStringId} | Update a localization string |


## count_localization_strings_async

> <Int32Envelope> count_localization_strings_async(tenant_id, opts)

Count localization strings

Counts all localization strings for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocalizationStringsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count localization strings
  result = api_instance.count_localization_strings_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->count_localization_strings_async: #{e}"
end
```

#### Using the count_localization_strings_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_localization_strings_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count localization strings
  data, status_code, headers = api_instance.count_localization_strings_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->count_localization_strings_async_with_http_info: #{e}"
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


## create_localization_string_async

> <EmptyEnvelope> create_localization_string_async(tenant_id, localization_string_create_dto, opts)

Create a localization string

Creates a new localization string for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocalizationStringsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
localization_string_create_dto = OpenapiClient::LocalizationStringCreateDto.new({base: 'base_example'}) # LocalizationStringCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a localization string
  result = api_instance.create_localization_string_async(tenant_id, localization_string_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->create_localization_string_async: #{e}"
end
```

#### Using the create_localization_string_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_localization_string_async_with_http_info(tenant_id, localization_string_create_dto, opts)

```ruby
begin
  # Create a localization string
  data, status_code, headers = api_instance.create_localization_string_async_with_http_info(tenant_id, localization_string_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->create_localization_string_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **localization_string_create_dto** | [**LocalizationStringCreateDto**](LocalizationStringCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_localization_string_async

> <EmptyEnvelope> delete_localization_string_async(tenant_id, localization_string_id, opts)

Delete a localization string

Deletes a localization string for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocalizationStringsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
localization_string_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a localization string
  result = api_instance.delete_localization_string_async(tenant_id, localization_string_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->delete_localization_string_async: #{e}"
end
```

#### Using the delete_localization_string_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_localization_string_async_with_http_info(tenant_id, localization_string_id, opts)

```ruby
begin
  # Delete a localization string
  data, status_code, headers = api_instance.delete_localization_string_async_with_http_info(tenant_id, localization_string_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->delete_localization_string_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **localization_string_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_localization_string_by_id_async

> <LocalizationStringDtoEnvelope> get_localization_string_by_id_async(tenant_id, localization_string_id, opts)

Get localization string by ID

Retrieves a specific localization string by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocalizationStringsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
localization_string_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get localization string by ID
  result = api_instance.get_localization_string_by_id_async(tenant_id, localization_string_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->get_localization_string_by_id_async: #{e}"
end
```

#### Using the get_localization_string_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LocalizationStringDtoEnvelope>, Integer, Hash)> get_localization_string_by_id_async_with_http_info(tenant_id, localization_string_id, opts)

```ruby
begin
  # Get localization string by ID
  data, status_code, headers = api_instance.get_localization_string_by_id_async_with_http_info(tenant_id, localization_string_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LocalizationStringDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->get_localization_string_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **localization_string_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LocalizationStringDtoEnvelope**](LocalizationStringDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_localization_strings_async

> <LocalizationStringDtoListEnvelope> get_localization_strings_async(tenant_id, opts)

Get localization strings

Retrieves all localization strings for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocalizationStringsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get localization strings
  result = api_instance.get_localization_strings_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->get_localization_strings_async: #{e}"
end
```

#### Using the get_localization_strings_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LocalizationStringDtoListEnvelope>, Integer, Hash)> get_localization_strings_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get localization strings
  data, status_code, headers = api_instance.get_localization_strings_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LocalizationStringDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->get_localization_strings_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LocalizationStringDtoListEnvelope**](LocalizationStringDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_localization_string_async

> <EmptyEnvelope> update_localization_string_async(tenant_id, localization_string_id, localization_string_update_dto, opts)

Update a localization string

Updates an existing localization string for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LocalizationStringsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
localization_string_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
localization_string_update_dto = OpenapiClient::LocalizationStringUpdateDto.new # LocalizationStringUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a localization string
  result = api_instance.update_localization_string_async(tenant_id, localization_string_id, localization_string_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->update_localization_string_async: #{e}"
end
```

#### Using the update_localization_string_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_localization_string_async_with_http_info(tenant_id, localization_string_id, localization_string_update_dto, opts)

```ruby
begin
  # Update a localization string
  data, status_code, headers = api_instance.update_localization_string_async_with_http_info(tenant_id, localization_string_id, localization_string_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LocalizationStringsApi->update_localization_string_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **localization_string_id** | **String** |  |  |
| **localization_string_update_dto** | [**LocalizationStringUpdateDto**](LocalizationStringUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

