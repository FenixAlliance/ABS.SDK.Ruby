# OpenapiClient::ExtendedOrderDto

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
| **order_lines_count** | **Integer** |  | [optional] |
| **quote_id** | **String** |  | [optional] |
| **wallet_id** | **String** |  | [optional] |
| **payment_term_id** | **String** |  | [optional] |
| **parent_order_id** | **String** |  | [optional] |
| **shipping_method_id** | **String** |  | [optional] |
| **billing_location_id** | **String** |  | [optional] |
| **shipping_location_id** | **String** |  | [optional] |
| **qualified_identifier** | **String** |  | [optional] |
| **cost_calculation_method** | **String** |  | [optional] |
| **freight_terms** | **String** |  | [optional] |
| **order_status** | **String** |  | [optional] |
| **requested_delivery_date** | **Time** |  | [optional] |
| **custom_tax_amount** | **Float** |  | [optional] |
| **custom_total_amount** | **Float** |  | [optional] |
| **custom_detail_amount** | **Float** |  | [optional] |
| **custom_profit_amount** | **Float** |  | [optional] |
| **custom_discounts_amount** | **Float** |  | [optional] |
| **custom_surcharges_amount** | **Float** |  | [optional] |
| **custom_shipping_tax_amount** | **Float** |  | [optional] |
| **custom_shipping_cost_amount** | **Float** |  | [optional] |
| **custom_withholding_tax_amount** | **Float** |  | [optional] |
| **user** | [**UserDto**](UserDto.md) |  | [optional] |
| **tenant** | [**TenantDto**](TenantDto.md) |  | [optional] |
| **individual** | [**ContactDto**](ContactDto.md) |  | [optional] |
| **organization** | [**ContactDto**](ContactDto.md) |  | [optional] |
| **receiver_tenant** | [**TenantDto**](TenantDto.md) |  | [optional] |
| **enrollment** | [**TenantEnrollmentDto**](TenantEnrollmentDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ExtendedOrderDto.new(
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
  order_lines_count: null,
  quote_id: null,
  wallet_id: null,
  payment_term_id: null,
  parent_order_id: null,
  shipping_method_id: null,
  billing_location_id: null,
  shipping_location_id: null,
  qualified_identifier: null,
  cost_calculation_method: null,
  freight_terms: null,
  order_status: null,
  requested_delivery_date: null,
  custom_tax_amount: null,
  custom_total_amount: null,
  custom_detail_amount: null,
  custom_profit_amount: null,
  custom_discounts_amount: null,
  custom_surcharges_amount: null,
  custom_shipping_tax_amount: null,
  custom_shipping_cost_amount: null,
  custom_withholding_tax_amount: null,
  user: null,
  tenant: null,
  individual: null,
  organization: null,
  receiver_tenant: null,
  enrollment: null
)
```

