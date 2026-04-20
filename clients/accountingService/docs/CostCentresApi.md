# OpenapiClient::CostCentresApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_cost_centre**](CostCentresApi.md#create_cost_centre) | **POST** /api/v2/AccountingService/CostCentres | Create a cost centre |
| [**create_cost_centre_budget**](CostCentresApi.md#create_cost_centre_budget) | **POST** /api/v2/AccountingService/CostCentres/CostCentreBudgets | Create a cost centre budget |
| [**create_cost_centre_group**](CostCentresApi.md#create_cost_centre_group) | **POST** /api/v2/AccountingService/CostCentres/CostCentreGroups | Create a cost centre group |
| [**delete_cost_centre**](CostCentresApi.md#delete_cost_centre) | **DELETE** /api/v2/AccountingService/CostCentres/{costCentreId} | Delete a cost centre |
| [**delete_cost_centre_budget**](CostCentresApi.md#delete_cost_centre_budget) | **DELETE** /api/v2/AccountingService/CostCentres/CostCentreBudgets/{budgetId} | Delete a cost centre budget |
| [**delete_cost_centre_group**](CostCentresApi.md#delete_cost_centre_group) | **DELETE** /api/v2/AccountingService/CostCentres/CostCentreGroups/{groupId} | Delete a cost centre group |
| [**get_cost_centre**](CostCentresApi.md#get_cost_centre) | **GET** /api/v2/AccountingService/CostCentres/{costCentreId} | Get a cost centre by id |
| [**get_cost_centre_budget**](CostCentresApi.md#get_cost_centre_budget) | **GET** /api/v2/AccountingService/CostCentres/CostCentreBudgets/{budgetId} | Get a cost centre budget by id |
| [**get_cost_centre_budgets**](CostCentresApi.md#get_cost_centre_budgets) | **GET** /api/v2/AccountingService/CostCentres/CostCentreBudgets | Get all cost centre budgets for a tenant |
| [**get_cost_centre_group**](CostCentresApi.md#get_cost_centre_group) | **GET** /api/v2/AccountingService/CostCentres/CostCentreGroups/{groupId} | Get a cost centre group by id |
| [**get_cost_centre_groups**](CostCentresApi.md#get_cost_centre_groups) | **GET** /api/v2/AccountingService/CostCentres/CostCentreGroups | Get all cost centre groups for a tenant |
| [**get_cost_centre_groups_count**](CostCentresApi.md#get_cost_centre_groups_count) | **GET** /api/v2/AccountingService/CostCentres/CostCentreGroups/Count | Get the count of cost centre groups for a tenant |
| [**get_cost_centres**](CostCentresApi.md#get_cost_centres) | **GET** /api/v2/AccountingService/CostCentres | Get all cost centres for a tenant |
| [**get_cost_centres_count**](CostCentresApi.md#get_cost_centres_count) | **GET** /api/v2/AccountingService/CostCentres/Count | Get the count of cost centres for a tenant |
| [**update_cost_centre**](CostCentresApi.md#update_cost_centre) | **PUT** /api/v2/AccountingService/CostCentres/{costCentreId} | Update a cost centre |
| [**update_cost_centre_budget**](CostCentresApi.md#update_cost_centre_budget) | **PUT** /api/v2/AccountingService/CostCentres/CostCentreBudgets/{budgetId} | Update a cost centre budget |
| [**update_cost_centre_group**](CostCentresApi.md#update_cost_centre_group) | **PUT** /api/v2/AccountingService/CostCentres/CostCentreGroups/{groupId} | Update a cost centre group |


## create_cost_centre

> <EmptyEnvelope> create_cost_centre(tenant_id, cost_centre_create_dto, opts)

Create a cost centre

Creates a new cost centre.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cost_centre_create_dto = OpenapiClient::CostCentreCreateDto.new # CostCentreCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a cost centre
  result = api_instance.create_cost_centre(tenant_id, cost_centre_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->create_cost_centre: #{e}"
end
```

#### Using the create_cost_centre_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_cost_centre_with_http_info(tenant_id, cost_centre_create_dto, opts)

```ruby
begin
  # Create a cost centre
  data, status_code, headers = api_instance.create_cost_centre_with_http_info(tenant_id, cost_centre_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->create_cost_centre_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **cost_centre_create_dto** | [**CostCentreCreateDto**](CostCentreCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_cost_centre_budget

> <EmptyEnvelope> create_cost_centre_budget(tenant_id, cost_centre_budget_create_dto, opts)

Create a cost centre budget

Creates a new cost centre budget.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cost_centre_budget_create_dto = OpenapiClient::CostCentreBudgetCreateDto.new # CostCentreBudgetCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a cost centre budget
  result = api_instance.create_cost_centre_budget(tenant_id, cost_centre_budget_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->create_cost_centre_budget: #{e}"
end
```

#### Using the create_cost_centre_budget_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_cost_centre_budget_with_http_info(tenant_id, cost_centre_budget_create_dto, opts)

```ruby
begin
  # Create a cost centre budget
  data, status_code, headers = api_instance.create_cost_centre_budget_with_http_info(tenant_id, cost_centre_budget_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->create_cost_centre_budget_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **cost_centre_budget_create_dto** | [**CostCentreBudgetCreateDto**](CostCentreBudgetCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_cost_centre_group

> <EmptyEnvelope> create_cost_centre_group(tenant_id, cost_centre_group_create_dto, opts)

Create a cost centre group

Creates a new cost centre group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cost_centre_group_create_dto = OpenapiClient::CostCentreGroupCreateDto.new # CostCentreGroupCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a cost centre group
  result = api_instance.create_cost_centre_group(tenant_id, cost_centre_group_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->create_cost_centre_group: #{e}"
end
```

#### Using the create_cost_centre_group_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_cost_centre_group_with_http_info(tenant_id, cost_centre_group_create_dto, opts)

```ruby
begin
  # Create a cost centre group
  data, status_code, headers = api_instance.create_cost_centre_group_with_http_info(tenant_id, cost_centre_group_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->create_cost_centre_group_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **cost_centre_group_create_dto** | [**CostCentreGroupCreateDto**](CostCentreGroupCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_cost_centre

> <EmptyEnvelope> delete_cost_centre(tenant_id, cost_centre_id, opts)

Delete a cost centre

Deletes a cost centre.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cost_centre_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a cost centre
  result = api_instance.delete_cost_centre(tenant_id, cost_centre_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->delete_cost_centre: #{e}"
end
```

#### Using the delete_cost_centre_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_cost_centre_with_http_info(tenant_id, cost_centre_id, opts)

```ruby
begin
  # Delete a cost centre
  data, status_code, headers = api_instance.delete_cost_centre_with_http_info(tenant_id, cost_centre_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->delete_cost_centre_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **cost_centre_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_cost_centre_budget

> <EmptyEnvelope> delete_cost_centre_budget(tenant_id, budget_id, opts)

Delete a cost centre budget

Deletes a cost centre budget.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a cost centre budget
  result = api_instance.delete_cost_centre_budget(tenant_id, budget_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->delete_cost_centre_budget: #{e}"
end
```

#### Using the delete_cost_centre_budget_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_cost_centre_budget_with_http_info(tenant_id, budget_id, opts)

```ruby
begin
  # Delete a cost centre budget
  data, status_code, headers = api_instance.delete_cost_centre_budget_with_http_info(tenant_id, budget_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->delete_cost_centre_budget_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_cost_centre_group

> <EmptyEnvelope> delete_cost_centre_group(tenant_id, group_id, opts)

Delete a cost centre group

Deletes a cost centre group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a cost centre group
  result = api_instance.delete_cost_centre_group(tenant_id, group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->delete_cost_centre_group: #{e}"
end
```

#### Using the delete_cost_centre_group_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_cost_centre_group_with_http_info(tenant_id, group_id, opts)

```ruby
begin
  # Delete a cost centre group
  data, status_code, headers = api_instance.delete_cost_centre_group_with_http_info(tenant_id, group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->delete_cost_centre_group_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cost_centre

> <CostCentreDtoEnvelope> get_cost_centre(tenant_id, cost_centre_id, opts)

Get a cost centre by id

Retrieves a cost centre by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cost_centre_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a cost centre by id
  result = api_instance.get_cost_centre(tenant_id, cost_centre_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre: #{e}"
end
```

#### Using the get_cost_centre_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CostCentreDtoEnvelope>, Integer, Hash)> get_cost_centre_with_http_info(tenant_id, cost_centre_id, opts)

```ruby
begin
  # Get a cost centre by id
  data, status_code, headers = api_instance.get_cost_centre_with_http_info(tenant_id, cost_centre_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CostCentreDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **cost_centre_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CostCentreDtoEnvelope**](CostCentreDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cost_centre_budget

> <CostCentreBudgetDtoEnvelope> get_cost_centre_budget(tenant_id, budget_id, opts)

Get a cost centre budget by id

Retrieves a cost centre budget by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a cost centre budget by id
  result = api_instance.get_cost_centre_budget(tenant_id, budget_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_budget: #{e}"
end
```

#### Using the get_cost_centre_budget_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CostCentreBudgetDtoEnvelope>, Integer, Hash)> get_cost_centre_budget_with_http_info(tenant_id, budget_id, opts)

```ruby
begin
  # Get a cost centre budget by id
  data, status_code, headers = api_instance.get_cost_centre_budget_with_http_info(tenant_id, budget_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CostCentreBudgetDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_budget_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CostCentreBudgetDtoEnvelope**](CostCentreBudgetDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cost_centre_budgets

> <CostCentreBudgetDtoListEnvelope> get_cost_centre_budgets(tenant_id, opts)

Get all cost centre budgets for a tenant

Retrieves all cost centre budgets for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all cost centre budgets for a tenant
  result = api_instance.get_cost_centre_budgets(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_budgets: #{e}"
end
```

#### Using the get_cost_centre_budgets_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CostCentreBudgetDtoListEnvelope>, Integer, Hash)> get_cost_centre_budgets_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all cost centre budgets for a tenant
  data, status_code, headers = api_instance.get_cost_centre_budgets_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CostCentreBudgetDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_budgets_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CostCentreBudgetDtoListEnvelope**](CostCentreBudgetDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cost_centre_group

> <CostCentreGroupDtoEnvelope> get_cost_centre_group(tenant_id, group_id, opts)

Get a cost centre group by id

Retrieves a cost centre group by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a cost centre group by id
  result = api_instance.get_cost_centre_group(tenant_id, group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_group: #{e}"
end
```

#### Using the get_cost_centre_group_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CostCentreGroupDtoEnvelope>, Integer, Hash)> get_cost_centre_group_with_http_info(tenant_id, group_id, opts)

```ruby
begin
  # Get a cost centre group by id
  data, status_code, headers = api_instance.get_cost_centre_group_with_http_info(tenant_id, group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CostCentreGroupDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_group_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CostCentreGroupDtoEnvelope**](CostCentreGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cost_centre_groups

> <CostCentreGroupDtoListEnvelope> get_cost_centre_groups(tenant_id, opts)

Get all cost centre groups for a tenant

Retrieves all cost centre groups for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all cost centre groups for a tenant
  result = api_instance.get_cost_centre_groups(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_groups: #{e}"
end
```

#### Using the get_cost_centre_groups_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CostCentreGroupDtoListEnvelope>, Integer, Hash)> get_cost_centre_groups_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all cost centre groups for a tenant
  data, status_code, headers = api_instance.get_cost_centre_groups_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CostCentreGroupDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_groups_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CostCentreGroupDtoListEnvelope**](CostCentreGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cost_centre_groups_count

> <Int32Envelope> get_cost_centre_groups_count(tenant_id, opts)

Get the count of cost centre groups for a tenant

Retrieves the count of cost centre groups for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of cost centre groups for a tenant
  result = api_instance.get_cost_centre_groups_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_groups_count: #{e}"
end
```

#### Using the get_cost_centre_groups_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_cost_centre_groups_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of cost centre groups for a tenant
  data, status_code, headers = api_instance.get_cost_centre_groups_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centre_groups_count_with_http_info: #{e}"
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


## get_cost_centres

> <CostCentreDtoListEnvelope> get_cost_centres(tenant_id, opts)

Get all cost centres for a tenant

Retrieves all cost centres for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all cost centres for a tenant
  result = api_instance.get_cost_centres(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centres: #{e}"
end
```

#### Using the get_cost_centres_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CostCentreDtoListEnvelope>, Integer, Hash)> get_cost_centres_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all cost centres for a tenant
  data, status_code, headers = api_instance.get_cost_centres_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CostCentreDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centres_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CostCentreDtoListEnvelope**](CostCentreDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cost_centres_count

> <Int32Envelope> get_cost_centres_count(tenant_id, opts)

Get the count of cost centres for a tenant

Retrieves the count of cost centres for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of cost centres for a tenant
  result = api_instance.get_cost_centres_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centres_count: #{e}"
end
```

#### Using the get_cost_centres_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_cost_centres_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of cost centres for a tenant
  data, status_code, headers = api_instance.get_cost_centres_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->get_cost_centres_count_with_http_info: #{e}"
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


## update_cost_centre

> <EmptyEnvelope> update_cost_centre(tenant_id, cost_centre_id, cost_centre_update_dto, opts)

Update a cost centre

Updates an existing cost centre.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cost_centre_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cost_centre_update_dto = OpenapiClient::CostCentreUpdateDto.new # CostCentreUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a cost centre
  result = api_instance.update_cost_centre(tenant_id, cost_centre_id, cost_centre_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->update_cost_centre: #{e}"
end
```

#### Using the update_cost_centre_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_cost_centre_with_http_info(tenant_id, cost_centre_id, cost_centre_update_dto, opts)

```ruby
begin
  # Update a cost centre
  data, status_code, headers = api_instance.update_cost_centre_with_http_info(tenant_id, cost_centre_id, cost_centre_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->update_cost_centre_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **cost_centre_id** | **String** |  |  |
| **cost_centre_update_dto** | [**CostCentreUpdateDto**](CostCentreUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_cost_centre_budget

> <EmptyEnvelope> update_cost_centre_budget(tenant_id, budget_id, cost_centre_budget_update_dto, opts)

Update a cost centre budget

Updates an existing cost centre budget.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
budget_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cost_centre_budget_update_dto = OpenapiClient::CostCentreBudgetUpdateDto.new # CostCentreBudgetUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a cost centre budget
  result = api_instance.update_cost_centre_budget(tenant_id, budget_id, cost_centre_budget_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->update_cost_centre_budget: #{e}"
end
```

#### Using the update_cost_centre_budget_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_cost_centre_budget_with_http_info(tenant_id, budget_id, cost_centre_budget_update_dto, opts)

```ruby
begin
  # Update a cost centre budget
  data, status_code, headers = api_instance.update_cost_centre_budget_with_http_info(tenant_id, budget_id, cost_centre_budget_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->update_cost_centre_budget_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **budget_id** | **String** |  |  |
| **cost_centre_budget_update_dto** | [**CostCentreBudgetUpdateDto**](CostCentreBudgetUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_cost_centre_group

> <EmptyEnvelope> update_cost_centre_group(tenant_id, group_id, cost_centre_group_update_dto, opts)

Update a cost centre group

Updates an existing cost centre group.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CostCentresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
group_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cost_centre_group_update_dto = OpenapiClient::CostCentreGroupUpdateDto.new # CostCentreGroupUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a cost centre group
  result = api_instance.update_cost_centre_group(tenant_id, group_id, cost_centre_group_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->update_cost_centre_group: #{e}"
end
```

#### Using the update_cost_centre_group_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_cost_centre_group_with_http_info(tenant_id, group_id, cost_centre_group_update_dto, opts)

```ruby
begin
  # Update a cost centre group
  data, status_code, headers = api_instance.update_cost_centre_group_with_http_info(tenant_id, group_id, cost_centre_group_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CostCentresApi->update_cost_centre_group_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **group_id** | **String** |  |  |
| **cost_centre_group_update_dto** | [**CostCentreGroupUpdateDto**](CostCentreGroupUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

