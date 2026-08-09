# OpenapiClient::BillingProfilesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_billing_profile_async**](BillingProfilesApi.md#create_billing_profile_async) | **POST** /api/v2/AccountingService/BillingProfiles | Creates a new billing profile |
| [**delete_billing_profile_async**](BillingProfilesApi.md#delete_billing_profile_async) | **DELETE** /api/v2/AccountingService/BillingProfiles/{billingProfileId} | Deletes a billing profile |
| [**get_billing_profile_by_id_async**](BillingProfilesApi.md#get_billing_profile_by_id_async) | **GET** /api/v2/AccountingService/BillingProfiles/{billingProfileId} | Gets a billing profile by id |
| [**get_billing_profiles_async**](BillingProfilesApi.md#get_billing_profiles_async) | **GET** /api/v2/AccountingService/BillingProfiles | Gets all billing profiles |
| [**get_billing_profiles_count_async**](BillingProfilesApi.md#get_billing_profiles_count_async) | **GET** /api/v2/AccountingService/BillingProfiles/Count | Gets the count of billing profiles |
| [**patch_billing_profile_async**](BillingProfilesApi.md#patch_billing_profile_async) | **PATCH** /api/v2/AccountingService/BillingProfiles/{billingProfileId} | Patch a billing profile |
| [**update_billing_profile_async**](BillingProfilesApi.md#update_billing_profile_async) | **PUT** /api/v2/AccountingService/BillingProfiles/{billingProfileId} | Updates an existing billing profile |


## create_billing_profile_async

> <EmptyEnvelope> create_billing_profile_async(tenant_id, billing_profile_create_dto, opts)

Creates a new billing profile

Adds a new billing profile record for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillingProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billing_profile_create_dto = OpenapiClient::BillingProfileCreateDto.new({tax_id: 'tax_id_example', phone: 'phone_example', email: 'email_example', address: 'address_example', postal_code: 'postal_code_example', business_name: 'business_name_example', commercial_name: 'commercial_name_example', country_id: 'country_id_example', state_id: 'state_id_example', city_id: 'city_id_example', fiscal_identification_type_id: 'fiscal_identification_type_id_example', fiscal_authority_id: 'fiscal_authority_id_example', fiscal_regime_id: 'fiscal_regime_id_example'}) # BillingProfileCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Creates a new billing profile
  result = api_instance.create_billing_profile_async(tenant_id, billing_profile_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->create_billing_profile_async: #{e}"
end
```

#### Using the create_billing_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_billing_profile_async_with_http_info(tenant_id, billing_profile_create_dto, opts)

```ruby
begin
  # Creates a new billing profile
  data, status_code, headers = api_instance.create_billing_profile_async_with_http_info(tenant_id, billing_profile_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->create_billing_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billing_profile_create_dto** | [**BillingProfileCreateDto**](BillingProfileCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_billing_profile_async

> <EmptyEnvelope> delete_billing_profile_async(tenant_id, billing_profile_id, opts)

Deletes a billing profile

Removes a billing profile from the system using its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillingProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billing_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a billing profile
  result = api_instance.delete_billing_profile_async(tenant_id, billing_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->delete_billing_profile_async: #{e}"
end
```

#### Using the delete_billing_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_billing_profile_async_with_http_info(tenant_id, billing_profile_id, opts)

```ruby
begin
  # Deletes a billing profile
  data, status_code, headers = api_instance.delete_billing_profile_async_with_http_info(tenant_id, billing_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->delete_billing_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billing_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_billing_profile_by_id_async

> <BillingProfileDtoEnvelope> get_billing_profile_by_id_async(tenant_id, billing_profile_id, opts)

Gets a billing profile by id

Retrieves a specific billing profile using its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillingProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billing_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a billing profile by id
  result = api_instance.get_billing_profile_by_id_async(tenant_id, billing_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->get_billing_profile_by_id_async: #{e}"
end
```

#### Using the get_billing_profile_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BillingProfileDtoEnvelope>, Integer, Hash)> get_billing_profile_by_id_async_with_http_info(tenant_id, billing_profile_id, opts)

```ruby
begin
  # Gets a billing profile by id
  data, status_code, headers = api_instance.get_billing_profile_by_id_async_with_http_info(tenant_id, billing_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BillingProfileDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->get_billing_profile_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billing_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BillingProfileDtoEnvelope**](BillingProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_billing_profiles_async

> <BillingProfileDtoIReadOnlyListEnvelope> get_billing_profiles_async(tenant_id, opts)

Gets all billing profiles

Fetches all billing profiles for a tenant with support for OData queries.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillingProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  billing_profile_dto_collection_query_parameters: OpenapiClient::BillingProfileDtoCollectionQueryParameters.new # BillingProfileDtoCollectionQueryParameters | 
}

begin
  # Gets all billing profiles
  result = api_instance.get_billing_profiles_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->get_billing_profiles_async: #{e}"
end
```

#### Using the get_billing_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BillingProfileDtoIReadOnlyListEnvelope>, Integer, Hash)> get_billing_profiles_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets all billing profiles
  data, status_code, headers = api_instance.get_billing_profiles_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BillingProfileDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->get_billing_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **billing_profile_dto_collection_query_parameters** | [**BillingProfileDtoCollectionQueryParameters**](BillingProfileDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BillingProfileDtoIReadOnlyListEnvelope**](BillingProfileDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_billing_profiles_count_async

> <Int32Envelope> get_billing_profiles_count_async(tenant_id, opts)

Gets the count of billing profiles

Returns the number of billing profiles for a tenant, supporting OData filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillingProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  billing_profile_dto_collection_query_parameters: OpenapiClient::BillingProfileDtoCollectionQueryParameters.new # BillingProfileDtoCollectionQueryParameters | 
}

begin
  # Gets the count of billing profiles
  result = api_instance.get_billing_profiles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->get_billing_profiles_count_async: #{e}"
end
```

#### Using the get_billing_profiles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_billing_profiles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the count of billing profiles
  data, status_code, headers = api_instance.get_billing_profiles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->get_billing_profiles_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **billing_profile_dto_collection_query_parameters** | [**BillingProfileDtoCollectionQueryParameters**](BillingProfileDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_billing_profile_async

> <EmptyEnvelope> patch_billing_profile_async(tenant_id, billing_profile_id, opts)

Patch a billing profile

Partially updates a billing profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillingProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billing_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a billing profile
  result = api_instance.patch_billing_profile_async(tenant_id, billing_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->patch_billing_profile_async: #{e}"
end
```

#### Using the patch_billing_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_billing_profile_async_with_http_info(tenant_id, billing_profile_id, opts)

```ruby
begin
  # Patch a billing profile
  data, status_code, headers = api_instance.patch_billing_profile_async_with_http_info(tenant_id, billing_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->patch_billing_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billing_profile_id** | **String** |  |  |
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


## update_billing_profile_async

> <EmptyEnvelope> update_billing_profile_async(tenant_id, billing_profile_id, billing_profile_update_dto, opts)

Updates an existing billing profile

Modifies an existing billing profile using the provided data.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BillingProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billing_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
billing_profile_update_dto = OpenapiClient::BillingProfileUpdateDto.new # BillingProfileUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Updates an existing billing profile
  result = api_instance.update_billing_profile_async(tenant_id, billing_profile_id, billing_profile_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->update_billing_profile_async: #{e}"
end
```

#### Using the update_billing_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_billing_profile_async_with_http_info(tenant_id, billing_profile_id, billing_profile_update_dto, opts)

```ruby
begin
  # Updates an existing billing profile
  data, status_code, headers = api_instance.update_billing_profile_async_with_http_info(tenant_id, billing_profile_id, billing_profile_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BillingProfilesApi->update_billing_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **billing_profile_id** | **String** |  |  |
| **billing_profile_update_dto** | [**BillingProfileUpdateDto**](BillingProfileUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

