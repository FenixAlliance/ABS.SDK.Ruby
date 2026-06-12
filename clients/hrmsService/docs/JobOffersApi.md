# OpenapiClient::JobOffersApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_job_offer_async**](JobOffersApi.md#create_job_offer_async) | **POST** /api/v2/HrmsService/JobOffers | Create a job offer |
| [**delete_job_offer_async**](JobOffersApi.md#delete_job_offer_async) | **DELETE** /api/v2/HrmsService/JobOffers/{jobOfferId} | Delete a job offer |
| [**get_job_offer_by_id_async**](JobOffersApi.md#get_job_offer_by_id_async) | **GET** /api/v2/HrmsService/JobOffers/{jobOfferId} | Get job offer by ID |
| [**get_job_offers_async**](JobOffersApi.md#get_job_offers_async) | **GET** /api/v2/HrmsService/JobOffers | Get job offers |
| [**get_job_offers_count_async**](JobOffersApi.md#get_job_offers_count_async) | **GET** /api/v2/HrmsService/JobOffers/Count | Count job offers |
| [**patch_job_offer_async**](JobOffersApi.md#patch_job_offer_async) | **PATCH** /api/v2/HrmsService/JobOffers/{jobOfferId} | Patch a job offer |
| [**update_job_offer_async**](JobOffersApi.md#update_job_offer_async) | **PUT** /api/v2/HrmsService/JobOffers/{jobOfferId} | Update a job offer |


## create_job_offer_async

> <EmptyEnvelope> create_job_offer_async(tenant_id, opts)

Create a job offer

Creates a new job offer for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOffersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_offer_create_dto: OpenapiClient::JobOfferCreateDto.new # JobOfferCreateDto | 
}

begin
  # Create a job offer
  result = api_instance.create_job_offer_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->create_job_offer_async: #{e}"
end
```

#### Using the create_job_offer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_job_offer_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a job offer
  data, status_code, headers = api_instance.create_job_offer_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->create_job_offer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_offer_create_dto** | [**JobOfferCreateDto**](JobOfferCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_job_offer_async

> <EmptyEnvelope> delete_job_offer_async(tenant_id, job_offer_id, opts)

Delete a job offer

Deletes a job offer for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOffersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_offer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a job offer
  result = api_instance.delete_job_offer_async(tenant_id, job_offer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->delete_job_offer_async: #{e}"
end
```

#### Using the delete_job_offer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_job_offer_async_with_http_info(tenant_id, job_offer_id, opts)

```ruby
begin
  # Delete a job offer
  data, status_code, headers = api_instance.delete_job_offer_async_with_http_info(tenant_id, job_offer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->delete_job_offer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_offer_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_offer_by_id_async

> <JobOfferDtoEnvelope> get_job_offer_by_id_async(tenant_id, job_offer_id, opts)

Get job offer by ID

Retrieves a specific job offer by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOffersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_offer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get job offer by ID
  result = api_instance.get_job_offer_by_id_async(tenant_id, job_offer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->get_job_offer_by_id_async: #{e}"
end
```

#### Using the get_job_offer_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobOfferDtoEnvelope>, Integer, Hash)> get_job_offer_by_id_async_with_http_info(tenant_id, job_offer_id, opts)

```ruby
begin
  # Get job offer by ID
  data, status_code, headers = api_instance.get_job_offer_by_id_async_with_http_info(tenant_id, job_offer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobOfferDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->get_job_offer_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_offer_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JobOfferDtoEnvelope**](JobOfferDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_offers_async

> <JobOfferDtoListEnvelope> get_job_offers_async(tenant_id, opts)

Get job offers

Retrieves job offers for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOffersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get job offers
  result = api_instance.get_job_offers_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->get_job_offers_async: #{e}"
end
```

#### Using the get_job_offers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobOfferDtoListEnvelope>, Integer, Hash)> get_job_offers_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get job offers
  data, status_code, headers = api_instance.get_job_offers_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobOfferDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->get_job_offers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JobOfferDtoListEnvelope**](JobOfferDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_job_offers_count_async

> <Int32Envelope> get_job_offers_count_async(tenant_id, opts)

Count job offers

Counts job offers for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOffersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count job offers
  result = api_instance.get_job_offers_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->get_job_offers_count_async: #{e}"
end
```

#### Using the get_job_offers_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_job_offers_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count job offers
  data, status_code, headers = api_instance.get_job_offers_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->get_job_offers_count_async_with_http_info: #{e}"
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


## patch_job_offer_async

> <EmptyEnvelope> patch_job_offer_async(tenant_id, job_offer_id, opts)

Patch a job offer

Partially updates an existing job offer for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOffersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_offer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a job offer
  result = api_instance.patch_job_offer_async(tenant_id, job_offer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->patch_job_offer_async: #{e}"
end
```

#### Using the patch_job_offer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_job_offer_async_with_http_info(tenant_id, job_offer_id, opts)

```ruby
begin
  # Patch a job offer
  data, status_code, headers = api_instance.patch_job_offer_async_with_http_info(tenant_id, job_offer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->patch_job_offer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_offer_id** | **String** |  |  |
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


## update_job_offer_async

> <EmptyEnvelope> update_job_offer_async(tenant_id, job_offer_id, opts)

Update a job offer

Updates an existing job offer for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::JobOffersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
job_offer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  job_offer_update_dto: OpenapiClient::JobOfferUpdateDto.new # JobOfferUpdateDto | 
}

begin
  # Update a job offer
  result = api_instance.update_job_offer_async(tenant_id, job_offer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->update_job_offer_async: #{e}"
end
```

#### Using the update_job_offer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_job_offer_async_with_http_info(tenant_id, job_offer_id, opts)

```ruby
begin
  # Update a job offer
  data, status_code, headers = api_instance.update_job_offer_async_with_http_info(tenant_id, job_offer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling JobOffersApi->update_job_offer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **job_offer_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **job_offer_update_dto** | [**JobOfferUpdateDto**](JobOfferUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

