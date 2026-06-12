# OpenapiClient::SharesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_share_class**](SharesApi.md#create_share_class) | **POST** /api/v2/AccountingService/Shares/Classes | Creates a new share class |
| [**create_share_issuance**](SharesApi.md#create_share_issuance) | **POST** /api/v2/AccountingService/Shares/Issuances | Creates a new share issuance |
| [**create_share_transfer**](SharesApi.md#create_share_transfer) | **POST** /api/v2/AccountingService/Shares/Transfers | Creates a new share transfer |
| [**create_share_transfer_reason**](SharesApi.md#create_share_transfer_reason) | **POST** /api/v2/AccountingService/Shares/TransferReasons | Creates a new share transfer reason |
| [**delete_share_class**](SharesApi.md#delete_share_class) | **DELETE** /api/v2/AccountingService/Shares/Classes/{shareClassId} | Deletes an existing share class |
| [**delete_share_issuance**](SharesApi.md#delete_share_issuance) | **DELETE** /api/v2/AccountingService/Shares/Issuances/{issuanceId} | Deletes an existing share issuance |
| [**delete_share_transfer**](SharesApi.md#delete_share_transfer) | **DELETE** /api/v2/AccountingService/Shares/Transfers/{transferId} | Deletes an existing share transfer |
| [**delete_share_transfer_reason**](SharesApi.md#delete_share_transfer_reason) | **DELETE** /api/v2/AccountingService/Shares/TransferReasons/{reasonId} | Deletes an existing share transfer reason |
| [**get_share_class**](SharesApi.md#get_share_class) | **GET** /api/v2/AccountingService/Shares/Classes/{shareClassId} | Gets a share class by id |
| [**get_share_classes**](SharesApi.md#get_share_classes) | **GET** /api/v2/AccountingService/Shares/Classes | Gets the current tenant share classes |
| [**get_share_classes_count**](SharesApi.md#get_share_classes_count) | **GET** /api/v2/AccountingService/Shares/Classes/Count | Gets the current tenant share classes count |
| [**get_share_issuance**](SharesApi.md#get_share_issuance) | **GET** /api/v2/AccountingService/Shares/Issuances/{issuanceId} | Gets a share issuance by id |
| [**get_share_issuances**](SharesApi.md#get_share_issuances) | **GET** /api/v2/AccountingService/Shares/Issuances | Gets the current tenant share issuances |
| [**get_share_issuances_count**](SharesApi.md#get_share_issuances_count) | **GET** /api/v2/AccountingService/Shares/Issuances/Count | Gets the current tenant share issuances count |
| [**get_share_transfer**](SharesApi.md#get_share_transfer) | **GET** /api/v2/AccountingService/Shares/Transfers/{transferId} | Gets a share transfer by id |
| [**get_share_transfer_reason**](SharesApi.md#get_share_transfer_reason) | **GET** /api/v2/AccountingService/Shares/TransferReasons/{reasonId} | Gets a share transfer reason by id |
| [**get_share_transfer_reasons**](SharesApi.md#get_share_transfer_reasons) | **GET** /api/v2/AccountingService/Shares/TransferReasons | Gets the current tenant share transfer reasons |
| [**get_share_transfer_reasons_count**](SharesApi.md#get_share_transfer_reasons_count) | **GET** /api/v2/AccountingService/Shares/TransferReasons/Count | Gets the current tenant share transfer reasons count |
| [**get_share_transfers**](SharesApi.md#get_share_transfers) | **GET** /api/v2/AccountingService/Shares/Transfers | Gets the current tenant share transfers |
| [**get_share_transfers_count**](SharesApi.md#get_share_transfers_count) | **GET** /api/v2/AccountingService/Shares/Transfers/Count | Gets the current tenant share transfers count |
| [**patch_share_class**](SharesApi.md#patch_share_class) | **PATCH** /api/v2/AccountingService/Shares/Classes/{shareClassId} | Patches a share class |
| [**patch_share_issuance**](SharesApi.md#patch_share_issuance) | **PATCH** /api/v2/AccountingService/Shares/Issuances/{issuanceId} | Patches a share issuance |
| [**patch_share_transfer**](SharesApi.md#patch_share_transfer) | **PATCH** /api/v2/AccountingService/Shares/Transfers/{transferId} | Patches a share transfer |
| [**patch_share_transfer_reason**](SharesApi.md#patch_share_transfer_reason) | **PATCH** /api/v2/AccountingService/Shares/TransferReasons/{reasonId} | Patches a share transfer reason |
| [**update_share_class**](SharesApi.md#update_share_class) | **PUT** /api/v2/AccountingService/Shares/Classes/{shareClassId} | Updates an existing share class |
| [**update_share_issuance**](SharesApi.md#update_share_issuance) | **PUT** /api/v2/AccountingService/Shares/Issuances/{issuanceId} | Updates an existing share issuance |
| [**update_share_transfer**](SharesApi.md#update_share_transfer) | **PUT** /api/v2/AccountingService/Shares/Transfers/{transferId} | Updates an existing share transfer |
| [**update_share_transfer_reason**](SharesApi.md#update_share_transfer_reason) | **PUT** /api/v2/AccountingService/Shares/TransferReasons/{reasonId} | Updates an existing share transfer reason |


## create_share_class

> <ShareClassDtoEnvelope> create_share_class(tenant_id, opts)

Creates a new share class

Creates a new share class.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  share_class_create_dto: OpenapiClient::ShareClassCreateDto.new # ShareClassCreateDto | 
}

begin
  # Creates a new share class
  result = api_instance.create_share_class(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->create_share_class: #{e}"
end
```

#### Using the create_share_class_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareClassDtoEnvelope>, Integer, Hash)> create_share_class_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new share class
  data, status_code, headers = api_instance.create_share_class_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareClassDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->create_share_class_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **share_class_create_dto** | [**ShareClassCreateDto**](ShareClassCreateDto.md) |  | [optional] |

### Return type

[**ShareClassDtoEnvelope**](ShareClassDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_share_issuance

> <ShareIssuanceDtoEnvelope> create_share_issuance(tenant_id, opts)

Creates a new share issuance

Creates a new share issuance.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  share_issuance_create_dto: OpenapiClient::ShareIssuanceCreateDto.new # ShareIssuanceCreateDto | 
}

begin
  # Creates a new share issuance
  result = api_instance.create_share_issuance(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->create_share_issuance: #{e}"
end
```

#### Using the create_share_issuance_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareIssuanceDtoEnvelope>, Integer, Hash)> create_share_issuance_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new share issuance
  data, status_code, headers = api_instance.create_share_issuance_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareIssuanceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->create_share_issuance_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **share_issuance_create_dto** | [**ShareIssuanceCreateDto**](ShareIssuanceCreateDto.md) |  | [optional] |

### Return type

[**ShareIssuanceDtoEnvelope**](ShareIssuanceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_share_transfer

> <ShareTransferDtoEnvelope> create_share_transfer(tenant_id, opts)

Creates a new share transfer

Creates a new share transfer.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  share_transfer_create_dto: OpenapiClient::ShareTransferCreateDto.new # ShareTransferCreateDto | 
}

begin
  # Creates a new share transfer
  result = api_instance.create_share_transfer(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->create_share_transfer: #{e}"
end
```

#### Using the create_share_transfer_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareTransferDtoEnvelope>, Integer, Hash)> create_share_transfer_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new share transfer
  data, status_code, headers = api_instance.create_share_transfer_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareTransferDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->create_share_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **share_transfer_create_dto** | [**ShareTransferCreateDto**](ShareTransferCreateDto.md) |  | [optional] |

### Return type

[**ShareTransferDtoEnvelope**](ShareTransferDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_share_transfer_reason

> <ShareTransferReasonDtoEnvelope> create_share_transfer_reason(tenant_id, opts)

Creates a new share transfer reason

Creates a new share transfer reason.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  share_transfer_reason_create_dto: OpenapiClient::ShareTransferReasonCreateDto.new # ShareTransferReasonCreateDto | 
}

begin
  # Creates a new share transfer reason
  result = api_instance.create_share_transfer_reason(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->create_share_transfer_reason: #{e}"
end
```

#### Using the create_share_transfer_reason_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareTransferReasonDtoEnvelope>, Integer, Hash)> create_share_transfer_reason_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new share transfer reason
  data, status_code, headers = api_instance.create_share_transfer_reason_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareTransferReasonDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->create_share_transfer_reason_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **share_transfer_reason_create_dto** | [**ShareTransferReasonCreateDto**](ShareTransferReasonCreateDto.md) |  | [optional] |

### Return type

[**ShareTransferReasonDtoEnvelope**](ShareTransferReasonDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_share_class

> delete_share_class(tenant_id, share_class_id, opts)

Deletes an existing share class

Deletes an existing share class.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
share_class_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes an existing share class
  api_instance.delete_share_class(tenant_id, share_class_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->delete_share_class: #{e}"
end
```

#### Using the delete_share_class_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_share_class_with_http_info(tenant_id, share_class_id, opts)

```ruby
begin
  # Deletes an existing share class
  data, status_code, headers = api_instance.delete_share_class_with_http_info(tenant_id, share_class_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->delete_share_class_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **share_class_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_share_issuance

> delete_share_issuance(tenant_id, issuance_id, opts)

Deletes an existing share issuance

Deletes an existing share issuance.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
issuance_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes an existing share issuance
  api_instance.delete_share_issuance(tenant_id, issuance_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->delete_share_issuance: #{e}"
end
```

#### Using the delete_share_issuance_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_share_issuance_with_http_info(tenant_id, issuance_id, opts)

```ruby
begin
  # Deletes an existing share issuance
  data, status_code, headers = api_instance.delete_share_issuance_with_http_info(tenant_id, issuance_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->delete_share_issuance_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **issuance_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_share_transfer

> delete_share_transfer(tenant_id, transfer_id, opts)

Deletes an existing share transfer

Deletes an existing share transfer.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes an existing share transfer
  api_instance.delete_share_transfer(tenant_id, transfer_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->delete_share_transfer: #{e}"
end
```

#### Using the delete_share_transfer_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_share_transfer_with_http_info(tenant_id, transfer_id, opts)

```ruby
begin
  # Deletes an existing share transfer
  data, status_code, headers = api_instance.delete_share_transfer_with_http_info(tenant_id, transfer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->delete_share_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_share_transfer_reason

> delete_share_transfer_reason(tenant_id, reason_id, opts)

Deletes an existing share transfer reason

Deletes an existing share transfer reason.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reason_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes an existing share transfer reason
  api_instance.delete_share_transfer_reason(tenant_id, reason_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->delete_share_transfer_reason: #{e}"
end
```

#### Using the delete_share_transfer_reason_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_share_transfer_reason_with_http_info(tenant_id, reason_id, opts)

```ruby
begin
  # Deletes an existing share transfer reason
  data, status_code, headers = api_instance.delete_share_transfer_reason_with_http_info(tenant_id, reason_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->delete_share_transfer_reason_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **reason_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_share_class

> <ShareClassDtoEnvelope> get_share_class(tenant_id, share_class_id, opts)

Gets a share class by id

Get a specific share class by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
share_class_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a share class by id
  result = api_instance.get_share_class(tenant_id, share_class_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_class: #{e}"
end
```

#### Using the get_share_class_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareClassDtoEnvelope>, Integer, Hash)> get_share_class_with_http_info(tenant_id, share_class_id, opts)

```ruby
begin
  # Gets a share class by id
  data, status_code, headers = api_instance.get_share_class_with_http_info(tenant_id, share_class_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareClassDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_class_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **share_class_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShareClassDtoEnvelope**](ShareClassDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_share_classes

> <ShareClassDtoListEnvelope> get_share_classes(tenant_id, opts)

Gets the current tenant share classes

Get the currently acting tenant share classes.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant share classes
  result = api_instance.get_share_classes(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_classes: #{e}"
end
```

#### Using the get_share_classes_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareClassDtoListEnvelope>, Integer, Hash)> get_share_classes_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant share classes
  data, status_code, headers = api_instance.get_share_classes_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareClassDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_classes_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShareClassDtoListEnvelope**](ShareClassDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_share_classes_count

> <Int32Envelope> get_share_classes_count(tenant_id, opts)

Gets the current tenant share classes count

Get the currently acting tenant share classes count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant share classes count
  result = api_instance.get_share_classes_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_classes_count: #{e}"
end
```

#### Using the get_share_classes_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_share_classes_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant share classes count
  data, status_code, headers = api_instance.get_share_classes_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_classes_count_with_http_info: #{e}"
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


## get_share_issuance

> <ShareIssuanceDtoEnvelope> get_share_issuance(tenant_id, issuance_id, opts)

Gets a share issuance by id

Get a specific share issuance by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
issuance_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a share issuance by id
  result = api_instance.get_share_issuance(tenant_id, issuance_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_issuance: #{e}"
end
```

#### Using the get_share_issuance_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareIssuanceDtoEnvelope>, Integer, Hash)> get_share_issuance_with_http_info(tenant_id, issuance_id, opts)

```ruby
begin
  # Gets a share issuance by id
  data, status_code, headers = api_instance.get_share_issuance_with_http_info(tenant_id, issuance_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareIssuanceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_issuance_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **issuance_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShareIssuanceDtoEnvelope**](ShareIssuanceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_share_issuances

> <ShareIssuanceDtoListEnvelope> get_share_issuances(tenant_id, opts)

Gets the current tenant share issuances

Get the currently acting tenant share issuances.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant share issuances
  result = api_instance.get_share_issuances(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_issuances: #{e}"
end
```

#### Using the get_share_issuances_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareIssuanceDtoListEnvelope>, Integer, Hash)> get_share_issuances_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant share issuances
  data, status_code, headers = api_instance.get_share_issuances_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareIssuanceDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_issuances_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShareIssuanceDtoListEnvelope**](ShareIssuanceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_share_issuances_count

> <Int32Envelope> get_share_issuances_count(tenant_id, opts)

Gets the current tenant share issuances count

Get the currently acting tenant share issuances count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant share issuances count
  result = api_instance.get_share_issuances_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_issuances_count: #{e}"
end
```

#### Using the get_share_issuances_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_share_issuances_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant share issuances count
  data, status_code, headers = api_instance.get_share_issuances_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_issuances_count_with_http_info: #{e}"
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


## get_share_transfer

> <ShareTransferDtoEnvelope> get_share_transfer(tenant_id, transfer_id, opts)

Gets a share transfer by id

Get a specific share transfer by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a share transfer by id
  result = api_instance.get_share_transfer(tenant_id, transfer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfer: #{e}"
end
```

#### Using the get_share_transfer_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareTransferDtoEnvelope>, Integer, Hash)> get_share_transfer_with_http_info(tenant_id, transfer_id, opts)

```ruby
begin
  # Gets a share transfer by id
  data, status_code, headers = api_instance.get_share_transfer_with_http_info(tenant_id, transfer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareTransferDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShareTransferDtoEnvelope**](ShareTransferDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_share_transfer_reason

> <ShareTransferReasonDtoEnvelope> get_share_transfer_reason(tenant_id, reason_id, opts)

Gets a share transfer reason by id

Get a specific share transfer reason by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reason_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a share transfer reason by id
  result = api_instance.get_share_transfer_reason(tenant_id, reason_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfer_reason: #{e}"
end
```

#### Using the get_share_transfer_reason_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareTransferReasonDtoEnvelope>, Integer, Hash)> get_share_transfer_reason_with_http_info(tenant_id, reason_id, opts)

```ruby
begin
  # Gets a share transfer reason by id
  data, status_code, headers = api_instance.get_share_transfer_reason_with_http_info(tenant_id, reason_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareTransferReasonDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfer_reason_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **reason_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShareTransferReasonDtoEnvelope**](ShareTransferReasonDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_share_transfer_reasons

> <ShareTransferReasonDtoListEnvelope> get_share_transfer_reasons(tenant_id, opts)

Gets the current tenant share transfer reasons

Get the currently acting tenant share transfer reasons.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant share transfer reasons
  result = api_instance.get_share_transfer_reasons(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfer_reasons: #{e}"
end
```

#### Using the get_share_transfer_reasons_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareTransferReasonDtoListEnvelope>, Integer, Hash)> get_share_transfer_reasons_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant share transfer reasons
  data, status_code, headers = api_instance.get_share_transfer_reasons_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareTransferReasonDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfer_reasons_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShareTransferReasonDtoListEnvelope**](ShareTransferReasonDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_share_transfer_reasons_count

> <Int32Envelope> get_share_transfer_reasons_count(tenant_id, opts)

Gets the current tenant share transfer reasons count

Get the currently acting tenant share transfer reasons count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant share transfer reasons count
  result = api_instance.get_share_transfer_reasons_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfer_reasons_count: #{e}"
end
```

#### Using the get_share_transfer_reasons_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_share_transfer_reasons_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant share transfer reasons count
  data, status_code, headers = api_instance.get_share_transfer_reasons_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfer_reasons_count_with_http_info: #{e}"
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


## get_share_transfers

> <ShareTransferDtoListEnvelope> get_share_transfers(tenant_id, opts)

Gets the current tenant share transfers

Get the currently acting tenant share transfers.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant share transfers
  result = api_instance.get_share_transfers(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfers: #{e}"
end
```

#### Using the get_share_transfers_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareTransferDtoListEnvelope>, Integer, Hash)> get_share_transfers_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant share transfers
  data, status_code, headers = api_instance.get_share_transfers_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareTransferDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfers_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ShareTransferDtoListEnvelope**](ShareTransferDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_share_transfers_count

> <Int32Envelope> get_share_transfers_count(tenant_id, opts)

Gets the current tenant share transfers count

Get the currently acting tenant share transfers count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the current tenant share transfers count
  result = api_instance.get_share_transfers_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfers_count: #{e}"
end
```

#### Using the get_share_transfers_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_share_transfers_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the current tenant share transfers count
  data, status_code, headers = api_instance.get_share_transfers_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->get_share_transfers_count_with_http_info: #{e}"
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


## patch_share_class

> <EmptyEnvelope> patch_share_class(tenant_id, share_class_id, opts)

Patches a share class

Partially updates a share class using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
share_class_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a share class
  result = api_instance.patch_share_class(tenant_id, share_class_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->patch_share_class: #{e}"
end
```

#### Using the patch_share_class_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_share_class_with_http_info(tenant_id, share_class_id, opts)

```ruby
begin
  # Patches a share class
  data, status_code, headers = api_instance.patch_share_class_with_http_info(tenant_id, share_class_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->patch_share_class_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **share_class_id** | **String** |  |  |
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


## patch_share_issuance

> <EmptyEnvelope> patch_share_issuance(tenant_id, issuance_id, opts)

Patches a share issuance

Partially updates a share issuance using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
issuance_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a share issuance
  result = api_instance.patch_share_issuance(tenant_id, issuance_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->patch_share_issuance: #{e}"
end
```

#### Using the patch_share_issuance_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_share_issuance_with_http_info(tenant_id, issuance_id, opts)

```ruby
begin
  # Patches a share issuance
  data, status_code, headers = api_instance.patch_share_issuance_with_http_info(tenant_id, issuance_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->patch_share_issuance_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **issuance_id** | **String** |  |  |
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


## patch_share_transfer

> <EmptyEnvelope> patch_share_transfer(tenant_id, transfer_id, opts)

Patches a share transfer

Partially updates a share transfer using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a share transfer
  result = api_instance.patch_share_transfer(tenant_id, transfer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->patch_share_transfer: #{e}"
end
```

#### Using the patch_share_transfer_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_share_transfer_with_http_info(tenant_id, transfer_id, opts)

```ruby
begin
  # Patches a share transfer
  data, status_code, headers = api_instance.patch_share_transfer_with_http_info(tenant_id, transfer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->patch_share_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |
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


## patch_share_transfer_reason

> <EmptyEnvelope> patch_share_transfer_reason(tenant_id, reason_id, opts)

Patches a share transfer reason

Partially updates a share transfer reason using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reason_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a share transfer reason
  result = api_instance.patch_share_transfer_reason(tenant_id, reason_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->patch_share_transfer_reason: #{e}"
end
```

#### Using the patch_share_transfer_reason_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_share_transfer_reason_with_http_info(tenant_id, reason_id, opts)

```ruby
begin
  # Patches a share transfer reason
  data, status_code, headers = api_instance.patch_share_transfer_reason_with_http_info(tenant_id, reason_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->patch_share_transfer_reason_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **reason_id** | **String** |  |  |
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


## update_share_class

> <ShareClassDtoEnvelope> update_share_class(tenant_id, share_class_id, opts)

Updates an existing share class

Updates an existing share class.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
share_class_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  share_class_update_dto: OpenapiClient::ShareClassUpdateDto.new # ShareClassUpdateDto | 
}

begin
  # Updates an existing share class
  result = api_instance.update_share_class(tenant_id, share_class_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->update_share_class: #{e}"
end
```

#### Using the update_share_class_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareClassDtoEnvelope>, Integer, Hash)> update_share_class_with_http_info(tenant_id, share_class_id, opts)

```ruby
begin
  # Updates an existing share class
  data, status_code, headers = api_instance.update_share_class_with_http_info(tenant_id, share_class_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareClassDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->update_share_class_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **share_class_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **share_class_update_dto** | [**ShareClassUpdateDto**](ShareClassUpdateDto.md) |  | [optional] |

### Return type

[**ShareClassDtoEnvelope**](ShareClassDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_share_issuance

> <ShareIssuanceDtoEnvelope> update_share_issuance(tenant_id, issuance_id, opts)

Updates an existing share issuance

Updates an existing share issuance.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
issuance_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  share_issuance_update_dto: OpenapiClient::ShareIssuanceUpdateDto.new # ShareIssuanceUpdateDto | 
}

begin
  # Updates an existing share issuance
  result = api_instance.update_share_issuance(tenant_id, issuance_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->update_share_issuance: #{e}"
end
```

#### Using the update_share_issuance_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareIssuanceDtoEnvelope>, Integer, Hash)> update_share_issuance_with_http_info(tenant_id, issuance_id, opts)

```ruby
begin
  # Updates an existing share issuance
  data, status_code, headers = api_instance.update_share_issuance_with_http_info(tenant_id, issuance_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareIssuanceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->update_share_issuance_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **issuance_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **share_issuance_update_dto** | [**ShareIssuanceUpdateDto**](ShareIssuanceUpdateDto.md) |  | [optional] |

### Return type

[**ShareIssuanceDtoEnvelope**](ShareIssuanceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_share_transfer

> <ShareTransferDtoEnvelope> update_share_transfer(tenant_id, transfer_id, opts)

Updates an existing share transfer

Updates an existing share transfer.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  share_transfer_update_dto: OpenapiClient::ShareTransferUpdateDto.new # ShareTransferUpdateDto | 
}

begin
  # Updates an existing share transfer
  result = api_instance.update_share_transfer(tenant_id, transfer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->update_share_transfer: #{e}"
end
```

#### Using the update_share_transfer_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareTransferDtoEnvelope>, Integer, Hash)> update_share_transfer_with_http_info(tenant_id, transfer_id, opts)

```ruby
begin
  # Updates an existing share transfer
  data, status_code, headers = api_instance.update_share_transfer_with_http_info(tenant_id, transfer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareTransferDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->update_share_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **share_transfer_update_dto** | [**ShareTransferUpdateDto**](ShareTransferUpdateDto.md) |  | [optional] |

### Return type

[**ShareTransferDtoEnvelope**](ShareTransferDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_share_transfer_reason

> <ShareTransferReasonDtoEnvelope> update_share_transfer_reason(tenant_id, reason_id, opts)

Updates an existing share transfer reason

Updates an existing share transfer reason.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SharesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
reason_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  share_transfer_reason_update_dto: OpenapiClient::ShareTransferReasonUpdateDto.new # ShareTransferReasonUpdateDto | 
}

begin
  # Updates an existing share transfer reason
  result = api_instance.update_share_transfer_reason(tenant_id, reason_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->update_share_transfer_reason: #{e}"
end
```

#### Using the update_share_transfer_reason_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ShareTransferReasonDtoEnvelope>, Integer, Hash)> update_share_transfer_reason_with_http_info(tenant_id, reason_id, opts)

```ruby
begin
  # Updates an existing share transfer reason
  data, status_code, headers = api_instance.update_share_transfer_reason_with_http_info(tenant_id, reason_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ShareTransferReasonDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SharesApi->update_share_transfer_reason_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **reason_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **share_transfer_reason_update_dto** | [**ShareTransferReasonUpdateDto**](ShareTransferReasonUpdateDto.md) |  | [optional] |

### Return type

[**ShareTransferReasonDtoEnvelope**](ShareTransferReasonDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

