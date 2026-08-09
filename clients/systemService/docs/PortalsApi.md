# OpenapiClient::PortalsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_system_portal**](PortalsApi.md#create_system_portal) | **POST** /api/v2/SystemService/Portals | Create a new system portal |
| [**delete_system_portal**](PortalsApi.md#delete_system_portal) | **DELETE** /api/v2/SystemService/Portals/{portalId} | Delete a system portal |
| [**get_system_portal_by_id**](PortalsApi.md#get_system_portal_by_id) | **GET** /api/v2/SystemService/Portals/{portalId} | Retrieve a single system portal by its ID |
| [**get_system_portals**](PortalsApi.md#get_system_portals) | **GET** /api/v2/SystemService/Portals | Retrieve a list of system portals |
| [**get_system_portals_count**](PortalsApi.md#get_system_portals_count) | **GET** /api/v2/SystemService/Portals/Count | Get the count of system portals |
| [**patch_system_portal**](PortalsApi.md#patch_system_portal) | **PATCH** /api/v2/SystemService/Portals/{portalId} | Partially update a system portal |
| [**update_system_portal**](PortalsApi.md#update_system_portal) | **PUT** /api/v2/SystemService/Portals/{portalId} | Update a system portal |


## create_system_portal

> <EmptyEnvelope> create_system_portal(opts)

Create a new system portal

Create a new web portal in the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_portal_create_dto: OpenapiClient::WebPortalCreateDto.new # WebPortalCreateDto | 
}

begin
  # Create a new system portal
  result = api_instance.create_system_portal(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->create_system_portal: #{e}"
end
```

#### Using the create_system_portal_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_system_portal_with_http_info(opts)

```ruby
begin
  # Create a new system portal
  data, status_code, headers = api_instance.create_system_portal_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->create_system_portal_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_portal_create_dto** | [**WebPortalCreateDto**](WebPortalCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_system_portal

> <EmptyEnvelope> delete_system_portal(portal_id, opts)

Delete a system portal

Delete a web portal from the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a system portal
  result = api_instance.delete_system_portal(portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->delete_system_portal: #{e}"
end
```

#### Using the delete_system_portal_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_system_portal_with_http_info(portal_id, opts)

```ruby
begin
  # Delete a system portal
  data, status_code, headers = api_instance.delete_system_portal_with_http_info(portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->delete_system_portal_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **portal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_portal_by_id

> <WebPortalDtoEnvelope> get_system_portal_by_id(portal_id, opts)

Retrieve a single system portal by its ID

Retrieve a single system portal by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single system portal by its ID
  result = api_instance.get_system_portal_by_id(portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_system_portal_by_id: #{e}"
end
```

#### Using the get_system_portal_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPortalDtoEnvelope>, Integer, Hash)> get_system_portal_by_id_with_http_info(portal_id, opts)

```ruby
begin
  # Retrieve a single system portal by its ID
  data, status_code, headers = api_instance.get_system_portal_by_id_with_http_info(portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPortalDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_system_portal_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **portal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_system_portals

> <WebPortalDtoListEnvelope> get_system_portals(opts)

Retrieve a list of system portals

Retrieve a list of all web portals in the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_portal_dto_collection_query_parameters: OpenapiClient::WebPortalDtoCollectionQueryParameters.new # WebPortalDtoCollectionQueryParameters | 
}

begin
  # Retrieve a list of system portals
  result = api_instance.get_system_portals(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_system_portals: #{e}"
end
```

#### Using the get_system_portals_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPortalDtoListEnvelope>, Integer, Hash)> get_system_portals_with_http_info(opts)

```ruby
begin
  # Retrieve a list of system portals
  data, status_code, headers = api_instance.get_system_portals_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPortalDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_system_portals_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_portal_dto_collection_query_parameters** | [**WebPortalDtoCollectionQueryParameters**](WebPortalDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**WebPortalDtoListEnvelope**](WebPortalDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_system_portals_count

> <Int32Envelope> get_system_portals_count(opts)

Get the count of system portals

Get the count of all web portals in the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_portal_dto_collection_query_parameters: OpenapiClient::WebPortalDtoCollectionQueryParameters.new # WebPortalDtoCollectionQueryParameters | 
}

begin
  # Get the count of system portals
  result = api_instance.get_system_portals_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_system_portals_count: #{e}"
end
```

#### Using the get_system_portals_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_system_portals_count_with_http_info(opts)

```ruby
begin
  # Get the count of system portals
  data, status_code, headers = api_instance.get_system_portals_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_system_portals_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_portal_dto_collection_query_parameters** | [**WebPortalDtoCollectionQueryParameters**](WebPortalDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_system_portal

> <EmptyEnvelope> patch_system_portal(portal_id, opts)

Partially update a system portal

Partially update an existing web portal in the system using a JSON Patch document

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially update a system portal
  result = api_instance.patch_system_portal(portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->patch_system_portal: #{e}"
end
```

#### Using the patch_system_portal_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_system_portal_with_http_info(portal_id, opts)

```ruby
begin
  # Partially update a system portal
  data, status_code, headers = api_instance.patch_system_portal_with_http_info(portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->patch_system_portal_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **portal_id** | **String** |  |  |
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


## update_system_portal

> <EmptyEnvelope> update_system_portal(portal_id, opts)

Update a system portal

Update an existing web portal in the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_portal_update_dto: OpenapiClient::WebPortalUpdateDto.new # WebPortalUpdateDto | 
}

begin
  # Update a system portal
  result = api_instance.update_system_portal(portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->update_system_portal: #{e}"
end
```

#### Using the update_system_portal_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_system_portal_with_http_info(portal_id, opts)

```ruby
begin
  # Update a system portal
  data, status_code, headers = api_instance.update_system_portal_with_http_info(portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->update_system_portal_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **portal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **web_portal_update_dto** | [**WebPortalUpdateDto**](WebPortalUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

