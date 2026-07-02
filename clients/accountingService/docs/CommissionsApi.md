# OpenapiClient::CommissionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_commission_async**](CommissionsApi.md#create_commission_async) | **POST** /api/v2/AccountingService/Commissions/Commissions | Create a commission |
| [**create_payment_commission_async**](CommissionsApi.md#create_payment_commission_async) | **POST** /api/v2/AccountingService/Commissions/PaymentCommissions | Create a payment commission |
| [**delete_commission_async**](CommissionsApi.md#delete_commission_async) | **DELETE** /api/v2/AccountingService/Commissions/Commissions/{commissionId} | Delete a commission |
| [**delete_payment_commission_async**](CommissionsApi.md#delete_payment_commission_async) | **DELETE** /api/v2/AccountingService/Commissions/PaymentCommissions/{paymentCommissionId} | Delete a payment commission |
| [**get_commission_async**](CommissionsApi.md#get_commission_async) | **GET** /api/v2/AccountingService/Commissions/Commissions/{commissionId} | Get a commission by id |
| [**get_commissions_async**](CommissionsApi.md#get_commissions_async) | **GET** /api/v2/AccountingService/Commissions/Commissions | Get all commissions for a tenant |
| [**get_commissions_count_async**](CommissionsApi.md#get_commissions_count_async) | **GET** /api/v2/AccountingService/Commissions/Commissions/Count | Get the count of commissions for a tenant |
| [**get_payment_commission_async**](CommissionsApi.md#get_payment_commission_async) | **GET** /api/v2/AccountingService/Commissions/PaymentCommissions/{paymentCommissionId} | Get a payment commission by id |
| [**get_payment_commissions_async**](CommissionsApi.md#get_payment_commissions_async) | **GET** /api/v2/AccountingService/Commissions/PaymentCommissions | Get all payment commissions for a tenant |
| [**get_payment_commissions_count_async**](CommissionsApi.md#get_payment_commissions_count_async) | **GET** /api/v2/AccountingService/Commissions/PaymentCommissions/Count | Get the count of payment commissions for a tenant |
| [**patch_commission_async**](CommissionsApi.md#patch_commission_async) | **PATCH** /api/v2/AccountingService/Commissions/Commissions/{commissionId} | Patch a commission |
| [**patch_payment_commission_async**](CommissionsApi.md#patch_payment_commission_async) | **PATCH** /api/v2/AccountingService/Commissions/PaymentCommissions/{paymentCommissionId} | Patch a payment commission |
| [**update_commission_async**](CommissionsApi.md#update_commission_async) | **PUT** /api/v2/AccountingService/Commissions/Commissions/{commissionId} | Update a commission |
| [**update_payment_commission_async**](CommissionsApi.md#update_payment_commission_async) | **PUT** /api/v2/AccountingService/Commissions/PaymentCommissions/{paymentCommissionId} | Update a payment commission |


## create_commission_async

> <EmptyEnvelope> create_commission_async(tenant_id, commission_create_dto, opts)

Create a commission

Creates a new commission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
commission_create_dto = OpenapiClient::CommissionCreateDto.new # CommissionCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a commission
  result = api_instance.create_commission_async(tenant_id, commission_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->create_commission_async: #{e}"
end
```

#### Using the create_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_commission_async_with_http_info(tenant_id, commission_create_dto, opts)

```ruby
begin
  # Create a commission
  data, status_code, headers = api_instance.create_commission_async_with_http_info(tenant_id, commission_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->create_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **commission_create_dto** | [**CommissionCreateDto**](CommissionCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_payment_commission_async

> <EmptyEnvelope> create_payment_commission_async(tenant_id, payment_commission_create_dto, opts)

Create a payment commission

Creates a new payment commission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_commission_create_dto = OpenapiClient::PaymentCommissionCreateDto.new # PaymentCommissionCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a payment commission
  result = api_instance.create_payment_commission_async(tenant_id, payment_commission_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->create_payment_commission_async: #{e}"
end
```

#### Using the create_payment_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_payment_commission_async_with_http_info(tenant_id, payment_commission_create_dto, opts)

```ruby
begin
  # Create a payment commission
  data, status_code, headers = api_instance.create_payment_commission_async_with_http_info(tenant_id, payment_commission_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->create_payment_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_commission_create_dto** | [**PaymentCommissionCreateDto**](PaymentCommissionCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_commission_async

> <EmptyEnvelope> delete_commission_async(tenant_id, commission_id, opts)

Delete a commission

Deletes a commission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
commission_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a commission
  result = api_instance.delete_commission_async(tenant_id, commission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->delete_commission_async: #{e}"
end
```

#### Using the delete_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_commission_async_with_http_info(tenant_id, commission_id, opts)

```ruby
begin
  # Delete a commission
  data, status_code, headers = api_instance.delete_commission_async_with_http_info(tenant_id, commission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->delete_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **commission_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_payment_commission_async

> <EmptyEnvelope> delete_payment_commission_async(tenant_id, payment_commission_id, opts)

Delete a payment commission

Deletes a payment commission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_commission_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a payment commission
  result = api_instance.delete_payment_commission_async(tenant_id, payment_commission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->delete_payment_commission_async: #{e}"
end
```

#### Using the delete_payment_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_payment_commission_async_with_http_info(tenant_id, payment_commission_id, opts)

```ruby
begin
  # Delete a payment commission
  data, status_code, headers = api_instance.delete_payment_commission_async_with_http_info(tenant_id, payment_commission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->delete_payment_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_commission_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_commission_async

> <CommissionDtoEnvelope> get_commission_async(tenant_id, commission_id, opts)

Get a commission by id

Retrieves a commission by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
commission_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a commission by id
  result = api_instance.get_commission_async(tenant_id, commission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_commission_async: #{e}"
end
```

#### Using the get_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CommissionDtoEnvelope>, Integer, Hash)> get_commission_async_with_http_info(tenant_id, commission_id, opts)

```ruby
begin
  # Get a commission by id
  data, status_code, headers = api_instance.get_commission_async_with_http_info(tenant_id, commission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CommissionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **commission_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CommissionDtoEnvelope**](CommissionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_commissions_async

> <CommissionDtoListEnvelope> get_commissions_async(tenant_id, opts)

Get all commissions for a tenant

Retrieves all commissions for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all commissions for a tenant
  result = api_instance.get_commissions_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_commissions_async: #{e}"
end
```

#### Using the get_commissions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CommissionDtoListEnvelope>, Integer, Hash)> get_commissions_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all commissions for a tenant
  data, status_code, headers = api_instance.get_commissions_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CommissionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_commissions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CommissionDtoListEnvelope**](CommissionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_commissions_count_async

> <Int32Envelope> get_commissions_count_async(tenant_id, opts)

Get the count of commissions for a tenant

Retrieves the count of commissions for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of commissions for a tenant
  result = api_instance.get_commissions_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_commissions_count_async: #{e}"
end
```

#### Using the get_commissions_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_commissions_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of commissions for a tenant
  data, status_code, headers = api_instance.get_commissions_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_commissions_count_async_with_http_info: #{e}"
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


## get_payment_commission_async

> <PaymentCommissionDtoEnvelope> get_payment_commission_async(tenant_id, payment_commission_id, opts)

Get a payment commission by id

Retrieves a payment commission by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_commission_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a payment commission by id
  result = api_instance.get_payment_commission_async(tenant_id, payment_commission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_payment_commission_async: #{e}"
end
```

#### Using the get_payment_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentCommissionDtoEnvelope>, Integer, Hash)> get_payment_commission_async_with_http_info(tenant_id, payment_commission_id, opts)

```ruby
begin
  # Get a payment commission by id
  data, status_code, headers = api_instance.get_payment_commission_async_with_http_info(tenant_id, payment_commission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentCommissionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_payment_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_commission_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentCommissionDtoEnvelope**](PaymentCommissionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_commissions_async

> <PaymentCommissionDtoListEnvelope> get_payment_commissions_async(tenant_id, opts)

Get all payment commissions for a tenant

Retrieves all payment commissions for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all payment commissions for a tenant
  result = api_instance.get_payment_commissions_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_payment_commissions_async: #{e}"
end
```

#### Using the get_payment_commissions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentCommissionDtoListEnvelope>, Integer, Hash)> get_payment_commissions_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all payment commissions for a tenant
  data, status_code, headers = api_instance.get_payment_commissions_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentCommissionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_payment_commissions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PaymentCommissionDtoListEnvelope**](PaymentCommissionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_payment_commissions_count_async

> <Int32Envelope> get_payment_commissions_count_async(tenant_id, opts)

Get the count of payment commissions for a tenant

Retrieves the count of payment commissions for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of payment commissions for a tenant
  result = api_instance.get_payment_commissions_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_payment_commissions_count_async: #{e}"
end
```

#### Using the get_payment_commissions_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_payment_commissions_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of payment commissions for a tenant
  data, status_code, headers = api_instance.get_payment_commissions_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->get_payment_commissions_count_async_with_http_info: #{e}"
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


## patch_commission_async

> <EmptyEnvelope> patch_commission_async(tenant_id, commission_id, opts)

Patch a commission

Partially updates an existing commission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
commission_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a commission
  result = api_instance.patch_commission_async(tenant_id, commission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->patch_commission_async: #{e}"
end
```

#### Using the patch_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_commission_async_with_http_info(tenant_id, commission_id, opts)

```ruby
begin
  # Patch a commission
  data, status_code, headers = api_instance.patch_commission_async_with_http_info(tenant_id, commission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->patch_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **commission_id** | **String** |  |  |
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


## patch_payment_commission_async

> <EmptyEnvelope> patch_payment_commission_async(tenant_id, payment_commission_id, opts)

Patch a payment commission

Partially updates an existing payment commission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_commission_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a payment commission
  result = api_instance.patch_payment_commission_async(tenant_id, payment_commission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->patch_payment_commission_async: #{e}"
end
```

#### Using the patch_payment_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_payment_commission_async_with_http_info(tenant_id, payment_commission_id, opts)

```ruby
begin
  # Patch a payment commission
  data, status_code, headers = api_instance.patch_payment_commission_async_with_http_info(tenant_id, payment_commission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->patch_payment_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_commission_id** | **String** |  |  |
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


## update_commission_async

> <EmptyEnvelope> update_commission_async(tenant_id, commission_id, commission_update_dto, opts)

Update a commission

Updates an existing commission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
commission_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
commission_update_dto = OpenapiClient::CommissionUpdateDto.new # CommissionUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a commission
  result = api_instance.update_commission_async(tenant_id, commission_id, commission_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->update_commission_async: #{e}"
end
```

#### Using the update_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_commission_async_with_http_info(tenant_id, commission_id, commission_update_dto, opts)

```ruby
begin
  # Update a commission
  data, status_code, headers = api_instance.update_commission_async_with_http_info(tenant_id, commission_id, commission_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->update_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **commission_id** | **String** |  |  |
| **commission_update_dto** | [**CommissionUpdateDto**](CommissionUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_payment_commission_async

> <EmptyEnvelope> update_payment_commission_async(tenant_id, payment_commission_id, payment_commission_update_dto, opts)

Update a payment commission

Updates an existing payment commission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CommissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_commission_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
payment_commission_update_dto = OpenapiClient::PaymentCommissionUpdateDto.new # PaymentCommissionUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a payment commission
  result = api_instance.update_payment_commission_async(tenant_id, payment_commission_id, payment_commission_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->update_payment_commission_async: #{e}"
end
```

#### Using the update_payment_commission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_payment_commission_async_with_http_info(tenant_id, payment_commission_id, payment_commission_update_dto, opts)

```ruby
begin
  # Update a payment commission
  data, status_code, headers = api_instance.update_payment_commission_async_with_http_info(tenant_id, payment_commission_id, payment_commission_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CommissionsApi->update_payment_commission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **payment_commission_id** | **String** |  |  |
| **payment_commission_update_dto** | [**PaymentCommissionUpdateDto**](PaymentCommissionUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

