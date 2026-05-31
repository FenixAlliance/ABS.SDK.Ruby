# OpenapiClient::QuotesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**calculate_quote**](QuotesApi.md#calculate_quote) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Calculate | Calculate a quote. |
| [**calculate_quote_line**](QuotesApi.md#calculate_quote_line) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId}/Calculate | Calculate a quote line. |
| [**close_quote**](QuotesApi.md#close_quote) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Close | Close a quote. |
| [**create_order_from_quote**](QuotesApi.md#create_order_from_quote) | **POST** /api/v2/QuotesService/Quotes/{quoteId}/Orders | Create an order from a quote. |
| [**create_quote**](QuotesApi.md#create_quote) | **POST** /api/v2/QuotesService/Quotes | Create a new quote. |
| [**create_quote_line**](QuotesApi.md#create_quote_line) | **POST** /api/v2/QuotesService/Quotes/{quoteId}/Lines | Create a new quote line. |
| [**delete_quote**](QuotesApi.md#delete_quote) | **DELETE** /api/v2/QuotesService/Quotes/{quoteId} | Delete a quote. |
| [**delete_quote_line**](QuotesApi.md#delete_quote_line) | **DELETE** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId} | Delete a quote line. |
| [**get_extended_quotes**](QuotesApi.md#get_extended_quotes) | **GET** /api/v2/QuotesService/Quotes/Extended | Get a list of extended quotes. |
| [**get_quote**](QuotesApi.md#get_quote) | **GET** /api/v2/QuotesService/Quotes/{quoteId} | Get a quote by ID. |
| [**get_quote_line**](QuotesApi.md#get_quote_line) | **GET** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId} | Get a quote line by ID. |
| [**get_quote_lines**](QuotesApi.md#get_quote_lines) | **GET** /api/v2/QuotesService/Quotes/{quoteId}/Lines | Get quote lines for a quote. |
| [**get_quote_lines_count**](QuotesApi.md#get_quote_lines_count) | **GET** /api/v2/QuotesService/Quotes/{quoteId}/Lines/Count | Get the count of quote lines. |
| [**get_quotes**](QuotesApi.md#get_quotes) | **GET** /api/v2/QuotesService/Quotes | Get a list of quotes. |
| [**get_quotes_count**](QuotesApi.md#get_quotes_count) | **GET** /api/v2/QuotesService/Quotes/Count | Get the count of quotes. |
| [**preview_quote_email_template**](QuotesApi.md#preview_quote_email_template) | **POST** /api/v2/QuotesService/Quotes/{quoteId}/Emails/Preview | Preview the rendered email for an invoice. |
| [**quote_line_exists**](QuotesApi.md#quote_line_exists) | **GET** /api/v2/QuotesService/Quotes/{quoteId}/Lines/Exists | Check if a quote line exists. |
| [**reopen_quote**](QuotesApi.md#reopen_quote) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Reopen | Reopen a closed quote. |
| [**send_quote_email**](QuotesApi.md#send_quote_email) | **POST** /api/v2/QuotesService/Quotes/{quoteId}/Emails/Send | Send a quote transactional email to recipients. |
| [**update_quote**](QuotesApi.md#update_quote) | **PUT** /api/v2/QuotesService/Quotes/{quoteId} | Update an existing quote. |
| [**update_quote_line**](QuotesApi.md#update_quote_line) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId} | Update a quote line. |
| [**upsert_quote_line**](QuotesApi.md#upsert_quote_line) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId}/Upsert | Upsert a quote line. |


## calculate_quote

> <EmptyEnvelope> calculate_quote(tenant_id, quote_id)

Calculate a quote.

Performs calculation logic for the specified quote.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Calculate a quote.
  result = api_instance.calculate_quote(tenant_id, quote_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->calculate_quote: #{e}"
end
```

#### Using the calculate_quote_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> calculate_quote_with_http_info(tenant_id, quote_id)

```ruby
begin
  # Calculate a quote.
  data, status_code, headers = api_instance.calculate_quote_with_http_info(tenant_id, quote_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->calculate_quote_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## calculate_quote_line

> <EmptyEnvelope> calculate_quote_line(tenant_id, quote_id, quote_line_id)

Calculate a quote line.

Performs calculation logic for the specified quote line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Calculate a quote line.
  result = api_instance.calculate_quote_line(tenant_id, quote_id, quote_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->calculate_quote_line: #{e}"
end
```

#### Using the calculate_quote_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> calculate_quote_line_with_http_info(tenant_id, quote_id, quote_line_id)

```ruby
begin
  # Calculate a quote line.
  data, status_code, headers = api_instance.calculate_quote_line_with_http_info(tenant_id, quote_id, quote_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->calculate_quote_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **quote_line_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## close_quote

> <EmptyEnvelope> close_quote(tenant_id, quote_id)

Close a quote.

Closes the specified quote for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Close a quote.
  result = api_instance.close_quote(tenant_id, quote_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->close_quote: #{e}"
end
```

#### Using the close_quote_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> close_quote_with_http_info(tenant_id, quote_id)

```ruby
begin
  # Close a quote.
  data, status_code, headers = api_instance.close_quote_with_http_info(tenant_id, quote_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->close_quote_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_order_from_quote

> <EmptyEnvelope> create_order_from_quote(tenant_id, quote_id)

Create an order from a quote.

Creates an order based on the specified quote for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Create an order from a quote.
  result = api_instance.create_order_from_quote(tenant_id, quote_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->create_order_from_quote: #{e}"
end
```

#### Using the create_order_from_quote_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_order_from_quote_with_http_info(tenant_id, quote_id)

```ruby
begin
  # Create an order from a quote.
  data, status_code, headers = api_instance.create_order_from_quote_with_http_info(tenant_id, quote_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->create_order_from_quote_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_quote

> <EmptyEnvelope> create_quote(tenant_id, opts)

Create a new quote.

Creates a new quote for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quote_create_dto: OpenapiClient::QuoteCreateDto.new # QuoteCreateDto | 
}

begin
  # Create a new quote.
  result = api_instance.create_quote(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->create_quote: #{e}"
end
```

#### Using the create_quote_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_quote_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new quote.
  data, status_code, headers = api_instance.create_quote_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->create_quote_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_create_dto** | [**QuoteCreateDto**](QuoteCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_quote_line

> <EmptyEnvelope> create_quote_line(tenant_id, quote_id, opts)

Create a new quote line.

Creates a new quote line for the specified quote and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quote_line_create_dto: OpenapiClient::QuoteLineCreateDto.new # QuoteLineCreateDto | 
}

begin
  # Create a new quote line.
  result = api_instance.create_quote_line(tenant_id, quote_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->create_quote_line: #{e}"
end
```

#### Using the create_quote_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_quote_line_with_http_info(tenant_id, quote_id, opts)

```ruby
begin
  # Create a new quote line.
  data, status_code, headers = api_instance.create_quote_line_with_http_info(tenant_id, quote_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->create_quote_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **quote_line_create_dto** | [**QuoteLineCreateDto**](QuoteLineCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_quote

> <EmptyEnvelope> delete_quote(quote_id, tenant_id)

Delete a quote.

Deletes the specified quote for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a quote.
  result = api_instance.delete_quote(quote_id, tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->delete_quote: #{e}"
end
```

#### Using the delete_quote_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_quote_with_http_info(quote_id, tenant_id)

```ruby
begin
  # Delete a quote.
  data, status_code, headers = api_instance.delete_quote_with_http_info(quote_id, tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->delete_quote_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **quote_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_quote_line

> <EmptyEnvelope> delete_quote_line(tenant_id, quote_id, quote_line_id)

Delete a quote line.

Deletes the specified quote line for the quote and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a quote line.
  result = api_instance.delete_quote_line(tenant_id, quote_id, quote_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->delete_quote_line: #{e}"
end
```

#### Using the delete_quote_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_quote_line_with_http_info(tenant_id, quote_id, quote_line_id)

```ruby
begin
  # Delete a quote line.
  data, status_code, headers = api_instance.delete_quote_line_with_http_info(tenant_id, quote_id, quote_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->delete_quote_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **quote_line_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_quotes

> <ExtendedQuoteDtoListEnvelope> get_extended_quotes(tenant_id)

Get a list of extended quotes.

Retrieves a list of extended quotes for the specified tenant, supporting OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get a list of extended quotes.
  result = api_instance.get_extended_quotes(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_extended_quotes: #{e}"
end
```

#### Using the get_extended_quotes_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedQuoteDtoListEnvelope>, Integer, Hash)> get_extended_quotes_with_http_info(tenant_id)

```ruby
begin
  # Get a list of extended quotes.
  data, status_code, headers = api_instance.get_extended_quotes_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedQuoteDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_extended_quotes_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**ExtendedQuoteDtoListEnvelope**](ExtendedQuoteDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_quote

> <QuoteDtoEnvelope> get_quote(tenant_id, quote_id)

Get a quote by ID.

Retrieves a single quote by its unique identifier for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get a quote by ID.
  result = api_instance.get_quote(tenant_id, quote_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote: #{e}"
end
```

#### Using the get_quote_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<QuoteDtoEnvelope>, Integer, Hash)> get_quote_with_http_info(tenant_id, quote_id)

```ruby
begin
  # Get a quote by ID.
  data, status_code, headers = api_instance.get_quote_with_http_info(tenant_id, quote_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <QuoteDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |

### Return type

[**QuoteDtoEnvelope**](QuoteDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_quote_line

> <QuoteLineDtoEnvelope> get_quote_line(tenant_id, quote_id, quote_line_id)

Get a quote line by ID.

Retrieves a single quote line by its unique identifier for the specified quote and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get a quote line by ID.
  result = api_instance.get_quote_line(tenant_id, quote_id, quote_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote_line: #{e}"
end
```

#### Using the get_quote_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<QuoteLineDtoEnvelope>, Integer, Hash)> get_quote_line_with_http_info(tenant_id, quote_id, quote_line_id)

```ruby
begin
  # Get a quote line by ID.
  data, status_code, headers = api_instance.get_quote_line_with_http_info(tenant_id, quote_id, quote_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <QuoteLineDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **quote_line_id** | **String** |  |  |

### Return type

[**QuoteLineDtoEnvelope**](QuoteLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_quote_lines

> <QuoteLineDtoListEnvelope> get_quote_lines(tenant_id, quote_id, opts)

Get quote lines for a quote.

Retrieves all quote lines for the specified quote and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
}

begin
  # Get quote lines for a quote.
  result = api_instance.get_quote_lines(tenant_id, quote_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote_lines: #{e}"
end
```

#### Using the get_quote_lines_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<QuoteLineDtoListEnvelope>, Integer, Hash)> get_quote_lines_with_http_info(tenant_id, quote_id, opts)

```ruby
begin
  # Get quote lines for a quote.
  data, status_code, headers = api_instance.get_quote_lines_with_http_info(tenant_id, quote_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <QuoteLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote_lines_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **item_id** | **String** |  | [optional] |

### Return type

[**QuoteLineDtoListEnvelope**](QuoteLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_quote_lines_count

> <Int32Envelope> get_quote_lines_count(tenant_id, quote_id)

Get the count of quote lines.

Retrieves the total count of quote lines for the specified quote and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get the count of quote lines.
  result = api_instance.get_quote_lines_count(tenant_id, quote_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote_lines_count: #{e}"
end
```

#### Using the get_quote_lines_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_quote_lines_count_with_http_info(tenant_id, quote_id)

```ruby
begin
  # Get the count of quote lines.
  data, status_code, headers = api_instance.get_quote_lines_count_with_http_info(tenant_id, quote_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote_lines_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_quotes

> <QuoteDtoListEnvelope> get_quotes(tenant_id)

Get a list of quotes.

Retrieves a list of quotes for the specified tenant, supporting OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get a list of quotes.
  result = api_instance.get_quotes(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quotes: #{e}"
end
```

#### Using the get_quotes_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<QuoteDtoListEnvelope>, Integer, Hash)> get_quotes_with_http_info(tenant_id)

```ruby
begin
  # Get a list of quotes.
  data, status_code, headers = api_instance.get_quotes_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <QuoteDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quotes_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**QuoteDtoListEnvelope**](QuoteDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_quotes_count

> <Int32Envelope> get_quotes_count(tenant_id)

Get the count of quotes.

Retrieves the total count of quotes for the specified tenant, supporting OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get the count of quotes.
  result = api_instance.get_quotes_count(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quotes_count: #{e}"
end
```

#### Using the get_quotes_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_quotes_count_with_http_info(tenant_id)

```ruby
begin
  # Get the count of quotes.
  data, status_code, headers = api_instance.get_quotes_count_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quotes_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## preview_quote_email_template

> preview_quote_email_template(quote_id, tenant_id, opts)

Preview the rendered email for an invoice.

This action is only available for users with the 'send_email' permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Preview the rendered email for an invoice.
  api_instance.preview_quote_email_template(quote_id, tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->preview_quote_email_template: #{e}"
end
```

#### Using the preview_quote_email_template_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> preview_quote_email_template_with_http_info(quote_id, tenant_id, opts)

```ruby
begin
  # Preview the rendered email for an invoice.
  data, status_code, headers = api_instance.preview_quote_email_template_with_http_info(quote_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->preview_quote_email_template_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **quote_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined


## quote_line_exists

> <BooleanEnvelope> quote_line_exists(tenant_id, quote_id, opts)

Check if a quote line exists.

Checks if a quote line exists for the specified quote and tenant, by quote line ID or item ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quote_line_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
}

begin
  # Check if a quote line exists.
  result = api_instance.quote_line_exists(tenant_id, quote_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->quote_line_exists: #{e}"
end
```

#### Using the quote_line_exists_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> quote_line_exists_with_http_info(tenant_id, quote_id, opts)

```ruby
begin
  # Check if a quote line exists.
  data, status_code, headers = api_instance.quote_line_exists_with_http_info(tenant_id, quote_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->quote_line_exists_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **quote_line_id** | **String** |  | [optional] |
| **item_id** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## reopen_quote

> <EmptyEnvelope> reopen_quote(tenant_id, quote_id)

Reopen a closed quote.

Reopens a previously closed quote for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Reopen a closed quote.
  result = api_instance.reopen_quote(tenant_id, quote_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->reopen_quote: #{e}"
end
```

#### Using the reopen_quote_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> reopen_quote_with_http_info(tenant_id, quote_id)

```ruby
begin
  # Reopen a closed quote.
  data, status_code, headers = api_instance.reopen_quote_with_http_info(tenant_id, quote_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->reopen_quote_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## send_quote_email

> <EmptyEnvelope> send_quote_email(tenant_id, quote_id, opts)

Send a quote transactional email to recipients.

This action is only available for users with the 'send_email' permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Send a quote transactional email to recipients.
  result = api_instance.send_quote_email(tenant_id, quote_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->send_quote_email: #{e}"
end
```

#### Using the send_quote_email_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> send_quote_email_with_http_info(tenant_id, quote_id, opts)

```ruby
begin
  # Send a quote transactional email to recipients.
  data, status_code, headers = api_instance.send_quote_email_with_http_info(tenant_id, quote_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->send_quote_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_quote

> <EmptyEnvelope> update_quote(tenant_id, quote_id, opts)

Update an existing quote.

Updates an existing quote for the specified tenant and quote ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quote_update_dto: OpenapiClient::QuoteUpdateDto.new # QuoteUpdateDto | 
}

begin
  # Update an existing quote.
  result = api_instance.update_quote(tenant_id, quote_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->update_quote: #{e}"
end
```

#### Using the update_quote_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_quote_with_http_info(tenant_id, quote_id, opts)

```ruby
begin
  # Update an existing quote.
  data, status_code, headers = api_instance.update_quote_with_http_info(tenant_id, quote_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->update_quote_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **quote_update_dto** | [**QuoteUpdateDto**](QuoteUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_quote_line

> <EmptyEnvelope> update_quote_line(tenant_id, quote_id, quote_line_id, opts)

Update a quote line.

Updates an existing quote line for the specified quote and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quote_line_update_dto: OpenapiClient::QuoteLineUpdateDto.new # QuoteLineUpdateDto | 
}

begin
  # Update a quote line.
  result = api_instance.update_quote_line(tenant_id, quote_id, quote_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->update_quote_line: #{e}"
end
```

#### Using the update_quote_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_quote_line_with_http_info(tenant_id, quote_id, quote_line_id, opts)

```ruby
begin
  # Update a quote line.
  data, status_code, headers = api_instance.update_quote_line_with_http_info(tenant_id, quote_id, quote_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->update_quote_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **quote_line_id** | **String** |  |  |
| **quote_line_update_dto** | [**QuoteLineUpdateDto**](QuoteLineUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## upsert_quote_line

> <EmptyEnvelope> upsert_quote_line(tenant_id, quote_id, quote_line_id, opts)

Upsert a quote line.

Creates or updates a quote line for the specified quote and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::QuotesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
quote_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  quote_line_upsert_dto: OpenapiClient::QuoteLineUpsertDto.new # QuoteLineUpsertDto | 
}

begin
  # Upsert a quote line.
  result = api_instance.upsert_quote_line(tenant_id, quote_id, quote_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->upsert_quote_line: #{e}"
end
```

#### Using the upsert_quote_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> upsert_quote_line_with_http_info(tenant_id, quote_id, quote_line_id, opts)

```ruby
begin
  # Upsert a quote line.
  data, status_code, headers = api_instance.upsert_quote_line_with_http_info(tenant_id, quote_id, quote_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->upsert_quote_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **quote_id** | **String** |  |  |
| **quote_line_id** | **String** |  |  |
| **quote_line_upsert_dto** | [**QuoteLineUpsertDto**](QuoteLineUpsertDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

