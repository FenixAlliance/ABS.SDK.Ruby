# OpenapiClient::LanguagesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_languages_async**](LanguagesApi.md#count_languages_async) | **GET** /api/v2/GlobeService/Languages/Count | Count languages |
| [**get_language_by_id_async**](LanguagesApi.md#get_language_by_id_async) | **GET** /api/v2/GlobeService/Languages/{languageId} | Get language by ID |
| [**get_languages_async**](LanguagesApi.md#get_languages_async) | **GET** /api/v2/GlobeService/Languages | Get all languages |


## count_languages_async

> <Int32Envelope> count_languages_async(opts)

Count languages

Returns the total number of supported languages, with optional OData filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LanguagesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  country_language_dto_collection_query_parameters: OpenapiClient::CountryLanguageDtoCollectionQueryParameters.new # CountryLanguageDtoCollectionQueryParameters | 
}

begin
  # Count languages
  result = api_instance.count_languages_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LanguagesApi->count_languages_async: #{e}"
end
```

#### Using the count_languages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_languages_async_with_http_info(opts)

```ruby
begin
  # Count languages
  data, status_code, headers = api_instance.count_languages_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LanguagesApi->count_languages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **country_language_dto_collection_query_parameters** | [**CountryLanguageDtoCollectionQueryParameters**](CountryLanguageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_language_by_id_async

> <CountryLanguageDtoEnvelope> get_language_by_id_async(language_id, opts)

Get language by ID

Retrieves a single language by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LanguagesApi.new
language_id = 'language_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get language by ID
  result = api_instance.get_language_by_id_async(language_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LanguagesApi->get_language_by_id_async: #{e}"
end
```

#### Using the get_language_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryLanguageDtoEnvelope>, Integer, Hash)> get_language_by_id_async_with_http_info(language_id, opts)

```ruby
begin
  # Get language by ID
  data, status_code, headers = api_instance.get_language_by_id_async_with_http_info(language_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryLanguageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LanguagesApi->get_language_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **language_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountryLanguageDtoEnvelope**](CountryLanguageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_languages_async

> <CountryLanguageDtoListEnvelope> get_languages_async(opts)

Get all languages

Retrieves the list of all supported languages with optional OData pagination and filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LanguagesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  country_language_dto_collection_query_parameters: OpenapiClient::CountryLanguageDtoCollectionQueryParameters.new # CountryLanguageDtoCollectionQueryParameters | 
}

begin
  # Get all languages
  result = api_instance.get_languages_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LanguagesApi->get_languages_async: #{e}"
end
```

#### Using the get_languages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryLanguageDtoListEnvelope>, Integer, Hash)> get_languages_async_with_http_info(opts)

```ruby
begin
  # Get all languages
  data, status_code, headers = api_instance.get_languages_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryLanguageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LanguagesApi->get_languages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **country_language_dto_collection_query_parameters** | [**CountryLanguageDtoCollectionQueryParameters**](CountryLanguageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CountryLanguageDtoListEnvelope**](CountryLanguageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

