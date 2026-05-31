# OpenapiClient::DealUnitsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**calculate_deal_unit_async**](DealUnitsApi.md#calculate_deal_unit_async) | **PUT** /api/v2/DealsService/DealUnits/{dealUnitId}/Calculate | Calculate a deal unit |
| [**calculate_deal_unit_line_async**](DealUnitsApi.md#calculate_deal_unit_line_async) | **PUT** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/{dealUnitLineId}/Calculate | Calculate a deal unit line |
| [**create_deal_unit_async**](DealUnitsApi.md#create_deal_unit_async) | **POST** /api/v2/DealsService/DealUnits | Create a deal unit |
| [**create_get_deal_unit_lines_async**](DealUnitsApi.md#create_get_deal_unit_lines_async) | **POST** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines | Create a deal unit line |
| [**delete_deal_unit_async**](DealUnitsApi.md#delete_deal_unit_async) | **DELETE** /api/v2/DealsService/DealUnits/{dealUnitId} | Delete a deal unit |
| [**delete_deal_unit_price_async**](DealUnitsApi.md#delete_deal_unit_price_async) | **DELETE** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/{dealUnitLineId} | Delete a deal unit line |
| [**get_deal_unit_async**](DealUnitsApi.md#get_deal_unit_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId} | Get deal unit by ID |
| [**get_deal_unit_lines_async**](DealUnitsApi.md#get_deal_unit_lines_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines | Get deal unit lines |
| [**get_deal_unit_lines_count_async**](DealUnitsApi.md#get_deal_unit_lines_count_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/Count | Get deal unit lines count |
| [**get_deal_unit_price_async**](DealUnitsApi.md#get_deal_unit_price_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/{dealUnitLineId} | Get a deal unit line by ID |
| [**get_deal_units_async**](DealUnitsApi.md#get_deal_units_async) | **GET** /api/v2/DealsService/DealUnits | Get deal units |
| [**get_deal_units_count_async**](DealUnitsApi.md#get_deal_units_count_async) | **GET** /api/v2/DealsService/DealUnits/Count | Get deal units count |
| [**get_extended_deal_unit_async**](DealUnitsApi.md#get_extended_deal_unit_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId}/Extended | Get extended deal unit by ID |
| [**get_extended_deal_units_async**](DealUnitsApi.md#get_extended_deal_units_async) | **GET** /api/v2/DealsService/DealUnits/Extended | Get extended deal units |
| [**update_deal_unit_async**](DealUnitsApi.md#update_deal_unit_async) | **PUT** /api/v2/DealsService/DealUnits/{dealUnitId} | Update a deal unit |
| [**update_deal_unit_price_async**](DealUnitsApi.md#update_deal_unit_price_async) | **PUT** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/{dealUnitLineId} | Update a deal unit line |


## calculate_deal_unit_async

> <EmptyEnvelope> calculate_deal_unit_async(tenant_id, deal_unit_id)

Calculate a deal unit

Triggers recalculation of totals and derived values for a specific deal unit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Calculate a deal unit
  result = api_instance.calculate_deal_unit_async(tenant_id, deal_unit_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->calculate_deal_unit_async: #{e}"
end
```

#### Using the calculate_deal_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> calculate_deal_unit_async_with_http_info(tenant_id, deal_unit_id)

```ruby
begin
  # Calculate a deal unit
  data, status_code, headers = api_instance.calculate_deal_unit_async_with_http_info(tenant_id, deal_unit_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->calculate_deal_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## calculate_deal_unit_line_async

> <EmptyEnvelope> calculate_deal_unit_line_async(tenant_id, deal_unit_id, deal_unit_line_id)

Calculate a deal unit line

Triggers recalculation of totals and derived values for a specific deal unit line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Calculate a deal unit line
  result = api_instance.calculate_deal_unit_line_async(tenant_id, deal_unit_id, deal_unit_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->calculate_deal_unit_line_async: #{e}"
end
```

#### Using the calculate_deal_unit_line_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> calculate_deal_unit_line_async_with_http_info(tenant_id, deal_unit_id, deal_unit_line_id)

```ruby
begin
  # Calculate a deal unit line
  data, status_code, headers = api_instance.calculate_deal_unit_line_async_with_http_info(tenant_id, deal_unit_id, deal_unit_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->calculate_deal_unit_line_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |
| **deal_unit_line_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_deal_unit_async

> <EmptyEnvelope> create_deal_unit_async(tenant_id, opts)

Create a deal unit

Creates a new deal unit for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  deal_unit_create_dto: OpenapiClient::DealUnitCreateDto.new # DealUnitCreateDto | 
}

begin
  # Create a deal unit
  result = api_instance.create_deal_unit_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->create_deal_unit_async: #{e}"
end
```

#### Using the create_deal_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_deal_unit_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a deal unit
  data, status_code, headers = api_instance.create_deal_unit_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->create_deal_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_create_dto** | [**DealUnitCreateDto**](DealUnitCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_get_deal_unit_lines_async

> <EmptyEnvelope> create_get_deal_unit_lines_async(tenant_id, deal_unit_id, opts)

Create a deal unit line

Creates a new line within a specific deal unit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  deal_unit_line_create_dto: OpenapiClient::DealUnitLineCreateDto.new # DealUnitLineCreateDto | 
}

begin
  # Create a deal unit line
  result = api_instance.create_get_deal_unit_lines_async(tenant_id, deal_unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->create_get_deal_unit_lines_async: #{e}"
end
```

#### Using the create_get_deal_unit_lines_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_get_deal_unit_lines_async_with_http_info(tenant_id, deal_unit_id, opts)

```ruby
begin
  # Create a deal unit line
  data, status_code, headers = api_instance.create_get_deal_unit_lines_async_with_http_info(tenant_id, deal_unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->create_get_deal_unit_lines_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |
| **deal_unit_line_create_dto** | [**DealUnitLineCreateDto**](DealUnitLineCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_deal_unit_async

> <EmptyEnvelope> delete_deal_unit_async(tenant_id, deal_unit_id)

Delete a deal unit

Deletes an existing deal unit by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a deal unit
  result = api_instance.delete_deal_unit_async(tenant_id, deal_unit_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->delete_deal_unit_async: #{e}"
end
```

#### Using the delete_deal_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_deal_unit_async_with_http_info(tenant_id, deal_unit_id)

```ruby
begin
  # Delete a deal unit
  data, status_code, headers = api_instance.delete_deal_unit_async_with_http_info(tenant_id, deal_unit_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->delete_deal_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_deal_unit_price_async

> <EmptyEnvelope> delete_deal_unit_price_async(tenant_id, deal_unit_id, deal_unit_line_id)

Delete a deal unit line

Deletes an existing line from a specific deal unit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a deal unit line
  result = api_instance.delete_deal_unit_price_async(tenant_id, deal_unit_id, deal_unit_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->delete_deal_unit_price_async: #{e}"
end
```

#### Using the delete_deal_unit_price_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_deal_unit_price_async_with_http_info(tenant_id, deal_unit_id, deal_unit_line_id)

```ruby
begin
  # Delete a deal unit line
  data, status_code, headers = api_instance.delete_deal_unit_price_async_with_http_info(tenant_id, deal_unit_id, deal_unit_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->delete_deal_unit_price_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |
| **deal_unit_line_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_async

> <DealUnitDtoEnvelope> get_deal_unit_async(tenant_id, deal_unit_id)

Get deal unit by ID

Retrieves a single deal unit by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get deal unit by ID
  result = api_instance.get_deal_unit_async(tenant_id, deal_unit_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_unit_async: #{e}"
end
```

#### Using the get_deal_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DealUnitDtoEnvelope>, Integer, Hash)> get_deal_unit_async_with_http_info(tenant_id, deal_unit_id)

```ruby
begin
  # Get deal unit by ID
  data, status_code, headers = api_instance.get_deal_unit_async_with_http_info(tenant_id, deal_unit_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DealUnitDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |

### Return type

[**DealUnitDtoEnvelope**](DealUnitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_lines_async

> <DealUnitLineDtoListEnvelope> get_deal_unit_lines_async(tenant_id, deal_unit_id, opts)

Get deal unit lines

Retrieves a list of lines for a specific deal unit with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
}

begin
  # Get deal unit lines
  result = api_instance.get_deal_unit_lines_async(tenant_id, deal_unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_unit_lines_async: #{e}"
end
```

#### Using the get_deal_unit_lines_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DealUnitLineDtoListEnvelope>, Integer, Hash)> get_deal_unit_lines_async_with_http_info(tenant_id, deal_unit_id, opts)

```ruby
begin
  # Get deal unit lines
  data, status_code, headers = api_instance.get_deal_unit_lines_async_with_http_info(tenant_id, deal_unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DealUnitLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_unit_lines_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |
| **item_id** | **String** |  | [optional] |

### Return type

[**DealUnitLineDtoListEnvelope**](DealUnitLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_lines_count_async

> <Int32Envelope> get_deal_unit_lines_count_async(tenant_id, deal_unit_id)

Get deal unit lines count

Returns the total count of lines for a specific deal unit with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get deal unit lines count
  result = api_instance.get_deal_unit_lines_count_async(tenant_id, deal_unit_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_unit_lines_count_async: #{e}"
end
```

#### Using the get_deal_unit_lines_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_deal_unit_lines_count_async_with_http_info(tenant_id, deal_unit_id)

```ruby
begin
  # Get deal unit lines count
  data, status_code, headers = api_instance.get_deal_unit_lines_count_async_with_http_info(tenant_id, deal_unit_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_unit_lines_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_price_async

> <DealUnitLineDtoEnvelope> get_deal_unit_price_async(tenant_id, deal_unit_id, deal_unit_line_id)

Get a deal unit line by ID

Retrieves a single deal unit line by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get a deal unit line by ID
  result = api_instance.get_deal_unit_price_async(tenant_id, deal_unit_id, deal_unit_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_unit_price_async: #{e}"
end
```

#### Using the get_deal_unit_price_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DealUnitLineDtoEnvelope>, Integer, Hash)> get_deal_unit_price_async_with_http_info(tenant_id, deal_unit_id, deal_unit_line_id)

```ruby
begin
  # Get a deal unit line by ID
  data, status_code, headers = api_instance.get_deal_unit_price_async_with_http_info(tenant_id, deal_unit_id, deal_unit_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DealUnitLineDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_unit_price_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |
| **deal_unit_line_id** | **String** |  |  |

### Return type

[**DealUnitLineDtoEnvelope**](DealUnitLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_units_async

> <DealUnitDtoListEnvelope> get_deal_units_async(tenant_id)

Get deal units

Retrieves a list of deal units for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get deal units
  result = api_instance.get_deal_units_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_units_async: #{e}"
end
```

#### Using the get_deal_units_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DealUnitDtoListEnvelope>, Integer, Hash)> get_deal_units_async_with_http_info(tenant_id)

```ruby
begin
  # Get deal units
  data, status_code, headers = api_instance.get_deal_units_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DealUnitDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_units_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**DealUnitDtoListEnvelope**](DealUnitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_units_count_async

> <Int32Envelope> get_deal_units_count_async(tenant_id)

Get deal units count

Returns the total count of deal units for the specified tenant with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get deal units count
  result = api_instance.get_deal_units_count_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_units_count_async: #{e}"
end
```

#### Using the get_deal_units_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_deal_units_count_async_with_http_info(tenant_id)

```ruby
begin
  # Get deal units count
  data, status_code, headers = api_instance.get_deal_units_count_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_deal_units_count_async_with_http_info: #{e}"
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


## get_extended_deal_unit_async

> <ExtendedDealUnitDtoEnvelope> get_extended_deal_unit_async(tenant_id, deal_unit_id)

Get extended deal unit by ID

Retrieves a single deal unit with extended details by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get extended deal unit by ID
  result = api_instance.get_extended_deal_unit_async(tenant_id, deal_unit_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_extended_deal_unit_async: #{e}"
end
```

#### Using the get_extended_deal_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedDealUnitDtoEnvelope>, Integer, Hash)> get_extended_deal_unit_async_with_http_info(tenant_id, deal_unit_id)

```ruby
begin
  # Get extended deal unit by ID
  data, status_code, headers = api_instance.get_extended_deal_unit_async_with_http_info(tenant_id, deal_unit_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedDealUnitDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_extended_deal_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |

### Return type

[**ExtendedDealUnitDtoEnvelope**](ExtendedDealUnitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_deal_units_async

> <ExtendedDealUnitDtoListEnvelope> get_extended_deal_units_async(tenant_id)

Get extended deal units

Retrieves a list of deal units with extended details for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get extended deal units
  result = api_instance.get_extended_deal_units_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_extended_deal_units_async: #{e}"
end
```

#### Using the get_extended_deal_units_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedDealUnitDtoListEnvelope>, Integer, Hash)> get_extended_deal_units_async_with_http_info(tenant_id)

```ruby
begin
  # Get extended deal units
  data, status_code, headers = api_instance.get_extended_deal_units_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedDealUnitDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->get_extended_deal_units_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**ExtendedDealUnitDtoListEnvelope**](ExtendedDealUnitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_deal_unit_async

> <EmptyEnvelope> update_deal_unit_async(tenant_id, deal_unit_id, opts)

Update a deal unit

Updates an existing deal unit by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  deal_unit_update_dto: OpenapiClient::DealUnitUpdateDto.new # DealUnitUpdateDto | 
}

begin
  # Update a deal unit
  result = api_instance.update_deal_unit_async(tenant_id, deal_unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->update_deal_unit_async: #{e}"
end
```

#### Using the update_deal_unit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_deal_unit_async_with_http_info(tenant_id, deal_unit_id, opts)

```ruby
begin
  # Update a deal unit
  data, status_code, headers = api_instance.update_deal_unit_async_with_http_info(tenant_id, deal_unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->update_deal_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |
| **deal_unit_update_dto** | [**DealUnitUpdateDto**](DealUnitUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_deal_unit_price_async

> <EmptyEnvelope> update_deal_unit_price_async(tenant_id, deal_unit_id, deal_unit_line_id, opts)

Update a deal unit line

Updates an existing line within a specific deal unit.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  deal_unit_line_update_dto: OpenapiClient::DealUnitLineUpdateDto.new # DealUnitLineUpdateDto | 
}

begin
  # Update a deal unit line
  result = api_instance.update_deal_unit_price_async(tenant_id, deal_unit_id, deal_unit_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->update_deal_unit_price_async: #{e}"
end
```

#### Using the update_deal_unit_price_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_deal_unit_price_async_with_http_info(tenant_id, deal_unit_id, deal_unit_line_id, opts)

```ruby
begin
  # Update a deal unit line
  data, status_code, headers = api_instance.update_deal_unit_price_async_with_http_info(tenant_id, deal_unit_id, deal_unit_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitsApi->update_deal_unit_price_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_id** | **String** |  |  |
| **deal_unit_line_id** | **String** |  |  |
| **deal_unit_line_update_dto** | [**DealUnitLineUpdateDto**](DealUnitLineUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

