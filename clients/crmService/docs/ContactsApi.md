# OpenapiClient::ContactsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_contact_async**](ContactsApi.md#create_contact_async) | **POST** /api/v2/CrmService/Contacts | Create a new contact |
| [**create_contact_email_async**](ContactsApi.md#create_contact_email_async) | **POST** /api/v2/CrmService/Contacts/{contactId}/Emails/Addresses | Add an email address to a contact |
| [**create_profile_for_contact_async**](ContactsApi.md#create_profile_for_contact_async) | **POST** /api/v2/CrmService/Contacts/{contactId}/Profiles | Create a contact profile |
| [**delete_contact_async**](ContactsApi.md#delete_contact_async) | **DELETE** /api/v2/CrmService/Contacts/{contactId} | Delete a contact |
| [**delete_contact_email_async**](ContactsApi.md#delete_contact_email_async) | **DELETE** /api/v2/CrmService/Contacts/{contactId}/Emails/{emailId} | Delete a contact email address |
| [**delete_profile_for_contact_async**](ContactsApi.md#delete_profile_for_contact_async) | **DELETE** /api/v2/CrmService/Contacts/{contactId}/Profiles/{profileId} | Delete a contact profile |
| [**get_business_owned_individual_async**](ContactsApi.md#get_business_owned_individual_async) | **GET** /api/v2/CrmService/Contacts/Individuals/{contactId} | Get a Contact of type Individual by ID |
| [**get_business_owned_individuals_async**](ContactsApi.md#get_business_owned_individuals_async) | **GET** /api/v2/CrmService/Contacts/Individuals | Get all contacts of type individual |
| [**get_business_owned_individuals_count_async**](ContactsApi.md#get_business_owned_individuals_count_async) | **GET** /api/v2/CrmService/Contacts/Individuals/Count | Get all contacts of type individual count |
| [**get_business_owned_organization_async**](ContactsApi.md#get_business_owned_organization_async) | **GET** /api/v2/CrmService/Contacts/Organizations/{contactId} | Get a Contact of type Organization by ID |
| [**get_business_owned_organizations_async**](ContactsApi.md#get_business_owned_organizations_async) | **GET** /api/v2/CrmService/Contacts/Organizations | Get all contacts of type organization |
| [**get_business_owned_organizations_count_async**](ContactsApi.md#get_business_owned_organizations_count_async) | **GET** /api/v2/CrmService/Contacts/Organizations/Count | Get all contacts of type organization count |
| [**get_contact_async**](ContactsApi.md#get_contact_async) | **GET** /api/v2/CrmService/Contacts/{contactId} | Get a contact by ID |
| [**get_contact_avatar_async**](ContactsApi.md#get_contact_avatar_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Avatar | Get a contact&#39;s avatar |
| [**get_contact_cart_async**](ContactsApi.md#get_contact_cart_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Cart | Get a contact&#39;s cart |
| [**get_contact_emails_async**](ContactsApi.md#get_contact_emails_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Emails | Get a contact&#39;s email addresses |
| [**get_contact_emails_count_async**](ContactsApi.md#get_contact_emails_count_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Emails/Count | Get contact email addresses count |
| [**get_contact_social_profile_async**](ContactsApi.md#get_contact_social_profile_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/SocialProfile | Get a contact&#39;s social profile |
| [**get_contact_wallet_async**](ContactsApi.md#get_contact_wallet_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Wallet | Get a contact&#39;s wallet |
| [**get_contacts_async**](ContactsApi.md#get_contacts_async) | **GET** /api/v2/CrmService/Contacts | Get all business owned contacts |
| [**get_contacts_count_async**](ContactsApi.md#get_contacts_count_async) | **GET** /api/v2/CrmService/Contacts/Count | Get all business owned contacts count |
| [**get_extended_business_owned_individuals_async**](ContactsApi.md#get_extended_business_owned_individuals_async) | **GET** /api/v2/CrmService/Contacts/Individuals/Extended | Get all contacts of type individual |
| [**get_extended_business_owned_organizations_async**](ContactsApi.md#get_extended_business_owned_organizations_async) | **GET** /api/v2/CrmService/Contacts/Organizations/Extended | Get all contacts of type organization |
| [**get_extended_contact_async**](ContactsApi.md#get_extended_contact_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Extended | Get a contact by ID |
| [**get_extended_contacts_async**](ContactsApi.md#get_extended_contacts_async) | **GET** /api/v2/CrmService/Contacts/Extended | Get all business owned contacts |
| [**get_individual_related_individuals_async**](ContactsApi.md#get_individual_related_individuals_async) | **GET** /api/v2/CrmService/Contacts/Individuals/{contactId}/Individuals | Get individual related individuals |
| [**get_individual_related_organizations_async**](ContactsApi.md#get_individual_related_organizations_async) | **GET** /api/v2/CrmService/Contacts/Individuals/{contactId}/Organizations | Get individual related organizations |
| [**get_organization_related_individuals_async**](ContactsApi.md#get_organization_related_individuals_async) | **GET** /api/v2/CrmService/Contacts/Organizations/{contactId}/Individuals | Get organization related individuals |
| [**get_organization_related_organizations_async**](ContactsApi.md#get_organization_related_organizations_async) | **GET** /api/v2/CrmService/Contacts/Organizations/{contactId}/Organizations | Get organization related organizations |
| [**get_profiles_for_contact_async**](ContactsApi.md#get_profiles_for_contact_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Profiles | Get a contact&#39;s social profiles |
| [**get_profiles_for_contact_count_async**](ContactsApi.md#get_profiles_for_contact_count_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Profiles/Count | Get contact profiles count |
| [**patch_contact_async**](ContactsApi.md#patch_contact_async) | **PATCH** /api/v2/CrmService/Contacts/{contactId} | Patch a contact |
| [**patch_contact_email_async**](ContactsApi.md#patch_contact_email_async) | **PATCH** /api/v2/CrmService/Contacts/{contactId}/Emails/{emailId} | Patch a contact email address |
| [**preview_contact_email_template**](ContactsApi.md#preview_contact_email_template) | **POST** /api/v2/CrmService/Contacts/{contactId}/Emails/Preview | Preview the rendered email for a contact. |
| [**send_contact_email**](ContactsApi.md#send_contact_email) | **POST** /api/v2/CrmService/Contacts/{contactId}/Emails/Send | Send an email to a contact. |
| [**update_contact_async**](ContactsApi.md#update_contact_async) | **PUT** /api/v2/CrmService/Contacts/{contactId} | Update a contact |
| [**update_contact_avatar_async**](ContactsApi.md#update_contact_avatar_async) | **POST** /api/v2/CrmService/Contacts/{contactId}/Avatar | Update a contact&#39;s avatar |
| [**update_contact_email_async**](ContactsApi.md#update_contact_email_async) | **PUT** /api/v2/CrmService/Contacts/{contactId}/Emails/{emailId} | Update a contact email address |
| [**update_profile_for_contact_async**](ContactsApi.md#update_profile_for_contact_async) | **PUT** /api/v2/CrmService/Contacts/{contactId}/Profiles/{profileId} | Update a contact profile |
| [**upsert_tenant_onto_another_tenant_contact_list_async**](ContactsApi.md#upsert_tenant_onto_another_tenant_contact_list_async) | **POST** /api/v2/CrmService/Contacts/Organizations/Upsert | Upsert a tenant onto another tenant&#39;s contact list |
| [**upsert_user_onto_another_tenant_contact_list_async**](ContactsApi.md#upsert_user_onto_another_tenant_contact_list_async) | **POST** /api/v2/CrmService/Contacts/Individuals/Upsert | Upsert a user onto a tenant&#39;s contact list |
| [**verify_contact_email_async**](ContactsApi.md#verify_contact_email_async) | **POST** /api/v2/CrmService/Contacts/{contactId}/Emails/{emailId}/Verify | Verify a contact email address |


## create_contact_async

> <EmptyEnvelope> create_contact_async(opts)

Create a new contact

Create a new contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_create_dto: OpenapiClient::ContactCreateDto.new({type: 'Individual', first_name: 'first_name_example', email: 'email_example'}) # ContactCreateDto | 
}

begin
  # Create a new contact
  result = api_instance.create_contact_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->create_contact_async: #{e}"
end
```

#### Using the create_contact_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_contact_async_with_http_info(opts)

```ruby
begin
  # Create a new contact
  data, status_code, headers = api_instance.create_contact_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->create_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_create_dto** | [**ContactCreateDto**](ContactCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_contact_email_async

> create_contact_email_async(tenant_id, contact_id, opts)

Add an email address to a contact

Creates a new email address for the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_email_create_dto: OpenapiClient::ContactEmailCreateDto.new # ContactEmailCreateDto | 
}

begin
  # Add an email address to a contact
  api_instance.create_contact_email_async(tenant_id, contact_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->create_contact_email_async: #{e}"
end
```

#### Using the create_contact_email_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_contact_email_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Add an email address to a contact
  data, status_code, headers = api_instance.create_contact_email_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->create_contact_email_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_email_create_dto** | [**ContactEmailCreateDto**](ContactEmailCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_profile_for_contact_async

> create_profile_for_contact_async(tenant_id, contact_id, opts)

Create a contact profile

Creates a new profile for the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_profile_create_dto: OpenapiClient::ContactProfileCreateDto.new # ContactProfileCreateDto | 
}

begin
  # Create a contact profile
  api_instance.create_profile_for_contact_async(tenant_id, contact_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->create_profile_for_contact_async: #{e}"
end
```

#### Using the create_profile_for_contact_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_profile_for_contact_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Create a contact profile
  data, status_code, headers = api_instance.create_profile_for_contact_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->create_profile_for_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
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


## delete_contact_async

> <EmptyEnvelope> delete_contact_async(tenant_id, contact_id, opts)

Delete a contact

Delete a contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact
  result = api_instance.delete_contact_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->delete_contact_async: #{e}"
end
```

#### Using the delete_contact_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_contact_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Delete a contact
  data, status_code, headers = api_instance.delete_contact_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->delete_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_contact_email_async

> delete_contact_email_async(tenant_id, contact_id, email_id, opts)

Delete a contact email address

Deletes an email address from the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact email address
  api_instance.delete_contact_email_async(tenant_id, contact_id, email_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->delete_contact_email_async: #{e}"
end
```

#### Using the delete_contact_email_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_contact_email_async_with_http_info(tenant_id, contact_id, email_id, opts)

```ruby
begin
  # Delete a contact email address
  data, status_code, headers = api_instance.delete_contact_email_async_with_http_info(tenant_id, contact_id, email_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->delete_contact_email_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **email_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_profile_for_contact_async

> delete_profile_for_contact_async(tenant_id, contact_id, profile_id, opts)

Delete a contact profile

Deletes a profile for the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a contact profile
  api_instance.delete_profile_for_contact_async(tenant_id, contact_id, profile_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->delete_profile_for_contact_async: #{e}"
end
```

#### Using the delete_profile_for_contact_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_profile_for_contact_async_with_http_info(tenant_id, contact_id, profile_id, opts)

```ruby
begin
  # Delete a contact profile
  data, status_code, headers = api_instance.delete_profile_for_contact_async_with_http_info(tenant_id, contact_id, profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->delete_profile_for_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_owned_individual_async

> <ContactDtoEnvelope> get_business_owned_individual_async(tenant_id, contact_id, opts)

Get a Contact of type Individual by ID

Get a Contact of type Individual by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a Contact of type Individual by ID
  result = api_instance.get_business_owned_individual_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_individual_async: #{e}"
end
```

#### Using the get_business_owned_individual_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoEnvelope>, Integer, Hash)> get_business_owned_individual_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a Contact of type Individual by ID
  data, status_code, headers = api_instance.get_business_owned_individual_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_individual_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_owned_individuals_async

> <ContactDtoListEnvelope> get_business_owned_individuals_async(tenant_id, opts)

Get all contacts of type individual

Get all contacts of type individual

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_dto_collection_query_parameters: OpenapiClient::ContactDtoCollectionQueryParameters.new # ContactDtoCollectionQueryParameters | 
}

begin
  # Get all contacts of type individual
  result = api_instance.get_business_owned_individuals_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_individuals_async: #{e}"
end
```

#### Using the get_business_owned_individuals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_business_owned_individuals_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contacts of type individual
  data, status_code, headers = api_instance.get_business_owned_individuals_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_individuals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_dto_collection_query_parameters** | [**ContactDtoCollectionQueryParameters**](ContactDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_business_owned_individuals_count_async

> <ContactDtoListEnvelope> get_business_owned_individuals_count_async(tenant_id, opts)

Get all contacts of type individual count

Get all contacts of type individual count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_dto_collection_query_parameters: OpenapiClient::ContactDtoCollectionQueryParameters.new # ContactDtoCollectionQueryParameters | 
}

begin
  # Get all contacts of type individual count
  result = api_instance.get_business_owned_individuals_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_individuals_count_async: #{e}"
end
```

#### Using the get_business_owned_individuals_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_business_owned_individuals_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contacts of type individual count
  data, status_code, headers = api_instance.get_business_owned_individuals_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_individuals_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_dto_collection_query_parameters** | [**ContactDtoCollectionQueryParameters**](ContactDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_business_owned_organization_async

> <ContactDtoEnvelope> get_business_owned_organization_async(tenant_id, contact_id, opts)

Get a Contact of type Organization by ID

Get a Contact of type Organization by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a Contact of type Organization by ID
  result = api_instance.get_business_owned_organization_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_organization_async: #{e}"
end
```

#### Using the get_business_owned_organization_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoEnvelope>, Integer, Hash)> get_business_owned_organization_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a Contact of type Organization by ID
  data, status_code, headers = api_instance.get_business_owned_organization_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_organization_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_business_owned_organizations_async

> <Array<ContactDto>> get_business_owned_organizations_async(tenant_id, opts)

Get all contacts of type organization

Get all contacts of type organization

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_dto_collection_query_parameters: OpenapiClient::ContactDtoCollectionQueryParameters.new # ContactDtoCollectionQueryParameters | 
}

begin
  # Get all contacts of type organization
  result = api_instance.get_business_owned_organizations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_organizations_async: #{e}"
end
```

#### Using the get_business_owned_organizations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<ContactDto>>, Integer, Hash)> get_business_owned_organizations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contacts of type organization
  data, status_code, headers = api_instance.get_business_owned_organizations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<ContactDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_organizations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_dto_collection_query_parameters** | [**ContactDtoCollectionQueryParameters**](ContactDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Array&lt;ContactDto&gt;**](ContactDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_business_owned_organizations_count_async

> <ContactDtoListEnvelope> get_business_owned_organizations_count_async(tenant_id, opts)

Get all contacts of type organization count

Get all contacts of type organization count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_dto_collection_query_parameters: OpenapiClient::ContactDtoCollectionQueryParameters.new # ContactDtoCollectionQueryParameters | 
}

begin
  # Get all contacts of type organization count
  result = api_instance.get_business_owned_organizations_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_organizations_count_async: #{e}"
end
```

#### Using the get_business_owned_organizations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_business_owned_organizations_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contacts of type organization count
  data, status_code, headers = api_instance.get_business_owned_organizations_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_business_owned_organizations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_dto_collection_query_parameters** | [**ContactDtoCollectionQueryParameters**](ContactDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_contact_async

> <ContactDtoEnvelope> get_contact_async(tenant_id, contact_id, opts)

Get a contact by ID

Get a contact by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a contact by ID
  result = api_instance.get_contact_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_async: #{e}"
end
```

#### Using the get_contact_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoEnvelope>, Integer, Hash)> get_contact_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a contact by ID
  data, status_code, headers = api_instance.get_contact_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_avatar_async

> <EmptyEnvelope> get_contact_avatar_async(tenant_id, contact_id, opts)

Get a contact's avatar

Get a contact's avatar

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a contact's avatar
  result = api_instance.get_contact_avatar_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_avatar_async: #{e}"
end
```

#### Using the get_contact_avatar_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_contact_avatar_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a contact's avatar
  data, status_code, headers = api_instance.get_contact_avatar_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_avatar_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_cart_async

> <CartDtoEnvelope> get_contact_cart_async(tenant_id, contact_id, opts)

Get a contact's cart

Get a contact's cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a contact's cart
  result = api_instance.get_contact_cart_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_cart_async: #{e}"
end
```

#### Using the get_contact_cart_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoEnvelope>, Integer, Hash)> get_contact_cart_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a contact's cart
  data, status_code, headers = api_instance.get_contact_cart_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_cart_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_emails_async

> <ContactEmailDtoListEnvelope> get_contact_emails_async(tenant_id, contact_id, opts)

Get a contact's email addresses

Get all email addresses for the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_email_dto_collection_query_parameters: OpenapiClient::ContactEmailDtoCollectionQueryParameters.new # ContactEmailDtoCollectionQueryParameters | 
}

begin
  # Get a contact's email addresses
  result = api_instance.get_contact_emails_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_emails_async: #{e}"
end
```

#### Using the get_contact_emails_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactEmailDtoListEnvelope>, Integer, Hash)> get_contact_emails_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a contact's email addresses
  data, status_code, headers = api_instance.get_contact_emails_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactEmailDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_emails_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_email_dto_collection_query_parameters** | [**ContactEmailDtoCollectionQueryParameters**](ContactEmailDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ContactEmailDtoListEnvelope**](ContactEmailDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_contact_emails_count_async

> <Int32Envelope> get_contact_emails_count_async(tenant_id, contact_id, opts)

Get contact email addresses count

Returns the count of email addresses for the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_email_dto_collection_query_parameters: OpenapiClient::ContactEmailDtoCollectionQueryParameters.new # ContactEmailDtoCollectionQueryParameters | 
}

begin
  # Get contact email addresses count
  result = api_instance.get_contact_emails_count_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_emails_count_async: #{e}"
end
```

#### Using the get_contact_emails_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_contact_emails_count_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get contact email addresses count
  data, status_code, headers = api_instance.get_contact_emails_count_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_emails_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_email_dto_collection_query_parameters** | [**ContactEmailDtoCollectionQueryParameters**](ContactEmailDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_contact_social_profile_async

> <SocialProfileDtoEnvelope> get_contact_social_profile_async(tenant_id, contact_id, opts)

Get a contact's social profile

Get a contact's social profile

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a contact's social profile
  result = api_instance.get_contact_social_profile_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_social_profile_async: #{e}"
end
```

#### Using the get_contact_social_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialProfileDtoEnvelope>, Integer, Hash)> get_contact_social_profile_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a contact's social profile
  data, status_code, headers = api_instance.get_contact_social_profile_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialProfileDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_social_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialProfileDtoEnvelope**](SocialProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contact_wallet_async

> <WalletDtoEnvelope> get_contact_wallet_async(tenant_id, contact_id, opts)

Get a contact's wallet

Get a contact's wallet

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a contact's wallet
  result = api_instance.get_contact_wallet_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_wallet_async: #{e}"
end
```

#### Using the get_contact_wallet_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WalletDtoEnvelope>, Integer, Hash)> get_contact_wallet_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a contact's wallet
  data, status_code, headers = api_instance.get_contact_wallet_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WalletDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contact_wallet_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WalletDtoEnvelope**](WalletDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_contacts_async

> <ContactDtoListEnvelope> get_contacts_async(tenant_id, opts)

Get all business owned contacts

Get all business owned contacts

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_dto_collection_query_parameters: OpenapiClient::ContactDtoCollectionQueryParameters.new # ContactDtoCollectionQueryParameters | 
}

begin
  # Get all business owned contacts
  result = api_instance.get_contacts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contacts_async: #{e}"
end
```

#### Using the get_contacts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_contacts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all business owned contacts
  data, status_code, headers = api_instance.get_contacts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contacts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_dto_collection_query_parameters** | [**ContactDtoCollectionQueryParameters**](ContactDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_contacts_count_async

> <ContactDtoListEnvelope> get_contacts_count_async(tenant_id, opts)

Get all business owned contacts count

Get all business owned contacts count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_dto_collection_query_parameters: OpenapiClient::ContactDtoCollectionQueryParameters.new # ContactDtoCollectionQueryParameters | 
}

begin
  # Get all business owned contacts count
  result = api_instance.get_contacts_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contacts_count_async: #{e}"
end
```

#### Using the get_contacts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_contacts_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all business owned contacts count
  data, status_code, headers = api_instance.get_contacts_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_contacts_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_dto_collection_query_parameters** | [**ContactDtoCollectionQueryParameters**](ContactDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_extended_business_owned_individuals_async

> <ExtendedContactDtoListEnvelope> get_extended_business_owned_individuals_async(tenant_id, opts)

Get all contacts of type individual

Get all contacts of type individual

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  extended_contact_dto_collection_query_parameters: OpenapiClient::ExtendedContactDtoCollectionQueryParameters.new # ExtendedContactDtoCollectionQueryParameters | 
}

begin
  # Get all contacts of type individual
  result = api_instance.get_extended_business_owned_individuals_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_extended_business_owned_individuals_async: #{e}"
end
```

#### Using the get_extended_business_owned_individuals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedContactDtoListEnvelope>, Integer, Hash)> get_extended_business_owned_individuals_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contacts of type individual
  data, status_code, headers = api_instance.get_extended_business_owned_individuals_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_extended_business_owned_individuals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **extended_contact_dto_collection_query_parameters** | [**ExtendedContactDtoCollectionQueryParameters**](ExtendedContactDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ExtendedContactDtoListEnvelope**](ExtendedContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_extended_business_owned_organizations_async

> <ExtendedContactDtoListEnvelope> get_extended_business_owned_organizations_async(tenant_id, opts)

Get all contacts of type organization

Get all contacts of type organization

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  extended_contact_dto_collection_query_parameters: OpenapiClient::ExtendedContactDtoCollectionQueryParameters.new # ExtendedContactDtoCollectionQueryParameters | 
}

begin
  # Get all contacts of type organization
  result = api_instance.get_extended_business_owned_organizations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_extended_business_owned_organizations_async: #{e}"
end
```

#### Using the get_extended_business_owned_organizations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedContactDtoListEnvelope>, Integer, Hash)> get_extended_business_owned_organizations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all contacts of type organization
  data, status_code, headers = api_instance.get_extended_business_owned_organizations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_extended_business_owned_organizations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **extended_contact_dto_collection_query_parameters** | [**ExtendedContactDtoCollectionQueryParameters**](ExtendedContactDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ExtendedContactDtoListEnvelope**](ExtendedContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_extended_contact_async

> <ExtendedContactDtoEnvelope> get_extended_contact_async(tenant_id, contact_id, opts)

Get a contact by ID

Get a contact by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a contact by ID
  result = api_instance.get_extended_contact_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_extended_contact_async: #{e}"
end
```

#### Using the get_extended_contact_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedContactDtoEnvelope>, Integer, Hash)> get_extended_contact_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a contact by ID
  data, status_code, headers = api_instance.get_extended_contact_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedContactDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_extended_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExtendedContactDtoEnvelope**](ExtendedContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_contacts_async

> <ExtendedContactDtoListEnvelope> get_extended_contacts_async(tenant_id, opts)

Get all business owned contacts

Get all business owned contacts

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  extended_contact_dto_collection_query_parameters: OpenapiClient::ExtendedContactDtoCollectionQueryParameters.new # ExtendedContactDtoCollectionQueryParameters | 
}

begin
  # Get all business owned contacts
  result = api_instance.get_extended_contacts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_extended_contacts_async: #{e}"
end
```

#### Using the get_extended_contacts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedContactDtoListEnvelope>, Integer, Hash)> get_extended_contacts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all business owned contacts
  data, status_code, headers = api_instance.get_extended_contacts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_extended_contacts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **extended_contact_dto_collection_query_parameters** | [**ExtendedContactDtoCollectionQueryParameters**](ExtendedContactDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ExtendedContactDtoListEnvelope**](ExtendedContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_individual_related_individuals_async

> <ContactDtoListEnvelope> get_individual_related_individuals_async(tenant_id, contact_id, opts)

Get individual related individuals

Get individual related individuals

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get individual related individuals
  result = api_instance.get_individual_related_individuals_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_individual_related_individuals_async: #{e}"
end
```

#### Using the get_individual_related_individuals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_individual_related_individuals_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get individual related individuals
  data, status_code, headers = api_instance.get_individual_related_individuals_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_individual_related_individuals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_individual_related_organizations_async

> <ContactDtoListEnvelope> get_individual_related_organizations_async(tenant_id, contact_id, opts)

Get individual related organizations

Get individual related organizations

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get individual related organizations
  result = api_instance.get_individual_related_organizations_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_individual_related_organizations_async: #{e}"
end
```

#### Using the get_individual_related_organizations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_individual_related_organizations_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get individual related organizations
  data, status_code, headers = api_instance.get_individual_related_organizations_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_individual_related_organizations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_organization_related_individuals_async

> <ContactDtoListEnvelope> get_organization_related_individuals_async(tenant_id, contact_id, opts)

Get organization related individuals

Get organization related individuals

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get organization related individuals
  result = api_instance.get_organization_related_individuals_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_organization_related_individuals_async: #{e}"
end
```

#### Using the get_organization_related_individuals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_organization_related_individuals_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get organization related individuals
  data, status_code, headers = api_instance.get_organization_related_individuals_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_organization_related_individuals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_organization_related_organizations_async

> <ContactDtoListEnvelope> get_organization_related_organizations_async(tenant_id, contact_id, opts)

Get organization related organizations

Get organization related organizations

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get organization related organizations
  result = api_instance.get_organization_related_organizations_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_organization_related_organizations_async: #{e}"
end
```

#### Using the get_organization_related_organizations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoListEnvelope>, Integer, Hash)> get_organization_related_organizations_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get organization related organizations
  data, status_code, headers = api_instance.get_organization_related_organizations_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_organization_related_organizations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_profiles_for_contact_async

> <ContactProfileDtoListEnvelope> get_profiles_for_contact_async(tenant_id, contact_id, opts)

Get a contact's social profiles

Get a contact's social profiles

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a contact's social profiles
  result = api_instance.get_profiles_for_contact_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_profiles_for_contact_async: #{e}"
end
```

#### Using the get_profiles_for_contact_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactProfileDtoListEnvelope>, Integer, Hash)> get_profiles_for_contact_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get a contact's social profiles
  data, status_code, headers = api_instance.get_profiles_for_contact_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_profiles_for_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactProfileDtoListEnvelope**](ContactProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_profiles_for_contact_count_async

> <Int32Envelope> get_profiles_for_contact_count_async(tenant_id, contact_id, opts)

Get contact profiles count

Returns the count of profiles for the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_profile_dto_collection_query_parameters: OpenapiClient::ContactProfileDtoCollectionQueryParameters.new # ContactProfileDtoCollectionQueryParameters | 
}

begin
  # Get contact profiles count
  result = api_instance.get_profiles_for_contact_count_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_profiles_for_contact_count_async: #{e}"
end
```

#### Using the get_profiles_for_contact_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_profiles_for_contact_count_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Get contact profiles count
  data, status_code, headers = api_instance.get_profiles_for_contact_count_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->get_profiles_for_contact_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_profile_dto_collection_query_parameters** | [**ContactProfileDtoCollectionQueryParameters**](ContactProfileDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_contact_async

> <EmptyEnvelope> patch_contact_async(tenant_id, contact_id, opts)

Patch a contact

Patch a contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a contact
  result = api_instance.patch_contact_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->patch_contact_async: #{e}"
end
```

#### Using the patch_contact_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_contact_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Patch a contact
  data, status_code, headers = api_instance.patch_contact_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->patch_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
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


## patch_contact_email_async

> patch_contact_email_async(tenant_id, contact_id, email_id, opts)

Patch a contact email address

Partially updates an existing email address for the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a contact email address
  api_instance.patch_contact_email_async(tenant_id, contact_id, email_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->patch_contact_email_async: #{e}"
end
```

#### Using the patch_contact_email_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_contact_email_async_with_http_info(tenant_id, contact_id, email_id, opts)

```ruby
begin
  # Patch a contact email address
  data, status_code, headers = api_instance.patch_contact_email_async_with_http_info(tenant_id, contact_id, email_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->patch_contact_email_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **email_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## preview_contact_email_template

> preview_contact_email_template(contact_id, opts)

Preview the rendered email for a contact.

This action is only available for global administrators (business_owner role).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Preview the rendered email for a contact.
  api_instance.preview_contact_email_template(contact_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->preview_contact_email_template: #{e}"
end
```

#### Using the preview_contact_email_template_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> preview_contact_email_template_with_http_info(contact_id, opts)

```ruby
begin
  # Preview the rendered email for a contact.
  data, status_code, headers = api_instance.preview_contact_email_template_with_http_info(contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->preview_contact_email_template_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined


## send_contact_email

> send_contact_email(contact_id, opts)

Send an email to a contact.

This action is only available for global administrators (business_owner role).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Send an email to a contact.
  api_instance.send_contact_email(contact_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->send_contact_email: #{e}"
end
```

#### Using the send_contact_email_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> send_contact_email_with_http_info(contact_id, opts)

```ruby
begin
  # Send an email to a contact.
  data, status_code, headers = api_instance.send_contact_email_with_http_info(contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->send_contact_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined


## update_contact_async

> <EmptyEnvelope> update_contact_async(tenant_id, contact_id, opts)

Update a contact

Update a contact

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_update_dto: OpenapiClient::ContactUpdateDto.new({type: 'Individual', email: 'email_example', first_name: 'first_name_example'}) # ContactUpdateDto | 
}

begin
  # Update a contact
  result = api_instance.update_contact_async(tenant_id, contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->update_contact_async: #{e}"
end
```

#### Using the update_contact_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_contact_async_with_http_info(tenant_id, contact_id, opts)

```ruby
begin
  # Update a contact
  data, status_code, headers = api_instance.update_contact_async_with_http_info(tenant_id, contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->update_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_update_dto** | [**ContactUpdateDto**](ContactUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_contact_avatar_async

> <EmptyEnvelope> update_contact_avatar_async(contact_id, opts)

Update a contact's avatar

Update a contact's avatar

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  avatar: File.new('/path/to/some/file') # File | 
}

begin
  # Update a contact's avatar
  result = api_instance.update_contact_avatar_async(contact_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->update_contact_avatar_async: #{e}"
end
```

#### Using the update_contact_avatar_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_contact_avatar_async_with_http_info(contact_id, opts)

```ruby
begin
  # Update a contact's avatar
  data, status_code, headers = api_instance.update_contact_avatar_async_with_http_info(contact_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->update_contact_avatar_async_with_http_info: #{e}"
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

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml


## update_contact_email_async

> update_contact_email_async(tenant_id, contact_id, email_id, opts)

Update a contact email address

Updates an existing email address for the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_email_update_dto: OpenapiClient::ContactEmailUpdateDto.new # ContactEmailUpdateDto | 
}

begin
  # Update a contact email address
  api_instance.update_contact_email_async(tenant_id, contact_id, email_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->update_contact_email_async: #{e}"
end
```

#### Using the update_contact_email_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_contact_email_async_with_http_info(tenant_id, contact_id, email_id, opts)

```ruby
begin
  # Update a contact email address
  data, status_code, headers = api_instance.update_contact_email_async_with_http_info(tenant_id, contact_id, email_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->update_contact_email_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **email_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **contact_email_update_dto** | [**ContactEmailUpdateDto**](ContactEmailUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_profile_for_contact_async

> update_profile_for_contact_async(tenant_id, contact_id, profile_id, opts)

Update a contact profile

Updates an existing profile for the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  contact_profile_update_dto: OpenapiClient::ContactProfileUpdateDto.new # ContactProfileUpdateDto | 
}

begin
  # Update a contact profile
  api_instance.update_profile_for_contact_async(tenant_id, contact_id, profile_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->update_profile_for_contact_async: #{e}"
end
```

#### Using the update_profile_for_contact_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_profile_for_contact_async_with_http_info(tenant_id, contact_id, profile_id, opts)

```ruby
begin
  # Update a contact profile
  data, status_code, headers = api_instance.update_profile_for_contact_async_with_http_info(tenant_id, contact_id, profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->update_profile_for_contact_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **profile_id** | **String** |  |  |
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


## upsert_tenant_onto_another_tenant_contact_list_async

> <ContactDtoEnvelope> upsert_tenant_onto_another_tenant_contact_list_async(tenant_id, related_tenant_id, opts)

Upsert a tenant onto another tenant's contact list

Upsert a tenant onto another tenant's contact list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
related_tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Upsert a tenant onto another tenant's contact list
  result = api_instance.upsert_tenant_onto_another_tenant_contact_list_async(tenant_id, related_tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->upsert_tenant_onto_another_tenant_contact_list_async: #{e}"
end
```

#### Using the upsert_tenant_onto_another_tenant_contact_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoEnvelope>, Integer, Hash)> upsert_tenant_onto_another_tenant_contact_list_async_with_http_info(tenant_id, related_tenant_id, opts)

```ruby
begin
  # Upsert a tenant onto another tenant's contact list
  data, status_code, headers = api_instance.upsert_tenant_onto_another_tenant_contact_list_async_with_http_info(tenant_id, related_tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->upsert_tenant_onto_another_tenant_contact_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **related_tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## upsert_user_onto_another_tenant_contact_list_async

> <ContactDtoEnvelope> upsert_user_onto_another_tenant_contact_list_async(tenant_id, related_user_id, opts)

Upsert a user onto a tenant's contact list

Upsert a user onto a tenant's contact list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
related_user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Upsert a user onto a tenant's contact list
  result = api_instance.upsert_user_onto_another_tenant_contact_list_async(tenant_id, related_user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->upsert_user_onto_another_tenant_contact_list_async: #{e}"
end
```

#### Using the upsert_user_onto_another_tenant_contact_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ContactDtoEnvelope>, Integer, Hash)> upsert_user_onto_another_tenant_contact_list_async_with_http_info(tenant_id, related_user_id, opts)

```ruby
begin
  # Upsert a user onto a tenant's contact list
  data, status_code, headers = api_instance.upsert_user_onto_another_tenant_contact_list_async_with_http_info(tenant_id, related_user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ContactDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->upsert_user_onto_another_tenant_contact_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **related_user_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## verify_contact_email_async

> verify_contact_email_async(tenant_id, contact_id, email_id, opts)

Verify a contact email address

Marks an email address as verified on the specified contact.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ContactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
contact_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
email_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Verify a contact email address
  api_instance.verify_contact_email_async(tenant_id, contact_id, email_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->verify_contact_email_async: #{e}"
end
```

#### Using the verify_contact_email_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> verify_contact_email_async_with_http_info(tenant_id, contact_id, email_id, opts)

```ruby
begin
  # Verify a contact email address
  data, status_code, headers = api_instance.verify_contact_email_async_with_http_info(tenant_id, contact_id, email_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ContactsApi->verify_contact_email_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **contact_id** | **String** |  |  |
| **email_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

