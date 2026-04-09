# OpenapiClient::InvoicesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**aggregate_invoice_discounts**](InvoicesApi.md#aggregate_invoice_discounts) | **POST** /api/v2/InvoicingService/Invoices/DiscountsAggregate | Aggregate invoice discounts. |
| [**aggregate_invoice_global_surcharges**](InvoicesApi.md#aggregate_invoice_global_surcharges) | **POST** /api/v2/InvoicingService/Invoices/GlobalSurchargesAggregate | Aggregate invoice global surcharges. |
| [**aggregate_invoice_tax_bases**](InvoicesApi.md#aggregate_invoice_tax_bases) | **POST** /api/v2/InvoicingService/Invoices/TaxBasesAggregate | Aggregate invoice tax bases. |
| [**aggregate_invoice_taxes**](InvoicesApi.md#aggregate_invoice_taxes) | **POST** /api/v2/InvoicingService/Invoices/TaxesAggregate | Aggregate invoice taxes. |
| [**aggregate_invoice_totals**](InvoicesApi.md#aggregate_invoice_totals) | **POST** /api/v2/InvoicingService/Invoices/TotalsAggregate | Aggregate invoice totals. |
| [**calculate_invoice**](InvoicesApi.md#calculate_invoice) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Calculate | Calculate an invoice. |
| [**calculate_invoice_line**](InvoicesApi.md#calculate_invoice_line) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Calculate | Calculate an invoice line. |
| [**create_invoice**](InvoicesApi.md#create_invoice) | **POST** /api/v2/InvoicingService/Invoices | Create a new invoice. |
| [**create_invoice_adjustment**](InvoicesApi.md#create_invoice_adjustment) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments | Create a new invoice adjustment. |
| [**create_invoice_line**](InvoicesApi.md#create_invoice_line) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines | Create a new invoice line. |
| [**create_invoice_line_tax**](InvoicesApi.md#create_invoice_line_tax) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes | Create a new tax for an invoice line. |
| [**create_invoice_reference**](InvoicesApi.md#create_invoice_reference) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/References | Create a new invoice reference. |
| [**delete_invoice**](InvoicesApi.md#delete_invoice) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId} | Delete an invoice. |
| [**delete_invoice_adjustment**](InvoicesApi.md#delete_invoice_adjustment) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments/{invoiceAdjustmentId} | Delete an invoice adjustment. |
| [**delete_invoice_line**](InvoicesApi.md#delete_invoice_line) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId} | Delete an invoice line. |
| [**delete_invoice_line_tax**](InvoicesApi.md#delete_invoice_line_tax) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes/{invoiceLineTaxId} | Delete a tax from an invoice line. |
| [**delete_invoice_reference**](InvoicesApi.md#delete_invoice_reference) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId}/References/{invoiceReferenceId} | Delete an invoice reference. |
| [**get_extended_invoice**](InvoicesApi.md#get_extended_invoice) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Extended | Get an extended invoice by ID. |
| [**get_extended_invoices**](InvoicesApi.md#get_extended_invoices) | **GET** /api/v2/InvoicingService/Invoices/Extended | Get a list of extended invoices. |
| [**get_extended_invoices_count**](InvoicesApi.md#get_extended_invoices_count) | **GET** /api/v2/InvoicingService/Invoices/Extended/Count | Get the count of extended invoices. |
| [**get_invoice**](InvoicesApi.md#get_invoice) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId} | Get an invoice by ID. |
| [**get_invoice_adjustment**](InvoicesApi.md#get_invoice_adjustment) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments/{invoiceAdjustmentId} | Get an invoice adjustment by ID. |
| [**get_invoice_adjustments**](InvoicesApi.md#get_invoice_adjustments) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments | Get invoice adjustments. |
| [**get_invoice_adjustments_count**](InvoicesApi.md#get_invoice_adjustments_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments/Count | Get the count of invoice adjustments. |
| [**get_invoice_line**](InvoicesApi.md#get_invoice_line) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId} | Get an invoice line by ID. |
| [**get_invoice_line_taxes**](InvoicesApi.md#get_invoice_line_taxes) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes | Get taxes for an invoice line. |
| [**get_invoice_line_taxes_count**](InvoicesApi.md#get_invoice_line_taxes_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes/Count | Get the count of taxes for an invoice line. |
| [**get_invoice_lines**](InvoicesApi.md#get_invoice_lines) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines | Get invoice lines. |
| [**get_invoice_lines_count**](InvoicesApi.md#get_invoice_lines_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/Count | Get the count of invoice lines. |
| [**get_invoice_payments**](InvoicesApi.md#get_invoice_payments) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Payments | Get payments for an invoice. |
| [**get_invoice_payments_count**](InvoicesApi.md#get_invoice_payments_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Payments/Count | Get the count of payments for an invoice. |
| [**get_invoice_reference**](InvoicesApi.md#get_invoice_reference) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/References/{invoiceReferenceId} | Get an invoice reference by ID. |
| [**get_invoice_references**](InvoicesApi.md#get_invoice_references) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/References | Get invoice references. |
| [**get_invoice_references_count**](InvoicesApi.md#get_invoice_references_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/References/Count | Get the count of invoice references. |
| [**get_invoices**](InvoicesApi.md#get_invoices) | **GET** /api/v2/InvoicingService/Invoices | Get a list of invoices. |
| [**get_invoices_count**](InvoicesApi.md#get_invoices_count) | **GET** /api/v2/InvoicingService/Invoices/Count | Get the count of invoices. |
| [**preview_invoice_email**](InvoicesApi.md#preview_invoice_email) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Emails/Preview | Preview the rendered email for an invoice. |
| [**send_invoice_email**](InvoicesApi.md#send_invoice_email) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Emails/Send | Send an invoice transactional email to recipients. |
| [**update_invoice**](InvoicesApi.md#update_invoice) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId} | Update an invoice. |
| [**update_invoice_adjustment**](InvoicesApi.md#update_invoice_adjustment) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments/{invoiceAdjustmentId} | Update an invoice adjustment. |
| [**update_invoice_line**](InvoicesApi.md#update_invoice_line) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId} | Update an invoice line. |
| [**update_invoice_line_tax**](InvoicesApi.md#update_invoice_line_tax) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes/{invoiceLineTaxId} | Update a tax for an invoice line. |
| [**update_invoice_reference**](InvoicesApi.md#update_invoice_reference) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/References/{invoiceReferenceId} | Update an invoice reference. |


## aggregate_invoice_discounts

> <MoneyEnvelope> aggregate_invoice_discounts(request_body, opts)

Aggregate invoice discounts.

Aggregates the discounts for the specified invoices.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
request_body = ['property_example'] # Array<String> | 
opts = {
  currency_id: 'currency_id_example' # String | 
}

begin
  # Aggregate invoice discounts.
  result = api_instance.aggregate_invoice_discounts(request_body, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_discounts: #{e}"
end
```

#### Using the aggregate_invoice_discounts_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> aggregate_invoice_discounts_with_http_info(request_body, opts)

```ruby
begin
  # Aggregate invoice discounts.
  data, status_code, headers = api_instance.aggregate_invoice_discounts_with_http_info(request_body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_discounts_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **request_body** | [**Array&lt;String&gt;**](String.md) |  |  |
| **currency_id** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## aggregate_invoice_global_surcharges

> <MoneyEnvelope> aggregate_invoice_global_surcharges(request_body, opts)

Aggregate invoice global surcharges.

Aggregates the global surcharges for the specified invoices.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
request_body = ['property_example'] # Array<String> | 
opts = {
  currency_id: 'currency_id_example' # String | 
}

begin
  # Aggregate invoice global surcharges.
  result = api_instance.aggregate_invoice_global_surcharges(request_body, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_global_surcharges: #{e}"
end
```

#### Using the aggregate_invoice_global_surcharges_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> aggregate_invoice_global_surcharges_with_http_info(request_body, opts)

```ruby
begin
  # Aggregate invoice global surcharges.
  data, status_code, headers = api_instance.aggregate_invoice_global_surcharges_with_http_info(request_body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_global_surcharges_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **request_body** | [**Array&lt;String&gt;**](String.md) |  |  |
| **currency_id** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## aggregate_invoice_tax_bases

> <MoneyEnvelope> aggregate_invoice_tax_bases(request_body, opts)

Aggregate invoice tax bases.

Aggregates the tax bases for the specified invoices.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
request_body = ['property_example'] # Array<String> | 
opts = {
  currency_id: 'currency_id_example' # String | 
}

begin
  # Aggregate invoice tax bases.
  result = api_instance.aggregate_invoice_tax_bases(request_body, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_tax_bases: #{e}"
end
```

#### Using the aggregate_invoice_tax_bases_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> aggregate_invoice_tax_bases_with_http_info(request_body, opts)

```ruby
begin
  # Aggregate invoice tax bases.
  data, status_code, headers = api_instance.aggregate_invoice_tax_bases_with_http_info(request_body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_tax_bases_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **request_body** | [**Array&lt;String&gt;**](String.md) |  |  |
| **currency_id** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## aggregate_invoice_taxes

> <MoneyEnvelope> aggregate_invoice_taxes(request_body, opts)

Aggregate invoice taxes.

Aggregates the taxes for the specified invoices.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
request_body = ['property_example'] # Array<String> | 
opts = {
  currency_id: 'currency_id_example' # String | 
}

begin
  # Aggregate invoice taxes.
  result = api_instance.aggregate_invoice_taxes(request_body, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_taxes: #{e}"
end
```

#### Using the aggregate_invoice_taxes_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> aggregate_invoice_taxes_with_http_info(request_body, opts)

```ruby
begin
  # Aggregate invoice taxes.
  data, status_code, headers = api_instance.aggregate_invoice_taxes_with_http_info(request_body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_taxes_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **request_body** | [**Array&lt;String&gt;**](String.md) |  |  |
| **currency_id** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## aggregate_invoice_totals

> <MoneyEnvelope> aggregate_invoice_totals(request_body, opts)

Aggregate invoice totals.

Aggregates the totals for the specified invoices.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
request_body = ['property_example'] # Array<String> | 
opts = {
  currency_id: 'currency_id_example' # String | 
}

begin
  # Aggregate invoice totals.
  result = api_instance.aggregate_invoice_totals(request_body, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_totals: #{e}"
end
```

#### Using the aggregate_invoice_totals_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> aggregate_invoice_totals_with_http_info(request_body, opts)

```ruby
begin
  # Aggregate invoice totals.
  data, status_code, headers = api_instance.aggregate_invoice_totals_with_http_info(request_body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->aggregate_invoice_totals_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **request_body** | [**Array&lt;String&gt;**](String.md) |  |  |
| **currency_id** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## calculate_invoice

> <EmptyEnvelope> calculate_invoice(tenant_id, invoice_id)

Calculate an invoice.

Calculates the totals and taxes for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Calculate an invoice.
  result = api_instance.calculate_invoice(tenant_id, invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->calculate_invoice: #{e}"
end
```

#### Using the calculate_invoice_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> calculate_invoice_with_http_info(tenant_id, invoice_id)

```ruby
begin
  # Calculate an invoice.
  data, status_code, headers = api_instance.calculate_invoice_with_http_info(tenant_id, invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->calculate_invoice_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## calculate_invoice_line

> <EmptyEnvelope> calculate_invoice_line(tenant_id, invoice_id, invoice_line_id)

Calculate an invoice line.

Calculates the totals and taxes for the specified invoice line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Calculate an invoice line.
  result = api_instance.calculate_invoice_line(tenant_id, invoice_id, invoice_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->calculate_invoice_line: #{e}"
end
```

#### Using the calculate_invoice_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> calculate_invoice_line_with_http_info(tenant_id, invoice_id, invoice_line_id)

```ruby
begin
  # Calculate an invoice line.
  data, status_code, headers = api_instance.calculate_invoice_line_with_http_info(tenant_id, invoice_id, invoice_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->calculate_invoice_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_invoice

> <EmptyEnvelope> create_invoice(tenant_id, opts)

Create a new invoice.

Creates a new invoice for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_create_dto: OpenapiClient::InvoiceCreateDto.new # InvoiceCreateDto | 
}

begin
  # Create a new invoice.
  result = api_instance.create_invoice(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice: #{e}"
end
```

#### Using the create_invoice_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_invoice_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new invoice.
  data, status_code, headers = api_instance.create_invoice_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_create_dto** | [**InvoiceCreateDto**](InvoiceCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_invoice_adjustment

> <EmptyEnvelope> create_invoice_adjustment(tenant_id, invoice_id, opts)

Create a new invoice adjustment.

Creates a new adjustment for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_adjustment_create_dto: OpenapiClient::InvoiceAdjustmentCreateDto.new # InvoiceAdjustmentCreateDto | 
}

begin
  # Create a new invoice adjustment.
  result = api_instance.create_invoice_adjustment(tenant_id, invoice_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice_adjustment: #{e}"
end
```

#### Using the create_invoice_adjustment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_invoice_adjustment_with_http_info(tenant_id, invoice_id, opts)

```ruby
begin
  # Create a new invoice adjustment.
  data, status_code, headers = api_instance.create_invoice_adjustment_with_http_info(tenant_id, invoice_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice_adjustment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_adjustment_create_dto** | [**InvoiceAdjustmentCreateDto**](InvoiceAdjustmentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_invoice_line

> <InvoiceLineDtoIReadOnlyListEnvelope> create_invoice_line(tenant_id, invoice_id, opts)

Create a new invoice line.

Creates a new invoice line for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_line_create_dto: OpenapiClient::InvoiceLineCreateDto.new # InvoiceLineCreateDto | 
}

begin
  # Create a new invoice line.
  result = api_instance.create_invoice_line(tenant_id, invoice_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice_line: #{e}"
end
```

#### Using the create_invoice_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceLineDtoIReadOnlyListEnvelope>, Integer, Hash)> create_invoice_line_with_http_info(tenant_id, invoice_id, opts)

```ruby
begin
  # Create a new invoice line.
  data, status_code, headers = api_instance.create_invoice_line_with_http_info(tenant_id, invoice_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceLineDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_create_dto** | [**InvoiceLineCreateDto**](InvoiceLineCreateDto.md) |  | [optional] |

### Return type

[**InvoiceLineDtoIReadOnlyListEnvelope**](InvoiceLineDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_invoice_line_tax

> <EmptyEnvelope> create_invoice_line_tax(tenant_id, invoice_id, invoice_line_id, opts)

Create a new tax for an invoice line.

Creates a new tax entry for the specified invoice line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_line_applied_tax_create_dto: OpenapiClient::InvoiceLineAppliedTaxCreateDto.new # InvoiceLineAppliedTaxCreateDto | 
}

begin
  # Create a new tax for an invoice line.
  result = api_instance.create_invoice_line_tax(tenant_id, invoice_id, invoice_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice_line_tax: #{e}"
end
```

#### Using the create_invoice_line_tax_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_invoice_line_tax_with_http_info(tenant_id, invoice_id, invoice_line_id, opts)

```ruby
begin
  # Create a new tax for an invoice line.
  data, status_code, headers = api_instance.create_invoice_line_tax_with_http_info(tenant_id, invoice_id, invoice_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice_line_tax_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_id** | **String** |  |  |
| **invoice_line_applied_tax_create_dto** | [**InvoiceLineAppliedTaxCreateDto**](InvoiceLineAppliedTaxCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_invoice_reference

> <EmptyEnvelope> create_invoice_reference(tenant_id, invoice_id, opts)

Create a new invoice reference.

Creates a new reference for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_reference_create_dto: OpenapiClient::InvoiceReferenceCreateDto.new # InvoiceReferenceCreateDto | 
}

begin
  # Create a new invoice reference.
  result = api_instance.create_invoice_reference(tenant_id, invoice_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice_reference: #{e}"
end
```

#### Using the create_invoice_reference_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_invoice_reference_with_http_info(tenant_id, invoice_id, opts)

```ruby
begin
  # Create a new invoice reference.
  data, status_code, headers = api_instance.create_invoice_reference_with_http_info(tenant_id, invoice_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->create_invoice_reference_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_reference_create_dto** | [**InvoiceReferenceCreateDto**](InvoiceReferenceCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_invoice

> <EmptyEnvelope> delete_invoice(tenant_id, invoice_id)

Delete an invoice.

Deletes the specified invoice for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete an invoice.
  result = api_instance.delete_invoice(tenant_id, invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice: #{e}"
end
```

#### Using the delete_invoice_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_invoice_with_http_info(tenant_id, invoice_id)

```ruby
begin
  # Delete an invoice.
  data, status_code, headers = api_instance.delete_invoice_with_http_info(tenant_id, invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_invoice_adjustment

> <EmptyEnvelope> delete_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_id)

Delete an invoice adjustment.

Deletes the specified adjustment from the invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_adjustment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete an invoice adjustment.
  result = api_instance.delete_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice_adjustment: #{e}"
end
```

#### Using the delete_invoice_adjustment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_invoice_adjustment_with_http_info(tenant_id, invoice_id, invoice_adjustment_id)

```ruby
begin
  # Delete an invoice adjustment.
  data, status_code, headers = api_instance.delete_invoice_adjustment_with_http_info(tenant_id, invoice_id, invoice_adjustment_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice_adjustment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_adjustment_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_invoice_line

> <EmptyEnvelope> delete_invoice_line(tenant_id, invoice_id, invoice_line_id)

Delete an invoice line.

Deletes the specified invoice line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete an invoice line.
  result = api_instance.delete_invoice_line(tenant_id, invoice_id, invoice_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice_line: #{e}"
end
```

#### Using the delete_invoice_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_invoice_line_with_http_info(tenant_id, invoice_id, invoice_line_id)

```ruby
begin
  # Delete an invoice line.
  data, status_code, headers = api_instance.delete_invoice_line_with_http_info(tenant_id, invoice_id, invoice_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_invoice_line_tax

> <EmptyEnvelope> delete_invoice_line_tax(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id)

Delete a tax from an invoice line.

Deletes the specified tax entry from the invoice line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_tax_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a tax from an invoice line.
  result = api_instance.delete_invoice_line_tax(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice_line_tax: #{e}"
end
```

#### Using the delete_invoice_line_tax_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_invoice_line_tax_with_http_info(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id)

```ruby
begin
  # Delete a tax from an invoice line.
  data, status_code, headers = api_instance.delete_invoice_line_tax_with_http_info(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice_line_tax_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_id** | **String** |  |  |
| **invoice_line_tax_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_invoice_reference

> <EmptyEnvelope> delete_invoice_reference(tenant_id, invoice_id, invoice_reference_id)

Delete an invoice reference.

Deletes the specified reference from the invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_reference_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete an invoice reference.
  result = api_instance.delete_invoice_reference(tenant_id, invoice_id, invoice_reference_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice_reference: #{e}"
end
```

#### Using the delete_invoice_reference_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_invoice_reference_with_http_info(tenant_id, invoice_id, invoice_reference_id)

```ruby
begin
  # Delete an invoice reference.
  data, status_code, headers = api_instance.delete_invoice_reference_with_http_info(tenant_id, invoice_id, invoice_reference_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->delete_invoice_reference_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_reference_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_invoice

> <InvoiceDtoEnvelope> get_extended_invoice(tenant_id, invoice_id)

Get an extended invoice by ID.

Retrieves the extended invoice details for the specified invoice ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get an extended invoice by ID.
  result = api_instance.get_extended_invoice(tenant_id, invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_extended_invoice: #{e}"
end
```

#### Using the get_extended_invoice_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceDtoEnvelope>, Integer, Hash)> get_extended_invoice_with_http_info(tenant_id, invoice_id)

```ruby
begin
  # Get an extended invoice by ID.
  data, status_code, headers = api_instance.get_extended_invoice_with_http_info(tenant_id, invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_extended_invoice_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |

### Return type

[**InvoiceDtoEnvelope**](InvoiceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_invoices

> <ExtendedInvoiceDtoListEnvelope> get_extended_invoices(tenant_id)

Get a list of extended invoices.

Retrieves a list of extended invoice details for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get a list of extended invoices.
  result = api_instance.get_extended_invoices(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_extended_invoices: #{e}"
end
```

#### Using the get_extended_invoices_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedInvoiceDtoListEnvelope>, Integer, Hash)> get_extended_invoices_with_http_info(tenant_id)

```ruby
begin
  # Get a list of extended invoices.
  data, status_code, headers = api_instance.get_extended_invoices_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedInvoiceDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_extended_invoices_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**ExtendedInvoiceDtoListEnvelope**](ExtendedInvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_invoices_count

> <Int32Envelope> get_extended_invoices_count(tenant_id)

Get the count of extended invoices.

Retrieves the total count of extended invoices for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get the count of extended invoices.
  result = api_instance.get_extended_invoices_count(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_extended_invoices_count: #{e}"
end
```

#### Using the get_extended_invoices_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_extended_invoices_count_with_http_info(tenant_id)

```ruby
begin
  # Get the count of extended invoices.
  data, status_code, headers = api_instance.get_extended_invoices_count_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_extended_invoices_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice

> <InvoiceDtoEnvelope> get_invoice(tenant_id, invoice_id)

Get an invoice by ID.

Retrieves the invoice details for the specified invoice ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get an invoice by ID.
  result = api_instance.get_invoice(tenant_id, invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice: #{e}"
end
```

#### Using the get_invoice_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceDtoEnvelope>, Integer, Hash)> get_invoice_with_http_info(tenant_id, invoice_id)

```ruby
begin
  # Get an invoice by ID.
  data, status_code, headers = api_instance.get_invoice_with_http_info(tenant_id, invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |

### Return type

[**InvoiceDtoEnvelope**](InvoiceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_adjustment

> <InvoiceAdjustmentDtoEnvelope> get_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_id)

Get an invoice adjustment by ID.

Retrieves the adjustment details for the specified invoice adjustment ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_adjustment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get an invoice adjustment by ID.
  result = api_instance.get_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_adjustment: #{e}"
end
```

#### Using the get_invoice_adjustment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceAdjustmentDtoEnvelope>, Integer, Hash)> get_invoice_adjustment_with_http_info(tenant_id, invoice_id, invoice_adjustment_id)

```ruby
begin
  # Get an invoice adjustment by ID.
  data, status_code, headers = api_instance.get_invoice_adjustment_with_http_info(tenant_id, invoice_id, invoice_adjustment_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceAdjustmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_adjustment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_adjustment_id** | **String** |  |  |

### Return type

[**InvoiceAdjustmentDtoEnvelope**](InvoiceAdjustmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_adjustments

> <InvoiceAdjustmentDtoIReadOnlyListEnvelope> get_invoice_adjustments(tenant_id, invoice_id)

Get invoice adjustments.

Retrieves the adjustments for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get invoice adjustments.
  result = api_instance.get_invoice_adjustments(tenant_id, invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_adjustments: #{e}"
end
```

#### Using the get_invoice_adjustments_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceAdjustmentDtoIReadOnlyListEnvelope>, Integer, Hash)> get_invoice_adjustments_with_http_info(tenant_id, invoice_id)

```ruby
begin
  # Get invoice adjustments.
  data, status_code, headers = api_instance.get_invoice_adjustments_with_http_info(tenant_id, invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceAdjustmentDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_adjustments_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |

### Return type

[**InvoiceAdjustmentDtoIReadOnlyListEnvelope**](InvoiceAdjustmentDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_adjustments_count

> <Int32Envelope> get_invoice_adjustments_count(tenant_id, invoice_id)

Get the count of invoice adjustments.

Retrieves the total count of adjustments for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get the count of invoice adjustments.
  result = api_instance.get_invoice_adjustments_count(tenant_id, invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_adjustments_count: #{e}"
end
```

#### Using the get_invoice_adjustments_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_invoice_adjustments_count_with_http_info(tenant_id, invoice_id)

```ruby
begin
  # Get the count of invoice adjustments.
  data, status_code, headers = api_instance.get_invoice_adjustments_count_with_http_info(tenant_id, invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_adjustments_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_line

> <InvoiceLineDtoEnvelope> get_invoice_line(tenant_id, invoice_id, invoice_line_id)

Get an invoice line by ID.

Retrieves the invoice line details for the specified invoice line ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get an invoice line by ID.
  result = api_instance.get_invoice_line(tenant_id, invoice_id, invoice_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_line: #{e}"
end
```

#### Using the get_invoice_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceLineDtoEnvelope>, Integer, Hash)> get_invoice_line_with_http_info(tenant_id, invoice_id, invoice_line_id)

```ruby
begin
  # Get an invoice line by ID.
  data, status_code, headers = api_instance.get_invoice_line_with_http_info(tenant_id, invoice_id, invoice_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceLineDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_id** | **String** |  |  |

### Return type

[**InvoiceLineDtoEnvelope**](InvoiceLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_line_taxes

> <InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope> get_invoice_line_taxes(tenant_id, invoice_id, invoice_line_id)

Get taxes for an invoice line.

Retrieves the taxes applied to the specified invoice line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get taxes for an invoice line.
  result = api_instance.get_invoice_line_taxes(tenant_id, invoice_id, invoice_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_line_taxes: #{e}"
end
```

#### Using the get_invoice_line_taxes_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope>, Integer, Hash)> get_invoice_line_taxes_with_http_info(tenant_id, invoice_id, invoice_line_id)

```ruby
begin
  # Get taxes for an invoice line.
  data, status_code, headers = api_instance.get_invoice_line_taxes_with_http_info(tenant_id, invoice_id, invoice_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_line_taxes_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_id** | **String** |  |  |

### Return type

[**InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope**](InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_line_taxes_count

> <Int32Envelope> get_invoice_line_taxes_count(tenant_id, invoice_id, invoice_line_id)

Get the count of taxes for an invoice line.

Retrieves the total count of taxes applied to the specified invoice line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get the count of taxes for an invoice line.
  result = api_instance.get_invoice_line_taxes_count(tenant_id, invoice_id, invoice_line_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_line_taxes_count: #{e}"
end
```

#### Using the get_invoice_line_taxes_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_invoice_line_taxes_count_with_http_info(tenant_id, invoice_id, invoice_line_id)

```ruby
begin
  # Get the count of taxes for an invoice line.
  data, status_code, headers = api_instance.get_invoice_line_taxes_count_with_http_info(tenant_id, invoice_id, invoice_line_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_line_taxes_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_lines

> <InvoiceLineDtoListEnvelope> get_invoice_lines(tenant_id, invoice_id, opts)

Get invoice lines.

Retrieves the invoice lines for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
}

begin
  # Get invoice lines.
  result = api_instance.get_invoice_lines(tenant_id, invoice_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_lines: #{e}"
end
```

#### Using the get_invoice_lines_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceLineDtoListEnvelope>, Integer, Hash)> get_invoice_lines_with_http_info(tenant_id, invoice_id, opts)

```ruby
begin
  # Get invoice lines.
  data, status_code, headers = api_instance.get_invoice_lines_with_http_info(tenant_id, invoice_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceLineDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_lines_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **item_id** | **String** |  | [optional] |

### Return type

[**InvoiceLineDtoListEnvelope**](InvoiceLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_lines_count

> <Int32Envelope> get_invoice_lines_count(tenant_id, invoice_id)

Get the count of invoice lines.

Retrieves the total count of invoice lines for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get the count of invoice lines.
  result = api_instance.get_invoice_lines_count(tenant_id, invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_lines_count: #{e}"
end
```

#### Using the get_invoice_lines_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_invoice_lines_count_with_http_info(tenant_id, invoice_id)

```ruby
begin
  # Get the count of invoice lines.
  data, status_code, headers = api_instance.get_invoice_lines_count_with_http_info(tenant_id, invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_lines_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_payments

> <PaymentDtoIReadOnlyListEnvelope> get_invoice_payments(invoice_id)

Get payments for an invoice.

Retrieves the list of payments related to the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get payments for an invoice.
  result = api_instance.get_invoice_payments(invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_payments: #{e}"
end
```

#### Using the get_invoice_payments_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaymentDtoIReadOnlyListEnvelope>, Integer, Hash)> get_invoice_payments_with_http_info(invoice_id)

```ruby
begin
  # Get payments for an invoice.
  data, status_code, headers = api_instance.get_invoice_payments_with_http_info(invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaymentDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_payments_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **invoice_id** | **String** |  |  |

### Return type

[**PaymentDtoIReadOnlyListEnvelope**](PaymentDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_payments_count

> <Int32Envelope> get_invoice_payments_count(invoice_id)

Get the count of payments for an invoice.

Retrieves the total count of payments for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get the count of payments for an invoice.
  result = api_instance.get_invoice_payments_count(invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_payments_count: #{e}"
end
```

#### Using the get_invoice_payments_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_invoice_payments_count_with_http_info(invoice_id)

```ruby
begin
  # Get the count of payments for an invoice.
  data, status_code, headers = api_instance.get_invoice_payments_count_with_http_info(invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_payments_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **invoice_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_reference

> <InvoiceReferenceDtoEnvelope> get_invoice_reference(tenant_id, invoice_id, invoice_reference_id)

Get an invoice reference by ID.

Retrieves the reference details for the specified invoice reference ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_reference_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get an invoice reference by ID.
  result = api_instance.get_invoice_reference(tenant_id, invoice_id, invoice_reference_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_reference: #{e}"
end
```

#### Using the get_invoice_reference_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceReferenceDtoEnvelope>, Integer, Hash)> get_invoice_reference_with_http_info(tenant_id, invoice_id, invoice_reference_id)

```ruby
begin
  # Get an invoice reference by ID.
  data, status_code, headers = api_instance.get_invoice_reference_with_http_info(tenant_id, invoice_id, invoice_reference_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceReferenceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_reference_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_reference_id** | **String** |  |  |

### Return type

[**InvoiceReferenceDtoEnvelope**](InvoiceReferenceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_references

> <InvoiceReferenceDtoIReadOnlyListEnvelope> get_invoice_references(tenant_id, invoice_id)

Get invoice references.

Retrieves the references for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get invoice references.
  result = api_instance.get_invoice_references(tenant_id, invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_references: #{e}"
end
```

#### Using the get_invoice_references_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceReferenceDtoIReadOnlyListEnvelope>, Integer, Hash)> get_invoice_references_with_http_info(tenant_id, invoice_id)

```ruby
begin
  # Get invoice references.
  data, status_code, headers = api_instance.get_invoice_references_with_http_info(tenant_id, invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceReferenceDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_references_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |

### Return type

[**InvoiceReferenceDtoIReadOnlyListEnvelope**](InvoiceReferenceDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoice_references_count

> <Int32Envelope> get_invoice_references_count(tenant_id, invoice_id)

Get the count of invoice references.

Retrieves the total count of references for the specified invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get the count of invoice references.
  result = api_instance.get_invoice_references_count(tenant_id, invoice_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_references_count: #{e}"
end
```

#### Using the get_invoice_references_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_invoice_references_count_with_http_info(tenant_id, invoice_id)

```ruby
begin
  # Get the count of invoice references.
  data, status_code, headers = api_instance.get_invoice_references_count_with_http_info(tenant_id, invoice_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoice_references_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoices

> <InvoiceDtoListEnvelope> get_invoices(tenant_id)

Get a list of invoices.

Retrieves a list of invoices for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get a list of invoices.
  result = api_instance.get_invoices(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoices: #{e}"
end
```

#### Using the get_invoices_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceDtoListEnvelope>, Integer, Hash)> get_invoices_with_http_info(tenant_id)

```ruby
begin
  # Get a list of invoices.
  data, status_code, headers = api_instance.get_invoices_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoices_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**InvoiceDtoListEnvelope**](InvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_invoices_count

> <Int32Envelope> get_invoices_count(tenant_id)

Get the count of invoices.

Retrieves the total count of invoices for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get the count of invoices.
  result = api_instance.get_invoices_count(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoices_count: #{e}"
end
```

#### Using the get_invoices_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_invoices_count_with_http_info(tenant_id)

```ruby
begin
  # Get the count of invoices.
  data, status_code, headers = api_instance.get_invoices_count_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->get_invoices_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## preview_invoice_email

> preview_invoice_email(invoice_id, tenant_id, opts)

Preview the rendered email for an invoice.

This action is only available for users with the 'send_email' permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Preview the rendered email for an invoice.
  api_instance.preview_invoice_email(invoice_id, tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->preview_invoice_email: #{e}"
end
```

#### Using the preview_invoice_email_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> preview_invoice_email_with_http_info(invoice_id, tenant_id, opts)

```ruby
begin
  # Preview the rendered email for an invoice.
  data, status_code, headers = api_instance.preview_invoice_email_with_http_info(invoice_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->preview_invoice_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **invoice_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined


## send_invoice_email

> <Envelope> send_invoice_email(tenant_id, invoice_id, opts)

Send an invoice transactional email to recipients.

This action is only available for users with the 'send_email' permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Send an invoice transactional email to recipients.
  result = api_instance.send_invoice_email(tenant_id, invoice_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->send_invoice_email: #{e}"
end
```

#### Using the send_invoice_email_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> send_invoice_email_with_http_info(tenant_id, invoice_id, opts)

```ruby
begin
  # Send an invoice transactional email to recipients.
  data, status_code, headers = api_instance.send_invoice_email_with_http_info(tenant_id, invoice_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->send_invoice_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_invoice

> <EmptyEnvelope> update_invoice(tenant_id, invoice_id, opts)

Update an invoice.

Updates the specified invoice for the tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_update_dto: OpenapiClient::InvoiceUpdateDto.new # InvoiceUpdateDto | 
}

begin
  # Update an invoice.
  result = api_instance.update_invoice(tenant_id, invoice_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice: #{e}"
end
```

#### Using the update_invoice_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_invoice_with_http_info(tenant_id, invoice_id, opts)

```ruby
begin
  # Update an invoice.
  data, status_code, headers = api_instance.update_invoice_with_http_info(tenant_id, invoice_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_update_dto** | [**InvoiceUpdateDto**](InvoiceUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_invoice_adjustment

> <EmptyEnvelope> update_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_id, opts)

Update an invoice adjustment.

Updates the specified adjustment for the invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_adjustment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_adjustment_update_dto: OpenapiClient::InvoiceAdjustmentUpdateDto.new # InvoiceAdjustmentUpdateDto | 
}

begin
  # Update an invoice adjustment.
  result = api_instance.update_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice_adjustment: #{e}"
end
```

#### Using the update_invoice_adjustment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_invoice_adjustment_with_http_info(tenant_id, invoice_id, invoice_adjustment_id, opts)

```ruby
begin
  # Update an invoice adjustment.
  data, status_code, headers = api_instance.update_invoice_adjustment_with_http_info(tenant_id, invoice_id, invoice_adjustment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice_adjustment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_adjustment_id** | **String** |  |  |
| **invoice_adjustment_update_dto** | [**InvoiceAdjustmentUpdateDto**](InvoiceAdjustmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_invoice_line

> <InvoiceLineDtoEnvelope> update_invoice_line(tenant_id, invoice_id, invoice_line_id, opts)

Update an invoice line.

Updates the specified invoice line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_line_update_dto: OpenapiClient::InvoiceLineUpdateDto.new # InvoiceLineUpdateDto | 
}

begin
  # Update an invoice line.
  result = api_instance.update_invoice_line(tenant_id, invoice_id, invoice_line_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice_line: #{e}"
end
```

#### Using the update_invoice_line_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InvoiceLineDtoEnvelope>, Integer, Hash)> update_invoice_line_with_http_info(tenant_id, invoice_id, invoice_line_id, opts)

```ruby
begin
  # Update an invoice line.
  data, status_code, headers = api_instance.update_invoice_line_with_http_info(tenant_id, invoice_id, invoice_line_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InvoiceLineDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice_line_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_id** | **String** |  |  |
| **invoice_line_update_dto** | [**InvoiceLineUpdateDto**](InvoiceLineUpdateDto.md) |  | [optional] |

### Return type

[**InvoiceLineDtoEnvelope**](InvoiceLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_invoice_line_tax

> <EmptyEnvelope> update_invoice_line_tax(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id, opts)

Update a tax for an invoice line.

Updates the specified tax entry for the invoice line.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_line_tax_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_line_applied_tax_update_dto: OpenapiClient::InvoiceLineAppliedTaxUpdateDto.new # InvoiceLineAppliedTaxUpdateDto | 
}

begin
  # Update a tax for an invoice line.
  result = api_instance.update_invoice_line_tax(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice_line_tax: #{e}"
end
```

#### Using the update_invoice_line_tax_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_invoice_line_tax_with_http_info(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id, opts)

```ruby
begin
  # Update a tax for an invoice line.
  data, status_code, headers = api_instance.update_invoice_line_tax_with_http_info(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice_line_tax_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_line_id** | **String** |  |  |
| **invoice_line_tax_id** | **String** |  |  |
| **invoice_line_applied_tax_update_dto** | [**InvoiceLineAppliedTaxUpdateDto**](InvoiceLineAppliedTaxUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_invoice_reference

> <EmptyEnvelope> update_invoice_reference(tenant_id, invoice_id, invoice_reference_id, opts)

Update an invoice reference.

Updates the specified reference for the invoice.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InvoicesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
invoice_reference_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  invoice_reference_update_dto: OpenapiClient::InvoiceReferenceUpdateDto.new # InvoiceReferenceUpdateDto | 
}

begin
  # Update an invoice reference.
  result = api_instance.update_invoice_reference(tenant_id, invoice_id, invoice_reference_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice_reference: #{e}"
end
```

#### Using the update_invoice_reference_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_invoice_reference_with_http_info(tenant_id, invoice_id, invoice_reference_id, opts)

```ruby
begin
  # Update an invoice reference.
  data, status_code, headers = api_instance.update_invoice_reference_with_http_info(tenant_id, invoice_id, invoice_reference_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InvoicesApi->update_invoice_reference_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **invoice_id** | **String** |  |  |
| **invoice_reference_id** | **String** |  |  |
| **invoice_reference_update_dto** | [**InvoiceReferenceUpdateDto**](InvoiceReferenceUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

