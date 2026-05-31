# OpenapiClient::ExtendedSalesLiteratureDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  | [optional] |
| **content** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **modified_date** | **Time** |  | [optional] |
| **expiration_date** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **sales_literature_type_id** | **String** |  | [optional] |
| **sales_literature_type** | [**SalesLiteratureTypeDto**](SalesLiteratureTypeDto.md) |  | [optional] |
| **tenant** | [**TenantDto**](TenantDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ExtendedSalesLiteratureDto.new(
  id: null,
  timestamp: null,
  title: null,
  content: null,
  description: null,
  modified_date: null,
  expiration_date: null,
  tenant_id: null,
  enrollment_id: null,
  sales_literature_type_id: null,
  sales_literature_type: null,
  tenant: null
)
```

