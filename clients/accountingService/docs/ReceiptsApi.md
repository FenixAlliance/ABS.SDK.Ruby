# OpenapiClient::ReceiptsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_receipt_async**](ReceiptsApi.md#create_receipt_async) | **POST** /api/v2/AccountingService/Receipts | Creates a new receipt |
| [**delete_receipt_async**](ReceiptsApi.md#delete_receipt_async) | **DELETE** /api/v2/AccountingService/Receipts/{receiptId} | Deletes a receipt |
| [**get_receipt_details_async**](ReceiptsApi.md#get_receipt_details_async) | **GET** /api/v2/AccountingService/Receipts/{receiptId} | Gets details of a receipt |
| [**get_receipts_async**](ReceiptsApi.md#get_receipts_async) | **GET** /api/v2/AccountingService/Receipts | Retrieves tenant receipts |
| [**get_receipts_count_async**](ReceiptsApi.md#get_receipts_count_async) | **GET** /api/v2/AccountingService/Receipts/Count | Gets count of tenant receipts |
| [**update_receipt_async**](ReceiptsApi.md#update_receipt_async) | **PUT** /api/v2/AccountingService/Receipts/{receiptId} | Updates a receipt |


## create_receipt_async

> <EmptyEnvelope> create_receipt_async(tenant_id, receipt_create_dto)

Creates a new receipt

Adds a new receipt record under the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReceiptsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
receipt_create_dto = OpenapiClient::ReceiptCreateDto.new # ReceiptCreateDto | 

begin
  # Creates a new receipt
  result = api_instance.create_receipt_async(tenant_id, receipt_create_dto)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->create_receipt_async: #{e}"
end
```

#### Using the create_receipt_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_receipt_async_with_http_info(tenant_id, receipt_create_dto)

```ruby
begin
  # Creates a new receipt
  data, status_code, headers = api_instance.create_receipt_async_with_http_info(tenant_id, receipt_create_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->create_receipt_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **receipt_create_dto** | [**ReceiptCreateDto**](ReceiptCreateDto.md) |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_receipt_async

> <EmptyEnvelope> delete_receipt_async(tenant_id, receipt_id)

Deletes a receipt

Removes an existing receipt from the tenant’s records.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReceiptsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
receipt_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a receipt
  result = api_instance.delete_receipt_async(tenant_id, receipt_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->delete_receipt_async: #{e}"
end
```

#### Using the delete_receipt_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_receipt_async_with_http_info(tenant_id, receipt_id)

```ruby
begin
  # Deletes a receipt
  data, status_code, headers = api_instance.delete_receipt_async_with_http_info(tenant_id, receipt_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->delete_receipt_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **receipt_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_receipt_details_async

> <ReceiptDtoEnvelope> get_receipt_details_async(tenant_id, receipt_id)

Gets details of a receipt

Retrieves a specific receipt by its ID for the given tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReceiptsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
receipt_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets details of a receipt
  result = api_instance.get_receipt_details_async(tenant_id, receipt_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->get_receipt_details_async: #{e}"
end
```

#### Using the get_receipt_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ReceiptDtoEnvelope>, Integer, Hash)> get_receipt_details_async_with_http_info(tenant_id, receipt_id)

```ruby
begin
  # Gets details of a receipt
  data, status_code, headers = api_instance.get_receipt_details_async_with_http_info(tenant_id, receipt_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ReceiptDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->get_receipt_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **receipt_id** | **String** |  |  |

### Return type

[**ReceiptDtoEnvelope**](ReceiptDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_receipts_async

> <ReceiptDtoIReadOnlyListEnvelope> get_receipts_async(tenant_id)

Retrieves tenant receipts

Fetches all receipts for a given tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReceiptsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Retrieves tenant receipts
  result = api_instance.get_receipts_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->get_receipts_async: #{e}"
end
```

#### Using the get_receipts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ReceiptDtoIReadOnlyListEnvelope>, Integer, Hash)> get_receipts_async_with_http_info(tenant_id)

```ruby
begin
  # Retrieves tenant receipts
  data, status_code, headers = api_instance.get_receipts_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ReceiptDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->get_receipts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**ReceiptDtoIReadOnlyListEnvelope**](ReceiptDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_receipts_count_async

> <Int32Envelope> get_receipts_count_async(tenant_id)

Gets count of tenant receipts

Returns total number of receipts for the tenant with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReceiptsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets count of tenant receipts
  result = api_instance.get_receipts_count_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->get_receipts_count_async: #{e}"
end
```

#### Using the get_receipts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_receipts_count_async_with_http_info(tenant_id)

```ruby
begin
  # Gets count of tenant receipts
  data, status_code, headers = api_instance.get_receipts_count_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->get_receipts_count_async_with_http_info: #{e}"
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


## update_receipt_async

> <EmptyEnvelope> update_receipt_async(tenant_id, receipt_id, receipt_update_dto)

Updates a receipt

Modifies the data of an existing receipt for the given tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ReceiptsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
receipt_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
receipt_update_dto = OpenapiClient::ReceiptUpdateDto.new # ReceiptUpdateDto | 

begin
  # Updates a receipt
  result = api_instance.update_receipt_async(tenant_id, receipt_id, receipt_update_dto)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->update_receipt_async: #{e}"
end
```

#### Using the update_receipt_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_receipt_async_with_http_info(tenant_id, receipt_id, receipt_update_dto)

```ruby
begin
  # Updates a receipt
  data, status_code, headers = api_instance.update_receipt_async_with_http_info(tenant_id, receipt_id, receipt_update_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ReceiptsApi->update_receipt_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **receipt_id** | **String** |  |  |
| **receipt_update_dto** | [**ReceiptUpdateDto**](ReceiptUpdateDto.md) |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

