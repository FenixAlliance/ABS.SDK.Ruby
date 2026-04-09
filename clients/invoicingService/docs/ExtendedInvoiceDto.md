# OpenapiClient::ExtendedInvoiceDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **closed** | **Boolean** |  | [optional] |
| **type** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **user_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **price_list_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **individual_id** | **String** |  | [optional] |
| **organization_id** | **String** |  | [optional] |
| **receiver_tenant_id** | **String** |  | [optional] |
| **first_name** | **String** |  | [optional] |
| **last_name** | **String** |  | [optional] |
| **company_name** | **String** |  | [optional] |
| **billing_email** | **String** |  | [optional] |
| **address_line1** | **String** |  | [optional] |
| **address_line2** | **String** |  | [optional] |
| **postal_code** | **String** |  | [optional] |
| **country_id** | **String** |  | [optional] |
| **state_id** | **String** |  | [optional] |
| **city_id** | **String** |  | [optional] |
| **customer_notes** | **String** |  | [optional] |
| **tax_calculation_method** | **String** |  | [optional] |
| **cost_calculation_method** | **String** |  | [optional] |
| **forex_rate** | **Float** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **total_detail** | **Float** |  | [optional] |
| **total_detail_currency_id** | **String** |  | [optional] |
| **total_profit** | **Float** |  | [optional] |
| **total_profit_currency_id** | **String** |  | [optional] |
| **total_discounts** | **Float** |  | [optional] |
| **total_discounts_currency_id** | **String** |  | [optional] |
| **total_surcharges** | **Float** |  | [optional] |
| **total_surcharges_currency_id** | **String** |  | [optional] |
| **total_tax_base** | **Float** |  | [optional] |
| **total_tax_base_currency_id** | **String** |  | [optional] |
| **total_taxes** | **Float** |  | [optional] |
| **total_taxes_currency_id** | **String** |  | [optional] |
| **total_shipping_cost** | **Float** |  | [optional] |
| **total_shipping_cost_currency_id** | **String** |  | [optional] |
| **total_shipping_tax** | **Float** |  | [optional] |
| **total_shipping_tax_currency_id** | **String** |  | [optional] |
| **total_withheld_tax** | **Float** |  | [optional] |
| **total_withheld_tax_currency_id** | **String** |  | [optional] |
| **total_global_discounts** | **Float** |  | [optional] |
| **total_global_discounts_currency_id** | **String** |  | [optional] |
| **total_global_surcharges** | **Float** |  | [optional] |
| **total_global_surcharges_currency_id** | **String** |  | [optional] |
| **total** | **Float** |  | [optional] |
| **total_currency_id** | **String** |  | [optional] |
| **total_detail_in_usd** | **Float** |  | [optional] |
| **total_profit_in_usd** | **Float** |  | [optional] |
| **total_discounts_in_usd** | **Float** |  | [optional] |
| **total_surcharges_in_usd** | **Float** |  | [optional] |
| **total_tax_base_in_usd** | **Float** |  | [optional] |
| **total_taxes_in_usd** | **Float** |  | [optional] |
| **total_withheld_taxes_in_usd** | **Float** |  | [optional] |
| **total_shipping_cost_in_usd** | **Float** |  | [optional] |
| **total_shipping_taxes_in_usd** | **Float** |  | [optional] |
| **total_global_discounts_in_usd** | **Float** |  | [optional] |
| **total_global_surcharges_in_usd** | **Float** |  | [optional] |
| **total_in_usd** | **Float** |  | [optional] |
| **paid** | **Boolean** |  | [optional] |
| **number** | **Integer** |  | [optional] |
| **notes** | **String** |  | [optional] |
| **order_id** | **String** |  | [optional] |
| **enumeration** | **String** |  | [optional] |
| **payment_mode_id** | **String** |  | [optional] |
| **enumeration_range_id** | **String** |  | [optional] |
| **emisor_billing_profile_id** | **String** |  | [optional] |
| **receiver_billing_profile_id** | **String** |  | [optional] |
| **emisor_wallet_account_id** | **String** |  | [optional] |
| **receiver_wallet_account_id** | **String** |  | [optional] |
| **payment_due** | **Time** |  | [optional] |
| **invoice_type** | **String** |  | [optional] |
| **document_type** | **String** |  | [optional] |
| **invoice_status** | **String** |  | [optional] |
| **tenant** | [**TenantDto**](TenantDto.md) |  | [optional] |
| **user** | [**SimpleUserDto**](SimpleUserDto.md) |  | [optional] |
| **receiver_tenant** | [**TenantDto**](TenantDto.md) |  | [optional] |
| **individual** | [**SimpleContactDto**](SimpleContactDto.md) |  | [optional] |
| **organization** | [**SimpleContactDto**](SimpleContactDto.md) |  | [optional] |
| **enrollment** | [**SimpleTenantEnrollmentDto**](SimpleTenantEnrollmentDto.md) |  | [optional] |
| **invoice_lines** | [**Array&lt;InvoiceLineDto&gt;**](InvoiceLineDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ExtendedInvoiceDto.new(
  id: null,
  timestamp: null,
  closed: null,
  type: null,
  title: null,
  user_id: null,
  tenant_id: null,
  description: null,
  price_list_id: null,
  enrollment_id: null,
  individual_id: null,
  organization_id: null,
  receiver_tenant_id: null,
  first_name: null,
  last_name: null,
  company_name: null,
  billing_email: null,
  address_line1: null,
  address_line2: null,
  postal_code: null,
  country_id: null,
  state_id: null,
  city_id: null,
  customer_notes: null,
  tax_calculation_method: null,
  cost_calculation_method: null,
  forex_rate: null,
  currency_id: null,
  total_detail: null,
  total_detail_currency_id: null,
  total_profit: null,
  total_profit_currency_id: null,
  total_discounts: null,
  total_discounts_currency_id: null,
  total_surcharges: null,
  total_surcharges_currency_id: null,
  total_tax_base: null,
  total_tax_base_currency_id: null,
  total_taxes: null,
  total_taxes_currency_id: null,
  total_shipping_cost: null,
  total_shipping_cost_currency_id: null,
  total_shipping_tax: null,
  total_shipping_tax_currency_id: null,
  total_withheld_tax: null,
  total_withheld_tax_currency_id: null,
  total_global_discounts: null,
  total_global_discounts_currency_id: null,
  total_global_surcharges: null,
  total_global_surcharges_currency_id: null,
  total: null,
  total_currency_id: null,
  total_detail_in_usd: null,
  total_profit_in_usd: null,
  total_discounts_in_usd: null,
  total_surcharges_in_usd: null,
  total_tax_base_in_usd: null,
  total_taxes_in_usd: null,
  total_withheld_taxes_in_usd: null,
  total_shipping_cost_in_usd: null,
  total_shipping_taxes_in_usd: null,
  total_global_discounts_in_usd: null,
  total_global_surcharges_in_usd: null,
  total_in_usd: null,
  paid: null,
  number: null,
  notes: null,
  order_id: null,
  enumeration: null,
  payment_mode_id: null,
  enumeration_range_id: null,
  emisor_billing_profile_id: null,
  receiver_billing_profile_id: null,
  emisor_wallet_account_id: null,
  receiver_wallet_account_id: null,
  payment_due: null,
  invoice_type: null,
  document_type: null,
  invoice_status: null,
  tenant: null,
  user: null,
  receiver_tenant: null,
  individual: null,
  organization: null,
  enrollment: null,
  invoice_lines: null
)
```

