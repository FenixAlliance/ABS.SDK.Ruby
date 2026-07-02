# OpenapiClient::RequiredSkillsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_required_skill_async**](RequiredSkillsApi.md#create_required_skill_async) | **POST** /api/v2/HrmsService/RequiredSkills | Create a required skill |
| [**delete_required_skill_async**](RequiredSkillsApi.md#delete_required_skill_async) | **DELETE** /api/v2/HrmsService/RequiredSkills/{requiredSkillId} | Delete a required skill |
| [**get_required_skill_by_id_async**](RequiredSkillsApi.md#get_required_skill_by_id_async) | **GET** /api/v2/HrmsService/RequiredSkills/{requiredSkillId} | Get required skill by ID |
| [**get_required_skills_async**](RequiredSkillsApi.md#get_required_skills_async) | **GET** /api/v2/HrmsService/RequiredSkills | Get required skills |
| [**get_required_skills_count_async**](RequiredSkillsApi.md#get_required_skills_count_async) | **GET** /api/v2/HrmsService/RequiredSkills/Count | Count required skills |
| [**patch_required_skill_async**](RequiredSkillsApi.md#patch_required_skill_async) | **PATCH** /api/v2/HrmsService/RequiredSkills/{requiredSkillId} | Patch a required skill |
| [**update_required_skill_async**](RequiredSkillsApi.md#update_required_skill_async) | **PUT** /api/v2/HrmsService/RequiredSkills/{requiredSkillId} | Update a required skill |


## create_required_skill_async

> <EmptyEnvelope> create_required_skill_async(tenant_id, opts)

Create a required skill

Creates a new required-skill record for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RequiredSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  required_skill_record_create_dto: OpenapiClient::RequiredSkillRecordCreateDto.new({skill_id: 'skill_id_example'}) # RequiredSkillRecordCreateDto | 
}

begin
  # Create a required skill
  result = api_instance.create_required_skill_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->create_required_skill_async: #{e}"
end
```

#### Using the create_required_skill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_required_skill_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a required skill
  data, status_code, headers = api_instance.create_required_skill_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->create_required_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **required_skill_record_create_dto** | [**RequiredSkillRecordCreateDto**](RequiredSkillRecordCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_required_skill_async

> <EmptyEnvelope> delete_required_skill_async(tenant_id, required_skill_id, opts)

Delete a required skill

Deletes a required-skill record for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RequiredSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
required_skill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a required skill
  result = api_instance.delete_required_skill_async(tenant_id, required_skill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->delete_required_skill_async: #{e}"
end
```

#### Using the delete_required_skill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_required_skill_async_with_http_info(tenant_id, required_skill_id, opts)

```ruby
begin
  # Delete a required skill
  data, status_code, headers = api_instance.delete_required_skill_async_with_http_info(tenant_id, required_skill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->delete_required_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **required_skill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_required_skill_by_id_async

> <RequiredSkillRecordDtoEnvelope> get_required_skill_by_id_async(tenant_id, required_skill_id, opts)

Get required skill by ID

Retrieves a specific required-skill record by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RequiredSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
required_skill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get required skill by ID
  result = api_instance.get_required_skill_by_id_async(tenant_id, required_skill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->get_required_skill_by_id_async: #{e}"
end
```

#### Using the get_required_skill_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RequiredSkillRecordDtoEnvelope>, Integer, Hash)> get_required_skill_by_id_async_with_http_info(tenant_id, required_skill_id, opts)

```ruby
begin
  # Get required skill by ID
  data, status_code, headers = api_instance.get_required_skill_by_id_async_with_http_info(tenant_id, required_skill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RequiredSkillRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->get_required_skill_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **required_skill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RequiredSkillRecordDtoEnvelope**](RequiredSkillRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_required_skills_async

> <RequiredSkillRecordDtoListEnvelope> get_required_skills_async(tenant_id, opts)

Get required skills

Retrieves required-skill records for the specified tenant. Filter by `$filter=JobOfferId eq '...'` or `EmployerProfileId eq '...'`.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RequiredSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get required skills
  result = api_instance.get_required_skills_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->get_required_skills_async: #{e}"
end
```

#### Using the get_required_skills_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RequiredSkillRecordDtoListEnvelope>, Integer, Hash)> get_required_skills_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get required skills
  data, status_code, headers = api_instance.get_required_skills_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RequiredSkillRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->get_required_skills_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RequiredSkillRecordDtoListEnvelope**](RequiredSkillRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_required_skills_count_async

> <Int32Envelope> get_required_skills_count_async(tenant_id, opts)

Count required skills

Counts required-skill records for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RequiredSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count required skills
  result = api_instance.get_required_skills_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->get_required_skills_count_async: #{e}"
end
```

#### Using the get_required_skills_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_required_skills_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count required skills
  data, status_code, headers = api_instance.get_required_skills_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->get_required_skills_count_async_with_http_info: #{e}"
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


## patch_required_skill_async

> <EmptyEnvelope> patch_required_skill_async(tenant_id, required_skill_id, opts)

Patch a required skill

Partially updates an existing required-skill record for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RequiredSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
required_skill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a required skill
  result = api_instance.patch_required_skill_async(tenant_id, required_skill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->patch_required_skill_async: #{e}"
end
```

#### Using the patch_required_skill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_required_skill_async_with_http_info(tenant_id, required_skill_id, opts)

```ruby
begin
  # Patch a required skill
  data, status_code, headers = api_instance.patch_required_skill_async_with_http_info(tenant_id, required_skill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->patch_required_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **required_skill_id** | **String** |  |  |
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


## update_required_skill_async

> <EmptyEnvelope> update_required_skill_async(tenant_id, required_skill_id, opts)

Update a required skill

Updates an existing required-skill record for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RequiredSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
required_skill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  required_skill_record_update_dto: OpenapiClient::RequiredSkillRecordUpdateDto.new # RequiredSkillRecordUpdateDto | 
}

begin
  # Update a required skill
  result = api_instance.update_required_skill_async(tenant_id, required_skill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->update_required_skill_async: #{e}"
end
```

#### Using the update_required_skill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_required_skill_async_with_http_info(tenant_id, required_skill_id, opts)

```ruby
begin
  # Update a required skill
  data, status_code, headers = api_instance.update_required_skill_async_with_http_info(tenant_id, required_skill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RequiredSkillsApi->update_required_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **required_skill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **required_skill_record_update_dto** | [**RequiredSkillRecordUpdateDto**](RequiredSkillRecordUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

