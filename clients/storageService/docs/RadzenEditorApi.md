# OpenapiClient::RadzenEditorApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**image**](RadzenEditorApi.md#image) | **POST** /api/v2/StorageService/RadzenEditor/Uploads/Image | Upload an image file |
| [**multiple**](RadzenEditorApi.md#multiple) | **POST** /api/v2/StorageService/RadzenEditor/Uploads/Multiple | Upload multiple files |
| [**post**](RadzenEditorApi.md#post) | **POST** /api/v2/StorageService/RadzenEditor/Uploads/{id} | Upload files by ID |
| [**single**](RadzenEditorApi.md#single) | **POST** /api/v2/StorageService/RadzenEditor/Uploads/Single | Upload a single file |
| [**specific**](RadzenEditorApi.md#specific) | **POST** /api/v2/StorageService/RadzenEditor/Uploads/Specific | Upload a specific file |


## image

> image(opts)

Upload an image file

Uploads an image file and returns its URL for editor embedding.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload an image file
  api_instance.image(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->image: #{e}"
end
```

#### Using the image_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> image_with_http_info(opts)

```ruby
begin
  # Upload an image file
  data, status_code, headers = api_instance.image_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->image_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
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


## multiple

> multiple(opts)

Upload multiple files

Uploads multiple files to tenant or user storage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  files: [File.new('/path/to/some/file')] # Array<File> | 
}

begin
  # Upload multiple files
  api_instance.multiple(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->multiple: #{e}"
end
```

#### Using the multiple_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> multiple_with_http_info(opts)

```ruby
begin
  # Upload multiple files
  data, status_code, headers = api_instance.multiple_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->multiple_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **files** | **Array&lt;File&gt;** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined


## post

> post(id, opts)

Upload files by ID

Uploads files associated with a specific resource ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
id = 56 # Integer | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  files: [File.new('/path/to/some/file')] # Array<File> | 
}

begin
  # Upload files by ID
  api_instance.post(id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->post: #{e}"
end
```

#### Using the post_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> post_with_http_info(id, opts)

```ruby
begin
  # Upload files by ID
  data, status_code, headers = api_instance.post_with_http_info(id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **Integer** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **files** | **Array&lt;File&gt;** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined


## single

> single(opts)

Upload a single file

Uploads a single file to tenant or user storage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload a single file
  api_instance.single(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->single: #{e}"
end
```

#### Using the single_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> single_with_http_info(opts)

```ruby
begin
  # Upload a single file
  data, status_code, headers = api_instance.single_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->single_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
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


## specific

> specific(opts)

Upload a specific file

Uploads a specific file to tenant or user storage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RadzenEditorApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload a specific file
  api_instance.specific(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->specific: #{e}"
end
```

#### Using the specific_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> specific_with_http_info(opts)

```ruby
begin
  # Upload a specific file
  data, status_code, headers = api_instance.specific_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling RadzenEditorApi->specific_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
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

