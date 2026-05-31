# OpenapiClient::MigrationsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**migrate**](MigrationsApi.md#migrate) | **POST** /api/v2/SystemService/Migrations/Migrate | Apply pending database migrations |
| [**migrations**](MigrationsApi.md#migrations) | **GET** /api/v2/SystemService/Migrations | Retrieve database migrations |


## migrate

> <StringListEnvelope> migrate(opts)

Apply pending database migrations

Applies all pending database migrations and returns the list of migrations that were applied.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MigrationsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Apply pending database migrations
  result = api_instance.migrate(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MigrationsApi->migrate: #{e}"
end
```

#### Using the migrate_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StringListEnvelope>, Integer, Hash)> migrate_with_http_info(opts)

```ruby
begin
  # Apply pending database migrations
  data, status_code, headers = api_instance.migrate_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StringListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MigrationsApi->migrate_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**StringListEnvelope**](StringListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## migrations

> <StringListEnvelope> migrations(opts)

Retrieve database migrations

Retrieves the list of applied or pending database migrations.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MigrationsApi.new
opts = {
  pending: true, # Boolean | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve database migrations
  result = api_instance.migrations(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MigrationsApi->migrations: #{e}"
end
```

#### Using the migrations_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StringListEnvelope>, Integer, Hash)> migrations_with_http_info(opts)

```ruby
begin
  # Retrieve database migrations
  data, status_code, headers = api_instance.migrations_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StringListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MigrationsApi->migrations_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **pending** | **Boolean** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**StringListEnvelope**](StringListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

