# OpenapiClient::CourseTeamMembershipsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_team_membership_async**](CourseTeamMembershipsApi.md#create_course_team_membership_async) | **POST** /api/v2/LearningService/CourseTeamMemberships | Create a course team membership |
| [**delete_course_team_membership_async**](CourseTeamMembershipsApi.md#delete_course_team_membership_async) | **DELETE** /api/v2/LearningService/CourseTeamMemberships/{membershipId} | Delete a course team membership |
| [**get_course_team_membership_by_id_async**](CourseTeamMembershipsApi.md#get_course_team_membership_by_id_async) | **GET** /api/v2/LearningService/CourseTeamMemberships/{membershipId} | Get course team membership by ID |
| [**get_course_team_memberships_async**](CourseTeamMembershipsApi.md#get_course_team_memberships_async) | **GET** /api/v2/LearningService/CourseTeamMemberships | Get all course team memberships |
| [**get_course_team_memberships_count_async**](CourseTeamMembershipsApi.md#get_course_team_memberships_count_async) | **GET** /api/v2/LearningService/CourseTeamMemberships/Count | Get course team memberships count |
| [**patch_course_team_membership_async**](CourseTeamMembershipsApi.md#patch_course_team_membership_async) | **PATCH** /api/v2/LearningService/CourseTeamMemberships/{membershipId} | Patch a course team membership |
| [**update_course_team_membership_async**](CourseTeamMembershipsApi.md#update_course_team_membership_async) | **PUT** /api/v2/LearningService/CourseTeamMemberships/{membershipId} | Update a course team membership |


## create_course_team_membership_async

> create_course_team_membership_async(tenant_id, opts)

Create a course team membership

Creates a new course team membership for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseTeamMembershipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_team_membership_create_dto: OpenapiClient::CourseTeamMembershipCreateDto.new({course_id: 'course_id_example', instructor_profile_id: 'instructor_profile_id_example'}) # CourseTeamMembershipCreateDto | 
}

begin
  # Create a course team membership
  api_instance.create_course_team_membership_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->create_course_team_membership_async: #{e}"
end
```

#### Using the create_course_team_membership_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_team_membership_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a course team membership
  data, status_code, headers = api_instance.create_course_team_membership_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->create_course_team_membership_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_team_membership_create_dto** | [**CourseTeamMembershipCreateDto**](CourseTeamMembershipCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_team_membership_async

> delete_course_team_membership_async(tenant_id, membership_id, opts)

Delete a course team membership

Deletes a course team membership by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseTeamMembershipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
membership_id = 'membership_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course team membership
  api_instance.delete_course_team_membership_async(tenant_id, membership_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->delete_course_team_membership_async: #{e}"
end
```

#### Using the delete_course_team_membership_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_team_membership_async_with_http_info(tenant_id, membership_id, opts)

```ruby
begin
  # Delete a course team membership
  data, status_code, headers = api_instance.delete_course_team_membership_async_with_http_info(tenant_id, membership_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->delete_course_team_membership_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **membership_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_team_membership_by_id_async

> <CourseTeamMembershipDto> get_course_team_membership_by_id_async(membership_id, opts)

Get course team membership by ID

Retrieves a specific course team membership by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseTeamMembershipsApi.new
membership_id = 'membership_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course team membership by ID
  result = api_instance.get_course_team_membership_by_id_async(membership_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->get_course_team_membership_by_id_async: #{e}"
end
```

#### Using the get_course_team_membership_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseTeamMembershipDto>, Integer, Hash)> get_course_team_membership_by_id_async_with_http_info(membership_id, opts)

```ruby
begin
  # Get course team membership by ID
  data, status_code, headers = api_instance.get_course_team_membership_by_id_async_with_http_info(membership_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseTeamMembershipDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->get_course_team_membership_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **membership_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseTeamMembershipDto**](CourseTeamMembershipDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_team_memberships_async

> <Array<CourseTeamMembershipDto>> get_course_team_memberships_async(tenant_id, opts)

Get all course team memberships

Retrieves all course team memberships for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseTeamMembershipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course team memberships
  result = api_instance.get_course_team_memberships_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->get_course_team_memberships_async: #{e}"
end
```

#### Using the get_course_team_memberships_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseTeamMembershipDto>>, Integer, Hash)> get_course_team_memberships_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course team memberships
  data, status_code, headers = api_instance.get_course_team_memberships_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseTeamMembershipDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->get_course_team_memberships_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseTeamMembershipDto&gt;**](CourseTeamMembershipDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_team_memberships_count_async

> Integer get_course_team_memberships_count_async(tenant_id, opts)

Get course team memberships count

Returns the count of course team memberships for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseTeamMembershipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course team memberships count
  result = api_instance.get_course_team_memberships_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->get_course_team_memberships_count_async: #{e}"
end
```

#### Using the get_course_team_memberships_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_team_memberships_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course team memberships count
  data, status_code, headers = api_instance.get_course_team_memberships_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->get_course_team_memberships_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_course_team_membership_async

> <EmptyEnvelope> patch_course_team_membership_async(tenant_id, membership_id, opts)

Patch a course team membership

Partially updates a course team membership for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseTeamMembershipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
membership_id = 'membership_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a course team membership
  result = api_instance.patch_course_team_membership_async(tenant_id, membership_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->patch_course_team_membership_async: #{e}"
end
```

#### Using the patch_course_team_membership_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_course_team_membership_async_with_http_info(tenant_id, membership_id, opts)

```ruby
begin
  # Patch a course team membership
  data, status_code, headers = api_instance.patch_course_team_membership_async_with_http_info(tenant_id, membership_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->patch_course_team_membership_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **membership_id** | **String** |  |  |
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


## update_course_team_membership_async

> update_course_team_membership_async(tenant_id, membership_id, opts)

Update a course team membership

Updates an existing course team membership.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseTeamMembershipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
membership_id = 'membership_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_team_membership_update_dto: OpenapiClient::CourseTeamMembershipUpdateDto.new # CourseTeamMembershipUpdateDto | 
}

begin
  # Update a course team membership
  api_instance.update_course_team_membership_async(tenant_id, membership_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->update_course_team_membership_async: #{e}"
end
```

#### Using the update_course_team_membership_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_team_membership_async_with_http_info(tenant_id, membership_id, opts)

```ruby
begin
  # Update a course team membership
  data, status_code, headers = api_instance.update_course_team_membership_async_with_http_info(tenant_id, membership_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseTeamMembershipsApi->update_course_team_membership_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **membership_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_team_membership_update_dto** | [**CourseTeamMembershipUpdateDto**](CourseTeamMembershipUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

