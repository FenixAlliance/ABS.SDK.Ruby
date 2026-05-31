# OpenapiClient::WebsiteThemesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_website_theme_async**](WebsiteThemesApi.md#create_website_theme_async) | **POST** /api/v2/ContentService/WebsiteThemes | Create a new website theme |
| [**delete_website_theme_async**](WebsiteThemesApi.md#delete_website_theme_async) | **DELETE** /api/v2/ContentService/WebsiteThemes/{id} | Delete a website theme |
| [**get_website_theme_by_id_async**](WebsiteThemesApi.md#get_website_theme_by_id_async) | **GET** /api/v2/ContentService/WebsiteThemes/{id} | Get website theme by ID |
| [**get_website_themes_async**](WebsiteThemesApi.md#get_website_themes_async) | **GET** /api/v2/ContentService/WebsiteThemes | Get all website themes |
| [**get_website_themes_count_async**](WebsiteThemesApi.md#get_website_themes_count_async) | **GET** /api/v2/ContentService/WebsiteThemes/Count | Get website themes count |
| [**update_website_theme_async**](WebsiteThemesApi.md#update_website_theme_async) | **PUT** /api/v2/ContentService/WebsiteThemes/{id} | Update a website theme |


## create_website_theme_async

> create_website_theme_async(tenant_id, opts)

Create a new website theme

Creates a new website theme for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebsiteThemesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  website_theme_create_dto: OpenapiClient::WebsiteThemeCreateDto.new({name: 'name_example'}) # WebsiteThemeCreateDto | 
}

begin
  # Create a new website theme
  api_instance.create_website_theme_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->create_website_theme_async: #{e}"
end
```

#### Using the create_website_theme_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_website_theme_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new website theme
  data, status_code, headers = api_instance.create_website_theme_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->create_website_theme_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **website_theme_create_dto** | [**WebsiteThemeCreateDto**](WebsiteThemeCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_website_theme_async

> delete_website_theme_async(tenant_id, id, opts)

Delete a website theme

Deletes a website theme for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebsiteThemesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a website theme
  api_instance.delete_website_theme_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->delete_website_theme_async: #{e}"
end
```

#### Using the delete_website_theme_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_website_theme_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a website theme
  data, status_code, headers = api_instance.delete_website_theme_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->delete_website_theme_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_website_theme_by_id_async

> <WebsiteThemeDto> get_website_theme_by_id_async(tenant_id, id, opts)

Get website theme by ID

Retrieves a specific website theme by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebsiteThemesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get website theme by ID
  result = api_instance.get_website_theme_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->get_website_theme_by_id_async: #{e}"
end
```

#### Using the get_website_theme_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebsiteThemeDto>, Integer, Hash)> get_website_theme_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get website theme by ID
  data, status_code, headers = api_instance.get_website_theme_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebsiteThemeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->get_website_theme_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebsiteThemeDto**](WebsiteThemeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_website_themes_async

> <WebsiteThemeDtoListEnvelope> get_website_themes_async(tenant_id, opts)

Get all website themes

Retrieves all website themes for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebsiteThemesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  o_data_query_options: OpenapiClient::WebsiteThemeDtoODataQueryOptions.new, # WebsiteThemeDtoODataQueryOptions | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all website themes
  result = api_instance.get_website_themes_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->get_website_themes_async: #{e}"
end
```

#### Using the get_website_themes_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebsiteThemeDtoListEnvelope>, Integer, Hash)> get_website_themes_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all website themes
  data, status_code, headers = api_instance.get_website_themes_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebsiteThemeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->get_website_themes_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **o_data_query_options** | [**WebsiteThemeDtoODataQueryOptions**](.md) |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebsiteThemeDtoListEnvelope**](WebsiteThemeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_website_themes_count_async

> <Int32Envelope> get_website_themes_count_async(tenant_id, opts)

Get website themes count

Returns the count of website themes for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebsiteThemesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  o_data_query_options: OpenapiClient::WebsiteThemeDtoODataQueryOptions.new, # WebsiteThemeDtoODataQueryOptions | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get website themes count
  result = api_instance.get_website_themes_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->get_website_themes_count_async: #{e}"
end
```

#### Using the get_website_themes_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_website_themes_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get website themes count
  data, status_code, headers = api_instance.get_website_themes_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->get_website_themes_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **o_data_query_options** | [**WebsiteThemeDtoODataQueryOptions**](.md) |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_website_theme_async

> update_website_theme_async(tenant_id, id, opts)

Update a website theme

Updates an existing website theme for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebsiteThemesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  website_theme_update_dto: OpenapiClient::WebsiteThemeUpdateDto.new # WebsiteThemeUpdateDto | 
}

begin
  # Update a website theme
  api_instance.update_website_theme_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->update_website_theme_async: #{e}"
end
```

#### Using the update_website_theme_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_website_theme_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a website theme
  data, status_code, headers = api_instance.update_website_theme_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebsiteThemesApi->update_website_theme_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **website_theme_update_dto** | [**WebsiteThemeUpdateDto**](WebsiteThemeUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

