# OpenapiClient::ServiceLevelAgreementsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_service_level_agreement_async**](ServiceLevelAgreementsApi.md#create_service_level_agreement_async) | **POST** /api/v2/ServicesService/ServiceLevelAgreements | Create a service level agreement |
| [**delete_service_level_agreement_async**](ServiceLevelAgreementsApi.md#delete_service_level_agreement_async) | **DELETE** /api/v2/ServicesService/ServiceLevelAgreements/{serviceLevelAgreementId} | Delete a service level agreement |
| [**get_service_level_agreement_by_id_async**](ServiceLevelAgreementsApi.md#get_service_level_agreement_by_id_async) | **GET** /api/v2/ServicesService/ServiceLevelAgreements/{serviceLevelAgreementId} | Get a service level agreement by ID |
| [**get_service_level_agreements_async**](ServiceLevelAgreementsApi.md#get_service_level_agreements_async) | **GET** /api/v2/ServicesService/ServiceLevelAgreements | Get all service level agreements |
| [**get_service_level_agreements_count_async**](ServiceLevelAgreementsApi.md#get_service_level_agreements_count_async) | **GET** /api/v2/ServicesService/ServiceLevelAgreements/Count | Get service level agreements count |
| [**update_service_level_agreement_async**](ServiceLevelAgreementsApi.md#update_service_level_agreement_async) | **PUT** /api/v2/ServicesService/ServiceLevelAgreements/{serviceLevelAgreementId} | Update a service level agreement |


## create_service_level_agreement_async

> <Envelope> create_service_level_agreement_async(tenant_id, opts)

Create a service level agreement

Creates a new service level agreement for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelAgreementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_level_agreement_create_dto: OpenapiClient::ServiceLevelAgreementCreateDto.new # ServiceLevelAgreementCreateDto | 
}

begin
  # Create a service level agreement
  result = api_instance.create_service_level_agreement_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->create_service_level_agreement_async: #{e}"
end
```

#### Using the create_service_level_agreement_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> create_service_level_agreement_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a service level agreement
  data, status_code, headers = api_instance.create_service_level_agreement_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->create_service_level_agreement_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_level_agreement_create_dto** | [**ServiceLevelAgreementCreateDto**](ServiceLevelAgreementCreateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_service_level_agreement_async

> <Envelope> delete_service_level_agreement_async(tenant_id, service_level_agreement_id, opts)

Delete a service level agreement

Deletes a service level agreement by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelAgreementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_level_agreement_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a service level agreement
  result = api_instance.delete_service_level_agreement_async(tenant_id, service_level_agreement_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->delete_service_level_agreement_async: #{e}"
end
```

#### Using the delete_service_level_agreement_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> delete_service_level_agreement_async_with_http_info(tenant_id, service_level_agreement_id, opts)

```ruby
begin
  # Delete a service level agreement
  data, status_code, headers = api_instance.delete_service_level_agreement_async_with_http_info(tenant_id, service_level_agreement_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->delete_service_level_agreement_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_level_agreement_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_level_agreement_by_id_async

> <ServiceLevelAgreementDtoEnvelope> get_service_level_agreement_by_id_async(tenant_id, service_level_agreement_id, opts)

Get a service level agreement by ID

Retrieves a service level agreement by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelAgreementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_level_agreement_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a service level agreement by ID
  result = api_instance.get_service_level_agreement_by_id_async(tenant_id, service_level_agreement_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->get_service_level_agreement_by_id_async: #{e}"
end
```

#### Using the get_service_level_agreement_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceLevelAgreementDtoEnvelope>, Integer, Hash)> get_service_level_agreement_by_id_async_with_http_info(tenant_id, service_level_agreement_id, opts)

```ruby
begin
  # Get a service level agreement by ID
  data, status_code, headers = api_instance.get_service_level_agreement_by_id_async_with_http_info(tenant_id, service_level_agreement_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceLevelAgreementDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->get_service_level_agreement_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_level_agreement_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceLevelAgreementDtoEnvelope**](ServiceLevelAgreementDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_level_agreements_async

> <ServiceLevelAgreementDtoIReadOnlyListEnvelope> get_service_level_agreements_async(tenant_id, opts)

Get all service level agreements

Retrieves all service level agreements for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelAgreementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all service level agreements
  result = api_instance.get_service_level_agreements_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->get_service_level_agreements_async: #{e}"
end
```

#### Using the get_service_level_agreements_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ServiceLevelAgreementDtoIReadOnlyListEnvelope>, Integer, Hash)> get_service_level_agreements_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all service level agreements
  data, status_code, headers = api_instance.get_service_level_agreements_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ServiceLevelAgreementDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->get_service_level_agreements_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ServiceLevelAgreementDtoIReadOnlyListEnvelope**](ServiceLevelAgreementDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_service_level_agreements_count_async

> <Int32Envelope> get_service_level_agreements_count_async(tenant_id, opts)

Get service level agreements count

Returns the count of service level agreements for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelAgreementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get service level agreements count
  result = api_instance.get_service_level_agreements_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->get_service_level_agreements_count_async: #{e}"
end
```

#### Using the get_service_level_agreements_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_service_level_agreements_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get service level agreements count
  data, status_code, headers = api_instance.get_service_level_agreements_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->get_service_level_agreements_count_async_with_http_info: #{e}"
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


## update_service_level_agreement_async

> <Envelope> update_service_level_agreement_async(tenant_id, service_level_agreement_id, opts)

Update a service level agreement

Updates an existing service level agreement.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ServiceLevelAgreementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
service_level_agreement_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  service_level_agreement_update_dto: OpenapiClient::ServiceLevelAgreementUpdateDto.new # ServiceLevelAgreementUpdateDto | 
}

begin
  # Update a service level agreement
  result = api_instance.update_service_level_agreement_async(tenant_id, service_level_agreement_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->update_service_level_agreement_async: #{e}"
end
```

#### Using the update_service_level_agreement_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> update_service_level_agreement_async_with_http_info(tenant_id, service_level_agreement_id, opts)

```ruby
begin
  # Update a service level agreement
  data, status_code, headers = api_instance.update_service_level_agreement_async_with_http_info(tenant_id, service_level_agreement_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ServiceLevelAgreementsApi->update_service_level_agreement_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **service_level_agreement_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **service_level_agreement_update_dto** | [**ServiceLevelAgreementUpdateDto**](ServiceLevelAgreementUpdateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

