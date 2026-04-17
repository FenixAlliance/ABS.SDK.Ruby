# OpenapiClient::LoansApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_loan_application_async**](LoansApi.md#create_loan_application_async) | **POST** /api/v2/AccountingService/Loans/Applications | Creates a loan application |
| [**create_loan_async**](LoansApi.md#create_loan_async) | **POST** /api/v2/AccountingService/Loans | Creates a new loan |
| [**delete_loan_application_async**](LoansApi.md#delete_loan_application_async) | **DELETE** /api/v2/AccountingService/Loans/Applications/{applicationId} | Deletes a loan application |
| [**delete_loan_async**](LoansApi.md#delete_loan_async) | **DELETE** /api/v2/AccountingService/Loans/{loanId} | Deletes a loan |
| [**get_loan_application_details_async**](LoansApi.md#get_loan_application_details_async) | **GET** /api/v2/AccountingService/Loans/Applications/{applicationId} | Gets a loan application by ID |
| [**get_loan_applications_async**](LoansApi.md#get_loan_applications_async) | **GET** /api/v2/AccountingService/Loans/Applications | Gets all loan applications |
| [**get_loan_applications_count_async**](LoansApi.md#get_loan_applications_count_async) | **GET** /api/v2/AccountingService/Loans/Applications/Count | Counts loan applications |
| [**get_loan_details_async**](LoansApi.md#get_loan_details_async) | **GET** /api/v2/AccountingService/Loans/{loanId} | Gets a loan by ID |
| [**get_loans_async**](LoansApi.md#get_loans_async) | **GET** /api/v2/AccountingService/Loans | Gets all loans |
| [**get_loans_count_async**](LoansApi.md#get_loans_count_async) | **GET** /api/v2/AccountingService/Loans/Count | Counts loans |
| [**update_loan_application_async**](LoansApi.md#update_loan_application_async) | **PUT** /api/v2/AccountingService/Loans/Applications/{applicationId} | Updates a loan application |
| [**update_loan_async**](LoansApi.md#update_loan_async) | **PUT** /api/v2/AccountingService/Loans/{loanId} | Updates a loan |


## create_loan_application_async

> <EmptyEnvelope> create_loan_application_async(tenant_id, loan_application_create_dto, opts)

Creates a loan application

Creates a new loan application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loan_application_create_dto = OpenapiClient::LoanApplicationCreateDto.new # LoanApplicationCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Creates a loan application
  result = api_instance.create_loan_application_async(tenant_id, loan_application_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->create_loan_application_async: #{e}"
end
```

#### Using the create_loan_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_loan_application_async_with_http_info(tenant_id, loan_application_create_dto, opts)

```ruby
begin
  # Creates a loan application
  data, status_code, headers = api_instance.create_loan_application_async_with_http_info(tenant_id, loan_application_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->create_loan_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loan_application_create_dto** | [**LoanApplicationCreateDto**](LoanApplicationCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_loan_async

> <EmptyEnvelope> create_loan_async(tenant_id, loan_create_dto, opts)

Creates a new loan

Creates a new loan for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loan_create_dto = OpenapiClient::LoanCreateDto.new # LoanCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Creates a new loan
  result = api_instance.create_loan_async(tenant_id, loan_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->create_loan_async: #{e}"
end
```

#### Using the create_loan_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_loan_async_with_http_info(tenant_id, loan_create_dto, opts)

```ruby
begin
  # Creates a new loan
  data, status_code, headers = api_instance.create_loan_async_with_http_info(tenant_id, loan_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->create_loan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loan_create_dto** | [**LoanCreateDto**](LoanCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_loan_application_async

> <EmptyEnvelope> delete_loan_application_async(tenant_id, application_id, opts)

Deletes a loan application

Deletes the specified loan application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a loan application
  result = api_instance.delete_loan_application_async(tenant_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->delete_loan_application_async: #{e}"
end
```

#### Using the delete_loan_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_loan_application_async_with_http_info(tenant_id, application_id, opts)

```ruby
begin
  # Deletes a loan application
  data, status_code, headers = api_instance.delete_loan_application_async_with_http_info(tenant_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->delete_loan_application_async_with_http_info: #{e}"
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

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_loan_async

> <EmptyEnvelope> delete_loan_async(tenant_id, loan_id, opts)

Deletes a loan

Deletes the specified loan.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loan_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deletes a loan
  result = api_instance.delete_loan_async(tenant_id, loan_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->delete_loan_async: #{e}"
end
```

#### Using the delete_loan_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_loan_async_with_http_info(tenant_id, loan_id, opts)

```ruby
begin
  # Deletes a loan
  data, status_code, headers = api_instance.delete_loan_async_with_http_info(tenant_id, loan_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->delete_loan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loan_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_loan_application_details_async

> <LoanApplicationDtoEnvelope> get_loan_application_details_async(tenant_id, application_id, opts)

Gets a loan application by ID

Retrieves the details of a loan application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a loan application by ID
  result = api_instance.get_loan_application_details_async(tenant_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loan_application_details_async: #{e}"
end
```

#### Using the get_loan_application_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LoanApplicationDtoEnvelope>, Integer, Hash)> get_loan_application_details_async_with_http_info(tenant_id, application_id, opts)

```ruby
begin
  # Gets a loan application by ID
  data, status_code, headers = api_instance.get_loan_application_details_async_with_http_info(tenant_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LoanApplicationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loan_application_details_async_with_http_info: #{e}"
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

[**LoanApplicationDtoEnvelope**](LoanApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_loan_applications_async

> <LoanApplicationDtoIReadOnlyListEnvelope> get_loan_applications_async(tenant_id, opts)

Gets all loan applications

Retrieves all loan applications for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets all loan applications
  result = api_instance.get_loan_applications_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loan_applications_async: #{e}"
end
```

#### Using the get_loan_applications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LoanApplicationDtoIReadOnlyListEnvelope>, Integer, Hash)> get_loan_applications_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets all loan applications
  data, status_code, headers = api_instance.get_loan_applications_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LoanApplicationDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loan_applications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LoanApplicationDtoIReadOnlyListEnvelope**](LoanApplicationDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_loan_applications_count_async

> <Int32Envelope> get_loan_applications_count_async(tenant_id, opts)

Counts loan applications

Gets the count of loan applications for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts loan applications
  result = api_instance.get_loan_applications_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loan_applications_count_async: #{e}"
end
```

#### Using the get_loan_applications_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_loan_applications_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts loan applications
  data, status_code, headers = api_instance.get_loan_applications_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loan_applications_count_async_with_http_info: #{e}"
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


## get_loan_details_async

> <LoanDtoEnvelope> get_loan_details_async(tenant_id, loan_id, opts)

Gets a loan by ID

Retrieves the details of a loan using its unique ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loan_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets a loan by ID
  result = api_instance.get_loan_details_async(tenant_id, loan_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loan_details_async: #{e}"
end
```

#### Using the get_loan_details_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LoanDtoEnvelope>, Integer, Hash)> get_loan_details_async_with_http_info(tenant_id, loan_id, opts)

```ruby
begin
  # Gets a loan by ID
  data, status_code, headers = api_instance.get_loan_details_async_with_http_info(tenant_id, loan_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LoanDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loan_details_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loan_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LoanDtoEnvelope**](LoanDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_loans_async

> <LoanDtoIReadOnlyListEnvelope> get_loans_async(tenant_id, opts)

Gets all loans

Retrieves all loans for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets all loans
  result = api_instance.get_loans_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loans_async: #{e}"
end
```

#### Using the get_loans_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<LoanDtoIReadOnlyListEnvelope>, Integer, Hash)> get_loans_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets all loans
  data, status_code, headers = api_instance.get_loans_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <LoanDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loans_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**LoanDtoIReadOnlyListEnvelope**](LoanDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_loans_count_async

> <Int32Envelope> get_loans_count_async(tenant_id, opts)

Counts loans

Gets the count of loans for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts loans
  result = api_instance.get_loans_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loans_count_async: #{e}"
end
```

#### Using the get_loans_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_loans_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts loans
  data, status_code, headers = api_instance.get_loans_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->get_loans_count_async_with_http_info: #{e}"
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


## update_loan_application_async

> <EmptyEnvelope> update_loan_application_async(tenant_id, application_id, body, opts)

Updates a loan application

Updates the specified loan application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
body = { ... } # Object | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Updates a loan application
  result = api_instance.update_loan_application_async(tenant_id, application_id, body, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->update_loan_application_async: #{e}"
end
```

#### Using the update_loan_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_loan_application_async_with_http_info(tenant_id, application_id, body, opts)

```ruby
begin
  # Updates a loan application
  data, status_code, headers = api_instance.update_loan_application_async_with_http_info(tenant_id, application_id, body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->update_loan_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **body** | **Object** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_loan_async

> <EmptyEnvelope> update_loan_async(tenant_id, loan_id, loan_update_dto, opts)

Updates a loan

Updates the specified loan.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::LoansApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loan_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
loan_update_dto = OpenapiClient::LoanUpdateDto.new # LoanUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Updates a loan
  result = api_instance.update_loan_async(tenant_id, loan_id, loan_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->update_loan_async: #{e}"
end
```

#### Using the update_loan_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_loan_async_with_http_info(tenant_id, loan_id, loan_update_dto, opts)

```ruby
begin
  # Updates a loan
  data, status_code, headers = api_instance.update_loan_async_with_http_info(tenant_id, loan_id, loan_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling LoansApi->update_loan_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **loan_id** | **String** |  |  |
| **loan_update_dto** | [**LoanUpdateDto**](LoanUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

