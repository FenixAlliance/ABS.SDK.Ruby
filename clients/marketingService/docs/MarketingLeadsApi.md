# OpenapiClient::MarketingLeadsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_marketing_lead_async**](MarketingLeadsApi.md#create_marketing_lead_async) | **POST** /api/v2/MarketingService/MarketingLeads | Create a marketing lead |
| [**delete_marketing_lead_async**](MarketingLeadsApi.md#delete_marketing_lead_async) | **DELETE** /api/v2/MarketingService/MarketingLeads/{marketingLeadId} | Delete a marketing lead |
| [**get_marketing_lead_details_async**](MarketingLeadsApi.md#get_marketing_lead_details_async) | **GET** /api/v2/MarketingService/MarketingLeads/{marketingLeadId} | Get marketing lead by ID |
| [**get_marketing_leads_count_async**](MarketingLeadsApi.md#get_marketing_leads_count_async) | **GET** /api/v2/MarketingService/MarketingLeads/Count | Get marketing leads count |
| [**get_marketing_leads_o_data_async**](MarketingLeadsApi.md#get_marketing_leads_o_data_async) | **GET** /api/v2/MarketingService/MarketingLeads | Get marketing leads |
| [**update_marketing_lead_async**](MarketingLeadsApi.md#update_marketing_lead_async) | **PUT** /api/v2/MarketingService/MarketingLeads/{marketingLeadId} | Update a marketing lead |


## create_marketing_lead_async

> <EmptyEnvelope> create_marketing_lead_async(tenant_id, marketing_lead_create_dto, opts)

Create a marketing lead

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingLeadsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_lead_create_dto = OpenapiClient::MarketingLeadCreateDto.new # MarketingLeadCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a marketing lead
  result = api_instance.create_marketing_lead_async(tenant_id, marketing_lead_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->create_marketing_lead_async: #{e}"
end
```

#### Using the create_marketing_lead_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_marketing_lead_async_with_http_info(tenant_id, marketing_lead_create_dto, opts)

```ruby
begin
  # Create a marketing lead
  data, status_code, headers = api_instance.create_marketing_lead_async_with_http_info(tenant_id, marketing_lead_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->create_marketing_lead_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketing_lead_create_dto** | [**MarketingLeadCreateDto**](MarketingLeadCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_marketing_lead_async

> <EmptyEnvelope> delete_marketing_lead_async(tenant_id, marketing_lead_id, opts)

Delete a marketing lead

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingLeadsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_lead_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a marketing lead
  result = api_instance.delete_marketing_lead_async(tenant_id, marketing_lead_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->delete_marketing_lead_async: #{e}"
end
```

#### Using the delete_marketing_lead_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_marketing_lead_async_with_http_info(tenant_id, marketing_lead_id, opts)

```ruby
begin
  # Delete a marketing lead
  data, status_code, headers = api_instance.delete_marketing_lead_async_with_http_info(tenant_id, marketing_lead_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->delete_marketing_lead_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketing_lead_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_lead_details_async

> <MarketingLeadDtoEnvelope> get_marketing_lead_details_async(tenant_id, marketing_lead_id, opts)

Get marketing lead by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingLeadsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_lead_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing lead by ID
  result = api_instance.get_marketing_lead_details_async(tenant_id, marketing_lead_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->get_marketing_lead_details_async: #{e}"
end
```

#### Using the get_marketing_lead_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MarketingLeadDtoEnvelope>, Integer, Hash)> get_marketing_lead_details_async_with_http_info(tenant_id, marketing_lead_id, opts)

```ruby
begin
  # Get marketing lead by ID
  data, status_code, headers = api_instance.get_marketing_lead_details_async_with_http_info(tenant_id, marketing_lead_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MarketingLeadDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->get_marketing_lead_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketing_lead_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MarketingLeadDtoEnvelope**](MarketingLeadDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_leads_count_async

> <Int32Envelope> get_marketing_leads_count_async(tenant_id, opts)

Get marketing leads count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingLeadsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing leads count
  result = api_instance.get_marketing_leads_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->get_marketing_leads_count_async: #{e}"
end
```

#### Using the get_marketing_leads_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_marketing_leads_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get marketing leads count
  data, status_code, headers = api_instance.get_marketing_leads_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->get_marketing_leads_count_async_with_http_info: #{e}"
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


## get_marketing_leads_o_data_async

> <MarketingLeadDtoListEnvelope> get_marketing_leads_o_data_async(tenant_id, opts)

Get marketing leads

Retrieves a collection of marketing leads for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingLeadsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing leads
  result = api_instance.get_marketing_leads_o_data_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->get_marketing_leads_o_data_async: #{e}"
end
```

#### Using the get_marketing_leads_o_data_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MarketingLeadDtoListEnvelope>, Integer, Hash)> get_marketing_leads_o_data_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get marketing leads
  data, status_code, headers = api_instance.get_marketing_leads_o_data_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MarketingLeadDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->get_marketing_leads_o_data_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MarketingLeadDtoListEnvelope**](MarketingLeadDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_marketing_lead_async

> <EmptyEnvelope> update_marketing_lead_async(tenant_id, marketing_lead_id, marketing_lead_update_dto, opts)

Update a marketing lead

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingLeadsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_lead_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_lead_update_dto = OpenapiClient::MarketingLeadUpdateDto.new # MarketingLeadUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a marketing lead
  result = api_instance.update_marketing_lead_async(tenant_id, marketing_lead_id, marketing_lead_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->update_marketing_lead_async: #{e}"
end
```

#### Using the update_marketing_lead_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_marketing_lead_async_with_http_info(tenant_id, marketing_lead_id, marketing_lead_update_dto, opts)

```ruby
begin
  # Update a marketing lead
  data, status_code, headers = api_instance.update_marketing_lead_async_with_http_info(tenant_id, marketing_lead_id, marketing_lead_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingLeadsApi->update_marketing_lead_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketing_lead_id** | **String** |  |  |
| **marketing_lead_update_dto** | [**MarketingLeadUpdateDto**](MarketingLeadUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

