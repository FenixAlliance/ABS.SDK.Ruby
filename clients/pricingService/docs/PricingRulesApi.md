# OpenapiClient::PricingRulesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_pricing_rule**](PricingRulesApi.md#create_pricing_rule) | **POST** /api/v2/PricingService/PricingRules | Create a new pricing rule |
| [**delete_pricing_rule**](PricingRulesApi.md#delete_pricing_rule) | **DELETE** /api/v2/PricingService/PricingRules/{pricingRuleId} | Delete a pricing rule |
| [**get_pricing_rule_by_id**](PricingRulesApi.md#get_pricing_rule_by_id) | **GET** /api/v2/PricingService/PricingRules/{pricingRuleId} | Get pricing rule by ID |
| [**get_pricing_rules**](PricingRulesApi.md#get_pricing_rules) | **GET** /api/v2/PricingService/PricingRules | Get all pricing rules |
| [**get_pricing_rules_count_async**](PricingRulesApi.md#get_pricing_rules_count_async) | **GET** /api/v2/PricingService/PricingRules/Count | Counts pricing rules |
| [**patch_pricing_rule**](PricingRulesApi.md#patch_pricing_rule) | **PATCH** /api/v2/PricingService/PricingRules/{pricingRuleId} | Patch a pricing rule |
| [**update_pricing_rule**](PricingRulesApi.md#update_pricing_rule) | **PUT** /api/v2/PricingService/PricingRules/Update | Update a pricing rule |


## create_pricing_rule

> <PricingRuleDtoEnvelope> create_pricing_rule(tenant_id, opts)

Create a new pricing rule

Creates a new pricing rule for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricingRulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  pricing_rule_create_dto: OpenapiClient::PricingRuleCreateDto.new # PricingRuleCreateDto | 
}

begin
  # Create a new pricing rule
  result = api_instance.create_pricing_rule(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->create_pricing_rule: #{e}"
end
```

#### Using the create_pricing_rule_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PricingRuleDtoEnvelope>, Integer, Hash)> create_pricing_rule_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new pricing rule
  data, status_code, headers = api_instance.create_pricing_rule_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PricingRuleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->create_pricing_rule_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **pricing_rule_create_dto** | [**PricingRuleCreateDto**](PricingRuleCreateDto.md) |  | [optional] |

### Return type

[**PricingRuleDtoEnvelope**](PricingRuleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_pricing_rule

> delete_pricing_rule(tenant_id, pricing_rule_id, opts)

Delete a pricing rule

Deletes a pricing rule for the specified tenant and rule ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricingRulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pricing_rule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a pricing rule
  api_instance.delete_pricing_rule(tenant_id, pricing_rule_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->delete_pricing_rule: #{e}"
end
```

#### Using the delete_pricing_rule_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_pricing_rule_with_http_info(tenant_id, pricing_rule_id, opts)

```ruby
begin
  # Delete a pricing rule
  data, status_code, headers = api_instance.delete_pricing_rule_with_http_info(tenant_id, pricing_rule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->delete_pricing_rule_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pricing_rule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_pricing_rule_by_id

> <PricingRuleDtoEnvelope> get_pricing_rule_by_id(tenant_id, pricing_rule_id, opts)

Get pricing rule by ID

Retrieves a pricing rule by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricingRulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pricing_rule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get pricing rule by ID
  result = api_instance.get_pricing_rule_by_id(tenant_id, pricing_rule_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->get_pricing_rule_by_id: #{e}"
end
```

#### Using the get_pricing_rule_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PricingRuleDtoEnvelope>, Integer, Hash)> get_pricing_rule_by_id_with_http_info(tenant_id, pricing_rule_id, opts)

```ruby
begin
  # Get pricing rule by ID
  data, status_code, headers = api_instance.get_pricing_rule_by_id_with_http_info(tenant_id, pricing_rule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PricingRuleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->get_pricing_rule_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pricing_rule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PricingRuleDtoEnvelope**](PricingRuleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_pricing_rules

> <PricingRuleDtoListEnvelope> get_pricing_rules(tenant_id, opts)

Get all pricing rules

Retrieves all pricing rules for the specified tenant, with optional OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricingRulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all pricing rules
  result = api_instance.get_pricing_rules(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->get_pricing_rules: #{e}"
end
```

#### Using the get_pricing_rules_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PricingRuleDtoListEnvelope>, Integer, Hash)> get_pricing_rules_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all pricing rules
  data, status_code, headers = api_instance.get_pricing_rules_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PricingRuleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->get_pricing_rules_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PricingRuleDtoListEnvelope**](PricingRuleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_pricing_rules_count_async

> <Int32Envelope> get_pricing_rules_count_async(tenant_id, opts)

Counts pricing rules

Gets the count of pricing rules for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricingRulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Counts pricing rules
  result = api_instance.get_pricing_rules_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->get_pricing_rules_count_async: #{e}"
end
```

#### Using the get_pricing_rules_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_pricing_rules_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Counts pricing rules
  data, status_code, headers = api_instance.get_pricing_rules_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->get_pricing_rules_count_async_with_http_info: #{e}"
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


## patch_pricing_rule

> patch_pricing_rule(tenant_id, pricing_rule_id, opts)

Patch a pricing rule

Partially updates a pricing rule using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricingRulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pricing_rule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a pricing rule
  api_instance.patch_pricing_rule(tenant_id, pricing_rule_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->patch_pricing_rule: #{e}"
end
```

#### Using the patch_pricing_rule_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_pricing_rule_with_http_info(tenant_id, pricing_rule_id, opts)

```ruby
begin
  # Patch a pricing rule
  data, status_code, headers = api_instance.patch_pricing_rule_with_http_info(tenant_id, pricing_rule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->patch_pricing_rule_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pricing_rule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_pricing_rule

> update_pricing_rule(tenant_id, pricing_rule_id, opts)

Update a pricing rule

Updates an existing pricing rule for the specified tenant and rule ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricingRulesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pricing_rule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  pricing_rule_update_dto: OpenapiClient::PricingRuleUpdateDto.new # PricingRuleUpdateDto | 
}

begin
  # Update a pricing rule
  api_instance.update_pricing_rule(tenant_id, pricing_rule_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->update_pricing_rule: #{e}"
end
```

#### Using the update_pricing_rule_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_pricing_rule_with_http_info(tenant_id, pricing_rule_id, opts)

```ruby
begin
  # Update a pricing rule
  data, status_code, headers = api_instance.update_pricing_rule_with_http_info(tenant_id, pricing_rule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricingRulesApi->update_pricing_rule_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pricing_rule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **pricing_rule_update_dto** | [**PricingRuleUpdateDto**](PricingRuleUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

