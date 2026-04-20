# OpenapiClient::UploadsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**save_file_async**](UploadsApi.md#save_file_async) | **POST** /api/v2/StorageService/Uploads | Upload a file |


## save_file_async

> <EmptyEnvelope> save_file_async(opts)

Upload a file

Uploads a file to tenant or user storage.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UploadsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
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
  # Upload a file
  result = api_instance.save_file_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UploadsApi->save_file_async: #{e}"
end
```

#### Using the save_file_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> save_file_async_with_http_info(opts)

```ruby
begin
  # Upload a file
  data, status_code, headers = api_instance.save_file_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UploadsApi->save_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
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
- **Accept**: application/json, application/xml

