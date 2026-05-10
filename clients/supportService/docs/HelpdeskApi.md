# OpenapiClient::HelpdeskApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_inquiry_request_async**](HelpdeskApi.md#create_inquiry_request_async) | **POST** /api/v2/SupportService/InquiryRequests | Create an inquiry request |
| [**create_knowledge_article_async**](HelpdeskApi.md#create_knowledge_article_async) | **POST** /api/v2/SupportService/KnowledgeArticles | Create a knowledge article |
| [**create_maintenance_visit_async**](HelpdeskApi.md#create_maintenance_visit_async) | **POST** /api/v2/SupportService/MaintenanceVisits | Create a maintenance visit |
| [**create_refund_request_async**](HelpdeskApi.md#create_refund_request_async) | **POST** /api/v2/SupportService/RefundRequests | Create a refund request |
| [**create_return_request_async**](HelpdeskApi.md#create_return_request_async) | **POST** /api/v2/SupportService/ReturnRequests | Create a return request |
| [**create_warranty_request_async**](HelpdeskApi.md#create_warranty_request_async) | **POST** /api/v2/SupportService/WarrantyRequests | Create a warranty request |
| [**delete_inquiry_request_async**](HelpdeskApi.md#delete_inquiry_request_async) | **DELETE** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Delete an inquiry request |
| [**delete_knowledge_article_async**](HelpdeskApi.md#delete_knowledge_article_async) | **DELETE** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Delete a knowledge article |
| [**delete_maintenance_visit_async**](HelpdeskApi.md#delete_maintenance_visit_async) | **DELETE** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Delete a maintenance visit |
| [**delete_refund_request_async**](HelpdeskApi.md#delete_refund_request_async) | **DELETE** /api/v2/SupportService/RefundRequests/{refundRequestId} | Delete a refund request |
| [**delete_return_request_async**](HelpdeskApi.md#delete_return_request_async) | **DELETE** /api/v2/SupportService/ReturnRequests/{returnRequestId} | Delete a return request |
| [**delete_warranty_request_async**](HelpdeskApi.md#delete_warranty_request_async) | **DELETE** /api/v2/SupportService/WarrantyRequests/{warrantyRequestId} | Delete a warranty request |
| [**get_inquiry_request_async**](HelpdeskApi.md#get_inquiry_request_async) | **GET** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Retrieve an inquiry request by ID |
| [**get_inquiry_requests_async**](HelpdeskApi.md#get_inquiry_requests_async) | **GET** /api/v2/SupportService/InquiryRequests | Retrieve inquiry requests |
| [**get_inquiry_requests_count_async**](HelpdeskApi.md#get_inquiry_requests_count_async) | **GET** /api/v2/SupportService/InquiryRequests/Count | Get inquiry requests count |
| [**get_knowledge_article_async**](HelpdeskApi.md#get_knowledge_article_async) | **GET** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Retrieve a knowledge article by ID |
| [**get_knowledge_articles_async**](HelpdeskApi.md#get_knowledge_articles_async) | **GET** /api/v2/SupportService/KnowledgeArticles | Retrieve knowledge articles |
| [**get_knowledge_articles_count_async**](HelpdeskApi.md#get_knowledge_articles_count_async) | **GET** /api/v2/SupportService/KnowledgeArticles/Count | Get knowledge articles count |
| [**get_maintenance_visit_async**](HelpdeskApi.md#get_maintenance_visit_async) | **GET** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Retrieve a maintenance visit by ID |
| [**get_maintenance_visits_async**](HelpdeskApi.md#get_maintenance_visits_async) | **GET** /api/v2/SupportService/MaintenanceVisits | Retrieve maintenance visits |
| [**get_maintenance_visits_count_async**](HelpdeskApi.md#get_maintenance_visits_count_async) | **GET** /api/v2/SupportService/MaintenanceVisits/Count | Get maintenance visits count |
| [**get_refund_request_async**](HelpdeskApi.md#get_refund_request_async) | **GET** /api/v2/SupportService/RefundRequests/{refundRequestId} | Retrieve a refund request by ID |
| [**get_refund_requests_async**](HelpdeskApi.md#get_refund_requests_async) | **GET** /api/v2/SupportService/RefundRequests | Retrieve refund requests |
| [**get_refund_requests_count_async**](HelpdeskApi.md#get_refund_requests_count_async) | **GET** /api/v2/SupportService/RefundRequests/Count | Get refund requests count |
| [**get_return_request_async**](HelpdeskApi.md#get_return_request_async) | **GET** /api/v2/SupportService/ReturnRequests/{returnRequestId} | Retrieve a return request by ID |
| [**get_return_requests_async**](HelpdeskApi.md#get_return_requests_async) | **GET** /api/v2/SupportService/ReturnRequests | Retrieve return requests |
| [**get_return_requests_count_async**](HelpdeskApi.md#get_return_requests_count_async) | **GET** /api/v2/SupportService/ReturnRequests/Count | Get return requests count |
| [**get_warranty_request_async**](HelpdeskApi.md#get_warranty_request_async) | **GET** /api/v2/SupportService/WarrantyRequests/{warrantyRequestId} | Retrieve a warranty request by ID |
| [**get_warranty_requests_async**](HelpdeskApi.md#get_warranty_requests_async) | **GET** /api/v2/SupportService/WarrantyRequests | Retrieve warranty requests |
| [**get_warranty_requests_count_async**](HelpdeskApi.md#get_warranty_requests_count_async) | **GET** /api/v2/SupportService/WarrantyRequests/Count | Get warranty requests count |
| [**update_inquiry_request_async**](HelpdeskApi.md#update_inquiry_request_async) | **PUT** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Update an inquiry request |
| [**update_knowledge_article_async**](HelpdeskApi.md#update_knowledge_article_async) | **PUT** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Update a knowledge article |
| [**update_maintenance_visit_async**](HelpdeskApi.md#update_maintenance_visit_async) | **PUT** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Update a maintenance visit |
| [**update_refund_request_async**](HelpdeskApi.md#update_refund_request_async) | **PUT** /api/v2/SupportService/RefundRequests/{refundRequestId} | Update a refund request |
| [**update_return_request_async**](HelpdeskApi.md#update_return_request_async) | **PUT** /api/v2/SupportService/ReturnRequests/{returnRequestId} | Update a return request |
| [**update_warranty_request_async**](HelpdeskApi.md#update_warranty_request_async) | **PUT** /api/v2/SupportService/WarrantyRequests/{warrantyRequestId} | Update a warranty request |


## create_inquiry_request_async

> <EmptyEnvelope> create_inquiry_request_async(tenant_id, opts)

Create an inquiry request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inquiry_request_create_dto: OpenapiClient::InquiryRequestCreateDto.new({name: 'name_example', email: 'email_example', message: 'message_example'}) # InquiryRequestCreateDto | 
}

begin
  # Create an inquiry request
  result = api_instance.create_inquiry_request_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_inquiry_request_async: #{e}"
end
```

#### Using the create_inquiry_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_inquiry_request_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an inquiry request
  data, status_code, headers = api_instance.create_inquiry_request_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_inquiry_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inquiry_request_create_dto** | [**InquiryRequestCreateDto**](InquiryRequestCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_knowledge_article_async

> <EmptyEnvelope> create_knowledge_article_async(tenant_id, opts)

Create a knowledge article

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  knowledge_article_create_dto: OpenapiClient::KnowledgeArticleCreateDto.new({title: 'title_example'}) # KnowledgeArticleCreateDto | 
}

begin
  # Create a knowledge article
  result = api_instance.create_knowledge_article_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_knowledge_article_async: #{e}"
end
```

#### Using the create_knowledge_article_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_knowledge_article_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a knowledge article
  data, status_code, headers = api_instance.create_knowledge_article_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_knowledge_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **knowledge_article_create_dto** | [**KnowledgeArticleCreateDto**](KnowledgeArticleCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_maintenance_visit_async

> <EmptyEnvelope> create_maintenance_visit_async(tenant_id, opts)

Create a maintenance visit

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  maintenance_visit_create_dto: OpenapiClient::MaintenanceVisitCreateDto.new # MaintenanceVisitCreateDto | 
}

begin
  # Create a maintenance visit
  result = api_instance.create_maintenance_visit_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_maintenance_visit_async: #{e}"
end
```

#### Using the create_maintenance_visit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_maintenance_visit_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a maintenance visit
  data, status_code, headers = api_instance.create_maintenance_visit_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_maintenance_visit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **maintenance_visit_create_dto** | [**MaintenanceVisitCreateDto**](MaintenanceVisitCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_refund_request_async

> <EmptyEnvelope> create_refund_request_async(tenant_id, opts)

Create a refund request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  refund_request_create_dto: OpenapiClient::RefundRequestCreateDto.new({title: 'title_example'}) # RefundRequestCreateDto | 
}

begin
  # Create a refund request
  result = api_instance.create_refund_request_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_refund_request_async: #{e}"
end
```

#### Using the create_refund_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_refund_request_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a refund request
  data, status_code, headers = api_instance.create_refund_request_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_refund_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **refund_request_create_dto** | [**RefundRequestCreateDto**](RefundRequestCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_return_request_async

> <EmptyEnvelope> create_return_request_async(tenant_id, opts)

Create a return request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  return_request_create_dto: OpenapiClient::ReturnRequestCreateDto.new({title: 'title_example'}) # ReturnRequestCreateDto | 
}

begin
  # Create a return request
  result = api_instance.create_return_request_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_return_request_async: #{e}"
end
```

#### Using the create_return_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_return_request_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a return request
  data, status_code, headers = api_instance.create_return_request_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_return_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **return_request_create_dto** | [**ReturnRequestCreateDto**](ReturnRequestCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_warranty_request_async

> <EmptyEnvelope> create_warranty_request_async(tenant_id, opts)

Create a warranty request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  warranty_request_create_dto: OpenapiClient::WarrantyRequestCreateDto.new({title: 'title_example'}) # WarrantyRequestCreateDto | 
}

begin
  # Create a warranty request
  result = api_instance.create_warranty_request_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_warranty_request_async: #{e}"
end
```

#### Using the create_warranty_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_warranty_request_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a warranty request
  data, status_code, headers = api_instance.create_warranty_request_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->create_warranty_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **warranty_request_create_dto** | [**WarrantyRequestCreateDto**](WarrantyRequestCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_inquiry_request_async

> <EmptyEnvelope> delete_inquiry_request_async(tenant_id, inquiry_request_id, opts)

Delete an inquiry request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
inquiry_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an inquiry request
  result = api_instance.delete_inquiry_request_async(tenant_id, inquiry_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_inquiry_request_async: #{e}"
end
```

#### Using the delete_inquiry_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)

```ruby
begin
  # Delete an inquiry request
  data, status_code, headers = api_instance.delete_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_inquiry_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **inquiry_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_knowledge_article_async

> <EmptyEnvelope> delete_knowledge_article_async(tenant_id, knowledge_article_id, opts)

Delete a knowledge article

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
knowledge_article_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a knowledge article
  result = api_instance.delete_knowledge_article_async(tenant_id, knowledge_article_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_knowledge_article_async: #{e}"
end
```

#### Using the delete_knowledge_article_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)

```ruby
begin
  # Delete a knowledge article
  data, status_code, headers = api_instance.delete_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_knowledge_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **knowledge_article_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_maintenance_visit_async

> <EmptyEnvelope> delete_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)

Delete a maintenance visit

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
maintenance_visit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a maintenance visit
  result = api_instance.delete_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_maintenance_visit_async: #{e}"
end
```

#### Using the delete_maintenance_visit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)

```ruby
begin
  # Delete a maintenance visit
  data, status_code, headers = api_instance.delete_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_maintenance_visit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **maintenance_visit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_refund_request_async

> <EmptyEnvelope> delete_refund_request_async(tenant_id, refund_request_id, opts)

Delete a refund request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a refund request
  result = api_instance.delete_refund_request_async(tenant_id, refund_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_refund_request_async: #{e}"
end
```

#### Using the delete_refund_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)

```ruby
begin
  # Delete a refund request
  data, status_code, headers = api_instance.delete_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_refund_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_return_request_async

> <EmptyEnvelope> delete_return_request_async(tenant_id, return_request_id, opts)

Delete a return request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a return request
  result = api_instance.delete_return_request_async(tenant_id, return_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_return_request_async: #{e}"
end
```

#### Using the delete_return_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_return_request_async_with_http_info(tenant_id, return_request_id, opts)

```ruby
begin
  # Delete a return request
  data, status_code, headers = api_instance.delete_return_request_async_with_http_info(tenant_id, return_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_return_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **return_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_warranty_request_async

> <EmptyEnvelope> delete_warranty_request_async(tenant_id, warranty_request_id, opts)

Delete a warranty request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a warranty request
  result = api_instance.delete_warranty_request_async(tenant_id, warranty_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_warranty_request_async: #{e}"
end
```

#### Using the delete_warranty_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)

```ruby
begin
  # Delete a warranty request
  data, status_code, headers = api_instance.delete_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->delete_warranty_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warranty_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_inquiry_request_async

> <InquiryRequestDtoEnvelope> get_inquiry_request_async(tenant_id, inquiry_request_id, opts)

Retrieve an inquiry request by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
inquiry_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve an inquiry request by ID
  result = api_instance.get_inquiry_request_async(tenant_id, inquiry_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_inquiry_request_async: #{e}"
end
```

#### Using the get_inquiry_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InquiryRequestDtoEnvelope>, Integer, Hash)> get_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)

```ruby
begin
  # Retrieve an inquiry request by ID
  data, status_code, headers = api_instance.get_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InquiryRequestDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_inquiry_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **inquiry_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InquiryRequestDtoEnvelope**](InquiryRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_inquiry_requests_async

> <InquiryRequestDtoListEnvelope> get_inquiry_requests_async(tenant_id, opts)

Retrieve inquiry requests

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve inquiry requests
  result = api_instance.get_inquiry_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_inquiry_requests_async: #{e}"
end
```

#### Using the get_inquiry_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InquiryRequestDtoListEnvelope>, Integer, Hash)> get_inquiry_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve inquiry requests
  data, status_code, headers = api_instance.get_inquiry_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InquiryRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_inquiry_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InquiryRequestDtoListEnvelope**](InquiryRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_inquiry_requests_count_async

> <Int32Envelope> get_inquiry_requests_count_async(tenant_id, opts)

Get inquiry requests count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get inquiry requests count
  result = api_instance.get_inquiry_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_inquiry_requests_count_async: #{e}"
end
```

#### Using the get_inquiry_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_inquiry_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get inquiry requests count
  data, status_code, headers = api_instance.get_inquiry_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_inquiry_requests_count_async_with_http_info: #{e}"
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


## get_knowledge_article_async

> <KnowledgeArticleDtoEnvelope> get_knowledge_article_async(tenant_id, knowledge_article_id, opts)

Retrieve a knowledge article by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
knowledge_article_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a knowledge article by ID
  result = api_instance.get_knowledge_article_async(tenant_id, knowledge_article_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_knowledge_article_async: #{e}"
end
```

#### Using the get_knowledge_article_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<KnowledgeArticleDtoEnvelope>, Integer, Hash)> get_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)

```ruby
begin
  # Retrieve a knowledge article by ID
  data, status_code, headers = api_instance.get_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <KnowledgeArticleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_knowledge_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **knowledge_article_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**KnowledgeArticleDtoEnvelope**](KnowledgeArticleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_knowledge_articles_async

> <KnowledgeArticleDtoListEnvelope> get_knowledge_articles_async(tenant_id, opts)

Retrieve knowledge articles

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve knowledge articles
  result = api_instance.get_knowledge_articles_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_knowledge_articles_async: #{e}"
end
```

#### Using the get_knowledge_articles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<KnowledgeArticleDtoListEnvelope>, Integer, Hash)> get_knowledge_articles_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve knowledge articles
  data, status_code, headers = api_instance.get_knowledge_articles_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <KnowledgeArticleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_knowledge_articles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**KnowledgeArticleDtoListEnvelope**](KnowledgeArticleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_knowledge_articles_count_async

> <Int32Envelope> get_knowledge_articles_count_async(tenant_id, opts)

Get knowledge articles count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get knowledge articles count
  result = api_instance.get_knowledge_articles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_knowledge_articles_count_async: #{e}"
end
```

#### Using the get_knowledge_articles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_knowledge_articles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get knowledge articles count
  data, status_code, headers = api_instance.get_knowledge_articles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_knowledge_articles_count_async_with_http_info: #{e}"
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


## get_maintenance_visit_async

> <MaintenanceVisitDtoEnvelope> get_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)

Retrieve a maintenance visit by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
maintenance_visit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a maintenance visit by ID
  result = api_instance.get_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_maintenance_visit_async: #{e}"
end
```

#### Using the get_maintenance_visit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MaintenanceVisitDtoEnvelope>, Integer, Hash)> get_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)

```ruby
begin
  # Retrieve a maintenance visit by ID
  data, status_code, headers = api_instance.get_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MaintenanceVisitDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_maintenance_visit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **maintenance_visit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MaintenanceVisitDtoEnvelope**](MaintenanceVisitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_maintenance_visits_async

> <MaintenanceVisitDtoListEnvelope> get_maintenance_visits_async(tenant_id, opts)

Retrieve maintenance visits

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve maintenance visits
  result = api_instance.get_maintenance_visits_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_maintenance_visits_async: #{e}"
end
```

#### Using the get_maintenance_visits_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MaintenanceVisitDtoListEnvelope>, Integer, Hash)> get_maintenance_visits_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve maintenance visits
  data, status_code, headers = api_instance.get_maintenance_visits_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MaintenanceVisitDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_maintenance_visits_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MaintenanceVisitDtoListEnvelope**](MaintenanceVisitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_maintenance_visits_count_async

> <Int32Envelope> get_maintenance_visits_count_async(tenant_id, opts)

Get maintenance visits count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get maintenance visits count
  result = api_instance.get_maintenance_visits_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_maintenance_visits_count_async: #{e}"
end
```

#### Using the get_maintenance_visits_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_maintenance_visits_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get maintenance visits count
  data, status_code, headers = api_instance.get_maintenance_visits_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_maintenance_visits_count_async_with_http_info: #{e}"
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


## get_refund_request_async

> <RefundRequestDtoEnvelope> get_refund_request_async(tenant_id, refund_request_id, opts)

Retrieve a refund request by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a refund request by ID
  result = api_instance.get_refund_request_async(tenant_id, refund_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_refund_request_async: #{e}"
end
```

#### Using the get_refund_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RefundRequestDtoEnvelope>, Integer, Hash)> get_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)

```ruby
begin
  # Retrieve a refund request by ID
  data, status_code, headers = api_instance.get_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RefundRequestDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_refund_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RefundRequestDtoEnvelope**](RefundRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_refund_requests_async

> <RefundRequestDtoListEnvelope> get_refund_requests_async(tenant_id, opts)

Retrieve refund requests

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve refund requests
  result = api_instance.get_refund_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_refund_requests_async: #{e}"
end
```

#### Using the get_refund_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RefundRequestDtoListEnvelope>, Integer, Hash)> get_refund_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve refund requests
  data, status_code, headers = api_instance.get_refund_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RefundRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_refund_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**RefundRequestDtoListEnvelope**](RefundRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_refund_requests_count_async

> <Int32Envelope> get_refund_requests_count_async(tenant_id, opts)

Get refund requests count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get refund requests count
  result = api_instance.get_refund_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_refund_requests_count_async: #{e}"
end
```

#### Using the get_refund_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_refund_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get refund requests count
  data, status_code, headers = api_instance.get_refund_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_refund_requests_count_async_with_http_info: #{e}"
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


## get_return_request_async

> <ReturnRequestDtoEnvelope> get_return_request_async(tenant_id, return_request_id, opts)

Retrieve a return request by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a return request by ID
  result = api_instance.get_return_request_async(tenant_id, return_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_return_request_async: #{e}"
end
```

#### Using the get_return_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ReturnRequestDtoEnvelope>, Integer, Hash)> get_return_request_async_with_http_info(tenant_id, return_request_id, opts)

```ruby
begin
  # Retrieve a return request by ID
  data, status_code, headers = api_instance.get_return_request_async_with_http_info(tenant_id, return_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ReturnRequestDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_return_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **return_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ReturnRequestDtoEnvelope**](ReturnRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_return_requests_async

> <ReturnRequestDtoListEnvelope> get_return_requests_async(tenant_id, opts)

Retrieve return requests

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve return requests
  result = api_instance.get_return_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_return_requests_async: #{e}"
end
```

#### Using the get_return_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ReturnRequestDtoListEnvelope>, Integer, Hash)> get_return_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve return requests
  data, status_code, headers = api_instance.get_return_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ReturnRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_return_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ReturnRequestDtoListEnvelope**](ReturnRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_return_requests_count_async

> <Int32Envelope> get_return_requests_count_async(tenant_id, opts)

Get return requests count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get return requests count
  result = api_instance.get_return_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_return_requests_count_async: #{e}"
end
```

#### Using the get_return_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_return_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get return requests count
  data, status_code, headers = api_instance.get_return_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_return_requests_count_async_with_http_info: #{e}"
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


## get_warranty_request_async

> <WarrantyRequestDtoEnvelope> get_warranty_request_async(tenant_id, warranty_request_id, opts)

Retrieve a warranty request by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a warranty request by ID
  result = api_instance.get_warranty_request_async(tenant_id, warranty_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_warranty_request_async: #{e}"
end
```

#### Using the get_warranty_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WarrantyRequestDtoEnvelope>, Integer, Hash)> get_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)

```ruby
begin
  # Retrieve a warranty request by ID
  data, status_code, headers = api_instance.get_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WarrantyRequestDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_warranty_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warranty_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WarrantyRequestDtoEnvelope**](WarrantyRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warranty_requests_async

> <WarrantyRequestDtoListEnvelope> get_warranty_requests_async(tenant_id, opts)

Retrieve warranty requests

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve warranty requests
  result = api_instance.get_warranty_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_warranty_requests_async: #{e}"
end
```

#### Using the get_warranty_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WarrantyRequestDtoListEnvelope>, Integer, Hash)> get_warranty_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve warranty requests
  data, status_code, headers = api_instance.get_warranty_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WarrantyRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_warranty_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WarrantyRequestDtoListEnvelope**](WarrantyRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warranty_requests_count_async

> <Int32Envelope> get_warranty_requests_count_async(tenant_id, opts)

Get warranty requests count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get warranty requests count
  result = api_instance.get_warranty_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_warranty_requests_count_async: #{e}"
end
```

#### Using the get_warranty_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_warranty_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get warranty requests count
  data, status_code, headers = api_instance.get_warranty_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->get_warranty_requests_count_async_with_http_info: #{e}"
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


## update_inquiry_request_async

> <EmptyEnvelope> update_inquiry_request_async(tenant_id, inquiry_request_id, opts)

Update an inquiry request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
inquiry_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  inquiry_request_update_dto: OpenapiClient::InquiryRequestUpdateDto.new # InquiryRequestUpdateDto | 
}

begin
  # Update an inquiry request
  result = api_instance.update_inquiry_request_async(tenant_id, inquiry_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_inquiry_request_async: #{e}"
end
```

#### Using the update_inquiry_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)

```ruby
begin
  # Update an inquiry request
  data, status_code, headers = api_instance.update_inquiry_request_async_with_http_info(tenant_id, inquiry_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_inquiry_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **inquiry_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **inquiry_request_update_dto** | [**InquiryRequestUpdateDto**](InquiryRequestUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_knowledge_article_async

> <EmptyEnvelope> update_knowledge_article_async(tenant_id, knowledge_article_id, opts)

Update a knowledge article

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
knowledge_article_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  knowledge_article_update_dto: OpenapiClient::KnowledgeArticleUpdateDto.new # KnowledgeArticleUpdateDto | 
}

begin
  # Update a knowledge article
  result = api_instance.update_knowledge_article_async(tenant_id, knowledge_article_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_knowledge_article_async: #{e}"
end
```

#### Using the update_knowledge_article_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)

```ruby
begin
  # Update a knowledge article
  data, status_code, headers = api_instance.update_knowledge_article_async_with_http_info(tenant_id, knowledge_article_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_knowledge_article_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **knowledge_article_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **knowledge_article_update_dto** | [**KnowledgeArticleUpdateDto**](KnowledgeArticleUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_maintenance_visit_async

> <EmptyEnvelope> update_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)

Update a maintenance visit

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
maintenance_visit_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  body: { ... } # Object | 
}

begin
  # Update a maintenance visit
  result = api_instance.update_maintenance_visit_async(tenant_id, maintenance_visit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_maintenance_visit_async: #{e}"
end
```

#### Using the update_maintenance_visit_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)

```ruby
begin
  # Update a maintenance visit
  data, status_code, headers = api_instance.update_maintenance_visit_async_with_http_info(tenant_id, maintenance_visit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_maintenance_visit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **maintenance_visit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **body** | **Object** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_refund_request_async

> <EmptyEnvelope> update_refund_request_async(tenant_id, refund_request_id, opts)

Update a refund request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
refund_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  refund_request_update_dto: OpenapiClient::RefundRequestUpdateDto.new # RefundRequestUpdateDto | 
}

begin
  # Update a refund request
  result = api_instance.update_refund_request_async(tenant_id, refund_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_refund_request_async: #{e}"
end
```

#### Using the update_refund_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)

```ruby
begin
  # Update a refund request
  data, status_code, headers = api_instance.update_refund_request_async_with_http_info(tenant_id, refund_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_refund_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **refund_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **refund_request_update_dto** | [**RefundRequestUpdateDto**](RefundRequestUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_return_request_async

> <EmptyEnvelope> update_return_request_async(tenant_id, return_request_id, opts)

Update a return request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
return_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  return_request_update_dto: OpenapiClient::ReturnRequestUpdateDto.new # ReturnRequestUpdateDto | 
}

begin
  # Update a return request
  result = api_instance.update_return_request_async(tenant_id, return_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_return_request_async: #{e}"
end
```

#### Using the update_return_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_return_request_async_with_http_info(tenant_id, return_request_id, opts)

```ruby
begin
  # Update a return request
  data, status_code, headers = api_instance.update_return_request_async_with_http_info(tenant_id, return_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_return_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **return_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **return_request_update_dto** | [**ReturnRequestUpdateDto**](ReturnRequestUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_warranty_request_async

> <EmptyEnvelope> update_warranty_request_async(tenant_id, warranty_request_id, opts)

Update a warranty request

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::HelpdeskApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warranty_request_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  warranty_request_update_dto: OpenapiClient::WarrantyRequestUpdateDto.new # WarrantyRequestUpdateDto | 
}

begin
  # Update a warranty request
  result = api_instance.update_warranty_request_async(tenant_id, warranty_request_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_warranty_request_async: #{e}"
end
```

#### Using the update_warranty_request_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)

```ruby
begin
  # Update a warranty request
  data, status_code, headers = api_instance.update_warranty_request_async_with_http_info(tenant_id, warranty_request_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling HelpdeskApi->update_warranty_request_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warranty_request_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **warranty_request_update_dto** | [**WarrantyRequestUpdateDto**](WarrantyRequestUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

