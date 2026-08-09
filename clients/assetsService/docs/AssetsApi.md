# OpenapiClient::AssetsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_asset**](AssetsApi.md#create_asset) | **POST** /api/v2/AssetsService/Assets | Creates a new asset |
| [**create_asset_asset_category**](AssetsApi.md#create_asset_asset_category) | **POST** /api/v2/AssetsService/Assets/Categories | Creates a new asset category |
| [**create_asset_depreciation_record**](AssetsApi.md#create_asset_depreciation_record) | **POST** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords | Creates a new depreciation record for an asset |
| [**create_asset_repair**](AssetsApi.md#create_asset_repair) | **POST** /api/v2/AssetsService/Assets/{assetId}/Repairs | Creates a new repair for an asset |
| [**create_asset_transfer**](AssetsApi.md#create_asset_transfer) | **POST** /api/v2/AssetsService/Assets/{assetId}/Transfers | Creates a new transfer for an asset |
| [**create_asset_value_amend**](AssetsApi.md#create_asset_value_amend) | **POST** /api/v2/AssetsService/Assets/{assetId}/ValueAmends | Creates a new value amendment for an asset |
| [**delete_asset**](AssetsApi.md#delete_asset) | **DELETE** /api/v2/AssetsService/Assets/{assetId} | Deletes an existing asset |
| [**delete_asset_asset_category**](AssetsApi.md#delete_asset_asset_category) | **DELETE** /api/v2/AssetsService/Assets/Categories/{categoryId} | Deletes an existing asset category |
| [**delete_asset_depreciation_record**](AssetsApi.md#delete_asset_depreciation_record) | **DELETE** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords/{recordId} | Deletes a depreciation record for an asset |
| [**delete_asset_repair**](AssetsApi.md#delete_asset_repair) | **DELETE** /api/v2/AssetsService/Assets/{assetId}/Repairs/{repairId} | Deletes a repair for an asset |
| [**delete_asset_transfer**](AssetsApi.md#delete_asset_transfer) | **DELETE** /api/v2/AssetsService/Assets/{assetId}/Transfers/{transferId} | Deletes a transfer for an asset |
| [**delete_asset_value_amend**](AssetsApi.md#delete_asset_value_amend) | **DELETE** /api/v2/AssetsService/Assets/{assetId}/ValueAmends/{amendId} | Deletes a value amendment for an asset |
| [**get_asset**](AssetsApi.md#get_asset) | **GET** /api/v2/AssetsService/Assets/{assetId} | Gets a specific asset by ID |
| [**get_asset_asset_categories**](AssetsApi.md#get_asset_asset_categories) | **GET** /api/v2/AssetsService/Assets/Categories | Gets all asset categories |
| [**get_asset_asset_categories_count**](AssetsApi.md#get_asset_asset_categories_count) | **GET** /api/v2/AssetsService/Assets/Categories/count | Gets the count of asset categories |
| [**get_asset_asset_category**](AssetsApi.md#get_asset_asset_category) | **GET** /api/v2/AssetsService/Assets/Categories/{categoryId} | Gets a specific asset category |
| [**get_asset_depreciation_record**](AssetsApi.md#get_asset_depreciation_record) | **GET** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords/{recordId} | Gets a specific depreciation record for an asset |
| [**get_asset_depreciation_records**](AssetsApi.md#get_asset_depreciation_records) | **GET** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords | Gets depreciation records for a specific asset |
| [**get_asset_depreciation_records_count**](AssetsApi.md#get_asset_depreciation_records_count) | **GET** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords/Count | Gets count of depreciation records for a specific asset |
| [**get_asset_repair**](AssetsApi.md#get_asset_repair) | **GET** /api/v2/AssetsService/Assets/{assetId}/Repairs/{repairId} | Gets a specific repair for an asset |
| [**get_asset_repairs**](AssetsApi.md#get_asset_repairs) | **GET** /api/v2/AssetsService/Assets/{assetId}/Repairs | Gets repairs for a specific asset |
| [**get_asset_repairs_count**](AssetsApi.md#get_asset_repairs_count) | **GET** /api/v2/AssetsService/Assets/{assetId}/Repairs/Count | Gets count of repairs for a specific asset |
| [**get_asset_transfer**](AssetsApi.md#get_asset_transfer) | **GET** /api/v2/AssetsService/Assets/{assetId}/Transfers/{transferId} | Gets a specific transfer for an asset |
| [**get_asset_transfers**](AssetsApi.md#get_asset_transfers) | **GET** /api/v2/AssetsService/Assets/{assetId}/Transfers | Gets transfers for a specific asset |
| [**get_asset_transfers_count**](AssetsApi.md#get_asset_transfers_count) | **GET** /api/v2/AssetsService/Assets/{assetId}/Transfers/Count | Gets count of transfers for a specific asset |
| [**get_asset_value_amend**](AssetsApi.md#get_asset_value_amend) | **GET** /api/v2/AssetsService/Assets/{assetId}/ValueAmends/{amendId} | Gets a specific value amendment for an asset |
| [**get_asset_value_amends**](AssetsApi.md#get_asset_value_amends) | **GET** /api/v2/AssetsService/Assets/{assetId}/ValueAmends | Gets value amendments for a specific asset |
| [**get_asset_value_amends_count**](AssetsApi.md#get_asset_value_amends_count) | **GET** /api/v2/AssetsService/Assets/{assetId}/ValueAmends/Count | Gets count of value amendments for a specific asset |
| [**get_assets**](AssetsApi.md#get_assets) | **GET** /api/v2/AssetsService/Assets | Gets all assets for the current tenant |
| [**get_assets_count**](AssetsApi.md#get_assets_count) | **GET** /api/v2/AssetsService/Assets/count | Gets the count of assets |
| [**patch_asset**](AssetsApi.md#patch_asset) | **PATCH** /api/v2/AssetsService/Assets/{assetId} | Partially updates an existing asset |
| [**patch_asset_asset_category**](AssetsApi.md#patch_asset_asset_category) | **PATCH** /api/v2/AssetsService/Assets/Categories/{categoryId} | Partially updates an existing asset category |
| [**patch_asset_depreciation_record**](AssetsApi.md#patch_asset_depreciation_record) | **PATCH** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords/{recordId} | Partially updates a depreciation record for an asset |
| [**patch_asset_repair**](AssetsApi.md#patch_asset_repair) | **PATCH** /api/v2/AssetsService/Assets/{assetId}/Repairs/{repairId} | Partially updates a repair for an asset |
| [**patch_asset_transfer**](AssetsApi.md#patch_asset_transfer) | **PATCH** /api/v2/AssetsService/Assets/{assetId}/Transfers/{transferId} | Partially updates a transfer for an asset |
| [**patch_asset_value_amend**](AssetsApi.md#patch_asset_value_amend) | **PATCH** /api/v2/AssetsService/Assets/{assetId}/ValueAmends/{amendId} | Partially updates a value amendment for an asset |
| [**update_asset**](AssetsApi.md#update_asset) | **PUT** /api/v2/AssetsService/Assets/{assetId} | Updates an existing asset |
| [**update_asset_asset_category**](AssetsApi.md#update_asset_asset_category) | **PUT** /api/v2/AssetsService/Assets/Categories/{categoryId} | Updates an existing asset category |
| [**update_asset_depreciation_record**](AssetsApi.md#update_asset_depreciation_record) | **PUT** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords/{recordId} | Updates a depreciation record for an asset |
| [**update_asset_repair**](AssetsApi.md#update_asset_repair) | **PUT** /api/v2/AssetsService/Assets/{assetId}/Repairs/{repairId} | Updates a repair for an asset |
| [**update_asset_transfer**](AssetsApi.md#update_asset_transfer) | **PUT** /api/v2/AssetsService/Assets/{assetId}/Transfers/{transferId} | Updates a transfer for an asset |
| [**update_asset_value_amend**](AssetsApi.md#update_asset_value_amend) | **PUT** /api/v2/AssetsService/Assets/{assetId}/ValueAmends/{amendId} | Updates a value amendment for an asset |


## create_asset

> <AssetDtoEnvelope> create_asset(tenant_id, opts)

Creates a new asset

Creates a new asset for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_create_dto: OpenapiClient::AssetCreateDto.new # AssetCreateDto | 
}

begin
  # Creates a new asset
  result = api_instance.create_asset(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset: #{e}"
end
```

#### Using the create_asset_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetDtoEnvelope>, Integer, Hash)> create_asset_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new asset
  data, status_code, headers = api_instance.create_asset_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_create_dto** | [**AssetCreateDto**](AssetCreateDto.md) |  | [optional] |

### Return type

[**AssetDtoEnvelope**](AssetDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_asset_asset_category

> <AssetCategoryDtoEnvelope> create_asset_asset_category(tenant_id, opts)

Creates a new asset category

Creates a new asset category for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_category_create_dto: OpenapiClient::AssetCategoryCreateDto.new # AssetCategoryCreateDto | 
}

begin
  # Creates a new asset category
  result = api_instance.create_asset_asset_category(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_asset_category: #{e}"
end
```

#### Using the create_asset_asset_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetCategoryDtoEnvelope>, Integer, Hash)> create_asset_asset_category_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new asset category
  data, status_code, headers = api_instance.create_asset_asset_category_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_category_create_dto** | [**AssetCategoryCreateDto**](AssetCategoryCreateDto.md) |  | [optional] |

### Return type

[**AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_asset_depreciation_record

> <EmptyEnvelope> create_asset_depreciation_record(tenant_id, asset_id, opts)

Creates a new depreciation record for an asset

Creates a new depreciation record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_depreciation_record_create_dto: OpenapiClient::AssetDepreciationRecordCreateDto.new # AssetDepreciationRecordCreateDto | 
}

begin
  # Creates a new depreciation record for an asset
  result = api_instance.create_asset_depreciation_record(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_depreciation_record: #{e}"
end
```

#### Using the create_asset_depreciation_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_asset_depreciation_record_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Creates a new depreciation record for an asset
  data, status_code, headers = api_instance.create_asset_depreciation_record_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_depreciation_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_depreciation_record_create_dto** | [**AssetDepreciationRecordCreateDto**](AssetDepreciationRecordCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_asset_repair

> <EmptyEnvelope> create_asset_repair(tenant_id, asset_id, opts)

Creates a new repair for an asset

Creates a new repair record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_repair_create_dto: OpenapiClient::AssetRepairCreateDto.new # AssetRepairCreateDto | 
}

begin
  # Creates a new repair for an asset
  result = api_instance.create_asset_repair(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_repair: #{e}"
end
```

#### Using the create_asset_repair_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_asset_repair_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Creates a new repair for an asset
  data, status_code, headers = api_instance.create_asset_repair_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_repair_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_repair_create_dto** | [**AssetRepairCreateDto**](AssetRepairCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_asset_transfer

> <EmptyEnvelope> create_asset_transfer(tenant_id, asset_id, opts)

Creates a new transfer for an asset

Creates a new transfer record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_transfer_create_dto: OpenapiClient::AssetTransferCreateDto.new # AssetTransferCreateDto | 
}

begin
  # Creates a new transfer for an asset
  result = api_instance.create_asset_transfer(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_transfer: #{e}"
end
```

#### Using the create_asset_transfer_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_asset_transfer_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Creates a new transfer for an asset
  data, status_code, headers = api_instance.create_asset_transfer_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_transfer_create_dto** | [**AssetTransferCreateDto**](AssetTransferCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_asset_value_amend

> <EmptyEnvelope> create_asset_value_amend(tenant_id, asset_id, opts)

Creates a new value amendment for an asset

Creates a new value amendment record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_value_amend_create_dto: OpenapiClient::AssetValueAmendCreateDto.new # AssetValueAmendCreateDto | 
}

begin
  # Creates a new value amendment for an asset
  result = api_instance.create_asset_value_amend(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_value_amend: #{e}"
end
```

#### Using the create_asset_value_amend_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_asset_value_amend_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Creates a new value amendment for an asset
  data, status_code, headers = api_instance.create_asset_value_amend_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->create_asset_value_amend_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_value_amend_create_dto** | [**AssetValueAmendCreateDto**](AssetValueAmendCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_asset

> delete_asset(tenant_id, asset_id)

Deletes an existing asset

Deletes an existing asset for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes an existing asset
  api_instance.delete_asset(tenant_id, asset_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset: #{e}"
end
```

#### Using the delete_asset_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_asset_with_http_info(tenant_id, asset_id)

```ruby
begin
  # Deletes an existing asset
  data, status_code, headers = api_instance.delete_asset_with_http_info(tenant_id, asset_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_asset_asset_category

> delete_asset_asset_category(tenant_id, category_id)

Deletes an existing asset category

Deletes an existing asset category for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes an existing asset category
  api_instance.delete_asset_asset_category(tenant_id, category_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_asset_category: #{e}"
end
```

#### Using the delete_asset_asset_category_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_asset_asset_category_with_http_info(tenant_id, category_id)

```ruby
begin
  # Deletes an existing asset category
  data, status_code, headers = api_instance.delete_asset_asset_category_with_http_info(tenant_id, category_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_asset_depreciation_record

> <EmptyEnvelope> delete_asset_depreciation_record(tenant_id, asset_id, record_id)

Deletes a depreciation record for an asset

Deletes a depreciation record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a depreciation record for an asset
  result = api_instance.delete_asset_depreciation_record(tenant_id, asset_id, record_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_depreciation_record: #{e}"
end
```

#### Using the delete_asset_depreciation_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_asset_depreciation_record_with_http_info(tenant_id, asset_id, record_id)

```ruby
begin
  # Deletes a depreciation record for an asset
  data, status_code, headers = api_instance.delete_asset_depreciation_record_with_http_info(tenant_id, asset_id, record_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_depreciation_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **record_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_asset_repair

> <EmptyEnvelope> delete_asset_repair(tenant_id, asset_id, repair_id)

Deletes a repair for an asset

Deletes a repair record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
repair_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a repair for an asset
  result = api_instance.delete_asset_repair(tenant_id, asset_id, repair_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_repair: #{e}"
end
```

#### Using the delete_asset_repair_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_asset_repair_with_http_info(tenant_id, asset_id, repair_id)

```ruby
begin
  # Deletes a repair for an asset
  data, status_code, headers = api_instance.delete_asset_repair_with_http_info(tenant_id, asset_id, repair_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_repair_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **repair_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_asset_transfer

> <EmptyEnvelope> delete_asset_transfer(tenant_id, asset_id, transfer_id)

Deletes a transfer for an asset

Deletes a transfer record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a transfer for an asset
  result = api_instance.delete_asset_transfer(tenant_id, asset_id, transfer_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_transfer: #{e}"
end
```

#### Using the delete_asset_transfer_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_asset_transfer_with_http_info(tenant_id, asset_id, transfer_id)

```ruby
begin
  # Deletes a transfer for an asset
  data, status_code, headers = api_instance.delete_asset_transfer_with_http_info(tenant_id, asset_id, transfer_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_asset_value_amend

> <EmptyEnvelope> delete_asset_value_amend(tenant_id, asset_id, amend_id)

Deletes a value amendment for an asset

Deletes a value amendment record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
amend_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a value amendment for an asset
  result = api_instance.delete_asset_value_amend(tenant_id, asset_id, amend_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_value_amend: #{e}"
end
```

#### Using the delete_asset_value_amend_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_asset_value_amend_with_http_info(tenant_id, asset_id, amend_id)

```ruby
begin
  # Deletes a value amendment for an asset
  data, status_code, headers = api_instance.delete_asset_value_amend_with_http_info(tenant_id, asset_id, amend_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->delete_asset_value_amend_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **amend_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset

> <AssetDtoEnvelope> get_asset(tenant_id, asset_id)

Gets a specific asset by ID

Retrieves a specific asset for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific asset by ID
  result = api_instance.get_asset(tenant_id, asset_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset: #{e}"
end
```

#### Using the get_asset_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetDtoEnvelope>, Integer, Hash)> get_asset_with_http_info(tenant_id, asset_id)

```ruby
begin
  # Gets a specific asset by ID
  data, status_code, headers = api_instance.get_asset_with_http_info(tenant_id, asset_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |

### Return type

[**AssetDtoEnvelope**](AssetDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_asset_categories

> <AssetCategoryDtoListEnvelope> get_asset_asset_categories(tenant_id, opts)

Gets all asset categories

Retrieves all asset categories for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_category_dto_collection_query_parameters: OpenapiClient::AssetCategoryDtoCollectionQueryParameters.new # AssetCategoryDtoCollectionQueryParameters | 
}

begin
  # Gets all asset categories
  result = api_instance.get_asset_asset_categories(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_asset_categories: #{e}"
end
```

#### Using the get_asset_asset_categories_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetCategoryDtoListEnvelope>, Integer, Hash)> get_asset_asset_categories_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets all asset categories
  data, status_code, headers = api_instance.get_asset_asset_categories_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_asset_categories_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_category_dto_collection_query_parameters** | [**AssetCategoryDtoCollectionQueryParameters**](AssetCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AssetCategoryDtoListEnvelope**](AssetCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_asset_categories_count

> <Int32Envelope> get_asset_asset_categories_count(tenant_id, opts)

Gets the count of asset categories

Returns the total number of asset categories for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_category_dto_collection_query_parameters: OpenapiClient::AssetCategoryDtoCollectionQueryParameters.new # AssetCategoryDtoCollectionQueryParameters | 
}

begin
  # Gets the count of asset categories
  result = api_instance.get_asset_asset_categories_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_asset_categories_count: #{e}"
end
```

#### Using the get_asset_asset_categories_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_asset_asset_categories_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the count of asset categories
  data, status_code, headers = api_instance.get_asset_asset_categories_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_asset_categories_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_category_dto_collection_query_parameters** | [**AssetCategoryDtoCollectionQueryParameters**](AssetCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_asset_category

> <AssetCategoryDtoEnvelope> get_asset_asset_category(tenant_id, category_id)

Gets a specific asset category

Retrieves a specific asset category for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific asset category
  result = api_instance.get_asset_asset_category(tenant_id, category_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_asset_category: #{e}"
end
```

#### Using the get_asset_asset_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetCategoryDtoEnvelope>, Integer, Hash)> get_asset_asset_category_with_http_info(tenant_id, category_id)

```ruby
begin
  # Gets a specific asset category
  data, status_code, headers = api_instance.get_asset_asset_category_with_http_info(tenant_id, category_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |

### Return type

[**AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_depreciation_record

> <AssetDepreciationRecordDtoEnvelope> get_asset_depreciation_record(tenant_id, asset_id, record_id)

Gets a specific depreciation record for an asset

Retrieves a specific depreciation record by ID for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific depreciation record for an asset
  result = api_instance.get_asset_depreciation_record(tenant_id, asset_id, record_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_depreciation_record: #{e}"
end
```

#### Using the get_asset_depreciation_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetDepreciationRecordDtoEnvelope>, Integer, Hash)> get_asset_depreciation_record_with_http_info(tenant_id, asset_id, record_id)

```ruby
begin
  # Gets a specific depreciation record for an asset
  data, status_code, headers = api_instance.get_asset_depreciation_record_with_http_info(tenant_id, asset_id, record_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetDepreciationRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_depreciation_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **record_id** | **String** |  |  |

### Return type

[**AssetDepreciationRecordDtoEnvelope**](AssetDepreciationRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_depreciation_records

> <AssetDepreciationRecordDtoListEnvelope> get_asset_depreciation_records(tenant_id, asset_id, opts)

Gets depreciation records for a specific asset

Retrieves all depreciation records for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_depreciation_record_dto_collection_query_parameters: OpenapiClient::AssetDepreciationRecordDtoCollectionQueryParameters.new # AssetDepreciationRecordDtoCollectionQueryParameters | 
}

begin
  # Gets depreciation records for a specific asset
  result = api_instance.get_asset_depreciation_records(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_depreciation_records: #{e}"
end
```

#### Using the get_asset_depreciation_records_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetDepreciationRecordDtoListEnvelope>, Integer, Hash)> get_asset_depreciation_records_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Gets depreciation records for a specific asset
  data, status_code, headers = api_instance.get_asset_depreciation_records_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetDepreciationRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_depreciation_records_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_depreciation_record_dto_collection_query_parameters** | [**AssetDepreciationRecordDtoCollectionQueryParameters**](AssetDepreciationRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AssetDepreciationRecordDtoListEnvelope**](AssetDepreciationRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_depreciation_records_count

> <Int32Envelope> get_asset_depreciation_records_count(tenant_id, asset_id, opts)

Gets count of depreciation records for a specific asset

Returns the total number of depreciation records for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_depreciation_record_dto_collection_query_parameters: OpenapiClient::AssetDepreciationRecordDtoCollectionQueryParameters.new # AssetDepreciationRecordDtoCollectionQueryParameters | 
}

begin
  # Gets count of depreciation records for a specific asset
  result = api_instance.get_asset_depreciation_records_count(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_depreciation_records_count: #{e}"
end
```

#### Using the get_asset_depreciation_records_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_asset_depreciation_records_count_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Gets count of depreciation records for a specific asset
  data, status_code, headers = api_instance.get_asset_depreciation_records_count_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_depreciation_records_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_depreciation_record_dto_collection_query_parameters** | [**AssetDepreciationRecordDtoCollectionQueryParameters**](AssetDepreciationRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_repair

> <AssetRepairDtoEnvelope> get_asset_repair(tenant_id, asset_id, repair_id)

Gets a specific repair for an asset

Retrieves a specific repair record by ID for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
repair_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific repair for an asset
  result = api_instance.get_asset_repair(tenant_id, asset_id, repair_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_repair: #{e}"
end
```

#### Using the get_asset_repair_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetRepairDtoEnvelope>, Integer, Hash)> get_asset_repair_with_http_info(tenant_id, asset_id, repair_id)

```ruby
begin
  # Gets a specific repair for an asset
  data, status_code, headers = api_instance.get_asset_repair_with_http_info(tenant_id, asset_id, repair_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetRepairDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_repair_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **repair_id** | **String** |  |  |

### Return type

[**AssetRepairDtoEnvelope**](AssetRepairDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_repairs

> <AssetRepairDtoListEnvelope> get_asset_repairs(tenant_id, asset_id, opts)

Gets repairs for a specific asset

Retrieves all repair records for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_repair_dto_collection_query_parameters: OpenapiClient::AssetRepairDtoCollectionQueryParameters.new # AssetRepairDtoCollectionQueryParameters | 
}

begin
  # Gets repairs for a specific asset
  result = api_instance.get_asset_repairs(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_repairs: #{e}"
end
```

#### Using the get_asset_repairs_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetRepairDtoListEnvelope>, Integer, Hash)> get_asset_repairs_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Gets repairs for a specific asset
  data, status_code, headers = api_instance.get_asset_repairs_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetRepairDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_repairs_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_repair_dto_collection_query_parameters** | [**AssetRepairDtoCollectionQueryParameters**](AssetRepairDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AssetRepairDtoListEnvelope**](AssetRepairDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_repairs_count

> <Int32Envelope> get_asset_repairs_count(tenant_id, asset_id, opts)

Gets count of repairs for a specific asset

Returns the total number of repair records for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_repair_dto_collection_query_parameters: OpenapiClient::AssetRepairDtoCollectionQueryParameters.new # AssetRepairDtoCollectionQueryParameters | 
}

begin
  # Gets count of repairs for a specific asset
  result = api_instance.get_asset_repairs_count(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_repairs_count: #{e}"
end
```

#### Using the get_asset_repairs_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_asset_repairs_count_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Gets count of repairs for a specific asset
  data, status_code, headers = api_instance.get_asset_repairs_count_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_repairs_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_repair_dto_collection_query_parameters** | [**AssetRepairDtoCollectionQueryParameters**](AssetRepairDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_transfer

> <AssetTransferDtoEnvelope> get_asset_transfer(tenant_id, asset_id, transfer_id)

Gets a specific transfer for an asset

Retrieves a specific transfer record by ID for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific transfer for an asset
  result = api_instance.get_asset_transfer(tenant_id, asset_id, transfer_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_transfer: #{e}"
end
```

#### Using the get_asset_transfer_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetTransferDtoEnvelope>, Integer, Hash)> get_asset_transfer_with_http_info(tenant_id, asset_id, transfer_id)

```ruby
begin
  # Gets a specific transfer for an asset
  data, status_code, headers = api_instance.get_asset_transfer_with_http_info(tenant_id, asset_id, transfer_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetTransferDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |

### Return type

[**AssetTransferDtoEnvelope**](AssetTransferDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_transfers

> <AssetTransferDtoListEnvelope> get_asset_transfers(tenant_id, asset_id, opts)

Gets transfers for a specific asset

Retrieves all transfer records for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_transfer_dto_collection_query_parameters: OpenapiClient::AssetTransferDtoCollectionQueryParameters.new # AssetTransferDtoCollectionQueryParameters | 
}

begin
  # Gets transfers for a specific asset
  result = api_instance.get_asset_transfers(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_transfers: #{e}"
end
```

#### Using the get_asset_transfers_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetTransferDtoListEnvelope>, Integer, Hash)> get_asset_transfers_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Gets transfers for a specific asset
  data, status_code, headers = api_instance.get_asset_transfers_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetTransferDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_transfers_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_transfer_dto_collection_query_parameters** | [**AssetTransferDtoCollectionQueryParameters**](AssetTransferDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AssetTransferDtoListEnvelope**](AssetTransferDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_transfers_count

> <Int32Envelope> get_asset_transfers_count(tenant_id, asset_id, opts)

Gets count of transfers for a specific asset

Returns the total number of transfer records for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_transfer_dto_collection_query_parameters: OpenapiClient::AssetTransferDtoCollectionQueryParameters.new # AssetTransferDtoCollectionQueryParameters | 
}

begin
  # Gets count of transfers for a specific asset
  result = api_instance.get_asset_transfers_count(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_transfers_count: #{e}"
end
```

#### Using the get_asset_transfers_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_asset_transfers_count_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Gets count of transfers for a specific asset
  data, status_code, headers = api_instance.get_asset_transfers_count_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_transfers_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_transfer_dto_collection_query_parameters** | [**AssetTransferDtoCollectionQueryParameters**](AssetTransferDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_value_amend

> <AssetValueAmendDtoEnvelope> get_asset_value_amend(tenant_id, asset_id, amend_id)

Gets a specific value amendment for an asset

Retrieves a specific value amendment record by ID for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
amend_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific value amendment for an asset
  result = api_instance.get_asset_value_amend(tenant_id, asset_id, amend_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_value_amend: #{e}"
end
```

#### Using the get_asset_value_amend_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetValueAmendDtoEnvelope>, Integer, Hash)> get_asset_value_amend_with_http_info(tenant_id, asset_id, amend_id)

```ruby
begin
  # Gets a specific value amendment for an asset
  data, status_code, headers = api_instance.get_asset_value_amend_with_http_info(tenant_id, asset_id, amend_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetValueAmendDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_value_amend_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **amend_id** | **String** |  |  |

### Return type

[**AssetValueAmendDtoEnvelope**](AssetValueAmendDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_value_amends

> <AssetValueAmendDtoListEnvelope> get_asset_value_amends(tenant_id, asset_id, opts)

Gets value amendments for a specific asset

Retrieves all value amendment records for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_value_amend_dto_collection_query_parameters: OpenapiClient::AssetValueAmendDtoCollectionQueryParameters.new # AssetValueAmendDtoCollectionQueryParameters | 
}

begin
  # Gets value amendments for a specific asset
  result = api_instance.get_asset_value_amends(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_value_amends: #{e}"
end
```

#### Using the get_asset_value_amends_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetValueAmendDtoListEnvelope>, Integer, Hash)> get_asset_value_amends_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Gets value amendments for a specific asset
  data, status_code, headers = api_instance.get_asset_value_amends_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetValueAmendDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_value_amends_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_value_amend_dto_collection_query_parameters** | [**AssetValueAmendDtoCollectionQueryParameters**](AssetValueAmendDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AssetValueAmendDtoListEnvelope**](AssetValueAmendDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_value_amends_count

> <Int32Envelope> get_asset_value_amends_count(tenant_id, asset_id, opts)

Gets count of value amendments for a specific asset

Returns the total number of value amendment records for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_value_amend_dto_collection_query_parameters: OpenapiClient::AssetValueAmendDtoCollectionQueryParameters.new # AssetValueAmendDtoCollectionQueryParameters | 
}

begin
  # Gets count of value amendments for a specific asset
  result = api_instance.get_asset_value_amends_count(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_value_amends_count: #{e}"
end
```

#### Using the get_asset_value_amends_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_asset_value_amends_count_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Gets count of value amendments for a specific asset
  data, status_code, headers = api_instance.get_asset_value_amends_count_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_asset_value_amends_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_value_amend_dto_collection_query_parameters** | [**AssetValueAmendDtoCollectionQueryParameters**](AssetValueAmendDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_assets

> <AssetDtoListEnvelope> get_assets(tenant_id, opts)

Gets all assets for the current tenant

Retrieves all assets for the authenticated tenant with optional filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_dto_collection_query_parameters: OpenapiClient::AssetDtoCollectionQueryParameters.new # AssetDtoCollectionQueryParameters | 
}

begin
  # Gets all assets for the current tenant
  result = api_instance.get_assets(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_assets: #{e}"
end
```

#### Using the get_assets_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetDtoListEnvelope>, Integer, Hash)> get_assets_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets all assets for the current tenant
  data, status_code, headers = api_instance.get_assets_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_assets_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_dto_collection_query_parameters** | [**AssetDtoCollectionQueryParameters**](AssetDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AssetDtoListEnvelope**](AssetDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_assets_count

> <Int32Envelope> get_assets_count(tenant_id, opts)

Gets the count of assets

Returns the total number of assets for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_dto_collection_query_parameters: OpenapiClient::AssetDtoCollectionQueryParameters.new # AssetDtoCollectionQueryParameters | 
}

begin
  # Gets the count of assets
  result = api_instance.get_assets_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_assets_count: #{e}"
end
```

#### Using the get_assets_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_assets_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the count of assets
  data, status_code, headers = api_instance.get_assets_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->get_assets_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_dto_collection_query_parameters** | [**AssetDtoCollectionQueryParameters**](AssetDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_asset

> <EmptyEnvelope> patch_asset(tenant_id, asset_id, opts)

Partially updates an existing asset

Applies a JSON Patch document to an existing asset for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates an existing asset
  result = api_instance.patch_asset(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset: #{e}"
end
```

#### Using the patch_asset_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_asset_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Partially updates an existing asset
  data, status_code, headers = api_instance.patch_asset_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_asset_asset_category

> <EmptyEnvelope> patch_asset_asset_category(tenant_id, category_id, opts)

Partially updates an existing asset category

Applies a JSON Patch document to an existing asset category for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates an existing asset category
  result = api_instance.patch_asset_asset_category(tenant_id, category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_asset_category: #{e}"
end
```

#### Using the patch_asset_asset_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_asset_asset_category_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Partially updates an existing asset category
  data, status_code, headers = api_instance.patch_asset_asset_category_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_asset_depreciation_record

> <EmptyEnvelope> patch_asset_depreciation_record(tenant_id, asset_id, record_id, opts)

Partially updates a depreciation record for an asset

Applies a JSON Patch document to an existing depreciation record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates a depreciation record for an asset
  result = api_instance.patch_asset_depreciation_record(tenant_id, asset_id, record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_depreciation_record: #{e}"
end
```

#### Using the patch_asset_depreciation_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_asset_depreciation_record_with_http_info(tenant_id, asset_id, record_id, opts)

```ruby
begin
  # Partially updates a depreciation record for an asset
  data, status_code, headers = api_instance.patch_asset_depreciation_record_with_http_info(tenant_id, asset_id, record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_depreciation_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **record_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_asset_repair

> <EmptyEnvelope> patch_asset_repair(tenant_id, asset_id, repair_id, opts)

Partially updates a repair for an asset

Applies a JSON Patch document to an existing repair record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
repair_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates a repair for an asset
  result = api_instance.patch_asset_repair(tenant_id, asset_id, repair_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_repair: #{e}"
end
```

#### Using the patch_asset_repair_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_asset_repair_with_http_info(tenant_id, asset_id, repair_id, opts)

```ruby
begin
  # Partially updates a repair for an asset
  data, status_code, headers = api_instance.patch_asset_repair_with_http_info(tenant_id, asset_id, repair_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_repair_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **repair_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_asset_transfer

> <EmptyEnvelope> patch_asset_transfer(tenant_id, asset_id, transfer_id, opts)

Partially updates a transfer for an asset

Applies a JSON Patch document to an existing transfer record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates a transfer for an asset
  result = api_instance.patch_asset_transfer(tenant_id, asset_id, transfer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_transfer: #{e}"
end
```

#### Using the patch_asset_transfer_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_asset_transfer_with_http_info(tenant_id, asset_id, transfer_id, opts)

```ruby
begin
  # Partially updates a transfer for an asset
  data, status_code, headers = api_instance.patch_asset_transfer_with_http_info(tenant_id, asset_id, transfer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_asset_value_amend

> <EmptyEnvelope> patch_asset_value_amend(tenant_id, asset_id, amend_id, opts)

Partially updates a value amendment for an asset

Applies a JSON Patch document to an existing value amendment record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
amend_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates a value amendment for an asset
  result = api_instance.patch_asset_value_amend(tenant_id, asset_id, amend_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_value_amend: #{e}"
end
```

#### Using the patch_asset_value_amend_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_asset_value_amend_with_http_info(tenant_id, asset_id, amend_id, opts)

```ruby
begin
  # Partially updates a value amendment for an asset
  data, status_code, headers = api_instance.patch_asset_value_amend_with_http_info(tenant_id, asset_id, amend_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->patch_asset_value_amend_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **amend_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_asset

> <AssetDtoEnvelope> update_asset(tenant_id, asset_id, opts)

Updates an existing asset

Updates an existing asset for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_update_dto: OpenapiClient::AssetUpdateDto.new # AssetUpdateDto | 
}

begin
  # Updates an existing asset
  result = api_instance.update_asset(tenant_id, asset_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset: #{e}"
end
```

#### Using the update_asset_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetDtoEnvelope>, Integer, Hash)> update_asset_with_http_info(tenant_id, asset_id, opts)

```ruby
begin
  # Updates an existing asset
  data, status_code, headers = api_instance.update_asset_with_http_info(tenant_id, asset_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **asset_update_dto** | [**AssetUpdateDto**](AssetUpdateDto.md) |  | [optional] |

### Return type

[**AssetDtoEnvelope**](AssetDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_asset_asset_category

> <AssetCategoryDtoEnvelope> update_asset_asset_category(tenant_id, category_id, opts)

Updates an existing asset category

Updates an existing asset category for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_category_update_dto: OpenapiClient::AssetCategoryUpdateDto.new # AssetCategoryUpdateDto | 
}

begin
  # Updates an existing asset category
  result = api_instance.update_asset_asset_category(tenant_id, category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_asset_category: #{e}"
end
```

#### Using the update_asset_asset_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetCategoryDtoEnvelope>, Integer, Hash)> update_asset_asset_category_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Updates an existing asset category
  data, status_code, headers = api_instance.update_asset_asset_category_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **asset_category_update_dto** | [**AssetCategoryUpdateDto**](AssetCategoryUpdateDto.md) |  | [optional] |

### Return type

[**AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_asset_depreciation_record

> <EmptyEnvelope> update_asset_depreciation_record(tenant_id, asset_id, record_id, opts)

Updates a depreciation record for an asset

Updates an existing depreciation record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_depreciation_record_update_dto: OpenapiClient::AssetDepreciationRecordUpdateDto.new # AssetDepreciationRecordUpdateDto | 
}

begin
  # Updates a depreciation record for an asset
  result = api_instance.update_asset_depreciation_record(tenant_id, asset_id, record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_depreciation_record: #{e}"
end
```

#### Using the update_asset_depreciation_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_asset_depreciation_record_with_http_info(tenant_id, asset_id, record_id, opts)

```ruby
begin
  # Updates a depreciation record for an asset
  data, status_code, headers = api_instance.update_asset_depreciation_record_with_http_info(tenant_id, asset_id, record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_depreciation_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **record_id** | **String** |  |  |
| **asset_depreciation_record_update_dto** | [**AssetDepreciationRecordUpdateDto**](AssetDepreciationRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_asset_repair

> <EmptyEnvelope> update_asset_repair(tenant_id, asset_id, repair_id, opts)

Updates a repair for an asset

Updates an existing repair record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
repair_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_repair_update_dto: OpenapiClient::AssetRepairUpdateDto.new # AssetRepairUpdateDto | 
}

begin
  # Updates a repair for an asset
  result = api_instance.update_asset_repair(tenant_id, asset_id, repair_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_repair: #{e}"
end
```

#### Using the update_asset_repair_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_asset_repair_with_http_info(tenant_id, asset_id, repair_id, opts)

```ruby
begin
  # Updates a repair for an asset
  data, status_code, headers = api_instance.update_asset_repair_with_http_info(tenant_id, asset_id, repair_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_repair_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **repair_id** | **String** |  |  |
| **asset_repair_update_dto** | [**AssetRepairUpdateDto**](AssetRepairUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_asset_transfer

> <EmptyEnvelope> update_asset_transfer(tenant_id, asset_id, transfer_id, opts)

Updates a transfer for an asset

Updates an existing transfer record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_transfer_update_dto: OpenapiClient::AssetTransferUpdateDto.new # AssetTransferUpdateDto | 
}

begin
  # Updates a transfer for an asset
  result = api_instance.update_asset_transfer(tenant_id, asset_id, transfer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_transfer: #{e}"
end
```

#### Using the update_asset_transfer_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_asset_transfer_with_http_info(tenant_id, asset_id, transfer_id, opts)

```ruby
begin
  # Updates a transfer for an asset
  data, status_code, headers = api_instance.update_asset_transfer_with_http_info(tenant_id, asset_id, transfer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_transfer_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |
| **asset_transfer_update_dto** | [**AssetTransferUpdateDto**](AssetTransferUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_asset_value_amend

> <EmptyEnvelope> update_asset_value_amend(tenant_id, asset_id, amend_id, opts)

Updates a value amendment for an asset

Updates an existing value amendment record for the specified asset.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
asset_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
amend_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_value_amend_update_dto: OpenapiClient::AssetValueAmendUpdateDto.new # AssetValueAmendUpdateDto | 
}

begin
  # Updates a value amendment for an asset
  result = api_instance.update_asset_value_amend(tenant_id, asset_id, amend_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_value_amend: #{e}"
end
```

#### Using the update_asset_value_amend_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_asset_value_amend_with_http_info(tenant_id, asset_id, amend_id, opts)

```ruby
begin
  # Updates a value amendment for an asset
  data, status_code, headers = api_instance.update_asset_value_amend_with_http_info(tenant_id, asset_id, amend_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetsApi->update_asset_value_amend_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_id** | **String** |  |  |
| **amend_id** | **String** |  |  |
| **asset_value_amend_update_dto** | [**AssetValueAmendUpdateDto**](AssetValueAmendUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

