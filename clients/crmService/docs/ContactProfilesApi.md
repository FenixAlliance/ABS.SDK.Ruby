# OpenapiClient::ContactProfilesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_contact_profile_async**](ContactProfilesApi.md#create_contact_profile_async) | **POST** /api/v2/CrmService/ContactProfiles | Create a new contact profile |
| [**delete_contact_profile_async**](ContactProfilesApi.md#delete_contact_profile_async) | **DELETE** /api/v2/CrmService/ContactProfiles/{id} | Delete a contact profile |
| [**get_contact_profile_by_id_async**](ContactProfilesApi.md#get_contact_profile_by_id_async) | **GET** /api/v2/CrmService/ContactProfiles/{id} | Get contact profile by ID |
| [**get_contact_profiles_async**](ContactProfilesApi.md#get_contact_profiles_async) | **GET** /api/v2/CrmService/ContactProfiles | Get all contact profiles |
| [**get_contact_profiles_count_async**](ContactProfilesApi.md#get_contact_profiles_count_async) | **GET** /api/v2/CrmService/ContactProfiles/Count | Get contact profiles count |
| [**get_partner_profiles_count_async**](ContactProfilesApi.md#get_partner_profiles_count_async) | **GET** /api/v2/CrmService/ContactProfiles/Partners/Count | Get partner profiles count |
| [**get_patient_profiles_count_async**](ContactProfilesApi.md#get_patient_profiles_count_async) | **GET** /api/v2/CrmService/ContactProfiles/Patients/Count | Get patient profiles count |
| [**patch_contact_profile_async**](ContactProfilesApi.md#patch_contact_profile_async) | **PATCH** /api/v2/CrmService/ContactProfiles/{id} | Patch a contact profile |
| [**update_contact_profile_async**](ContactProfilesApi.md#update_contact_profile_async) | **PUT** /api/v2/CrmService/ContactProfiles/{id} | Update a contact profile |


## create_contact_profile_async

> create_contact_profile_async(tenant_id, opts)

Create a new contact profile

Creates a new contact profile for the specified tenant. The ContactId must be provided in the request body.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_profile_create_dto: OpenapiClient::ContactProfileCreateDto.new # ContactProfileCreateDto | 
}

begin
  # Create a new contact profile
  api_instance.create_contact_profile_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->create_contact_profile_async: #{e}"
end
```

#### Using the create_contact_profile_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_contact_profile_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new contact profile
  data, status_code, headers = api_instance.create_contact_profile_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->create_contact_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_profile_create_dto** | [**ContactProfileCreateDto**](ContactProfileCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_contact_profile_async

> delete_contact_profile_async(tenant_id, id, opts)

Delete a contact profile

Deletes a contact profile for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact profile
  api_instance.delete_contact_profile_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->delete_contact_profile_async: #{e}"
end
```

#### Using the delete_contact_profile_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_contact_profile_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a contact profile
  data, status_code, headers = api_instance.delete_contact_profile_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->delete_contact_profile_async_with_http_info: #{e}"
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


## get_contact_profile_by_id_async

> <ContactProfileDto> get_contact_profile_by_id_async(tenant_id, id, opts)

Get contact profile by ID

Retrieves a specific contact profile by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get contact profile by ID
  result = api_instance.get_contact_profile_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_contact_profile_by_id_async: #{e}"
end
```

#### Using the get_contact_profile_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactProfileDto>, Integer, Hash)> get_contact_profile_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get contact profile by ID
  data, status_code, headers = api_instance.get_contact_profile_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactProfileDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_contact_profile_by_id_async_with_http_info: #{e}"
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

[**ContactProfileDto**](ContactProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_profiles_async

> <ContactProfileDtoListEnvelope> get_contact_profiles_async(tenant_id, opts)

Get all contact profiles

Retrieves all contact profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all contact profiles
  result = api_instance.get_contact_profiles_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_contact_profiles_async: #{e}"
end
```

#### Using the get_contact_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactProfileDtoListEnvelope>, Integer, Hash)> get_contact_profiles_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contact profiles
  data, status_code, headers = api_instance.get_contact_profiles_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_contact_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactProfileDtoListEnvelope**](ContactProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_profiles_count_async

> <Int32Envelope> get_contact_profiles_count_async(tenant_id, opts)

Get contact profiles count

Returns the count of contact profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get contact profiles count
  result = api_instance.get_contact_profiles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_contact_profiles_count_async: #{e}"
end
```

#### Using the get_contact_profiles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_contact_profiles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get contact profiles count
  data, status_code, headers = api_instance.get_contact_profiles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_contact_profiles_count_async_with_http_info: #{e}"
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


## get_partner_profiles_count_async

> <Int32Envelope> get_partner_profiles_count_async(tenant_id, opts)

Get partner profiles count

Returns the count of partner contact profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get partner profiles count
  result = api_instance.get_partner_profiles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_partner_profiles_count_async: #{e}"
end
```

#### Using the get_partner_profiles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_partner_profiles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get partner profiles count
  data, status_code, headers = api_instance.get_partner_profiles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_partner_profiles_count_async_with_http_info: #{e}"
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


## get_patient_profiles_count_async

> <Int32Envelope> get_patient_profiles_count_async(tenant_id, opts)

Get patient profiles count

Returns the count of patient contact profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get patient profiles count
  result = api_instance.get_patient_profiles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_patient_profiles_count_async: #{e}"
end
```

#### Using the get_patient_profiles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_patient_profiles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get patient profiles count
  data, status_code, headers = api_instance.get_patient_profiles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->get_patient_profiles_count_async_with_http_info: #{e}"
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


## patch_contact_profile_async

> <EmptyEnvelope> patch_contact_profile_async(tenant_id, id, opts)

Patch a contact profile

Patch a contact profile

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a contact profile
  result = api_instance.patch_contact_profile_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->patch_contact_profile_async: #{e}"
end
```

#### Using the patch_contact_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_contact_profile_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a contact profile
  data, status_code, headers = api_instance.patch_contact_profile_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->patch_contact_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
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


## update_contact_profile_async

> update_contact_profile_async(tenant_id, id, opts)

Update a contact profile

Updates an existing contact profile for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_profile_update_dto: OpenapiClient::ContactProfileUpdateDto.new # ContactProfileUpdateDto | 
}

begin
  # Update a contact profile
  api_instance.update_contact_profile_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->update_contact_profile_async: #{e}"
end
```

#### Using the update_contact_profile_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_contact_profile_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a contact profile
  data, status_code, headers = api_instance.update_contact_profile_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactProfilesApi->update_contact_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_profile_update_dto** | [**ContactProfileUpdateDto**](ContactProfileUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

