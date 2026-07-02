# OpenapiClient::NewslettersApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_newsletter_async**](NewslettersApi.md#create_newsletter_async) | **POST** /api/v2/MarketingService/Newsletters | Create a newsletter |
| [**delete_newsletter_async**](NewslettersApi.md#delete_newsletter_async) | **DELETE** /api/v2/MarketingService/Newsletters/{newsletterId} | Delete a newsletter |
| [**get_newsletter_details_async**](NewslettersApi.md#get_newsletter_details_async) | **GET** /api/v2/MarketingService/Newsletters/{newsletterId} | Get newsletter by ID |
| [**get_newsletter_o_data_async**](NewslettersApi.md#get_newsletter_o_data_async) | **GET** /api/v2/MarketingService/Newsletters | Get newsletters |
| [**get_newsletters_count_async**](NewslettersApi.md#get_newsletters_count_async) | **GET** /api/v2/MarketingService/Newsletters/Count | Get newsletters count |
| [**patch_newsletter_async**](NewslettersApi.md#patch_newsletter_async) | **PATCH** /api/v2/MarketingService/Newsletters/{newsletterId} | Patch a newsletter |
| [**update_newsletter_async**](NewslettersApi.md#update_newsletter_async) | **PUT** /api/v2/MarketingService/Newsletters/{newsletterId} | Update a newsletter |


## create_newsletter_async

> <EmptyEnvelope> create_newsletter_async(tenant_id, newsletter_create_dto, opts)

Create a newsletter

Creates a new newsletter for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewslettersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_create_dto = OpenapiClient::NewsletterCreateDto.new # NewsletterCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a newsletter
  result = api_instance.create_newsletter_async(tenant_id, newsletter_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->create_newsletter_async: #{e}"
end
```

#### Using the create_newsletter_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_newsletter_async_with_http_info(tenant_id, newsletter_create_dto, opts)

```ruby
begin
  # Create a newsletter
  data, status_code, headers = api_instance.create_newsletter_async_with_http_info(tenant_id, newsletter_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->create_newsletter_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **newsletter_create_dto** | [**NewsletterCreateDto**](NewsletterCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_newsletter_async

> <EmptyEnvelope> delete_newsletter_async(tenant_id, newsletter_id, opts)

Delete a newsletter

Deletes a newsletter by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewslettersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a newsletter
  result = api_instance.delete_newsletter_async(tenant_id, newsletter_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->delete_newsletter_async: #{e}"
end
```

#### Using the delete_newsletter_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_newsletter_async_with_http_info(tenant_id, newsletter_id, opts)

```ruby
begin
  # Delete a newsletter
  data, status_code, headers = api_instance.delete_newsletter_async_with_http_info(tenant_id, newsletter_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->delete_newsletter_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **newsletter_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_newsletter_details_async

> <NewsletterDtoEnvelope> get_newsletter_details_async(tenant_id, newsletter_id, opts)

Get newsletter by ID

Retrieves the details of a specific newsletter by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewslettersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get newsletter by ID
  result = api_instance.get_newsletter_details_async(tenant_id, newsletter_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->get_newsletter_details_async: #{e}"
end
```

#### Using the get_newsletter_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<NewsletterDtoEnvelope>, Integer, Hash)> get_newsletter_details_async_with_http_info(tenant_id, newsletter_id, opts)

```ruby
begin
  # Get newsletter by ID
  data, status_code, headers = api_instance.get_newsletter_details_async_with_http_info(tenant_id, newsletter_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <NewsletterDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->get_newsletter_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **newsletter_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**NewsletterDtoEnvelope**](NewsletterDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_newsletter_o_data_async

> get_newsletter_o_data_async(tenant_id, opts)

Get newsletters

Retrieves a collection of newsletters for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewslettersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get newsletters
  api_instance.get_newsletter_o_data_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->get_newsletter_o_data_async: #{e}"
end
```

#### Using the get_newsletter_o_data_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_newsletter_o_data_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get newsletters
  data, status_code, headers = api_instance.get_newsletter_o_data_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->get_newsletter_o_data_async_with_http_info: #{e}"
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
- **Accept**: application/json, application/xml


## get_newsletters_count_async

> <Int32Envelope> get_newsletters_count_async(tenant_id, opts)

Get newsletters count

Returns the count of newsletters for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewslettersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get newsletters count
  result = api_instance.get_newsletters_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->get_newsletters_count_async: #{e}"
end
```

#### Using the get_newsletters_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_newsletters_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get newsletters count
  data, status_code, headers = api_instance.get_newsletters_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->get_newsletters_count_async_with_http_info: #{e}"
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


## patch_newsletter_async

> <EmptyEnvelope> patch_newsletter_async(tenant_id, newsletter_id, opts)

Patch a newsletter

Partially updates a newsletter by its ID using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewslettersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a newsletter
  result = api_instance.patch_newsletter_async(tenant_id, newsletter_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->patch_newsletter_async: #{e}"
end
```

#### Using the patch_newsletter_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_newsletter_async_with_http_info(tenant_id, newsletter_id, opts)

```ruby
begin
  # Patch a newsletter
  data, status_code, headers = api_instance.patch_newsletter_async_with_http_info(tenant_id, newsletter_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->patch_newsletter_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **newsletter_id** | **String** |  |  |
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


## update_newsletter_async

> <EmptyEnvelope> update_newsletter_async(tenant_id, newsletter_id, newsletter_update_dto, opts)

Update a newsletter

Updates an existing newsletter by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NewslettersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
newsletter_update_dto = OpenapiClient::NewsletterUpdateDto.new # NewsletterUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a newsletter
  result = api_instance.update_newsletter_async(tenant_id, newsletter_id, newsletter_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->update_newsletter_async: #{e}"
end
```

#### Using the update_newsletter_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_newsletter_async_with_http_info(tenant_id, newsletter_id, newsletter_update_dto, opts)

```ruby
begin
  # Update a newsletter
  data, status_code, headers = api_instance.update_newsletter_async_with_http_info(tenant_id, newsletter_id, newsletter_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NewslettersApi->update_newsletter_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **newsletter_id** | **String** |  |  |
| **newsletter_update_dto** | [**NewsletterUpdateDto**](NewsletterUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

