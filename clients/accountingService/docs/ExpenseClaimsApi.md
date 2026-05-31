# OpenapiClient::ExpenseClaimsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_expense_claim**](ExpenseClaimsApi.md#create_expense_claim) | **POST** /api/v2/AccountingService/ExpenseClaims | Create an expense claim |
| [**delete_expense_claim**](ExpenseClaimsApi.md#delete_expense_claim) | **DELETE** /api/v2/AccountingService/ExpenseClaims/{expenseClaimId} | Delete an expense claim |
| [**get_expense_claim**](ExpenseClaimsApi.md#get_expense_claim) | **GET** /api/v2/AccountingService/ExpenseClaims/{expenseClaimId} | Get an expense claim by id |
| [**get_expense_claims**](ExpenseClaimsApi.md#get_expense_claims) | **GET** /api/v2/AccountingService/ExpenseClaims | Get all expense claims for a tenant |
| [**get_expense_claims_count**](ExpenseClaimsApi.md#get_expense_claims_count) | **GET** /api/v2/AccountingService/ExpenseClaims/Count | Get the count of expense claims for a tenant |
| [**update_expense_claim**](ExpenseClaimsApi.md#update_expense_claim) | **PUT** /api/v2/AccountingService/ExpenseClaims/{expenseClaimId} | Update an expense claim |


## create_expense_claim

> <EmptyEnvelope> create_expense_claim(tenant_id, expense_claim_create_dto, opts)

Create an expense claim

Creates a new expense claim.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseClaimsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_claim_create_dto = OpenapiClient::ExpenseClaimCreateDto.new # ExpenseClaimCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create an expense claim
  result = api_instance.create_expense_claim(tenant_id, expense_claim_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->create_expense_claim: #{e}"
end
```

#### Using the create_expense_claim_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_expense_claim_with_http_info(tenant_id, expense_claim_create_dto, opts)

```ruby
begin
  # Create an expense claim
  data, status_code, headers = api_instance.create_expense_claim_with_http_info(tenant_id, expense_claim_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->create_expense_claim_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **expense_claim_create_dto** | [**ExpenseClaimCreateDto**](ExpenseClaimCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_expense_claim

> <EmptyEnvelope> delete_expense_claim(tenant_id, expense_claim_id, opts)

Delete an expense claim

Deletes an expense claim.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseClaimsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_claim_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an expense claim
  result = api_instance.delete_expense_claim(tenant_id, expense_claim_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->delete_expense_claim: #{e}"
end
```

#### Using the delete_expense_claim_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_expense_claim_with_http_info(tenant_id, expense_claim_id, opts)

```ruby
begin
  # Delete an expense claim
  data, status_code, headers = api_instance.delete_expense_claim_with_http_info(tenant_id, expense_claim_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->delete_expense_claim_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **expense_claim_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_expense_claim

> <ExpenseClaimDtoEnvelope> get_expense_claim(tenant_id, expense_claim_id, opts)

Get an expense claim by id

Retrieves an expense claim by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseClaimsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_claim_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get an expense claim by id
  result = api_instance.get_expense_claim(tenant_id, expense_claim_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->get_expense_claim: #{e}"
end
```

#### Using the get_expense_claim_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExpenseClaimDtoEnvelope>, Integer, Hash)> get_expense_claim_with_http_info(tenant_id, expense_claim_id, opts)

```ruby
begin
  # Get an expense claim by id
  data, status_code, headers = api_instance.get_expense_claim_with_http_info(tenant_id, expense_claim_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExpenseClaimDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->get_expense_claim_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **expense_claim_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExpenseClaimDtoEnvelope**](ExpenseClaimDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_expense_claims

> <ExpenseClaimDtoListEnvelope> get_expense_claims(tenant_id, opts)

Get all expense claims for a tenant

Retrieves all expense claims for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseClaimsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all expense claims for a tenant
  result = api_instance.get_expense_claims(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->get_expense_claims: #{e}"
end
```

#### Using the get_expense_claims_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExpenseClaimDtoListEnvelope>, Integer, Hash)> get_expense_claims_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all expense claims for a tenant
  data, status_code, headers = api_instance.get_expense_claims_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExpenseClaimDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->get_expense_claims_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExpenseClaimDtoListEnvelope**](ExpenseClaimDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_expense_claims_count

> <Int32Envelope> get_expense_claims_count(tenant_id, opts)

Get the count of expense claims for a tenant

Retrieves the count of expense claims for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseClaimsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of expense claims for a tenant
  result = api_instance.get_expense_claims_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->get_expense_claims_count: #{e}"
end
```

#### Using the get_expense_claims_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_expense_claims_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of expense claims for a tenant
  data, status_code, headers = api_instance.get_expense_claims_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->get_expense_claims_count_with_http_info: #{e}"
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


## update_expense_claim

> <EmptyEnvelope> update_expense_claim(tenant_id, expense_claim_id, expense_claim_update_dto, opts)

Update an expense claim

Updates an existing expense claim.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExpenseClaimsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_claim_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
expense_claim_update_dto = OpenapiClient::ExpenseClaimUpdateDto.new # ExpenseClaimUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update an expense claim
  result = api_instance.update_expense_claim(tenant_id, expense_claim_id, expense_claim_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->update_expense_claim: #{e}"
end
```

#### Using the update_expense_claim_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_expense_claim_with_http_info(tenant_id, expense_claim_id, expense_claim_update_dto, opts)

```ruby
begin
  # Update an expense claim
  data, status_code, headers = api_instance.update_expense_claim_with_http_info(tenant_id, expense_claim_id, expense_claim_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExpenseClaimsApi->update_expense_claim_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **expense_claim_id** | **String** |  |  |
| **expense_claim_update_dto** | [**ExpenseClaimUpdateDto**](ExpenseClaimUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

