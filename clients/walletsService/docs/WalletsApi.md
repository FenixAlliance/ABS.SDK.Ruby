# OpenapiClient::WalletsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_wallet_location_async**](WalletsApi.md#create_wallet_location_async) | **POST** /api/v2/WalletsService/Wallets/{walletId}/Locations | Create Wallet Location |
| [**delete_wallet_location_async**](WalletsApi.md#delete_wallet_location_async) | **DELETE** /api/v2/WalletsService/Wallets/{walletId}/Locations/{locationId} | Delete Wallet Location |
| [**get_incoming_payments_async**](WalletsApi.md#get_incoming_payments_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Incoming | Get Incoming Payments |
| [**get_incoming_payments_count_async**](WalletsApi.md#get_incoming_payments_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Incoming/Count | Get Incoming Payments Count |
| [**get_incoming_wallet_invoices_async**](WalletsApi.md#get_incoming_wallet_invoices_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Incoming | Get Incoming Wallet Invoices |
| [**get_incoming_wallet_invoices_count_async**](WalletsApi.md#get_incoming_wallet_invoices_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Incoming/Count | Get Incoming Wallet Invoices Count |
| [**get_outgoing_payments_async**](WalletsApi.md#get_outgoing_payments_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Outgoing | Get Outgoing Payments |
| [**get_outgoing_payments_count_async**](WalletsApi.md#get_outgoing_payments_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Outgoing/Count | Get Outgoing Payments Count |
| [**get_outgoing_wallet_invoices_async**](WalletsApi.md#get_outgoing_wallet_invoices_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Outgoing | Get Outgoing Wallet Invoices |
| [**get_outgoing_wallet_invoices_count_async**](WalletsApi.md#get_outgoing_wallet_invoices_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Outgoing/Count | Get Outgoing Wallet Invoices Count |
| [**get_wallet_details_async**](WalletsApi.md#get_wallet_details_async) | **GET** /api/v2/WalletsService/Wallets/{walletId} | Get Wallet Details |
| [**get_wallet_extended_orders_async**](WalletsApi.md#get_wallet_extended_orders_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Orders/Extended | Get Wallet Extended Orders |
| [**get_wallet_invoices_async**](WalletsApi.md#get_wallet_invoices_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices | Get Wallet Invoices |
| [**get_wallet_invoices_count_async**](WalletsApi.md#get_wallet_invoices_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Count | Get Wallet Invoices Count |
| [**get_wallet_location_async**](WalletsApi.md#get_wallet_location_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Locations/{locationId} | Get Wallet Location |
| [**get_wallet_locations_async**](WalletsApi.md#get_wallet_locations_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Locations | Get Wallet Locations |
| [**get_wallet_locations_count_async**](WalletsApi.md#get_wallet_locations_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Locations/Count | Get Wallet Locations Count |
| [**get_wallet_orders_async**](WalletsApi.md#get_wallet_orders_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Orders | Get Wallet Orders |
| [**get_wallet_orders_count_async**](WalletsApi.md#get_wallet_orders_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Orders/Count | Get Wallet Orders Count |
| [**get_wallet_payments_async**](WalletsApi.md#get_wallet_payments_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments | Get Wallet Payments |
| [**get_wallet_payments_count_async**](WalletsApi.md#get_wallet_payments_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Count | Get Wallet Payments Count |
| [**update_wallet_location_async**](WalletsApi.md#update_wallet_location_async) | **PUT** /api/v2/WalletsService/Wallets/{walletId}/Locations/{locationId} | Update Wallet Location |


## create_wallet_location_async

> <EmptyEnvelope> create_wallet_location_async(wallet_id, opts)

Create Wallet Location

Create a new location for a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  location_create_dto: OpenapiClient::LocationCreateDto.new # LocationCreateDto | 
}

begin
  # Create Wallet Location
  result = api_instance.create_wallet_location_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->create_wallet_location_async: #{e}"
end
```

#### Using the create_wallet_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_wallet_location_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Create Wallet Location
  data, status_code, headers = api_instance.create_wallet_location_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->create_wallet_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **location_create_dto** | [**LocationCreateDto**](LocationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_wallet_location_async

> <EmptyEnvelope> delete_wallet_location_async(wallet_id, location_id, opts)

Delete Wallet Location

Delete a specific location of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
location_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete Wallet Location
  result = api_instance.delete_wallet_location_async(wallet_id, location_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->delete_wallet_location_async: #{e}"
end
```

#### Using the delete_wallet_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_wallet_location_async_with_http_info(wallet_id, location_id, opts)

```ruby
begin
  # Delete Wallet Location
  data, status_code, headers = api_instance.delete_wallet_location_async_with_http_info(wallet_id, location_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->delete_wallet_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **location_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_incoming_payments_async

> <PaymentDtoListEnvelope> get_incoming_payments_async(wallet_id, opts)

Get Incoming Payments

Get incoming payments of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Incoming Payments
  result = api_instance.get_incoming_payments_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_incoming_payments_async: #{e}"
end
```

#### Using the get_incoming_payments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentDtoListEnvelope>, Integer, Hash)> get_incoming_payments_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Incoming Payments
  data, status_code, headers = api_instance.get_incoming_payments_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_incoming_payments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_incoming_payments_count_async

> <Int32Envelope> get_incoming_payments_count_async(wallet_id, opts)

Get Incoming Payments Count

Get incoming payments count of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Incoming Payments Count
  result = api_instance.get_incoming_payments_count_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_incoming_payments_count_async: #{e}"
end
```

#### Using the get_incoming_payments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_incoming_payments_count_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Incoming Payments Count
  data, status_code, headers = api_instance.get_incoming_payments_count_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_incoming_payments_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_incoming_wallet_invoices_async

> <InvoiceDtoListEnvelope> get_incoming_wallet_invoices_async(wallet_id, opts)

Get Incoming Wallet Invoices

Get incoming invoices of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Incoming Wallet Invoices
  result = api_instance.get_incoming_wallet_invoices_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_incoming_wallet_invoices_async: #{e}"
end
```

#### Using the get_incoming_wallet_invoices_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceDtoListEnvelope>, Integer, Hash)> get_incoming_wallet_invoices_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Incoming Wallet Invoices
  data, status_code, headers = api_instance.get_incoming_wallet_invoices_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_incoming_wallet_invoices_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InvoiceDtoListEnvelope**](InvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_incoming_wallet_invoices_count_async

> <Int32Envelope> get_incoming_wallet_invoices_count_async(wallet_id, opts)

Get Incoming Wallet Invoices Count

Get incoming invoices count of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Incoming Wallet Invoices Count
  result = api_instance.get_incoming_wallet_invoices_count_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_incoming_wallet_invoices_count_async: #{e}"
end
```

#### Using the get_incoming_wallet_invoices_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_incoming_wallet_invoices_count_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Incoming Wallet Invoices Count
  data, status_code, headers = api_instance.get_incoming_wallet_invoices_count_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_incoming_wallet_invoices_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_outgoing_payments_async

> <PaymentDtoListEnvelope> get_outgoing_payments_async(wallet_id, opts)

Get Outgoing Payments

Get outgoing payments of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Outgoing Payments
  result = api_instance.get_outgoing_payments_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_outgoing_payments_async: #{e}"
end
```

#### Using the get_outgoing_payments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentDtoListEnvelope>, Integer, Hash)> get_outgoing_payments_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Outgoing Payments
  data, status_code, headers = api_instance.get_outgoing_payments_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_outgoing_payments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_outgoing_payments_count_async

> <Int32Envelope> get_outgoing_payments_count_async(wallet_id, opts)

Get Outgoing Payments Count

Get outgoing payments count of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Outgoing Payments Count
  result = api_instance.get_outgoing_payments_count_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_outgoing_payments_count_async: #{e}"
end
```

#### Using the get_outgoing_payments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_outgoing_payments_count_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Outgoing Payments Count
  data, status_code, headers = api_instance.get_outgoing_payments_count_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_outgoing_payments_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_outgoing_wallet_invoices_async

> <InvoiceDtoListEnvelope> get_outgoing_wallet_invoices_async(wallet_id, opts)

Get Outgoing Wallet Invoices

Get outgoing invoices of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Outgoing Wallet Invoices
  result = api_instance.get_outgoing_wallet_invoices_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_outgoing_wallet_invoices_async: #{e}"
end
```

#### Using the get_outgoing_wallet_invoices_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceDtoListEnvelope>, Integer, Hash)> get_outgoing_wallet_invoices_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Outgoing Wallet Invoices
  data, status_code, headers = api_instance.get_outgoing_wallet_invoices_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_outgoing_wallet_invoices_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InvoiceDtoListEnvelope**](InvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_outgoing_wallet_invoices_count_async

> <Int32Envelope> get_outgoing_wallet_invoices_count_async(wallet_id, opts)

Get Outgoing Wallet Invoices Count

Get outgoing invoices count of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Outgoing Wallet Invoices Count
  result = api_instance.get_outgoing_wallet_invoices_count_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_outgoing_wallet_invoices_count_async: #{e}"
end
```

#### Using the get_outgoing_wallet_invoices_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_outgoing_wallet_invoices_count_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Outgoing Wallet Invoices Count
  data, status_code, headers = api_instance.get_outgoing_wallet_invoices_count_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_outgoing_wallet_invoices_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_details_async

> <WalletDtoEnvelope> get_wallet_details_async(wallet_id, opts)

Get Wallet Details

Get details of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Details
  result = api_instance.get_wallet_details_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_details_async: #{e}"
end
```

#### Using the get_wallet_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WalletDtoEnvelope>, Integer, Hash)> get_wallet_details_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Details
  data, status_code, headers = api_instance.get_wallet_details_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WalletDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WalletDtoEnvelope**](WalletDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_extended_orders_async

> <ExtendedOrderDtoListEnvelope> get_wallet_extended_orders_async(wallet_id, opts)

Get Wallet Extended Orders

Get extended orders of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Extended Orders
  result = api_instance.get_wallet_extended_orders_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_extended_orders_async: #{e}"
end
```

#### Using the get_wallet_extended_orders_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedOrderDtoListEnvelope>, Integer, Hash)> get_wallet_extended_orders_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Extended Orders
  data, status_code, headers = api_instance.get_wallet_extended_orders_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedOrderDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_extended_orders_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExtendedOrderDtoListEnvelope**](ExtendedOrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_invoices_async

> <InvoiceDtoListEnvelope> get_wallet_invoices_async(wallet_id, opts)

Get Wallet Invoices

Get invoices of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Invoices
  result = api_instance.get_wallet_invoices_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_invoices_async: #{e}"
end
```

#### Using the get_wallet_invoices_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceDtoListEnvelope>, Integer, Hash)> get_wallet_invoices_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Invoices
  data, status_code, headers = api_instance.get_wallet_invoices_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_invoices_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InvoiceDtoListEnvelope**](InvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_invoices_count_async

> <Int32Envelope> get_wallet_invoices_count_async(wallet_id, opts)

Get Wallet Invoices Count

Get invoices count of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Invoices Count
  result = api_instance.get_wallet_invoices_count_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_invoices_count_async: #{e}"
end
```

#### Using the get_wallet_invoices_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_wallet_invoices_count_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Invoices Count
  data, status_code, headers = api_instance.get_wallet_invoices_count_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_invoices_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_location_async

> <LocationDtoEnvelope> get_wallet_location_async(wallet_id, location_id, opts)

Get Wallet Location

Get a specific location of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
location_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Location
  result = api_instance.get_wallet_location_async(wallet_id, location_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_location_async: #{e}"
end
```

#### Using the get_wallet_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LocationDtoEnvelope>, Integer, Hash)> get_wallet_location_async_with_http_info(wallet_id, location_id, opts)

```ruby
begin
  # Get Wallet Location
  data, status_code, headers = api_instance.get_wallet_location_async_with_http_info(wallet_id, location_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LocationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **location_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LocationDtoEnvelope**](LocationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_locations_async

> <LocationDtoListEnvelope> get_wallet_locations_async(wallet_id, opts)

Get Wallet Locations

Get locations of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Locations
  result = api_instance.get_wallet_locations_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_locations_async: #{e}"
end
```

#### Using the get_wallet_locations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LocationDtoListEnvelope>, Integer, Hash)> get_wallet_locations_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Locations
  data, status_code, headers = api_instance.get_wallet_locations_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LocationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_locations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LocationDtoListEnvelope**](LocationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_locations_count_async

> <Int32Envelope> get_wallet_locations_count_async(wallet_id, opts)

Get Wallet Locations Count

Get locations count of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Locations Count
  result = api_instance.get_wallet_locations_count_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_locations_count_async: #{e}"
end
```

#### Using the get_wallet_locations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_wallet_locations_count_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Locations Count
  data, status_code, headers = api_instance.get_wallet_locations_count_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_locations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_orders_async

> <OrderDtoListEnvelope> get_wallet_orders_async(wallet_id, opts)

Get Wallet Orders

Get orders of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Orders
  result = api_instance.get_wallet_orders_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_orders_async: #{e}"
end
```

#### Using the get_wallet_orders_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OrderDtoListEnvelope>, Integer, Hash)> get_wallet_orders_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Orders
  data, status_code, headers = api_instance.get_wallet_orders_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OrderDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_orders_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OrderDtoListEnvelope**](OrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_orders_count_async

> <Int32Envelope> get_wallet_orders_count_async(wallet_id, opts)

Get Wallet Orders Count

Get orders count of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Orders Count
  result = api_instance.get_wallet_orders_count_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_orders_count_async: #{e}"
end
```

#### Using the get_wallet_orders_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_wallet_orders_count_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Orders Count
  data, status_code, headers = api_instance.get_wallet_orders_count_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_orders_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_payments_async

> <PaymentDtoListEnvelope> get_wallet_payments_async(wallet_id, opts)

Get Wallet Payments

Get payments of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Payments
  result = api_instance.get_wallet_payments_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_payments_async: #{e}"
end
```

#### Using the get_wallet_payments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentDtoListEnvelope>, Integer, Hash)> get_wallet_payments_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Payments
  data, status_code, headers = api_instance.get_wallet_payments_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_payments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_wallet_payments_count_async

> <Int32Envelope> get_wallet_payments_count_async(wallet_id, opts)

Get Wallet Payments Count

Get payments count of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Wallet Payments Count
  result = api_instance.get_wallet_payments_count_async(wallet_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_payments_count_async: #{e}"
end
```

#### Using the get_wallet_payments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_wallet_payments_count_async_with_http_info(wallet_id, opts)

```ruby
begin
  # Get Wallet Payments Count
  data, status_code, headers = api_instance.get_wallet_payments_count_async_with_http_info(wallet_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->get_wallet_payments_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_wallet_location_async

> <EmptyEnvelope> update_wallet_location_async(wallet_id, location_id, opts)

Update Wallet Location

Update a specific location of a specific wallet by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WalletsApi.new
wallet_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
location_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  location_update_dto: OpenapiClient::LocationUpdateDto.new # LocationUpdateDto | 
}

begin
  # Update Wallet Location
  result = api_instance.update_wallet_location_async(wallet_id, location_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->update_wallet_location_async: #{e}"
end
```

#### Using the update_wallet_location_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_wallet_location_async_with_http_info(wallet_id, location_id, opts)

```ruby
begin
  # Update Wallet Location
  data, status_code, headers = api_instance.update_wallet_location_async_with_http_info(wallet_id, location_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WalletsApi->update_wallet_location_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **wallet_id** | **String** |  |  |
| **location_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **location_update_dto** | [**LocationUpdateDto**](LocationUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

