# OpenapiClient::InvitationsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**accept_tenant_invitation**](InvitationsApi.md#accept_tenant_invitation) | **POST** /api/v2/TenantsService/Invitations/{invitationId}/Accept | Accept an invitation to join a tenant |
| [**decline_tenant_invitation**](InvitationsApi.md#decline_tenant_invitation) | **POST** /api/v2/TenantsService/Invitations/{invitationId}/Decline | Decline an invitation to join a tenant |
| [**delete_tenant_invitation**](InvitationsApi.md#delete_tenant_invitation) | **DELETE** /api/v2/TenantsService/Invitations/{invitationId} | Delete a tenant invitation |
| [**get_tenant_invitation_by_id**](InvitationsApi.md#get_tenant_invitation_by_id) | **GET** /api/v2/TenantsService/Invitations/{invitationId} | Get a tenant invitation by its ID |
| [**get_tenant_invitations**](InvitationsApi.md#get_tenant_invitations) | **GET** /api/v2/TenantsService/Invitations | Retrieve a list of tenant invitations |
| [**get_tenant_invitations_count**](InvitationsApi.md#get_tenant_invitations_count) | **GET** /api/v2/TenantsService/Invitations/Count | Get the count of tenant invitations |
| [**send_tenant_invitation**](InvitationsApi.md#send_tenant_invitation) | **POST** /api/v2/TenantsService/Invitations | Send an invitation to a user to join a tenant |


## accept_tenant_invitation

> <EmptyEnvelope> accept_tenant_invitation(invitation_id, opts)

Accept an invitation to join a tenant

Accept an invitation to join a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvitationsApi.new
invitation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Accept an invitation to join a tenant
  result = api_instance.accept_tenant_invitation(invitation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->accept_tenant_invitation: #{e}"
end
```

#### Using the accept_tenant_invitation_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> accept_tenant_invitation_with_http_info(invitation_id, opts)

```ruby
begin
  # Accept an invitation to join a tenant
  data, status_code, headers = api_instance.accept_tenant_invitation_with_http_info(invitation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->accept_tenant_invitation_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **invitation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## decline_tenant_invitation

> <EmptyEnvelope> decline_tenant_invitation(invitation_id, opts)

Decline an invitation to join a tenant

Decline an invitation to join a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvitationsApi.new
invitation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Decline an invitation to join a tenant
  result = api_instance.decline_tenant_invitation(invitation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->decline_tenant_invitation: #{e}"
end
```

#### Using the decline_tenant_invitation_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> decline_tenant_invitation_with_http_info(invitation_id, opts)

```ruby
begin
  # Decline an invitation to join a tenant
  data, status_code, headers = api_instance.decline_tenant_invitation_with_http_info(invitation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->decline_tenant_invitation_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **invitation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_tenant_invitation

> <EmptyEnvelope> delete_tenant_invitation(tenant_id, invitation_id, opts)

Delete a tenant invitation

Delete a tenant invitation

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvitationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invitation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant invitation
  result = api_instance.delete_tenant_invitation(tenant_id, invitation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->delete_tenant_invitation: #{e}"
end
```

#### Using the delete_tenant_invitation_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_invitation_with_http_info(tenant_id, invitation_id, opts)

```ruby
begin
  # Delete a tenant invitation
  data, status_code, headers = api_instance.delete_tenant_invitation_with_http_info(tenant_id, invitation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->delete_tenant_invitation_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invitation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_invitation_by_id

> <TenantInvitationDtoEnvelope> get_tenant_invitation_by_id(tenant_id, invitation_id, opts)

Get a tenant invitation by its ID

Get a tenant invitation by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvitationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invitation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a tenant invitation by its ID
  result = api_instance.get_tenant_invitation_by_id(tenant_id, invitation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->get_tenant_invitation_by_id: #{e}"
end
```

#### Using the get_tenant_invitation_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantInvitationDtoEnvelope>, Integer, Hash)> get_tenant_invitation_by_id_with_http_info(tenant_id, invitation_id, opts)

```ruby
begin
  # Get a tenant invitation by its ID
  data, status_code, headers = api_instance.get_tenant_invitation_by_id_with_http_info(tenant_id, invitation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantInvitationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->get_tenant_invitation_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invitation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantInvitationDtoEnvelope**](TenantInvitationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_invitations

> <TenantInvitationDtoListEnvelope> get_tenant_invitations(tenant_id, opts)

Retrieve a list of tenant invitations

Retrieve a list of tenant invitations

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvitationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant invitations
  result = api_instance.get_tenant_invitations(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->get_tenant_invitations: #{e}"
end
```

#### Using the get_tenant_invitations_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantInvitationDtoListEnvelope>, Integer, Hash)> get_tenant_invitations_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant invitations
  data, status_code, headers = api_instance.get_tenant_invitations_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantInvitationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->get_tenant_invitations_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_invitations_count

> <Int32Envelope> get_tenant_invitations_count(tenant_id, opts)

Get the count of tenant invitations

Get the count of tenant invitations

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvitationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant invitations
  result = api_instance.get_tenant_invitations_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->get_tenant_invitations_count: #{e}"
end
```

#### Using the get_tenant_invitations_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_invitations_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant invitations
  data, status_code, headers = api_instance.get_tenant_invitations_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->get_tenant_invitations_count_with_http_info: #{e}"
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


## send_tenant_invitation

> <EmptyEnvelope> send_tenant_invitation(tenant_id, opts)

Send an invitation to a user to join a tenant

Send an invitation to a user to join a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvitationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_invitation_create_dto: OpenapiClient::TenantInvitationCreateDto.new({user_email: 'user_email_example'}) # TenantInvitationCreateDto | 
}

begin
  # Send an invitation to a user to join a tenant
  result = api_instance.send_tenant_invitation(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->send_tenant_invitation: #{e}"
end
```

#### Using the send_tenant_invitation_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> send_tenant_invitation_with_http_info(tenant_id, opts)

```ruby
begin
  # Send an invitation to a user to join a tenant
  data, status_code, headers = api_instance.send_tenant_invitation_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvitationsApi->send_tenant_invitation_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_invitation_create_dto** | [**TenantInvitationCreateDto**](TenantInvitationCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

