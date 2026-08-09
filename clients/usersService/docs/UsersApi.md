# OpenapiClient::UsersApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_current_user_followers_async**](UsersApi.md#count_current_user_followers_async) | **GET** /api/v2/Me/Followers/Count | Count the social profiles that follow the current user |
| [**count_current_user_follows_async**](UsersApi.md#count_current_user_follows_async) | **GET** /api/v2/Me/Follows/Count | Count the social profiles that the current user follows |
| [**count_current_user_notifications_async**](UsersApi.md#count_current_user_notifications_async) | **GET** /api/v2/Me/Notifications/Count | Count the notifications for the current user |
| [**count_current_user_tenants_async**](UsersApi.md#count_current_user_tenants_async) | **GET** /api/v2/Me/Tenants/Count | Count the tenants that the current user is enrolled in |
| [**get_current_user_addresses_async**](UsersApi.md#get_current_user_addresses_async) | **GET** /api/v2/Me/Addresses | Get the list of addresses for the current user |
| [**get_current_user_async**](UsersApi.md#get_current_user_async) | **GET** /api/v2/Me | Gets the current user |
| [**get_current_user_avatar_async**](UsersApi.md#get_current_user_avatar_async) | **GET** /api/v2/Me/Avatar | Get the current user&#39;s avatar |
| [**get_current_user_cart_async**](UsersApi.md#get_current_user_cart_async) | **GET** /api/v2/Me/Cart | Get the current user&#39;s cart |
| [**get_current_user_enrollments_async**](UsersApi.md#get_current_user_enrollments_async) | **GET** /api/v2/Me/Enrollments | Get the list of enrollments for the current user |
| [**get_current_user_enrollments_extended_async**](UsersApi.md#get_current_user_enrollments_extended_async) | **GET** /api/v2/Me/Enrollments/Extended | Get the list of enrollments for the current user |
| [**get_current_user_followers_async**](UsersApi.md#get_current_user_followers_async) | **GET** /api/v2/Me/Followers | Get the social profiles that follow the current user |
| [**get_current_user_follows_async**](UsersApi.md#get_current_user_follows_async) | **GET** /api/v2/Me/Follows | Get the social profiles that the current user follows |
| [**get_current_user_invitation_async**](UsersApi.md#get_current_user_invitation_async) | **GET** /api/v2/Me/Invitations | Get the list of tenant enrollment invitations for the current user |
| [**get_current_user_notifications_async**](UsersApi.md#get_current_user_notifications_async) | **GET** /api/v2/Me/Notifications | Get the list of notifications for the current user |
| [**get_current_user_settings_async**](UsersApi.md#get_current_user_settings_async) | **GET** /api/v2/Me/Settings | Get the settings for the current user |
| [**get_current_user_social_profile_async**](UsersApi.md#get_current_user_social_profile_async) | **GET** /api/v2/Me/SocialProfile | Get the current user&#39;s social profile |
| [**get_current_user_tenants_async**](UsersApi.md#get_current_user_tenants_async) | **GET** /api/v2/Me/Tenants | Get the tenants that the current user is enrolled in |
| [**get_current_user_tenants_extended_async**](UsersApi.md#get_current_user_tenants_extended_async) | **GET** /api/v2/Me/Tenants/Extended | Get the tenants that the current user is enrolled in |
| [**get_current_user_wallet_async**](UsersApi.md#get_current_user_wallet_async) | **GET** /api/v2/Me/Wallet | Get the current user&#39;s billing profile |
| [**get_enrollment_async**](UsersApi.md#get_enrollment_async) | **GET** /api/v2/Me/Enrollments/{enrollmentId} | Get a single TenantEnrollment by its ID |
| [**get_extended_current_user_async**](UsersApi.md#get_extended_current_user_async) | **GET** /api/v2/Me/Extended | Get the current user&#39;s extended profile |
| [**patch_current_user_async**](UsersApi.md#patch_current_user_async) | **PATCH** /api/v2/Me | Partially update the current user&#39;s profile |
| [**update_avatar_async**](UsersApi.md#update_avatar_async) | **POST** /api/v2/Me/Avatar | Update the current user&#39;s avatar |
| [**update_current_user_async**](UsersApi.md#update_current_user_async) | **PUT** /api/v2/Me | Update the current user&#39;s profile |
| [**update_current_user_settings_async**](UsersApi.md#update_current_user_settings_async) | **PUT** /api/v2/Me/Settings | Update the settings for the current user |


## count_current_user_followers_async

> <Int32Envelope> count_current_user_followers_async(opts)

Count the social profiles that follow the current user

Count the social profiles that follow the current user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  follow_record_dto_collection_query_parameters: OpenapiClient::FollowRecordDtoCollectionQueryParameters.new # FollowRecordDtoCollectionQueryParameters | 
}

begin
  # Count the social profiles that follow the current user
  result = api_instance.count_current_user_followers_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->count_current_user_followers_async: #{e}"
end
```

#### Using the count_current_user_followers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_current_user_followers_async_with_http_info(opts)

```ruby
begin
  # Count the social profiles that follow the current user
  data, status_code, headers = api_instance.count_current_user_followers_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->count_current_user_followers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **follow_record_dto_collection_query_parameters** | [**FollowRecordDtoCollectionQueryParameters**](FollowRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## count_current_user_follows_async

> <Int32Envelope> count_current_user_follows_async(opts)

Count the social profiles that the current user follows

Count the social profiles that the current user follows

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  follow_record_dto_collection_query_parameters: OpenapiClient::FollowRecordDtoCollectionQueryParameters.new # FollowRecordDtoCollectionQueryParameters | 
}

begin
  # Count the social profiles that the current user follows
  result = api_instance.count_current_user_follows_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->count_current_user_follows_async: #{e}"
end
```

#### Using the count_current_user_follows_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_current_user_follows_async_with_http_info(opts)

```ruby
begin
  # Count the social profiles that the current user follows
  data, status_code, headers = api_instance.count_current_user_follows_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->count_current_user_follows_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **follow_record_dto_collection_query_parameters** | [**FollowRecordDtoCollectionQueryParameters**](FollowRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## count_current_user_notifications_async

> <Int32Envelope> count_current_user_notifications_async(opts)

Count the notifications for the current user

Count the notifications for the current user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  notification_dto_collection_query_parameters: OpenapiClient::NotificationDtoCollectionQueryParameters.new # NotificationDtoCollectionQueryParameters | 
}

begin
  # Count the notifications for the current user
  result = api_instance.count_current_user_notifications_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->count_current_user_notifications_async: #{e}"
end
```

#### Using the count_current_user_notifications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_current_user_notifications_async_with_http_info(opts)

```ruby
begin
  # Count the notifications for the current user
  data, status_code, headers = api_instance.count_current_user_notifications_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->count_current_user_notifications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **notification_dto_collection_query_parameters** | [**NotificationDtoCollectionQueryParameters**](NotificationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## count_current_user_tenants_async

> <Int32Envelope> count_current_user_tenants_async(opts)

Count the tenants that the current user is enrolled in

Count the tenants that the current user is enrolled in

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_dto_collection_query_parameters: OpenapiClient::TenantDtoCollectionQueryParameters.new # TenantDtoCollectionQueryParameters | 
}

begin
  # Count the tenants that the current user is enrolled in
  result = api_instance.count_current_user_tenants_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->count_current_user_tenants_async: #{e}"
end
```

#### Using the count_current_user_tenants_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_current_user_tenants_async_with_http_info(opts)

```ruby
begin
  # Count the tenants that the current user is enrolled in
  data, status_code, headers = api_instance.count_current_user_tenants_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->count_current_user_tenants_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_dto_collection_query_parameters** | [**TenantDtoCollectionQueryParameters**](TenantDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_addresses_async

> <AddressDtoListEnvelope> get_current_user_addresses_async(opts)

Get the list of addresses for the current user

Get the list of addresses for the current user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  address_dto_collection_query_parameters: OpenapiClient::AddressDtoCollectionQueryParameters.new # AddressDtoCollectionQueryParameters | 
}

begin
  # Get the list of addresses for the current user
  result = api_instance.get_current_user_addresses_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_addresses_async: #{e}"
end
```

#### Using the get_current_user_addresses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AddressDtoListEnvelope>, Integer, Hash)> get_current_user_addresses_async_with_http_info(opts)

```ruby
begin
  # Get the list of addresses for the current user
  data, status_code, headers = api_instance.get_current_user_addresses_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AddressDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_addresses_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **address_dto_collection_query_parameters** | [**AddressDtoCollectionQueryParameters**](AddressDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AddressDtoListEnvelope**](AddressDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_async

> <UserDtoEnvelope> get_current_user_async(opts)

Gets the current user

Get the currently acting user.

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
  # Gets the current user
  result = api_instance.get_current_user_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_async: #{e}"
end
```

#### Using the get_current_user_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UserDtoEnvelope>, Integer, Hash)> get_current_user_async_with_http_info(opts)

```ruby
begin
  # Gets the current user
  data, status_code, headers = api_instance.get_current_user_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UserDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UserDtoEnvelope**](UserDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_avatar_async

> File get_current_user_avatar_async(opts)

Get the current user's avatar

Get the current user's avatar

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
  # Get the current user's avatar
  result = api_instance.get_current_user_avatar_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_avatar_async: #{e}"
end
```

#### Using the get_current_user_avatar_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(File, Integer, Hash)> get_current_user_avatar_async_with_http_info(opts)

```ruby
begin
  # Get the current user's avatar
  data, status_code, headers = api_instance.get_current_user_avatar_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => File
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_avatar_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_cart_async

> <CartDtoEnvelope> get_current_user_cart_async(opts)

Get the current user's cart

Get the current user's cart

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
  # Get the current user's cart
  result = api_instance.get_current_user_cart_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_cart_async: #{e}"
end
```

#### Using the get_current_user_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoEnvelope>, Integer, Hash)> get_current_user_cart_async_with_http_info(opts)

```ruby
begin
  # Get the current user's cart
  data, status_code, headers = api_instance.get_current_user_cart_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_enrollments_async

> <TenantEnrollmentDtoListEnvelope> get_current_user_enrollments_async(opts)

Get the list of enrollments for the current user

Get the list of enrollments for the current user

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
  # Get the list of enrollments for the current user
  result = api_instance.get_current_user_enrollments_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_enrollments_async: #{e}"
end
```

#### Using the get_current_user_enrollments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantEnrollmentDtoListEnvelope>, Integer, Hash)> get_current_user_enrollments_async_with_http_info(opts)

```ruby
begin
  # Get the list of enrollments for the current user
  data, status_code, headers = api_instance.get_current_user_enrollments_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_enrollments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantEnrollmentDtoListEnvelope**](TenantEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_enrollments_extended_async

> <ExtendedTenantEnrollmentDtoListEnvelope> get_current_user_enrollments_extended_async(opts)

Get the list of enrollments for the current user

Get the list of enrollments for the current user

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
  # Get the list of enrollments for the current user
  result = api_instance.get_current_user_enrollments_extended_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_enrollments_extended_async: #{e}"
end
```

#### Using the get_current_user_enrollments_extended_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedTenantEnrollmentDtoListEnvelope>, Integer, Hash)> get_current_user_enrollments_extended_async_with_http_info(opts)

```ruby
begin
  # Get the list of enrollments for the current user
  data, status_code, headers = api_instance.get_current_user_enrollments_extended_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedTenantEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_enrollments_extended_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExtendedTenantEnrollmentDtoListEnvelope**](ExtendedTenantEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_followers_async

> <FollowRecordDtoListEnvelope> get_current_user_followers_async(opts)

Get the social profiles that follow the current user

Get the social profiles that follow the current user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  follow_record_dto_collection_query_parameters: OpenapiClient::FollowRecordDtoCollectionQueryParameters.new # FollowRecordDtoCollectionQueryParameters | 
}

begin
  # Get the social profiles that follow the current user
  result = api_instance.get_current_user_followers_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_followers_async: #{e}"
end
```

#### Using the get_current_user_followers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FollowRecordDtoListEnvelope>, Integer, Hash)> get_current_user_followers_async_with_http_info(opts)

```ruby
begin
  # Get the social profiles that follow the current user
  data, status_code, headers = api_instance.get_current_user_followers_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FollowRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_followers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **follow_record_dto_collection_query_parameters** | [**FollowRecordDtoCollectionQueryParameters**](FollowRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**FollowRecordDtoListEnvelope**](FollowRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_follows_async

> <FollowRecordDtoListEnvelope> get_current_user_follows_async(opts)

Get the social profiles that the current user follows

Get the social profiles that the current user follows

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  follow_record_dto_collection_query_parameters: OpenapiClient::FollowRecordDtoCollectionQueryParameters.new # FollowRecordDtoCollectionQueryParameters | 
}

begin
  # Get the social profiles that the current user follows
  result = api_instance.get_current_user_follows_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_follows_async: #{e}"
end
```

#### Using the get_current_user_follows_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FollowRecordDtoListEnvelope>, Integer, Hash)> get_current_user_follows_async_with_http_info(opts)

```ruby
begin
  # Get the social profiles that the current user follows
  data, status_code, headers = api_instance.get_current_user_follows_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FollowRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_follows_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **follow_record_dto_collection_query_parameters** | [**FollowRecordDtoCollectionQueryParameters**](FollowRecordDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**FollowRecordDtoListEnvelope**](FollowRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_invitation_async

> <TenantInvitationDtoListEnvelope> get_current_user_invitation_async(opts)

Get the list of tenant enrollment invitations for the current user

Get the list of tenant enrollment invitations for the current user

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
  # Get the list of tenant enrollment invitations for the current user
  result = api_instance.get_current_user_invitation_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_invitation_async: #{e}"
end
```

#### Using the get_current_user_invitation_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantInvitationDtoListEnvelope>, Integer, Hash)> get_current_user_invitation_async_with_http_info(opts)

```ruby
begin
  # Get the list of tenant enrollment invitations for the current user
  data, status_code, headers = api_instance.get_current_user_invitation_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantInvitationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_invitation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_notifications_async

> <NotificationDtoListEnvelope> get_current_user_notifications_async(opts)

Get the list of notifications for the current user

Get the list of notifications for the current user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  notification_dto_collection_query_parameters: OpenapiClient::NotificationDtoCollectionQueryParameters.new # NotificationDtoCollectionQueryParameters | 
}

begin
  # Get the list of notifications for the current user
  result = api_instance.get_current_user_notifications_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_notifications_async: #{e}"
end
```

#### Using the get_current_user_notifications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<NotificationDtoListEnvelope>, Integer, Hash)> get_current_user_notifications_async_with_http_info(opts)

```ruby
begin
  # Get the list of notifications for the current user
  data, status_code, headers = api_instance.get_current_user_notifications_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <NotificationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_notifications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **notification_dto_collection_query_parameters** | [**NotificationDtoCollectionQueryParameters**](NotificationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**NotificationDtoListEnvelope**](NotificationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_settings_async

> <UserSettingsDtoEnvelope> get_current_user_settings_async(opts)

Get the settings for the current user

Get the settings for the current user

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
  # Get the settings for the current user
  result = api_instance.get_current_user_settings_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_settings_async: #{e}"
end
```

#### Using the get_current_user_settings_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UserSettingsDtoEnvelope>, Integer, Hash)> get_current_user_settings_async_with_http_info(opts)

```ruby
begin
  # Get the settings for the current user
  data, status_code, headers = api_instance.get_current_user_settings_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UserSettingsDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_settings_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UserSettingsDtoEnvelope**](UserSettingsDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_social_profile_async

> <SocialProfileDtoEnvelope> get_current_user_social_profile_async(opts)

Get the current user's social profile

Get the current user's social profile

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
  # Get the current user's social profile
  result = api_instance.get_current_user_social_profile_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_social_profile_async: #{e}"
end
```

#### Using the get_current_user_social_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialProfileDtoEnvelope>, Integer, Hash)> get_current_user_social_profile_async_with_http_info(opts)

```ruby
begin
  # Get the current user's social profile
  data, status_code, headers = api_instance.get_current_user_social_profile_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialProfileDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_social_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialProfileDtoEnvelope**](SocialProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_tenants_async

> <TenantDtoListEnvelope> get_current_user_tenants_async(opts)

Get the tenants that the current user is enrolled in

Get the tenants that the current user is enrolled in

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_dto_collection_query_parameters: OpenapiClient::TenantDtoCollectionQueryParameters.new # TenantDtoCollectionQueryParameters | 
}

begin
  # Get the tenants that the current user is enrolled in
  result = api_instance.get_current_user_tenants_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_tenants_async: #{e}"
end
```

#### Using the get_current_user_tenants_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDtoListEnvelope>, Integer, Hash)> get_current_user_tenants_async_with_http_info(opts)

```ruby
begin
  # Get the tenants that the current user is enrolled in
  data, status_code, headers = api_instance.get_current_user_tenants_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_tenants_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_dto_collection_query_parameters** | [**TenantDtoCollectionQueryParameters**](TenantDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TenantDtoListEnvelope**](TenantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_tenants_extended_async

> <ExtendedTenantDtoListEnvelope> get_current_user_tenants_extended_async(opts)

Get the tenants that the current user is enrolled in

Get the tenants that the current user is enrolled in

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
  # Get the tenants that the current user is enrolled in
  result = api_instance.get_current_user_tenants_extended_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_tenants_extended_async: #{e}"
end
```

#### Using the get_current_user_tenants_extended_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedTenantDtoListEnvelope>, Integer, Hash)> get_current_user_tenants_extended_async_with_http_info(opts)

```ruby
begin
  # Get the tenants that the current user is enrolled in
  data, status_code, headers = api_instance.get_current_user_tenants_extended_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedTenantDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_tenants_extended_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExtendedTenantDtoListEnvelope**](ExtendedTenantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_current_user_wallet_async

> <WalletDtoEnvelope> get_current_user_wallet_async(opts)

Get the current user's billing profile

Get the current user's billing profile

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
  # Get the current user's billing profile
  result = api_instance.get_current_user_wallet_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_wallet_async: #{e}"
end
```

#### Using the get_current_user_wallet_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WalletDtoEnvelope>, Integer, Hash)> get_current_user_wallet_async_with_http_info(opts)

```ruby
begin
  # Get the current user's billing profile
  data, status_code, headers = api_instance.get_current_user_wallet_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WalletDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_current_user_wallet_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WalletDtoEnvelope**](WalletDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_enrollment_async

> <TenantEnrollmentDtoEnvelope> get_enrollment_async(enrollment_id, opts)

Get a single TenantEnrollment by its ID

Get a single TenantEnrollment by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a single TenantEnrollment by its ID
  result = api_instance.get_enrollment_async(enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_enrollment_async: #{e}"
end
```

#### Using the get_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantEnrollmentDtoEnvelope>, Integer, Hash)> get_enrollment_async_with_http_info(enrollment_id, opts)

```ruby
begin
  # Get a single TenantEnrollment by its ID
  data, status_code, headers = api_instance.get_enrollment_async_with_http_info(enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantEnrollmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantEnrollmentDtoEnvelope**](TenantEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## get_extended_current_user_async

> <ExtendedUserDtoEnvelope> get_extended_current_user_async(opts)

Get the current user's extended profile

Get the current user's extended profile

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
  # Get the current user's extended profile
  result = api_instance.get_extended_current_user_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_extended_current_user_async: #{e}"
end
```

#### Using the get_extended_current_user_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedUserDtoEnvelope>, Integer, Hash)> get_extended_current_user_async_with_http_info(opts)

```ruby
begin
  # Get the current user's extended profile
  data, status_code, headers = api_instance.get_extended_current_user_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedUserDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->get_extended_current_user_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExtendedUserDtoEnvelope**](ExtendedUserDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data


## patch_current_user_async

> <EmptyEnvelope> patch_current_user_async(opts)

Partially update the current user's profile

Partially update the current user's profile

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially update the current user's profile
  result = api_instance.patch_current_user_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->patch_current_user_async: #{e}"
end
```

#### Using the patch_current_user_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_current_user_async_with_http_info(opts)

```ruby
begin
  # Partially update the current user's profile
  data, status_code, headers = api_instance.patch_current_user_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->patch_current_user_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## update_avatar_async

> <EmptyEnvelope> update_avatar_async(opts)

Update the current user's avatar

Update the current user's avatar

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  avatar: File.new('/path/to/some/file') # File | 
}

begin
  # Update the current user's avatar
  result = api_instance.update_avatar_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->update_avatar_async: #{e}"
end
```

#### Using the update_avatar_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_avatar_async_with_http_info(opts)

```ruby
begin
  # Update the current user's avatar
  data, status_code, headers = api_instance.update_avatar_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->update_avatar_async_with_http_info: #{e}"
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

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml, multipart/form-data


## update_current_user_async

> <EmptyEnvelope> update_current_user_async(opts)

Update the current user's profile

Update the current user's profile

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  user_update_dto: OpenapiClient::UserUpdateDto.new # UserUpdateDto | 
}

begin
  # Update the current user's profile
  result = api_instance.update_current_user_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->update_current_user_async: #{e}"
end
```

#### Using the update_current_user_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_current_user_async_with_http_info(opts)

```ruby
begin
  # Update the current user's profile
  data, status_code, headers = api_instance.update_current_user_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->update_current_user_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **user_update_dto** | [**UserUpdateDto**](UserUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data


## update_current_user_settings_async

> <UserSettingsDtoEnvelope> update_current_user_settings_async(opts)

Update the settings for the current user

Update the settings for the current user

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::UsersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  user_settings_update_dto: OpenapiClient::UserSettingsUpdateDto.new({date_format: 'date_format_example', currency_format: 'currency_format_example', date_time_format: 'date_time_format_example', site_theme: 'System'}) # UserSettingsUpdateDto | 
}

begin
  # Update the settings for the current user
  result = api_instance.update_current_user_settings_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->update_current_user_settings_async: #{e}"
end
```

#### Using the update_current_user_settings_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UserSettingsDtoEnvelope>, Integer, Hash)> update_current_user_settings_async_with_http_info(opts)

```ruby
begin
  # Update the settings for the current user
  data, status_code, headers = api_instance.update_current_user_settings_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UserSettingsDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling UsersApi->update_current_user_settings_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **user_settings_update_dto** | [**UserSettingsUpdateDto**](UserSettingsUpdateDto.md) |  | [optional] |

### Return type

[**UserSettingsDtoEnvelope**](UserSettingsDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data

