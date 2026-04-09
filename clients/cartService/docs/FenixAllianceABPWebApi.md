# OpenapiClient::FenixAllianceABPWebApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**forgot_password_post**](FenixAllianceABPWebApi.md#forgot_password_post) | **POST** /forgotPassword |  |
| [**health_get**](FenixAllianceABPWebApi.md#health_get) | **GET** /health |  |
| [**hello_get**](FenixAllianceABPWebApi.md#hello_get) | **GET** /hello |  |
| [**login_post**](FenixAllianceABPWebApi.md#login_post) | **POST** /login |  |
| [**manage2fa_post**](FenixAllianceABPWebApi.md#manage2fa_post) | **POST** /manage/2fa |  |
| [**manage_info_get**](FenixAllianceABPWebApi.md#manage_info_get) | **GET** /manage/info |  |
| [**manage_info_post**](FenixAllianceABPWebApi.md#manage_info_post) | **POST** /manage/info |  |
| [**map_identity_api_confirm_email**](FenixAllianceABPWebApi.md#map_identity_api_confirm_email) | **GET** /confirmEmail |  |
| [**refresh_post**](FenixAllianceABPWebApi.md#refresh_post) | **POST** /refresh |  |
| [**register_post**](FenixAllianceABPWebApi.md#register_post) | **POST** /register |  |
| [**resend_confirmation_email_post**](FenixAllianceABPWebApi.md#resend_confirmation_email_post) | **POST** /resendConfirmationEmail |  |
| [**reset_password_post**](FenixAllianceABPWebApi.md#reset_password_post) | **POST** /resetPassword |  |
| [**version_get**](FenixAllianceABPWebApi.md#version_get) | **GET** /version |  |


## forgot_password_post

> forgot_password_post(forgot_password_request)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new
forgot_password_request = OpenapiClient::ForgotPasswordRequest.new({email: 'email_example'}) # ForgotPasswordRequest | 

begin
  
  api_instance.forgot_password_post(forgot_password_request)
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->forgot_password_post: #{e}"
end
```

#### Using the forgot_password_post_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> forgot_password_post_with_http_info(forgot_password_request)

```ruby
begin
  
  data, status_code, headers = api_instance.forgot_password_post_with_http_info(forgot_password_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->forgot_password_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **forgot_password_request** | [**ForgotPasswordRequest**](ForgotPasswordRequest.md) |  |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/problem+json


## health_get

> health_get



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new

begin
  
  api_instance.health_get
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->health_get: #{e}"
end
```

#### Using the health_get_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> health_get_with_http_info

```ruby
begin
  
  data, status_code, headers = api_instance.health_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->health_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## hello_get

> hello_get



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new

begin
  
  api_instance.hello_get
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->hello_get: #{e}"
end
```

#### Using the hello_get_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> hello_get_with_http_info

```ruby
begin
  
  data, status_code, headers = api_instance.hello_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->hello_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## login_post

> <AccessTokenResponse> login_post(login_request, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new
login_request = OpenapiClient::LoginRequest.new({email: 'email_example', password: 'password_example'}) # LoginRequest | 
opts = {
  use_cookies: true, # Boolean | 
  use_session_cookies: true # Boolean | 
}

begin
  
  result = api_instance.login_post(login_request, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->login_post: #{e}"
end
```

#### Using the login_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccessTokenResponse>, Integer, Hash)> login_post_with_http_info(login_request, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.login_post_with_http_info(login_request, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccessTokenResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->login_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **login_request** | [**LoginRequest**](LoginRequest.md) |  |  |
| **use_cookies** | **Boolean** |  | [optional] |
| **use_session_cookies** | **Boolean** |  | [optional] |

### Return type

[**AccessTokenResponse**](AccessTokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## manage2fa_post

> <TwoFactorResponse> manage2fa_post(two_factor_request)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new
two_factor_request = OpenapiClient::TwoFactorRequest.new # TwoFactorRequest | 

begin
  
  result = api_instance.manage2fa_post(two_factor_request)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->manage2fa_post: #{e}"
end
```

#### Using the manage2fa_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TwoFactorResponse>, Integer, Hash)> manage2fa_post_with_http_info(two_factor_request)

```ruby
begin
  
  data, status_code, headers = api_instance.manage2fa_post_with_http_info(two_factor_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TwoFactorResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->manage2fa_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **two_factor_request** | [**TwoFactorRequest**](TwoFactorRequest.md) |  |  |

### Return type

[**TwoFactorResponse**](TwoFactorResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json


## manage_info_get

> <InfoResponse> manage_info_get



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new

begin
  
  result = api_instance.manage_info_get
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->manage_info_get: #{e}"
end
```

#### Using the manage_info_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InfoResponse>, Integer, Hash)> manage_info_get_with_http_info

```ruby
begin
  
  data, status_code, headers = api_instance.manage_info_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InfoResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->manage_info_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**InfoResponse**](InfoResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json


## manage_info_post

> <InfoResponse> manage_info_post(info_request)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new
info_request = OpenapiClient::InfoRequest.new # InfoRequest | 

begin
  
  result = api_instance.manage_info_post(info_request)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->manage_info_post: #{e}"
end
```

#### Using the manage_info_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InfoResponse>, Integer, Hash)> manage_info_post_with_http_info(info_request)

```ruby
begin
  
  data, status_code, headers = api_instance.manage_info_post_with_http_info(info_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InfoResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->manage_info_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **info_request** | [**InfoRequest**](InfoRequest.md) |  |  |

### Return type

[**InfoResponse**](InfoResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json


## map_identity_api_confirm_email

> map_identity_api_confirm_email(user_id, code, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new
user_id = 'user_id_example' # String | 
code = 'code_example' # String | 
opts = {
  changed_email: 'changed_email_example' # String | 
}

begin
  
  api_instance.map_identity_api_confirm_email(user_id, code, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->map_identity_api_confirm_email: #{e}"
end
```

#### Using the map_identity_api_confirm_email_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> map_identity_api_confirm_email_with_http_info(user_id, code, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.map_identity_api_confirm_email_with_http_info(user_id, code, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->map_identity_api_confirm_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
| **code** | **String** |  |  |
| **changed_email** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## refresh_post

> <AccessTokenResponse> refresh_post(refresh_request)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new
refresh_request = OpenapiClient::RefreshRequest.new({refresh_token: 'refresh_token_example'}) # RefreshRequest | 

begin
  
  result = api_instance.refresh_post(refresh_request)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->refresh_post: #{e}"
end
```

#### Using the refresh_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AccessTokenResponse>, Integer, Hash)> refresh_post_with_http_info(refresh_request)

```ruby
begin
  
  data, status_code, headers = api_instance.refresh_post_with_http_info(refresh_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AccessTokenResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->refresh_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **refresh_request** | [**RefreshRequest**](RefreshRequest.md) |  |  |

### Return type

[**AccessTokenResponse**](AccessTokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## register_post

> register_post(register_request)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new
register_request = OpenapiClient::RegisterRequest.new({email: 'email_example', password: 'password_example'}) # RegisterRequest | 

begin
  
  api_instance.register_post(register_request)
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->register_post: #{e}"
end
```

#### Using the register_post_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> register_post_with_http_info(register_request)

```ruby
begin
  
  data, status_code, headers = api_instance.register_post_with_http_info(register_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->register_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **register_request** | [**RegisterRequest**](RegisterRequest.md) |  |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/problem+json


## resend_confirmation_email_post

> resend_confirmation_email_post(resend_confirmation_email_request)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new
resend_confirmation_email_request = OpenapiClient::ResendConfirmationEmailRequest.new({email: 'email_example'}) # ResendConfirmationEmailRequest | 

begin
  
  api_instance.resend_confirmation_email_post(resend_confirmation_email_request)
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->resend_confirmation_email_post: #{e}"
end
```

#### Using the resend_confirmation_email_post_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> resend_confirmation_email_post_with_http_info(resend_confirmation_email_request)

```ruby
begin
  
  data, status_code, headers = api_instance.resend_confirmation_email_post_with_http_info(resend_confirmation_email_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->resend_confirmation_email_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **resend_confirmation_email_request** | [**ResendConfirmationEmailRequest**](ResendConfirmationEmailRequest.md) |  |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## reset_password_post

> reset_password_post(reset_password_request)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new
reset_password_request = OpenapiClient::ResetPasswordRequest.new({email: 'email_example', reset_code: 'reset_code_example', new_password: 'new_password_example'}) # ResetPasswordRequest | 

begin
  
  api_instance.reset_password_post(reset_password_request)
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->reset_password_post: #{e}"
end
```

#### Using the reset_password_post_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> reset_password_post_with_http_info(reset_password_request)

```ruby
begin
  
  data, status_code, headers = api_instance.reset_password_post_with_http_info(reset_password_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->reset_password_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **reset_password_request** | [**ResetPasswordRequest**](ResetPasswordRequest.md) |  |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/problem+json


## version_get

> version_get



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::FenixAllianceABPWebApi.new

begin
  
  api_instance.version_get
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->version_get: #{e}"
end
```

#### Using the version_get_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> version_get_with_http_info

```ruby
begin
  
  data, status_code, headers = api_instance.version_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling FenixAllianceABPWebApi->version_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

