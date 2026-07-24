# OpenapiClient::LicenseFeaturesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_license_feature_async**](LicenseFeaturesApi.md#create_license_feature_async) | **POST** /api/v2/LicensingService/LicenseFeatures | Create a new license feature |
| [**delete_license_feature_async**](LicenseFeaturesApi.md#delete_license_feature_async) | **DELETE** /api/v2/LicensingService/LicenseFeatures/{id} | Delete a license feature |
| [**get_license_feature_by_id_async**](LicenseFeaturesApi.md#get_license_feature_by_id_async) | **GET** /api/v2/LicensingService/LicenseFeatures/{id} | Get license feature by ID |
| [**get_license_features_async**](LicenseFeaturesApi.md#get_license_features_async) | **GET** /api/v2/LicensingService/LicenseFeatures | Get all license features |
| [**get_license_features_count_async**](LicenseFeaturesApi.md#get_license_features_count_async) | **GET** /api/v2/LicensingService/LicenseFeatures/Count | Get license features count |
| [**patch_license_feature_async**](LicenseFeaturesApi.md#patch_license_feature_async) | **PATCH** /api/v2/LicensingService/LicenseFeatures/{id} | Patch a license feature |
| [**update_license_feature_async**](LicenseFeaturesApi.md#update_license_feature_async) | **PUT** /api/v2/LicensingService/LicenseFeatures/{id} | Update a license feature |


## create_license_feature_async

> create_license_feature_async(tenant_id, opts)

Create a new license feature

Creates a new license feature for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseFeaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_feature_create_dto: OpenapiClient::LicenseFeatureCreateDto.new({key: 'key_example', value: 'value_example', name: 'name_example'}) # LicenseFeatureCreateDto | 
}

begin
  # Create a new license feature
  api_instance.create_license_feature_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->create_license_feature_async: #{e}"
end
```

#### Using the create_license_feature_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_license_feature_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new license feature
  data, status_code, headers = api_instance.create_license_feature_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->create_license_feature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_feature_create_dto** | [**LicenseFeatureCreateDto**](LicenseFeatureCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_license_feature_async

> delete_license_feature_async(tenant_id, id, opts)

Delete a license feature

Deletes a license feature for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseFeaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a license feature
  api_instance.delete_license_feature_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->delete_license_feature_async: #{e}"
end
```

#### Using the delete_license_feature_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_license_feature_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a license feature
  data, status_code, headers = api_instance.delete_license_feature_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->delete_license_feature_async_with_http_info: #{e}"
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


## get_license_feature_by_id_async

> <LicenseFeatureDto> get_license_feature_by_id_async(tenant_id, id, opts)

Get license feature by ID

Retrieves a specific license feature by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseFeaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get license feature by ID
  result = api_instance.get_license_feature_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->get_license_feature_by_id_async: #{e}"
end
```

#### Using the get_license_feature_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseFeatureDto>, Integer, Hash)> get_license_feature_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get license feature by ID
  data, status_code, headers = api_instance.get_license_feature_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseFeatureDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->get_license_feature_by_id_async_with_http_info: #{e}"
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

[**LicenseFeatureDto**](LicenseFeatureDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_license_features_async

> <LicenseFeatureDtoListEnvelope> get_license_features_async(tenant_id, opts)

Get all license features

Retrieves all license features for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseFeaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all license features
  result = api_instance.get_license_features_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->get_license_features_async: #{e}"
end
```

#### Using the get_license_features_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LicenseFeatureDtoListEnvelope>, Integer, Hash)> get_license_features_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all license features
  data, status_code, headers = api_instance.get_license_features_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LicenseFeatureDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->get_license_features_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LicenseFeatureDtoListEnvelope**](LicenseFeatureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_license_features_count_async

> <Int32Envelope> get_license_features_count_async(tenant_id, opts)

Get license features count

Returns the count of license features for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseFeaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get license features count
  result = api_instance.get_license_features_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->get_license_features_count_async: #{e}"
end
```

#### Using the get_license_features_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_license_features_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get license features count
  data, status_code, headers = api_instance.get_license_features_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->get_license_features_count_async_with_http_info: #{e}"
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


## patch_license_feature_async

> <EmptyEnvelope> patch_license_feature_async(tenant_id, id, opts)

Patch a license feature

Patch a license feature for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseFeaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a license feature
  result = api_instance.patch_license_feature_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->patch_license_feature_async: #{e}"
end
```

#### Using the patch_license_feature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_license_feature_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a license feature
  data, status_code, headers = api_instance.patch_license_feature_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->patch_license_feature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
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


## update_license_feature_async

> update_license_feature_async(tenant_id, id, opts)

Update a license feature

Updates an existing license feature for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LicenseFeaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  license_feature_update_dto: OpenapiClient::LicenseFeatureUpdateDto.new # LicenseFeatureUpdateDto | 
}

begin
  # Update a license feature
  api_instance.update_license_feature_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->update_license_feature_async: #{e}"
end
```

#### Using the update_license_feature_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_license_feature_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a license feature
  data, status_code, headers = api_instance.update_license_feature_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling LicenseFeaturesApi->update_license_feature_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **license_feature_update_dto** | [**LicenseFeatureUpdateDto**](LicenseFeatureUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

