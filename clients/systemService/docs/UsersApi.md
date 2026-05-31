# OpenapiClient::UsersApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**admin_preview_user_email_template**](UsersApi.md#admin_preview_user_email_template) | **POST** /api/v2/SystemService/Users/{userId}/Emails/Preview | Preview the rendered email for a user. |
| [**admin_send_user_email**](UsersApi.md#admin_send_user_email) | **POST** /api/v2/SystemService/Users/{userId}/Emails/Send | Send an email to a user. |
| [**create_account_holder_async**](UsersApi.md#create_account_holder_async) | **POST** /api/v2/SystemService/Users | Create a new user |
| [**delete_account_holder_async**](UsersApi.md#delete_account_holder_async) | **DELETE** /api/v2/SystemService/Users/{userId} | Delete a user |
| [**get_extended_account_holder_async**](UsersApi.md#get_extended_account_holder_async) | **GET** /api/v2/SystemService/Users/{userId}/Extended | Retrieve an extended user by ID |
| [**get_extended_users_async**](UsersApi.md#get_extended_users_async) | **GET** /api/v2/SystemService/Users/Extended | Retrieve a list of extended users |
| [**get_extended_users_count_async**](UsersApi.md#get_extended_users_count_async) | **GET** /api/v2/SystemService/Users/Extended/Count | Get the count of extended users |
| [**get_user_async**](UsersApi.md#get_user_async) | **GET** /api/v2/SystemService/Users/{userId} | Retrieve a user by ID |
| [**get_users_async**](UsersApi.md#get_users_async) | **GET** /api/v2/SystemService/Users | Retrieve a list of users |
| [**get_users_count_async**](UsersApi.md#get_users_count_async) | **GET** /api/v2/SystemService/Users/Count | Get the count of users |
| [**update_account_holder_async**](UsersApi.md#update_account_holder_async) | **PUT** /api/v2/SystemService/Users/{userId} | Update a user |


## admin_preview_user_email_template

> admin_preview_user_email_template(user_id, opts)

Preview the rendered email for a user.

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Preview the rendered email for a user.
  api_instance.admin_preview_user_email_template(user_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->admin_preview_user_email_template: #{e}"
end
```

#### Using the admin_preview_user_email_template_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> admin_preview_user_email_template_with_http_info(user_id, opts)

```ruby
begin
  # Preview the rendered email for a user.
  data, status_code, headers = api_instance.admin_preview_user_email_template_with_http_info(user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->admin_preview_user_email_template_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## admin_send_user_email

> <EmptyEnvelope> admin_send_user_email(user_id, opts)

Send an email to a user.

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Send an email to a user.
  result = api_instance.admin_send_user_email(user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->admin_send_user_email: #{e}"
end
```

#### Using the admin_send_user_email_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> admin_send_user_email_with_http_info(user_id, opts)

```ruby
begin
  # Send an email to a user.
  data, status_code, headers = api_instance.admin_send_user_email_with_http_info(user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->admin_send_user_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_account_holder_async

> <EmptyEnvelope> create_account_holder_async(opts)

Create a new user

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  user_create_dto: OpenapiClient::UserCreateDto.new # UserCreateDto | 
}

begin
  # Create a new user
  result = api_instance.create_account_holder_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->create_account_holder_async: #{e}"
end
```

#### Using the create_account_holder_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_account_holder_async_with_http_info(opts)

```ruby
begin
  # Create a new user
  data, status_code, headers = api_instance.create_account_holder_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->create_account_holder_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **user_create_dto** | [**UserCreateDto**](UserCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_account_holder_async

> <EmptyEnvelope> delete_account_holder_async(user_id, opts)

Delete a user

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a user
  result = api_instance.delete_account_holder_async(user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->delete_account_holder_async: #{e}"
end
```

#### Using the delete_account_holder_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_account_holder_async_with_http_info(user_id, opts)

```ruby
begin
  # Delete a user
  data, status_code, headers = api_instance.delete_account_holder_async_with_http_info(user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->delete_account_holder_async_with_http_info: #{e}"
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
- **Accept**: application/json, application/xml


## get_extended_account_holder_async

> <ExtendedUserDtoEnvelope> get_extended_account_holder_async(user_id, opts)

Retrieve an extended user by ID

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
user_id = 'user_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve an extended user by ID
  result = api_instance.get_extended_account_holder_async(user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_extended_account_holder_async: #{e}"
end
```

#### Using the get_extended_account_holder_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedUserDtoEnvelope>, Integer, Hash)> get_extended_account_holder_async_with_http_info(user_id, opts)

```ruby
begin
  # Retrieve an extended user by ID
  data, status_code, headers = api_instance.get_extended_account_holder_async_with_http_info(user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedUserDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_extended_account_holder_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExtendedUserDtoEnvelope**](ExtendedUserDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_users_async

> <ExtendedUserDtoListEnvelope> get_extended_users_async(opts)

Retrieve a list of extended users

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of extended users
  result = api_instance.get_extended_users_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_extended_users_async: #{e}"
end
```

#### Using the get_extended_users_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedUserDtoListEnvelope>, Integer, Hash)> get_extended_users_async_with_http_info(opts)

```ruby
begin
  # Retrieve a list of extended users
  data, status_code, headers = api_instance.get_extended_users_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedUserDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_extended_users_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExtendedUserDtoListEnvelope**](ExtendedUserDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_users_count_async

> <Int32Envelope> get_extended_users_count_async(opts)

Get the count of extended users

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of extended users
  result = api_instance.get_extended_users_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_extended_users_count_async: #{e}"
end
```

#### Using the get_extended_users_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_extended_users_count_async_with_http_info(opts)

```ruby
begin
  # Get the count of extended users
  data, status_code, headers = api_instance.get_extended_users_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_extended_users_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_user_async

> <UserDtoEnvelope> get_user_async(user_id, opts)

Retrieve a user by ID

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
user_id = 'user_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a user by ID
  result = api_instance.get_user_async(user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_user_async: #{e}"
end
```

#### Using the get_user_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UserDtoEnvelope>, Integer, Hash)> get_user_async_with_http_info(user_id, opts)

```ruby
begin
  # Retrieve a user by ID
  data, status_code, headers = api_instance.get_user_async_with_http_info(user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UserDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_user_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UserDtoEnvelope**](UserDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_users_async

> <UserDtoListEnvelope> get_users_async(opts)

Retrieve a list of users

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of users
  result = api_instance.get_users_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_users_async: #{e}"
end
```

#### Using the get_users_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UserDtoListEnvelope>, Integer, Hash)> get_users_async_with_http_info(opts)

```ruby
begin
  # Retrieve a list of users
  data, status_code, headers = api_instance.get_users_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UserDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_users_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UserDtoListEnvelope**](UserDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_users_count_async

> <Int32Envelope> get_users_count_async(opts)

Get the count of users

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of users
  result = api_instance.get_users_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_users_count_async: #{e}"
end
```

#### Using the get_users_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_users_count_async_with_http_info(opts)

```ruby
begin
  # Get the count of users
  data, status_code, headers = api_instance.get_users_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_users_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_account_holder_async

> <EmptyEnvelope> update_account_holder_async(user_id, opts)

Update a user

This action is only available for global administrators.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  user_update_dto: OpenapiClient::UserUpdateDto.new # UserUpdateDto | 
}

begin
  # Update a user
  result = api_instance.update_account_holder_async(user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->update_account_holder_async: #{e}"
end
```

#### Using the update_account_holder_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_account_holder_async_with_http_info(user_id, opts)

```ruby
begin
  # Update a user
  data, status_code, headers = api_instance.update_account_holder_async_with_http_info(user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->update_account_holder_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **user_update_dto** | [**UserUpdateDto**](UserUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

