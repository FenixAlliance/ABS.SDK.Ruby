# OpenapiClient::FilesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_file_async**](FilesApi.md#create_file_async) | **POST** /api/v2/StorageService/Files |  |
| [**delete_file_async**](FilesApi.md#delete_file_async) | **DELETE** /api/v2/StorageService/Files/{fileId} |  |
| [**download_file_async**](FilesApi.md#download_file_async) | **GET** /api/v2/StorageService/Files/{fileId}/Raw |  |
| [**get_file_async**](FilesApi.md#get_file_async) | **GET** /api/v2/StorageService/Files/{fileId} |  |
| [**get_file_thumbnail_async**](FilesApi.md#get_file_thumbnail_async) | **GET** /api/v2/StorageService/Files/{fileId}/Thumbnail |  |
| [**get_files_async**](FilesApi.md#get_files_async) | **GET** /api/v2/StorageService/Files |  |
| [**get_files_count_async**](FilesApi.md#get_files_count_async) | **GET** /api/v2/StorageService/Files/Count |  |
| [**update_file_async**](FilesApi.md#update_file_async) | **PUT** /api/v2/StorageService/Files/{fileId} |  |


## create_file_async

> <EmptyEnvelope> create_file_async(opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FilesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file'), # File | 
  notes: 'notes_example', # String | 
  title: 'title_example', # String | 
  author: 'author_example', # String | 
  is_folder: true, # Boolean | 
  file_name: 'file_name_example', # String | 
  abstract: 'abstract_example', # String | 
  key_words: 'key_words_example', # String | 
  valid_response: true, # Boolean | 
  parent_file_upload_id: 'parent_file_upload_id_example', # String | 
  file_path: 'file_path_example', # String | 
  public_access_type: 'false', # String | 
  purpose: 'Unknown', # String | 
  social_profile_id_value: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  app_file_content: 'BYTE_ARRAY_DATA_HERE', # String | 
  app_file_sha256: 'app_file_sha256_example', # String | 
  app_file_created_at_utc: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  app_file_user_id_value: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  app_file_tenant_id_value: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  app_file_enrollment_id_value: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  app_file_source: 'Unknown', # String | 
  app_file_length: 789, # Integer | 
  app_file_name: 'app_file_name_example', # String | 
  app_file_file_name: 'app_file_file_name_example', # String | 
  app_file_last_modified: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  app_file_size: 789, # Integer | 
  app_file_content_type: 'app_file_content_type_example', # String | 
  app_file_content_disposition: 'app_file_content_disposition_example', # String | 
  app_file_headers: { key: 'inner_example'}, # Hash<String, String> | 
  id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  timestamp: Time.parse('2013-10-20T19:20:30+01:00') # Time | 
}

begin
  
  result = api_instance.create_file_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->create_file_async: #{e}"
end
```

#### Using the create_file_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_file_async_with_http_info(opts)

```ruby
begin
  
  data, status_code, headers = api_instance.create_file_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->create_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |
| **notes** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **author** | **String** |  | [optional] |
| **is_folder** | **Boolean** |  | [optional] |
| **file_name** | **String** |  | [optional] |
| **abstract** | **String** |  | [optional] |
| **key_words** | **String** |  | [optional] |
| **valid_response** | **Boolean** |  | [optional] |
| **parent_file_upload_id** | **String** |  | [optional] |
| **file_path** | **String** |  | [optional] |
| **public_access_type** | **String** |  | [optional] |
| **purpose** | **String** |  | [optional] |
| **social_profile_id_value** | **String** |  | [optional] |
| **app_file_content** | **String** |  | [optional] |
| **app_file_sha256** | **String** |  | [optional] |
| **app_file_created_at_utc** | **Time** |  | [optional] |
| **app_file_user_id_value** | **String** |  | [optional] |
| **app_file_tenant_id_value** | **String** |  | [optional] |
| **app_file_enrollment_id_value** | **String** |  | [optional] |
| **app_file_source** | **String** |  | [optional] |
| **app_file_length** | **Integer** |  | [optional] |
| **app_file_name** | **String** |  | [optional] |
| **app_file_file_name** | **String** |  | [optional] |
| **app_file_last_modified** | **Time** |  | [optional] |
| **app_file_size** | **Integer** |  | [optional] |
| **app_file_content_type** | **String** |  | [optional] |
| **app_file_content_disposition** | **String** |  | [optional] |
| **app_file_headers** | [**Hash&lt;String, String&gt;**](Hash.md) |  | [optional] |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, image/png


## delete_file_async

> <EmptyEnvelope> delete_file_async(file_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FilesApi.new
file_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.delete_file_async(file_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->delete_file_async: #{e}"
end
```

#### Using the delete_file_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_file_async_with_http_info(file_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.delete_file_async_with_http_info(file_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->delete_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## download_file_async

> File download_file_async(file_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FilesApi.new
file_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.download_file_async(file_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->download_file_async: #{e}"
end
```

#### Using the download_file_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(File, Integer, Hash)> download_file_async_with_http_info(file_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.download_file_async_with_http_info(file_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => File
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->download_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## get_file_async

> <FileUploadDtoEnvelope> get_file_async(file_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FilesApi.new
file_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.get_file_async(file_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->get_file_async: #{e}"
end
```

#### Using the get_file_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FileUploadDtoEnvelope>, Integer, Hash)> get_file_async_with_http_info(file_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.get_file_async_with_http_info(file_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FileUploadDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->get_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FileUploadDtoEnvelope**](FileUploadDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## get_file_thumbnail_async

> File get_file_thumbnail_async(file_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FilesApi.new
file_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.get_file_thumbnail_async(file_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->get_file_thumbnail_async: #{e}"
end
```

#### Using the get_file_thumbnail_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(File, Integer, Hash)> get_file_thumbnail_async_with_http_info(file_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.get_file_thumbnail_async_with_http_info(file_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => File
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->get_file_thumbnail_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## get_files_async

> <FileUploadDtoEnvelope> get_files_async(opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FilesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.get_files_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->get_files_async: #{e}"
end
```

#### Using the get_files_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FileUploadDtoEnvelope>, Integer, Hash)> get_files_async_with_http_info(opts)

```ruby
begin
  
  data, status_code, headers = api_instance.get_files_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FileUploadDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->get_files_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**FileUploadDtoEnvelope**](FileUploadDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## get_files_count_async

> Integer get_files_count_async(opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FilesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.get_files_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->get_files_count_async: #{e}"
end
```

#### Using the get_files_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_files_count_async_with_http_info(opts)

```ruby
begin
  
  data, status_code, headers = api_instance.get_files_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->get_files_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## update_file_async

> <EmptyEnvelope> update_file_async(file_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FilesApi.new
file_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file'), # File | 
  notes: 'notes_example', # String | 
  metadata: 'metadata_example', # String | 
  title: 'title_example', # String | 
  author: 'author_example', # String | 
  is_folder: true, # Boolean | 
  file_name: 'file_name_example', # String | 
  abstract: 'abstract_example', # String | 
  key_words: 'key_words_example', # String | 
  valid_response: true, # Boolean | 
  parent_file_upload_id: 'parent_file_upload_id_example', # String | 
  file_path: 'file_path_example', # String | 
  app_file_content: 'BYTE_ARRAY_DATA_HERE', # String | 
  app_file_sha256: 'app_file_sha256_example', # String | 
  app_file_created_at_utc: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  app_file_user_id_value: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  app_file_tenant_id_value: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  app_file_enrollment_id_value: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  app_file_source: 'Unknown', # String | 
  app_file_length: 789, # Integer | 
  app_file_name: 'app_file_name_example', # String | 
  app_file_file_name: 'app_file_file_name_example', # String | 
  app_file_last_modified: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  app_file_size: 789, # Integer | 
  app_file_content_type: 'app_file_content_type_example', # String | 
  app_file_content_disposition: 'app_file_content_disposition_example', # String | 
  app_file_headers: { key: 'inner_example'} # Hash<String, String> | 
}

begin
  
  result = api_instance.update_file_async(file_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->update_file_async: #{e}"
end
```

#### Using the update_file_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_file_async_with_http_info(file_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.update_file_async_with_http_info(file_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FilesApi->update_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |
| **notes** | **String** |  | [optional] |
| **metadata** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **author** | **String** |  | [optional] |
| **is_folder** | **Boolean** |  | [optional] |
| **file_name** | **String** |  | [optional] |
| **abstract** | **String** |  | [optional] |
| **key_words** | **String** |  | [optional] |
| **valid_response** | **Boolean** |  | [optional] |
| **parent_file_upload_id** | **String** |  | [optional] |
| **file_path** | **String** |  | [optional] |
| **app_file_content** | **String** |  | [optional] |
| **app_file_sha256** | **String** |  | [optional] |
| **app_file_created_at_utc** | **Time** |  | [optional] |
| **app_file_user_id_value** | **String** |  | [optional] |
| **app_file_tenant_id_value** | **String** |  | [optional] |
| **app_file_enrollment_id_value** | **String** |  | [optional] |
| **app_file_source** | **String** |  | [optional] |
| **app_file_length** | **Integer** |  | [optional] |
| **app_file_name** | **String** |  | [optional] |
| **app_file_file_name** | **String** |  | [optional] |
| **app_file_last_modified** | **Time** |  | [optional] |
| **app_file_size** | **Integer** |  | [optional] |
| **app_file_content_type** | **String** |  | [optional] |
| **app_file_content_disposition** | **String** |  | [optional] |
| **app_file_headers** | [**Hash&lt;String, String&gt;**](Hash.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, image/png

