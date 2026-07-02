# OpenapiClient::OAuthApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**check_password_sign_in_async**](OAuthApi.md#check_password_sign_in_async) | **GET** /api/v2/OAuth/SignIn | Check password sign-in |
| [**get**](OAuthApi.md#get) | **GET** /api/v2/OAuth/WhoAmI | Get current user identity |
| [**get_jw_ks**](OAuthApi.md#get_jw_ks) | **GET** /api/v2/OAuth/{applicationId}/Keys | Get JSON Web Key Set |
| [**get_open_id_configuration**](OAuthApi.md#get_open_id_configuration) | **GET** /api/v2/OAuth/{tenantId}/{applicationId}/.Well-Known/OpenId-Configuration | Get OpenID configuration |
| [**get_permissions**](OAuthApi.md#get_permissions) | **GET** /api/v2/OAuth/Permissions | Get user permissions |
| [**password_sign_in_async**](OAuthApi.md#password_sign_in_async) | **POST** /api/v2/OAuth/SignIn | Sign in with password |
| [**token**](OAuthApi.md#token) | **POST** /api/v2/OAuth/Token | Get OAuth token |


## check_password_sign_in_async

> <UserCreateDtoEnvelope> check_password_sign_in_async(opts)

Check password sign-in

Verifies sign-in credentials and returns user details without creating a session.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Check password sign-in
  result = api_instance.check_password_sign_in_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->check_password_sign_in_async: #{e}"
end
```

#### Using the check_password_sign_in_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UserCreateDtoEnvelope>, Integer, Hash)> check_password_sign_in_async_with_http_info(opts)

```ruby
begin
  # Check password sign-in
  data, status_code, headers = api_instance.check_password_sign_in_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UserCreateDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->check_password_sign_in_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UserCreateDtoEnvelope**](UserCreateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get

> <AuthResultEnvelope> get(opts)

Get current user identity

Returns the authorization result for the authenticated user, including identity and tenant context.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user identity
  result = api_instance.get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->get: #{e}"
end
```

#### Using the get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AuthResultEnvelope>, Integer, Hash)> get_with_http_info(opts)

```ruby
begin
  # Get current user identity
  data, status_code, headers = api_instance.get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AuthResultEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AuthResultEnvelope**](AuthResultEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_jw_ks

> <JsonWebKeySetEnvelope> get_jw_ks(application_id, opts)

Get JSON Web Key Set

Retrieves the signing keys (JWKS) for a specific application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApi.new
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get JSON Web Key Set
  result = api_instance.get_jw_ks(application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->get_jw_ks: #{e}"
end
```

#### Using the get_jw_ks_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JsonWebKeySetEnvelope>, Integer, Hash)> get_jw_ks_with_http_info(application_id, opts)

```ruby
begin
  # Get JSON Web Key Set
  data, status_code, headers = api_instance.get_jw_ks_with_http_info(application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JsonWebKeySetEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->get_jw_ks_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**JsonWebKeySetEnvelope**](JsonWebKeySetEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_open_id_configuration

> <OpenIdConfigurationEnvelope> get_open_id_configuration(tenant_id, application_id, opts)

Get OpenID configuration

Retrieves the OpenID Connect discovery document for a specific application within a tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get OpenID configuration
  result = api_instance.get_open_id_configuration(tenant_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->get_open_id_configuration: #{e}"
end
```

#### Using the get_open_id_configuration_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OpenIdConfigurationEnvelope>, Integer, Hash)> get_open_id_configuration_with_http_info(tenant_id, application_id, opts)

```ruby
begin
  # Get OpenID configuration
  data, status_code, headers = api_instance.get_open_id_configuration_with_http_info(tenant_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OpenIdConfigurationEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->get_open_id_configuration_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OpenIdConfigurationEnvelope**](OpenIdConfigurationEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_permissions

> <StringListEnvelope> get_permissions(tenant_id, opts)

Get user permissions

Retrieves the list of permission identifiers for a specific user within a tenant context.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  user_id: 'user_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get user permissions
  result = api_instance.get_permissions(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->get_permissions: #{e}"
end
```

#### Using the get_permissions_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StringListEnvelope>, Integer, Hash)> get_permissions_with_http_info(tenant_id, opts)

```ruby
begin
  # Get user permissions
  data, status_code, headers = api_instance.get_permissions_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StringListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->get_permissions_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **user_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**StringListEnvelope**](StringListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## password_sign_in_async

> <JsonWebTokenEnvelope> password_sign_in_async(opts)

Sign in with password

Authenticates a user using email and password credentials.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signin_model: OpenapiClient::SigninModel.new # SigninModel | 
}

begin
  # Sign in with password
  result = api_instance.password_sign_in_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->password_sign_in_async: #{e}"
end
```

#### Using the password_sign_in_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JsonWebTokenEnvelope>, Integer, Hash)> password_sign_in_async_with_http_info(opts)

```ruby
begin
  # Sign in with password
  data, status_code, headers = api_instance.password_sign_in_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JsonWebTokenEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->password_sign_in_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signin_model** | [**SigninModel**](SigninModel.md) |  | [optional] |

### Return type

[**JsonWebTokenEnvelope**](JsonWebTokenEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## token

> <JsonWebTokenEnvelope> token(opts)

Get OAuth token

Generates an OAuth token based on the provided credentials or grant type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OAuthApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  o_auth_token_request: OpenapiClient::OAuthTokenRequest.new # OAuthTokenRequest | 
}

begin
  # Get OAuth token
  result = api_instance.token(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->token: #{e}"
end
```

#### Using the token_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JsonWebTokenEnvelope>, Integer, Hash)> token_with_http_info(opts)

```ruby
begin
  # Get OAuth token
  data, status_code, headers = api_instance.token_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JsonWebTokenEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OAuthApi->token_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **o_auth_token_request** | [**OAuthTokenRequest**](OAuthTokenRequest.md) |  | [optional] |

### Return type

[**JsonWebTokenEnvelope**](JsonWebTokenEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

