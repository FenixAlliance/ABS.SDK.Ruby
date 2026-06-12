# OpenapiClient::MaintenanceVisitsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_maintenance_visit_async**](MaintenanceVisitsApi.md#create_maintenance_visit_async) | **POST** /api/v2/SupportService/MaintenanceVisits | Create a maintenance visit |
| [**delete_maintenance_visit_async**](MaintenanceVisitsApi.md#delete_maintenance_visit_async) | **DELETE** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Delete a maintenance visit |
| [**get_maintenance_visit_async**](MaintenanceVisitsApi.md#get_maintenance_visit_async) | **GET** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Retrieve a maintenance visit by ID |
| [**get_maintenance_visits_async**](MaintenanceVisitsApi.md#get_maintenance_visits_async) | **GET** /api/v2/SupportService/MaintenanceVisits | Retrieve maintenance visits |
| [**get_maintenance_visits_count_async**](MaintenanceVisitsApi.md#get_maintenance_visits_count_async) | **GET** /api/v2/SupportService/MaintenanceVisits/Count | Get maintenance visits count |
| [**patch_maintenance_visit_async**](MaintenanceVisitsApi.md#patch_maintenance_visit_async) | **PATCH** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Patch a maintenance visit |
| [**update_maintenance_visit_async**](MaintenanceVisitsApi.md#update_maintenance_visit_async) | **PUT** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Update a maintenance visit |


## create_maintenance_visit_async

> <EmptyEnvelope> create_maintenance_visit_async(tenant_id, opts)

Create a maintenance visit

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MaintenanceVisitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  maintenance_visit_create_dto: OpenapiClient::MaintenanceVisitCreateDto.new # MaintenanceVisitCreateDto | 
}

begin
  # Create a maintenance visit
  result = api_instance.create_maintenance_visit_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->create_maintenance_visit_async: #{e}"
end
```

#### Using the create_maintenance_visit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_maintenance_visit_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a maintenance visit
  data, status_code, headers = api_instance.create_maintenance_visit_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->create_maintenance_visit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **maintenance_visit_create_dto** | [**MaintenanceVisitCreateDto**](MaintenanceVisitCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_maintenance_visit_async

> <EmptyEnvelope> delete_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)

Delete a maintenance visit

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MaintenanceVisitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
maintenance_visit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a maintenance visit
  result = api_instance.delete_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->delete_maintenance_visit_async: #{e}"
end
```

#### Using the delete_maintenance_visit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)

```ruby
begin
  # Delete a maintenance visit
  data, status_code, headers = api_instance.delete_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->delete_maintenance_visit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **maintenance_visit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_maintenance_visit_async

> <MaintenanceVisitDtoEnvelope> get_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)

Retrieve a maintenance visit by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MaintenanceVisitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
maintenance_visit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a maintenance visit by ID
  result = api_instance.get_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->get_maintenance_visit_async: #{e}"
end
```

#### Using the get_maintenance_visit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MaintenanceVisitDtoEnvelope>, Integer, Hash)> get_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)

```ruby
begin
  # Retrieve a maintenance visit by ID
  data, status_code, headers = api_instance.get_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MaintenanceVisitDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->get_maintenance_visit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **maintenance_visit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MaintenanceVisitDtoEnvelope**](MaintenanceVisitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_maintenance_visits_async

> <MaintenanceVisitDtoListEnvelope> get_maintenance_visits_async(tenant_id, opts)

Retrieve maintenance visits

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MaintenanceVisitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve maintenance visits
  result = api_instance.get_maintenance_visits_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->get_maintenance_visits_async: #{e}"
end
```

#### Using the get_maintenance_visits_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MaintenanceVisitDtoListEnvelope>, Integer, Hash)> get_maintenance_visits_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve maintenance visits
  data, status_code, headers = api_instance.get_maintenance_visits_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MaintenanceVisitDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->get_maintenance_visits_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MaintenanceVisitDtoListEnvelope**](MaintenanceVisitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_maintenance_visits_count_async

> <Int32Envelope> get_maintenance_visits_count_async(tenant_id, opts)

Get maintenance visits count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MaintenanceVisitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get maintenance visits count
  result = api_instance.get_maintenance_visits_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->get_maintenance_visits_count_async: #{e}"
end
```

#### Using the get_maintenance_visits_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_maintenance_visits_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get maintenance visits count
  data, status_code, headers = api_instance.get_maintenance_visits_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->get_maintenance_visits_count_async_with_http_info: #{e}"
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


## patch_maintenance_visit_async

> <EmptyEnvelope> patch_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)

Patch a maintenance visit

Partially updates an existing maintenance visit by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MaintenanceVisitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
maintenance_visit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a maintenance visit
  result = api_instance.patch_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->patch_maintenance_visit_async: #{e}"
end
```

#### Using the patch_maintenance_visit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)

```ruby
begin
  # Patch a maintenance visit
  data, status_code, headers = api_instance.patch_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->patch_maintenance_visit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **maintenance_visit_id** | **String** |  |  |
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


## update_maintenance_visit_async

> <EmptyEnvelope> update_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)

Update a maintenance visit

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MaintenanceVisitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
maintenance_visit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  body: { ... } # Object | 
}

begin
  # Update a maintenance visit
  result = api_instance.update_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->update_maintenance_visit_async: #{e}"
end
```

#### Using the update_maintenance_visit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)

```ruby
begin
  # Update a maintenance visit
  data, status_code, headers = api_instance.update_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MaintenanceVisitsApi->update_maintenance_visit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **maintenance_visit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **body** | **Object** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

