# OpenapiClient::DealUnitFlowsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_deal_unit_flow_async**](DealUnitFlowsApi.md#create_deal_unit_flow_async) | **POST** /api/v2/DealsService/DealUnitFlows | Create a deal unit flow |
| [**create_deal_unit_flow_stage_async**](DealUnitFlowsApi.md#create_deal_unit_flow_stage_async) | **POST** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId}/Stages | Create a deal unit flow stage |
| [**delete_deal_unit_flow_async**](DealUnitFlowsApi.md#delete_deal_unit_flow_async) | **DELETE** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId} | Delete a deal unit flow |
| [**delete_deal_unit_flow_stage_async**](DealUnitFlowsApi.md#delete_deal_unit_flow_stage_async) | **DELETE** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId}/Stages/{dealUnitFlowStageId} | Delete a deal unit flow stage |
| [**get_deal_unit_flow_async**](DealUnitFlowsApi.md#get_deal_unit_flow_async) | **GET** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId} | Get deal unit flow by ID |
| [**get_deal_unit_flow_stage_async**](DealUnitFlowsApi.md#get_deal_unit_flow_stage_async) | **GET** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId}/Stages/{dealUnitFlowStageId} | Get a deal unit flow stage by ID |
| [**get_deal_unit_flow_stages_async**](DealUnitFlowsApi.md#get_deal_unit_flow_stages_async) | **GET** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId}/Stages | Get stages for a deal unit flow |
| [**get_deal_unit_flow_stages_count_async**](DealUnitFlowsApi.md#get_deal_unit_flow_stages_count_async) | **GET** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId}/Stages/Count | Get stages count for a deal unit flow |
| [**get_deal_unit_flows_async**](DealUnitFlowsApi.md#get_deal_unit_flows_async) | **GET** /api/v2/DealsService/DealUnitFlows | Get deal unit flows |
| [**get_deal_unit_flows_count_async**](DealUnitFlowsApi.md#get_deal_unit_flows_count_async) | **GET** /api/v2/DealsService/DealUnitFlows/Count | Get deal unit flows count |
| [**patch_deal_unit_flow_async**](DealUnitFlowsApi.md#patch_deal_unit_flow_async) | **PATCH** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId} | Patch a deal unit flow |
| [**patch_deal_unit_flow_stage_async**](DealUnitFlowsApi.md#patch_deal_unit_flow_stage_async) | **PATCH** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId}/Stages/{dealUnitFlowStageId} | Patch a deal unit flow stage |
| [**update_deal_unit_flow_async**](DealUnitFlowsApi.md#update_deal_unit_flow_async) | **PUT** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId} | Update a deal unit flow |
| [**update_deal_unit_flow_stage_async**](DealUnitFlowsApi.md#update_deal_unit_flow_stage_async) | **PUT** /api/v2/DealsService/DealUnitFlows/{dealUnitFlowId}/Stages/{dealUnitFlowStageId} | Update a deal unit flow stage |


## create_deal_unit_flow_async

> <EmptyEnvelope> create_deal_unit_flow_async(tenant_id, opts)

Create a deal unit flow

Creates a new deal unit flow for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  deal_unit_flow_create_dto: OpenapiClient::DealUnitFlowCreateDto.new # DealUnitFlowCreateDto | 
}

begin
  # Create a deal unit flow
  result = api_instance.create_deal_unit_flow_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->create_deal_unit_flow_async: #{e}"
end
```

#### Using the create_deal_unit_flow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_deal_unit_flow_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a deal unit flow
  data, status_code, headers = api_instance.create_deal_unit_flow_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->create_deal_unit_flow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_create_dto** | [**DealUnitFlowCreateDto**](DealUnitFlowCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_deal_unit_flow_stage_async

> <EmptyEnvelope> create_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, opts)

Create a deal unit flow stage

Creates a new stage within a specific deal unit flow.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  deal_unit_flow_stage_create_dto: OpenapiClient::DealUnitFlowStageCreateDto.new # DealUnitFlowStageCreateDto | 
}

begin
  # Create a deal unit flow stage
  result = api_instance.create_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->create_deal_unit_flow_stage_async: #{e}"
end
```

#### Using the create_deal_unit_flow_stage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, opts)

```ruby
begin
  # Create a deal unit flow stage
  data, status_code, headers = api_instance.create_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->create_deal_unit_flow_stage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |
| **deal_unit_flow_stage_create_dto** | [**DealUnitFlowStageCreateDto**](DealUnitFlowStageCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_deal_unit_flow_async

> <EmptyEnvelope> delete_deal_unit_flow_async(tenant_id, deal_unit_flow_id)

Delete a deal unit flow

Deletes an existing deal unit flow by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a deal unit flow
  result = api_instance.delete_deal_unit_flow_async(tenant_id, deal_unit_flow_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->delete_deal_unit_flow_async: #{e}"
end
```

#### Using the delete_deal_unit_flow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_deal_unit_flow_async_with_http_info(tenant_id, deal_unit_flow_id)

```ruby
begin
  # Delete a deal unit flow
  data, status_code, headers = api_instance.delete_deal_unit_flow_async_with_http_info(tenant_id, deal_unit_flow_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->delete_deal_unit_flow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_deal_unit_flow_stage_async

> <EmptyEnvelope> delete_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id)

Delete a deal unit flow stage

Deletes an existing stage from a specific deal unit flow.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_stage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a deal unit flow stage
  result = api_instance.delete_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->delete_deal_unit_flow_stage_async: #{e}"
end
```

#### Using the delete_deal_unit_flow_stage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id)

```ruby
begin
  # Delete a deal unit flow stage
  data, status_code, headers = api_instance.delete_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->delete_deal_unit_flow_stage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |
| **deal_unit_flow_stage_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_flow_async

> <DealUnitFlowDtoEnvelope> get_deal_unit_flow_async(tenant_id, deal_unit_flow_id)

Get deal unit flow by ID

Retrieves a single deal unit flow by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get deal unit flow by ID
  result = api_instance.get_deal_unit_flow_async(tenant_id, deal_unit_flow_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flow_async: #{e}"
end
```

#### Using the get_deal_unit_flow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DealUnitFlowDtoEnvelope>, Integer, Hash)> get_deal_unit_flow_async_with_http_info(tenant_id, deal_unit_flow_id)

```ruby
begin
  # Get deal unit flow by ID
  data, status_code, headers = api_instance.get_deal_unit_flow_async_with_http_info(tenant_id, deal_unit_flow_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DealUnitFlowDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |

### Return type

[**DealUnitFlowDtoEnvelope**](DealUnitFlowDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_flow_stage_async

> <DealUnitFlowStageDtoEnvelope> get_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id)

Get a deal unit flow stage by ID

Retrieves a single stage for a specific deal unit flow by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_stage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get a deal unit flow stage by ID
  result = api_instance.get_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flow_stage_async: #{e}"
end
```

#### Using the get_deal_unit_flow_stage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DealUnitFlowStageDtoEnvelope>, Integer, Hash)> get_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id)

```ruby
begin
  # Get a deal unit flow stage by ID
  data, status_code, headers = api_instance.get_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DealUnitFlowStageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flow_stage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |
| **deal_unit_flow_stage_id** | **String** |  |  |

### Return type

[**DealUnitFlowStageDtoEnvelope**](DealUnitFlowStageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_flow_stages_async

> <DealUnitFlowStageDtoListEnvelope> get_deal_unit_flow_stages_async(tenant_id, deal_unit_flow_id)

Get stages for a deal unit flow

Retrieves a list of stages for a specific deal unit flow with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get stages for a deal unit flow
  result = api_instance.get_deal_unit_flow_stages_async(tenant_id, deal_unit_flow_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flow_stages_async: #{e}"
end
```

#### Using the get_deal_unit_flow_stages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DealUnitFlowStageDtoListEnvelope>, Integer, Hash)> get_deal_unit_flow_stages_async_with_http_info(tenant_id, deal_unit_flow_id)

```ruby
begin
  # Get stages for a deal unit flow
  data, status_code, headers = api_instance.get_deal_unit_flow_stages_async_with_http_info(tenant_id, deal_unit_flow_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DealUnitFlowStageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flow_stages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |

### Return type

[**DealUnitFlowStageDtoListEnvelope**](DealUnitFlowStageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_flow_stages_count_async

> <Int32Envelope> get_deal_unit_flow_stages_count_async(tenant_id, deal_unit_flow_id)

Get stages count for a deal unit flow

Returns the total count of stages for a specific deal unit flow with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get stages count for a deal unit flow
  result = api_instance.get_deal_unit_flow_stages_count_async(tenant_id, deal_unit_flow_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flow_stages_count_async: #{e}"
end
```

#### Using the get_deal_unit_flow_stages_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_deal_unit_flow_stages_count_async_with_http_info(tenant_id, deal_unit_flow_id)

```ruby
begin
  # Get stages count for a deal unit flow
  data, status_code, headers = api_instance.get_deal_unit_flow_stages_count_async_with_http_info(tenant_id, deal_unit_flow_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flow_stages_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_flows_async

> <DealUnitFlowDtoListEnvelope> get_deal_unit_flows_async(tenant_id)

Get deal unit flows

Retrieves a list of deal unit flows for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get deal unit flows
  result = api_instance.get_deal_unit_flows_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flows_async: #{e}"
end
```

#### Using the get_deal_unit_flows_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<DealUnitFlowDtoListEnvelope>, Integer, Hash)> get_deal_unit_flows_async_with_http_info(tenant_id)

```ruby
begin
  # Get deal unit flows
  data, status_code, headers = api_instance.get_deal_unit_flows_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <DealUnitFlowDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flows_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**DealUnitFlowDtoListEnvelope**](DealUnitFlowDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_deal_unit_flows_count_async

> <Int32Envelope> get_deal_unit_flows_count_async(tenant_id)

Get deal unit flows count

Returns the total count of deal unit flows for the specified tenant with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get deal unit flows count
  result = api_instance.get_deal_unit_flows_count_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flows_count_async: #{e}"
end
```

#### Using the get_deal_unit_flows_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_deal_unit_flows_count_async_with_http_info(tenant_id)

```ruby
begin
  # Get deal unit flows count
  data, status_code, headers = api_instance.get_deal_unit_flows_count_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->get_deal_unit_flows_count_async_with_http_info: #{e}"
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


## patch_deal_unit_flow_async

> <EmptyEnvelope> patch_deal_unit_flow_async(tenant_id, deal_unit_flow_id, opts)

Patch a deal unit flow

Partially updates an existing deal unit flow by its unique identifier using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a deal unit flow
  result = api_instance.patch_deal_unit_flow_async(tenant_id, deal_unit_flow_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->patch_deal_unit_flow_async: #{e}"
end
```

#### Using the patch_deal_unit_flow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_deal_unit_flow_async_with_http_info(tenant_id, deal_unit_flow_id, opts)

```ruby
begin
  # Patch a deal unit flow
  data, status_code, headers = api_instance.patch_deal_unit_flow_async_with_http_info(tenant_id, deal_unit_flow_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->patch_deal_unit_flow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_deal_unit_flow_stage_async

> <EmptyEnvelope> patch_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id, opts)

Patch a deal unit flow stage

Partially updates an existing stage within a specific deal unit flow using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_stage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a deal unit flow stage
  result = api_instance.patch_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->patch_deal_unit_flow_stage_async: #{e}"
end
```

#### Using the patch_deal_unit_flow_stage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id, opts)

```ruby
begin
  # Patch a deal unit flow stage
  data, status_code, headers = api_instance.patch_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->patch_deal_unit_flow_stage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |
| **deal_unit_flow_stage_id** | **String** |  |  |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_deal_unit_flow_async

> <EmptyEnvelope> update_deal_unit_flow_async(tenant_id, deal_unit_flow_id, opts)

Update a deal unit flow

Updates an existing deal unit flow by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  deal_unit_flow_update_dto: OpenapiClient::DealUnitFlowUpdateDto.new # DealUnitFlowUpdateDto | 
}

begin
  # Update a deal unit flow
  result = api_instance.update_deal_unit_flow_async(tenant_id, deal_unit_flow_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->update_deal_unit_flow_async: #{e}"
end
```

#### Using the update_deal_unit_flow_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_deal_unit_flow_async_with_http_info(tenant_id, deal_unit_flow_id, opts)

```ruby
begin
  # Update a deal unit flow
  data, status_code, headers = api_instance.update_deal_unit_flow_async_with_http_info(tenant_id, deal_unit_flow_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->update_deal_unit_flow_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |
| **deal_unit_flow_update_dto** | [**DealUnitFlowUpdateDto**](DealUnitFlowUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_deal_unit_flow_stage_async

> <EmptyEnvelope> update_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id, opts)

Update a deal unit flow stage

Updates an existing stage within a specific deal unit flow.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::DealUnitFlowsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
deal_unit_flow_stage_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  deal_unit_flow_stage_update_dto: OpenapiClient::DealUnitFlowStageUpdateDto.new # DealUnitFlowStageUpdateDto | 
}

begin
  # Update a deal unit flow stage
  result = api_instance.update_deal_unit_flow_stage_async(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->update_deal_unit_flow_stage_async: #{e}"
end
```

#### Using the update_deal_unit_flow_stage_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id, opts)

```ruby
begin
  # Update a deal unit flow stage
  data, status_code, headers = api_instance.update_deal_unit_flow_stage_async_with_http_info(tenant_id, deal_unit_flow_id, deal_unit_flow_stage_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling DealUnitFlowsApi->update_deal_unit_flow_stage_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **deal_unit_flow_id** | **String** |  |  |
| **deal_unit_flow_stage_id** | **String** |  |  |
| **deal_unit_flow_stage_update_dto** | [**DealUnitFlowStageUpdateDto**](DealUnitFlowStageUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

