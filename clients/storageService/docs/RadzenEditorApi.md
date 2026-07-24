# OpenapiClient::RadzenEditorApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**radzen_upload_image**](RadzenEditorApi.md#radzen_upload_image) | **POST** /api/v2/fs/radzen/tenants/{tenantId}/upload/image | Upload an editor image to tenant storage. |
| [**radzen_upload_image_scoped**](RadzenEditorApi.md#radzen_upload_image_scoped) | **POST** /api/v2/fs/radzen/tenants/{tenantId}/{recordType}/{recordId}/upload/image | Upload an editor image scoped to a record. |
| [**radzen_upload_single**](RadzenEditorApi.md#radzen_upload_single) | **POST** /api/v2/fs/radzen/tenants/{tenantId}/upload/single | Upload a single editor file to tenant storage. |
| [**radzen_upload_single_scoped**](RadzenEditorApi.md#radzen_upload_single_scoped) | **POST** /api/v2/fs/radzen/tenants/{tenantId}/{recordType}/{recordId}/upload/single | Upload a single editor file scoped to a record. |
| [**radzen_upload_stream**](RadzenEditorApi.md#radzen_upload_stream) | **PUT** /api/v2/fs/radzen/tenants/{tenantId}/upload/stream | Chunked editor upload (not implemented). |
| [**radzen_upload_stream_scoped**](RadzenEditorApi.md#radzen_upload_stream_scoped) | **PUT** /api/v2/fs/radzen/tenants/{tenantId}/{recordType}/{recordId}/upload/stream | Chunked editor upload scoped to a record (not implemented). |
| [**radzen_upload_user_image**](RadzenEditorApi.md#radzen_upload_user_image) | **POST** /api/v2/fs/radzen/users/upload/image | Upload an editor image to user storage. |
| [**radzen_upload_user_image_scoped**](RadzenEditorApi.md#radzen_upload_user_image_scoped) | **POST** /api/v2/fs/radzen/users/{recordType}/{recordId}/upload/image | Upload a user editor image scoped to a record. |


## radzen_upload_image

> radzen_upload_image(tenant_id, opts)

Upload an editor image to tenant storage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  visibility: 'visibility_example', # String | 
  social_profile_id: 'social_profile_id_example', # String | 
  purpose: 'purpose_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload an editor image to tenant storage.
  api_instance.radzen_upload_image(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_image: #{e}"
end
```

#### Using the radzen_upload_image_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> radzen_upload_image_with_http_info(tenant_id, opts)

```ruby
begin
  # Upload an editor image to tenant storage.
  data, status_code, headers = api_instance.radzen_upload_image_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_image_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **visibility** | **String** |  | [optional] |
| **social_profile_id** | **String** |  | [optional] |
| **purpose** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined


## radzen_upload_image_scoped

> radzen_upload_image_scoped(tenant_id, record_type, record_id, opts)

Upload an editor image scoped to a record.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
record_type = 'record_type_example' # String | 
record_id = 'record_id_example' # String | 
opts = {
  visibility: 'visibility_example', # String | 
  social_profile_id: 'social_profile_id_example', # String | 
  purpose: 'purpose_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload an editor image scoped to a record.
  api_instance.radzen_upload_image_scoped(tenant_id, record_type, record_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_image_scoped: #{e}"
end
```

#### Using the radzen_upload_image_scoped_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> radzen_upload_image_scoped_with_http_info(tenant_id, record_type, record_id, opts)

```ruby
begin
  # Upload an editor image scoped to a record.
  data, status_code, headers = api_instance.radzen_upload_image_scoped_with_http_info(tenant_id, record_type, record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_image_scoped_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **record_type** | **String** |  |  |
| **record_id** | **String** |  |  |
| **visibility** | **String** |  | [optional] |
| **social_profile_id** | **String** |  | [optional] |
| **purpose** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined


## radzen_upload_single

> radzen_upload_single(tenant_id, opts)

Upload a single editor file to tenant storage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload a single editor file to tenant storage.
  api_instance.radzen_upload_single(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_single: #{e}"
end
```

#### Using the radzen_upload_single_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> radzen_upload_single_with_http_info(tenant_id, opts)

```ruby
begin
  # Upload a single editor file to tenant storage.
  data, status_code, headers = api_instance.radzen_upload_single_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_single_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined


## radzen_upload_single_scoped

> radzen_upload_single_scoped(tenant_id, record_type, record_id, opts)

Upload a single editor file scoped to a record.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
record_type = 'record_type_example' # String | 
record_id = 'record_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload a single editor file scoped to a record.
  api_instance.radzen_upload_single_scoped(tenant_id, record_type, record_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_single_scoped: #{e}"
end
```

#### Using the radzen_upload_single_scoped_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> radzen_upload_single_scoped_with_http_info(tenant_id, record_type, record_id, opts)

```ruby
begin
  # Upload a single editor file scoped to a record.
  data, status_code, headers = api_instance.radzen_upload_single_scoped_with_http_info(tenant_id, record_type, record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_single_scoped_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **record_type** | **String** |  |  |
| **record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined


## radzen_upload_stream

> radzen_upload_stream(tenant_id, opts)

Chunked editor upload (not implemented).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
tenant_id = 'tenant_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Chunked editor upload (not implemented).
  api_instance.radzen_upload_stream(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_stream: #{e}"
end
```

#### Using the radzen_upload_stream_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> radzen_upload_stream_with_http_info(tenant_id, opts)

```ruby
begin
  # Chunked editor upload (not implemented).
  data, status_code, headers = api_instance.radzen_upload_stream_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_stream_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## radzen_upload_stream_scoped

> radzen_upload_stream_scoped(tenant_id, record_type, record_id, opts)

Chunked editor upload scoped to a record (not implemented).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
tenant_id = 'tenant_id_example' # String | 
record_type = 'record_type_example' # String | 
record_id = 'record_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Chunked editor upload scoped to a record (not implemented).
  api_instance.radzen_upload_stream_scoped(tenant_id, record_type, record_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_stream_scoped: #{e}"
end
```

#### Using the radzen_upload_stream_scoped_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> radzen_upload_stream_scoped_with_http_info(tenant_id, record_type, record_id, opts)

```ruby
begin
  # Chunked editor upload scoped to a record (not implemented).
  data, status_code, headers = api_instance.radzen_upload_stream_scoped_with_http_info(tenant_id, record_type, record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_stream_scoped_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **record_type** | **String** |  |  |
| **record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## radzen_upload_user_image

> radzen_upload_user_image(opts)

Upload an editor image to user storage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
opts = {
  visibility: 'visibility_example', # String | 
  social_profile_id: 'social_profile_id_example', # String | 
  purpose: 'purpose_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload an editor image to user storage.
  api_instance.radzen_upload_user_image(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_user_image: #{e}"
end
```

#### Using the radzen_upload_user_image_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> radzen_upload_user_image_with_http_info(opts)

```ruby
begin
  # Upload an editor image to user storage.
  data, status_code, headers = api_instance.radzen_upload_user_image_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_user_image_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **visibility** | **String** |  | [optional] |
| **social_profile_id** | **String** |  | [optional] |
| **purpose** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined


## radzen_upload_user_image_scoped

> radzen_upload_user_image_scoped(record_type, record_id, opts)

Upload a user editor image scoped to a record.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
record_type = 'record_type_example' # String | 
record_id = 'record_id_example' # String | 
opts = {
  visibility: 'visibility_example', # String | 
  social_profile_id: 'social_profile_id_example', # String | 
  purpose: 'purpose_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload a user editor image scoped to a record.
  api_instance.radzen_upload_user_image_scoped(record_type, record_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_user_image_scoped: #{e}"
end
```

#### Using the radzen_upload_user_image_scoped_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> radzen_upload_user_image_scoped_with_http_info(record_type, record_id, opts)

```ruby
begin
  # Upload a user editor image scoped to a record.
  data, status_code, headers = api_instance.radzen_upload_user_image_scoped_with_http_info(record_type, record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->radzen_upload_user_image_scoped_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **record_type** | **String** |  |  |
| **record_id** | **String** |  |  |
| **visibility** | **String** |  | [optional] |
| **social_profile_id** | **String** |  | [optional] |
| **purpose** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined

