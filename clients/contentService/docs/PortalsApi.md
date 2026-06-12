# OpenapiClient::PortalsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**bind_web_portal_domain_async**](PortalsApi.md#bind_web_portal_domain_async) | **POST** /api/v2/ContentService/Portals/{portalId}/DomainBindings/{businessDomainId} | Bind a domain to a web portal |
| [**count_portals_async**](PortalsApi.md#count_portals_async) | **GET** /api/v2/ContentService/Portals/Count | Count portals |
| [**create_web_portal_async**](PortalsApi.md#create_web_portal_async) | **POST** /api/v2/ContentService/Portals | Create a new web portal |
| [**delete_web_portal_async**](PortalsApi.md#delete_web_portal_async) | **DELETE** /api/v2/ContentService/Portals/{portalId} | Delete a web portal |
| [**get_current_web_portal_async**](PortalsApi.md#get_current_web_portal_async) | **GET** /api/v2/ContentService/Portals/Current | Get the current portal |
| [**get_current_web_portal_options_async**](PortalsApi.md#get_current_web_portal_options_async) | **GET** /api/v2/ContentService/Portals/Current/Options | Get the current portal&#39;s options |
| [**get_portals_async**](PortalsApi.md#get_portals_async) | **GET** /api/v2/ContentService/Portals | Get portals |
| [**get_root_web_portal_async**](PortalsApi.md#get_root_web_portal_async) | **GET** /api/v2/ContentService/Portals/Root | Get the root portal |
| [**get_web_portal_by_id_async**](PortalsApi.md#get_web_portal_by_id_async) | **GET** /api/v2/ContentService/Portals/{portalId} | Get a web portal by its ID |
| [**get_web_portal_domain_bindings_async**](PortalsApi.md#get_web_portal_domain_bindings_async) | **GET** /api/v2/ContentService/Portals/{portalId}/DomainBindings | Get a web portal&#39;s bound domains |
| [**get_web_portal_options_async**](PortalsApi.md#get_web_portal_options_async) | **GET** /api/v2/ContentService/Portals/{portalId}/Options | Get a web portal&#39;s options by its ID |
| [**get_web_portal_settings_async**](PortalsApi.md#get_web_portal_settings_async) | **GET** /api/v2/ContentService/Portals/{portalId}/Settings | Get a web portal&#39;s settings by its ID |
| [**initialize_current_web_portal_async**](PortalsApi.md#initialize_current_web_portal_async) | **POST** /api/v2/ContentService/Portals/Initialize | Initialize the current portal |
| [**patch_web_portal_async**](PortalsApi.md#patch_web_portal_async) | **PATCH** /api/v2/ContentService/Portals/{portalId} | Partially update a web portal |
| [**search_web_portal_async**](PortalsApi.md#search_web_portal_async) | **GET** /api/v2/ContentService/Portals/Search | Search for a portal by its domain |
| [**unbind_web_portal_domain_async**](PortalsApi.md#unbind_web_portal_domain_async) | **DELETE** /api/v2/ContentService/Portals/{portalId}/DomainBindings/{businessDomainId} | Unbind a domain from a web portal |
| [**update_web_portal_async**](PortalsApi.md#update_web_portal_async) | **PUT** /api/v2/ContentService/Portals/{portalId} | Update an existing web portal |
| [**update_web_portal_settings_async**](PortalsApi.md#update_web_portal_settings_async) | **PUT** /api/v2/ContentService/Portals/{portalId}/Settings | Update a web portal&#39;s settings |


## bind_web_portal_domain_async

> <EmptyEnvelope> bind_web_portal_domain_async(tenant_id, portal_id, business_domain_id, opts)

Bind a domain to a web portal

Bind a verified BusinessDomain to a web portal

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_domain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Bind a domain to a web portal
  result = api_instance.bind_web_portal_domain_async(tenant_id, portal_id, business_domain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->bind_web_portal_domain_async: #{e}"
end
```

#### Using the bind_web_portal_domain_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> bind_web_portal_domain_async_with_http_info(tenant_id, portal_id, business_domain_id, opts)

```ruby
begin
  # Bind a domain to a web portal
  data, status_code, headers = api_instance.bind_web_portal_domain_async_with_http_info(tenant_id, portal_id, business_domain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->bind_web_portal_domain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **portal_id** | **String** |  |  |
| **business_domain_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## count_portals_async

> <Int32Envelope> count_portals_async(tenant_id, opts)

Count portals

Counts all portals for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count portals
  result = api_instance.count_portals_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->count_portals_async: #{e}"
end
```

#### Using the count_portals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_portals_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count portals
  data, status_code, headers = api_instance.count_portals_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->count_portals_async_with_http_info: #{e}"
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


## create_web_portal_async

> <EmptyEnvelope> create_web_portal_async(tenant_id, opts)

Create a new web portal

Create a new web portal

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_portal_create_dto: OpenapiClient::WebPortalCreateDto.new # WebPortalCreateDto | 
}

begin
  # Create a new web portal
  result = api_instance.create_web_portal_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->create_web_portal_async: #{e}"
end
```

#### Using the create_web_portal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_web_portal_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new web portal
  data, status_code, headers = api_instance.create_web_portal_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->create_web_portal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## delete_web_portal_async

> <EmptyEnvelope> delete_web_portal_async(tenant_id, portal_id, opts)

Delete a web portal

Delete a web portal

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a web portal
  result = api_instance.delete_web_portal_async(tenant_id, portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->delete_web_portal_async: #{e}"
end
```

#### Using the delete_web_portal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_web_portal_async_with_http_info(tenant_id, portal_id, opts)

```ruby
begin
  # Delete a web portal
  data, status_code, headers = api_instance.delete_web_portal_async_with_http_info(tenant_id, portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->delete_web_portal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_current_web_portal_async

> <WebPortalDtoEnvelope> get_current_web_portal_async(opts)

Get the current portal

Get the current portal of the this server instance

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the current portal
  result = api_instance.get_current_web_portal_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_current_web_portal_async: #{e}"
end
```

#### Using the get_current_web_portal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPortalDtoEnvelope>, Integer, Hash)> get_current_web_portal_async_with_http_info(opts)

```ruby
begin
  # Get the current portal
  data, status_code, headers = api_instance.get_current_web_portal_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPortalDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_current_web_portal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_current_web_portal_options_async

> <PortalOptionsEnvelope> get_current_web_portal_options_async(opts)

Get the current portal's options

Get the current portal's options for the current user.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the current portal's options
  result = api_instance.get_current_web_portal_options_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_current_web_portal_options_async: #{e}"
end
```

#### Using the get_current_web_portal_options_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PortalOptionsEnvelope>, Integer, Hash)> get_current_web_portal_options_async_with_http_info(opts)

```ruby
begin
  # Get the current portal's options
  data, status_code, headers = api_instance.get_current_web_portal_options_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PortalOptionsEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_current_web_portal_options_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PortalOptionsEnvelope**](PortalOptionsEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_portals_async

> <WebPortalDtoListEnvelope> get_portals_async(tenant_id, opts)

Get portals

Retrieves all portals for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get portals
  result = api_instance.get_portals_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_portals_async: #{e}"
end
```

#### Using the get_portals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPortalDtoListEnvelope>, Integer, Hash)> get_portals_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get portals
  data, status_code, headers = api_instance.get_portals_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPortalDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_portals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPortalDtoListEnvelope**](WebPortalDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_root_web_portal_async

> <WebPortalDtoEnvelope> get_root_web_portal_async(opts)

Get the root portal

Get the root portal of the this server instance

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the root portal
  result = api_instance.get_root_web_portal_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_root_web_portal_async: #{e}"
end
```

#### Using the get_root_web_portal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPortalDtoEnvelope>, Integer, Hash)> get_root_web_portal_async_with_http_info(opts)

```ruby
begin
  # Get the root portal
  data, status_code, headers = api_instance.get_root_web_portal_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPortalDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_root_web_portal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_portal_by_id_async

> <WebPortalDtoEnvelope> get_web_portal_by_id_async(portal_id, opts)

Get a web portal by its ID

Get a web portal by its ID

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
  # Get a web portal by its ID
  result = api_instance.get_web_portal_by_id_async(portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_web_portal_by_id_async: #{e}"
end
```

#### Using the get_web_portal_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPortalDtoEnvelope>, Integer, Hash)> get_web_portal_by_id_async_with_http_info(portal_id, opts)

```ruby
begin
  # Get a web portal by its ID
  data, status_code, headers = api_instance.get_web_portal_by_id_async_with_http_info(portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPortalDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_web_portal_by_id_async_with_http_info: #{e}"
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


## get_web_portal_domain_bindings_async

> <BusinessDomainDtoListEnvelope> get_web_portal_domain_bindings_async(tenant_id, portal_id, opts)

Get a web portal's bound domains

Get the BusinessDomains bound to a web portal

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a web portal's bound domains
  result = api_instance.get_web_portal_domain_bindings_async(tenant_id, portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_web_portal_domain_bindings_async: #{e}"
end
```

#### Using the get_web_portal_domain_bindings_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessDomainDtoListEnvelope>, Integer, Hash)> get_web_portal_domain_bindings_async_with_http_info(tenant_id, portal_id, opts)

```ruby
begin
  # Get a web portal's bound domains
  data, status_code, headers = api_instance.get_web_portal_domain_bindings_async_with_http_info(tenant_id, portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessDomainDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_web_portal_domain_bindings_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **portal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BusinessDomainDtoListEnvelope**](BusinessDomainDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_portal_options_async

> <PortalOptionsEnvelope> get_web_portal_options_async(portal_id, opts)

Get a web portal's options by its ID

Get a web portal's options by its ID

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
  # Get a web portal's options by its ID
  result = api_instance.get_web_portal_options_async(portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_web_portal_options_async: #{e}"
end
```

#### Using the get_web_portal_options_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PortalOptionsEnvelope>, Integer, Hash)> get_web_portal_options_async_with_http_info(portal_id, opts)

```ruby
begin
  # Get a web portal's options by its ID
  data, status_code, headers = api_instance.get_web_portal_options_async_with_http_info(portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PortalOptionsEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_web_portal_options_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **portal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PortalOptionsEnvelope**](PortalOptionsEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_web_portal_settings_async

> <PortalSettingsEnvelope> get_web_portal_settings_async(portal_id, opts)

Get a web portal's settings by its ID

Get a web portal's settings by its ID

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
  # Get a web portal's settings by its ID
  result = api_instance.get_web_portal_settings_async(portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_web_portal_settings_async: #{e}"
end
```

#### Using the get_web_portal_settings_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PortalSettingsEnvelope>, Integer, Hash)> get_web_portal_settings_async_with_http_info(portal_id, opts)

```ruby
begin
  # Get a web portal's settings by its ID
  data, status_code, headers = api_instance.get_web_portal_settings_async_with_http_info(portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PortalSettingsEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->get_web_portal_settings_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **portal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PortalSettingsEnvelope**](PortalSettingsEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## initialize_current_web_portal_async

> <WebPortalDtoEnvelope> initialize_current_web_portal_async(opts)

Initialize the current portal

Initialize the current portal for the current user.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Initialize the current portal
  result = api_instance.initialize_current_web_portal_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->initialize_current_web_portal_async: #{e}"
end
```

#### Using the initialize_current_web_portal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPortalDtoEnvelope>, Integer, Hash)> initialize_current_web_portal_async_with_http_info(opts)

```ruby
begin
  # Initialize the current portal
  data, status_code, headers = api_instance.initialize_current_web_portal_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPortalDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->initialize_current_web_portal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_web_portal_async

> <EmptyEnvelope> patch_web_portal_async(tenant_id, portal_id, opts)

Partially update a web portal

Partially update a web portal

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Partially update a web portal
  result = api_instance.patch_web_portal_async(tenant_id, portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->patch_web_portal_async: #{e}"
end
```

#### Using the patch_web_portal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_web_portal_async_with_http_info(tenant_id, portal_id, opts)

```ruby
begin
  # Partially update a web portal
  data, status_code, headers = api_instance.patch_web_portal_async_with_http_info(tenant_id, portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->patch_web_portal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **portal_id** | **String** |  |  |
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


## search_web_portal_async

> <WebPortalDtoEnvelope> search_web_portal_async(domain, opts)

Search for a portal by its domain

Search for a portal by its domain

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
domain = 'domain_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Search for a portal by its domain
  result = api_instance.search_web_portal_async(domain, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->search_web_portal_async: #{e}"
end
```

#### Using the search_web_portal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPortalDtoEnvelope>, Integer, Hash)> search_web_portal_async_with_http_info(domain, opts)

```ruby
begin
  # Search for a portal by its domain
  data, status_code, headers = api_instance.search_web_portal_async_with_http_info(domain, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPortalDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->search_web_portal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **domain** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## unbind_web_portal_domain_async

> <EmptyEnvelope> unbind_web_portal_domain_async(tenant_id, portal_id, business_domain_id, opts)

Unbind a domain from a web portal

Unbind a BusinessDomain from a web portal

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
business_domain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Unbind a domain from a web portal
  result = api_instance.unbind_web_portal_domain_async(tenant_id, portal_id, business_domain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->unbind_web_portal_domain_async: #{e}"
end
```

#### Using the unbind_web_portal_domain_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> unbind_web_portal_domain_async_with_http_info(tenant_id, portal_id, business_domain_id, opts)

```ruby
begin
  # Unbind a domain from a web portal
  data, status_code, headers = api_instance.unbind_web_portal_domain_async_with_http_info(tenant_id, portal_id, business_domain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->unbind_web_portal_domain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **portal_id** | **String** |  |  |
| **business_domain_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_web_portal_async

> <EmptyEnvelope> update_web_portal_async(tenant_id, portal_id, opts)

Update an existing web portal

Update an existing web portal

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  web_portal_update_dto: OpenapiClient::WebPortalUpdateDto.new # WebPortalUpdateDto | 
}

begin
  # Update an existing web portal
  result = api_instance.update_web_portal_async(tenant_id, portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->update_web_portal_async: #{e}"
end
```

#### Using the update_web_portal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_web_portal_async_with_http_info(tenant_id, portal_id, opts)

```ruby
begin
  # Update an existing web portal
  data, status_code, headers = api_instance.update_web_portal_async_with_http_info(tenant_id, portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->update_web_portal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## update_web_portal_settings_async

> <EmptyEnvelope> update_web_portal_settings_async(tenant_id, portal_id, opts)

Update a web portal's settings

Update a web portal's settings (Options) by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PortalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
portal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  portal_settings: OpenapiClient::PortalSettings.new # PortalSettings | 
}

begin
  # Update a web portal's settings
  result = api_instance.update_web_portal_settings_async(tenant_id, portal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->update_web_portal_settings_async: #{e}"
end
```

#### Using the update_web_portal_settings_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_web_portal_settings_async_with_http_info(tenant_id, portal_id, opts)

```ruby
begin
  # Update a web portal's settings
  data, status_code, headers = api_instance.update_web_portal_settings_async_with_http_info(tenant_id, portal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PortalsApi->update_web_portal_settings_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **portal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **portal_settings** | [**PortalSettings**](PortalSettings.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

