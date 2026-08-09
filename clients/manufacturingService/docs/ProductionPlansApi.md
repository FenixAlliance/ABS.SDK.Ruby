# OpenapiClient::ProductionPlansApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_production_plan_async**](ProductionPlansApi.md#create_production_plan_async) | **POST** /api/v2/ManufacturingService/ProductionPlans | Create a new production plan |
| [**delete_production_plan_async**](ProductionPlansApi.md#delete_production_plan_async) | **DELETE** /api/v2/ManufacturingService/ProductionPlans/{id} | Delete a production plan |
| [**get_production_plan_by_id_async**](ProductionPlansApi.md#get_production_plan_by_id_async) | **GET** /api/v2/ManufacturingService/ProductionPlans/{id} | Get production plan by ID |
| [**get_production_plans_async**](ProductionPlansApi.md#get_production_plans_async) | **GET** /api/v2/ManufacturingService/ProductionPlans | Get all production plans |
| [**get_production_plans_count_async**](ProductionPlansApi.md#get_production_plans_count_async) | **GET** /api/v2/ManufacturingService/ProductionPlans/Count | Get production plans count |
| [**patch_production_plan_async**](ProductionPlansApi.md#patch_production_plan_async) | **PATCH** /api/v2/ManufacturingService/ProductionPlans/{id} | Patch a production plan |
| [**update_production_plan_async**](ProductionPlansApi.md#update_production_plan_async) | **PUT** /api/v2/ManufacturingService/ProductionPlans/{id} | Update a production plan |


## create_production_plan_async

> create_production_plan_async(tenant_id, opts)

Create a new production plan

Creates a new production plan for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProductionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  production_plan_create_dto: OpenapiClient::ProductionPlanCreateDto.new({title: 'title_example'}) # ProductionPlanCreateDto | 
}

begin
  # Create a new production plan
  api_instance.create_production_plan_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->create_production_plan_async: #{e}"
end
```

#### Using the create_production_plan_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_production_plan_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new production plan
  data, status_code, headers = api_instance.create_production_plan_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->create_production_plan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **production_plan_create_dto** | [**ProductionPlanCreateDto**](ProductionPlanCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_production_plan_async

> delete_production_plan_async(tenant_id, id, opts)

Delete a production plan

Deletes a production plan for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProductionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a production plan
  api_instance.delete_production_plan_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->delete_production_plan_async: #{e}"
end
```

#### Using the delete_production_plan_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_production_plan_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a production plan
  data, status_code, headers = api_instance.delete_production_plan_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->delete_production_plan_async_with_http_info: #{e}"
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


## get_production_plan_by_id_async

> <ProductionPlanDto> get_production_plan_by_id_async(tenant_id, id, opts)

Get production plan by ID

Retrieves a specific production plan by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProductionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get production plan by ID
  result = api_instance.get_production_plan_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->get_production_plan_by_id_async: #{e}"
end
```

#### Using the get_production_plan_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProductionPlanDto>, Integer, Hash)> get_production_plan_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get production plan by ID
  data, status_code, headers = api_instance.get_production_plan_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProductionPlanDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->get_production_plan_by_id_async_with_http_info: #{e}"
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

[**ProductionPlanDto**](ProductionPlanDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_production_plans_async

> <ProductionPlanDtoListEnvelope> get_production_plans_async(tenant_id, opts)

Get all production plans

Retrieves all production plans for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProductionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  production_plan_dto_collection_query_parameters: OpenapiClient::ProductionPlanDtoCollectionQueryParameters.new # ProductionPlanDtoCollectionQueryParameters | 
}

begin
  # Get all production plans
  result = api_instance.get_production_plans_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->get_production_plans_async: #{e}"
end
```

#### Using the get_production_plans_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ProductionPlanDtoListEnvelope>, Integer, Hash)> get_production_plans_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all production plans
  data, status_code, headers = api_instance.get_production_plans_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ProductionPlanDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->get_production_plans_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **production_plan_dto_collection_query_parameters** | [**ProductionPlanDtoCollectionQueryParameters**](ProductionPlanDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ProductionPlanDtoListEnvelope**](ProductionPlanDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_production_plans_count_async

> <Int32Envelope> get_production_plans_count_async(tenant_id, opts)

Get production plans count

Returns the count of production plans for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProductionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  production_plan_dto_collection_query_parameters: OpenapiClient::ProductionPlanDtoCollectionQueryParameters.new # ProductionPlanDtoCollectionQueryParameters | 
}

begin
  # Get production plans count
  result = api_instance.get_production_plans_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->get_production_plans_count_async: #{e}"
end
```

#### Using the get_production_plans_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_production_plans_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get production plans count
  data, status_code, headers = api_instance.get_production_plans_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->get_production_plans_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **production_plan_dto_collection_query_parameters** | [**ProductionPlanDtoCollectionQueryParameters**](ProductionPlanDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_production_plan_async

> <EmptyEnvelope> patch_production_plan_async(tenant_id, id, opts)

Patch a production plan

Patch a production plan

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProductionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a production plan
  result = api_instance.patch_production_plan_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->patch_production_plan_async: #{e}"
end
```

#### Using the patch_production_plan_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_production_plan_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a production plan
  data, status_code, headers = api_instance.patch_production_plan_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->patch_production_plan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_production_plan_async

> update_production_plan_async(tenant_id, id, opts)

Update a production plan

Updates an existing production plan for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ProductionPlansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  production_plan_update_dto: OpenapiClient::ProductionPlanUpdateDto.new # ProductionPlanUpdateDto | 
}

begin
  # Update a production plan
  api_instance.update_production_plan_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->update_production_plan_async: #{e}"
end
```

#### Using the update_production_plan_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_production_plan_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a production plan
  data, status_code, headers = api_instance.update_production_plan_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ProductionPlansApi->update_production_plan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **production_plan_update_dto** | [**ProductionPlanUpdateDto**](ProductionPlanUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

