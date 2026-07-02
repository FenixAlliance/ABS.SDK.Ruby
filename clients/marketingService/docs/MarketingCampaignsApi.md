# OpenapiClient::MarketingCampaignsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_marketing_campaign_async**](MarketingCampaignsApi.md#create_marketing_campaign_async) | **POST** /api/v2/MarketingService/MarketingCampaigns | Create a marketing campaign |
| [**delete_marketing_campaign_async**](MarketingCampaignsApi.md#delete_marketing_campaign_async) | **DELETE** /api/v2/MarketingService/MarketingCampaigns/{marketingcampaignId} | Delete a marketing campaign |
| [**get_marketing_campaign_details_async**](MarketingCampaignsApi.md#get_marketing_campaign_details_async) | **GET** /api/v2/MarketingService/MarketingCampaigns/{marketingcampaignId} | Get marketing campaign by ID |
| [**get_marketing_campaign_o_data_async**](MarketingCampaignsApi.md#get_marketing_campaign_o_data_async) | **GET** /api/v2/MarketingService/MarketingCampaigns | Get marketing campaigns |
| [**get_marketing_campaigns_count_async**](MarketingCampaignsApi.md#get_marketing_campaigns_count_async) | **GET** /api/v2/MarketingService/MarketingCampaigns/Count | Get marketing campaigns count |
| [**patch_marketing_campaign_async**](MarketingCampaignsApi.md#patch_marketing_campaign_async) | **PATCH** /api/v2/MarketingService/MarketingCampaigns/{marketingcampaignId} | Patch a marketing campaign |
| [**update_marketing_campaign_async**](MarketingCampaignsApi.md#update_marketing_campaign_async) | **PUT** /api/v2/MarketingService/MarketingCampaigns/{marketingcampaignId} | Update a marketing campaign |


## create_marketing_campaign_async

> <EmptyEnvelope> create_marketing_campaign_async(tenant_id, marketing_campaign_create_dto, opts)

Create a marketing campaign

Creates a new marketing campaign for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingCampaignsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_campaign_create_dto = OpenapiClient::MarketingCampaignCreateDto.new # MarketingCampaignCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a marketing campaign
  result = api_instance.create_marketing_campaign_async(tenant_id, marketing_campaign_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->create_marketing_campaign_async: #{e}"
end
```

#### Using the create_marketing_campaign_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_marketing_campaign_async_with_http_info(tenant_id, marketing_campaign_create_dto, opts)

```ruby
begin
  # Create a marketing campaign
  data, status_code, headers = api_instance.create_marketing_campaign_async_with_http_info(tenant_id, marketing_campaign_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->create_marketing_campaign_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketing_campaign_create_dto** | [**MarketingCampaignCreateDto**](MarketingCampaignCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_marketing_campaign_async

> <EmptyEnvelope> delete_marketing_campaign_async(tenant_id, marketingcampaign_id, opts)

Delete a marketing campaign

Deletes a marketing campaign by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingCampaignsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketingcampaign_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a marketing campaign
  result = api_instance.delete_marketing_campaign_async(tenant_id, marketingcampaign_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->delete_marketing_campaign_async: #{e}"
end
```

#### Using the delete_marketing_campaign_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_marketing_campaign_async_with_http_info(tenant_id, marketingcampaign_id, opts)

```ruby
begin
  # Delete a marketing campaign
  data, status_code, headers = api_instance.delete_marketing_campaign_async_with_http_info(tenant_id, marketingcampaign_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->delete_marketing_campaign_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketingcampaign_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_campaign_details_async

> <MarketingCampaignDtoEnvelope> get_marketing_campaign_details_async(tenant_id, marketingcampaign_id, opts)

Get marketing campaign by ID

Retrieves the details of a specific marketing campaign by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingCampaignsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketingcampaign_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing campaign by ID
  result = api_instance.get_marketing_campaign_details_async(tenant_id, marketingcampaign_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->get_marketing_campaign_details_async: #{e}"
end
```

#### Using the get_marketing_campaign_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MarketingCampaignDtoEnvelope>, Integer, Hash)> get_marketing_campaign_details_async_with_http_info(tenant_id, marketingcampaign_id, opts)

```ruby
begin
  # Get marketing campaign by ID
  data, status_code, headers = api_instance.get_marketing_campaign_details_async_with_http_info(tenant_id, marketingcampaign_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MarketingCampaignDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->get_marketing_campaign_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketingcampaign_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MarketingCampaignDtoEnvelope**](MarketingCampaignDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_campaign_o_data_async

> get_marketing_campaign_o_data_async(tenant_id, opts)

Get marketing campaigns

Retrieves a collection of marketing campaigns for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingCampaignsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing campaigns
  api_instance.get_marketing_campaign_o_data_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->get_marketing_campaign_o_data_async: #{e}"
end
```

#### Using the get_marketing_campaign_o_data_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_marketing_campaign_o_data_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get marketing campaigns
  data, status_code, headers = api_instance.get_marketing_campaign_o_data_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->get_marketing_campaign_o_data_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_marketing_campaigns_count_async

> <Int32Envelope> get_marketing_campaigns_count_async(tenant_id, opts)

Get marketing campaigns count

Returns the count of marketing campaigns for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingCampaignsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get marketing campaigns count
  result = api_instance.get_marketing_campaigns_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->get_marketing_campaigns_count_async: #{e}"
end
```

#### Using the get_marketing_campaigns_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_marketing_campaigns_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get marketing campaigns count
  data, status_code, headers = api_instance.get_marketing_campaigns_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->get_marketing_campaigns_count_async_with_http_info: #{e}"
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


## patch_marketing_campaign_async

> <EmptyEnvelope> patch_marketing_campaign_async(tenant_id, marketingcampaign_id, opts)

Patch a marketing campaign

Partially updates a marketing campaign by its ID using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingCampaignsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketingcampaign_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a marketing campaign
  result = api_instance.patch_marketing_campaign_async(tenant_id, marketingcampaign_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->patch_marketing_campaign_async: #{e}"
end
```

#### Using the patch_marketing_campaign_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_marketing_campaign_async_with_http_info(tenant_id, marketingcampaign_id, opts)

```ruby
begin
  # Patch a marketing campaign
  data, status_code, headers = api_instance.patch_marketing_campaign_async_with_http_info(tenant_id, marketingcampaign_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->patch_marketing_campaign_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketingcampaign_id** | **String** |  |  |
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


## update_marketing_campaign_async

> <EmptyEnvelope> update_marketing_campaign_async(tenant_id, marketingcampaign_id, marketing_campaign_update_dto, opts)

Update a marketing campaign

Updates an existing marketing campaign by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarketingCampaignsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketingcampaign_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
marketing_campaign_update_dto = OpenapiClient::MarketingCampaignUpdateDto.new # MarketingCampaignUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a marketing campaign
  result = api_instance.update_marketing_campaign_async(tenant_id, marketingcampaign_id, marketing_campaign_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->update_marketing_campaign_async: #{e}"
end
```

#### Using the update_marketing_campaign_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_marketing_campaign_async_with_http_info(tenant_id, marketingcampaign_id, marketing_campaign_update_dto, opts)

```ruby
begin
  # Update a marketing campaign
  data, status_code, headers = api_instance.update_marketing_campaign_async_with_http_info(tenant_id, marketingcampaign_id, marketing_campaign_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarketingCampaignsApi->update_marketing_campaign_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **marketingcampaign_id** | **String** |  |  |
| **marketing_campaign_update_dto** | [**MarketingCampaignUpdateDto**](MarketingCampaignUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

