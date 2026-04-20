# OpenapiClient::AvatarsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_avatar**](AvatarsApi.md#get_avatar) | **GET** /api/v2/StorageService/Avatars/{socialProfileId} | Get the avatar for a given social profile. |
| [**get_contact_avatar**](AvatarsApi.md#get_contact_avatar) | **GET** /api/v2/StorageService/Avatars/Contact/{contactId} | Get the avatar for a given contact. |
| [**get_current_user_avatar**](AvatarsApi.md#get_current_user_avatar) | **GET** /api/v2/StorageService/Avatars/User | Get the avatar for the current user. |
| [**get_tenant_avatar**](AvatarsApi.md#get_tenant_avatar) | **GET** /api/v2/StorageService/Avatars/Tenant/{tenantId} | Get the avatar for a given tenant. |
| [**get_user_avatar**](AvatarsApi.md#get_user_avatar) | **GET** /api/v2/StorageService/Avatars/User/{userId} | Get the avatar for a given user. |
| [**update_contact_avatar**](AvatarsApi.md#update_contact_avatar) | **POST** /api/v2/StorageService/Avatars/Contacts/{contactId} | Update the avatar for a given contact. |
| [**update_tenant_avatar**](AvatarsApi.md#update_tenant_avatar) | **POST** /api/v2/StorageService/Avatars/Tenant/{tenantId} | Update the avatar for a given tenant. |
| [**update_user_avatar**](AvatarsApi.md#update_user_avatar) | **POST** /api/v2/StorageService/Avatars/User | Update the avatar for the current user. |


## get_avatar

> <EmptyEnvelope> get_avatar(social_profile_id, opts)

Get the avatar for a given social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AvatarsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the avatar for a given social profile.
  result = api_instance.get_avatar(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_avatar: #{e}"
end
```

#### Using the get_avatar_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_avatar_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get the avatar for a given social profile.
  data, status_code, headers = api_instance.get_avatar_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_avatar_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## get_contact_avatar

> <EmptyEnvelope> get_contact_avatar(contact_id, opts)

Get the avatar for a given contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AvatarsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the avatar for a given contact.
  result = api_instance.get_contact_avatar(contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_contact_avatar: #{e}"
end
```

#### Using the get_contact_avatar_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_contact_avatar_with_http_info(contact_id, opts)

```ruby
begin
  # Get the avatar for a given contact.
  data, status_code, headers = api_instance.get_contact_avatar_with_http_info(contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_contact_avatar_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## get_current_user_avatar

> <EmptyEnvelope> get_current_user_avatar(opts)

Get the avatar for the current user.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AvatarsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the avatar for the current user.
  result = api_instance.get_current_user_avatar(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_current_user_avatar: #{e}"
end
```

#### Using the get_current_user_avatar_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_current_user_avatar_with_http_info(opts)

```ruby
begin
  # Get the avatar for the current user.
  data, status_code, headers = api_instance.get_current_user_avatar_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_current_user_avatar_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## get_tenant_avatar

> <EmptyEnvelope> get_tenant_avatar(tenant_id, opts)

Get the avatar for a given tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AvatarsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the avatar for a given tenant.
  result = api_instance.get_tenant_avatar(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_tenant_avatar: #{e}"
end
```

#### Using the get_tenant_avatar_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_tenant_avatar_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the avatar for a given tenant.
  data, status_code, headers = api_instance.get_tenant_avatar_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_tenant_avatar_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## get_user_avatar

> <EmptyEnvelope> get_user_avatar(user_id, opts)

Get the avatar for a given user.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AvatarsApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the avatar for a given user.
  result = api_instance.get_user_avatar(user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_user_avatar: #{e}"
end
```

#### Using the get_user_avatar_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_user_avatar_with_http_info(user_id, opts)

```ruby
begin
  # Get the avatar for a given user.
  data, status_code, headers = api_instance.get_user_avatar_with_http_info(user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->get_user_avatar_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png


## update_contact_avatar

> <EmptyEnvelope> update_contact_avatar(contact_id, opts)

Update the avatar for a given contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AvatarsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  avatar: File.new('/path/to/some/file') # File | 
}

begin
  # Update the avatar for a given contact.
  result = api_instance.update_contact_avatar(contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->update_contact_avatar: #{e}"
end
```

#### Using the update_contact_avatar_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_contact_avatar_with_http_info(contact_id, opts)

```ruby
begin
  # Update the avatar for a given contact.
  data, status_code, headers = api_instance.update_contact_avatar_with_http_info(contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->update_contact_avatar_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **avatar** | **File** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, image/png


## update_tenant_avatar

> <EmptyEnvelope> update_tenant_avatar(tenant_id, opts)

Update the avatar for a given tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AvatarsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  avatar: File.new('/path/to/some/file') # File | 
}

begin
  # Update the avatar for a given tenant.
  result = api_instance.update_tenant_avatar(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->update_tenant_avatar: #{e}"
end
```

#### Using the update_tenant_avatar_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_avatar_with_http_info(tenant_id, opts)

```ruby
begin
  # Update the avatar for a given tenant.
  data, status_code, headers = api_instance.update_tenant_avatar_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->update_tenant_avatar_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **avatar** | **File** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, image/png


## update_user_avatar

> <EmptyEnvelope> update_user_avatar(opts)

Update the avatar for the current user.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AvatarsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  avatar: File.new('/path/to/some/file') # File | 
}

begin
  # Update the avatar for the current user.
  result = api_instance.update_user_avatar(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->update_user_avatar: #{e}"
end
```

#### Using the update_user_avatar_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_user_avatar_with_http_info(opts)

```ruby
begin
  # Update the avatar for the current user.
  data, status_code, headers = api_instance.update_user_avatar_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AvatarsApi->update_user_avatar_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **avatar** | **File** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, image/png

