# OpenapiClient::DealUnitUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **closed** | **Boolean** |  | [optional] |
| **title** | **String** |  | [optional] |
| **user_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **price_list_id** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **individual_id** | **String** |  | [optional] |
| **payment_term_id** | **String** |  | [optional] |
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
| **billing_location_id** | **String** |  | [optional] |
| **shipping_location_id** | **String** |  | [optional] |
| **shipping_method_id** | **String** |  | [optional] |
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
| **total_shipping_tax** | **Float** |  | [optional] |
| **total_shipping_tax_currency_id** | **String** |  | [optional] |
| **total_shipping_cost** | **Float** |  | [optional] |
| **total_shipping_cost_currency_id** | **String** |  | [optional] |
| **total_global_discounts** | **Float** |  | [optional] |
| **total_global_discounts_currency_id** | **String** |  | [optional] |
| **total_global_surcharges** | **Float** |  | [optional] |
| **total_global_surcharges_currency_id** | **String** |  | [optional] |
| **total_withheld_tax** | **Float** |  | [optional] |
| **total_withheld_tax_currency_id** | **String** |  | [optional] |
| **total_tax_base** | **Float** |  | [optional] |
| **total_tax_base_currency_id** | **String** |  | [optional] |
| **total_taxes** | **Float** |  | [optional] |
| **total_taxes_currency_id** | **String** |  | [optional] |
| **total** | **Float** |  | [optional] |
| **total_currency_id** | **String** |  | [optional] |
| **cost_calculation_method** | **String** |  | [optional] |
| **tax_calculation_method** | **String** |  | [optional] |
| **ordered** | **Boolean** |  | [optional] |
| **cart_id** | **String** |  | [optional] |
| **deal_unit_feed_id** | **String** |  | [optional] |
| **deal_unit_flow_id** | **String** |  | [optional] |
| **deal_unit_flow_stage_id** | **String** |  | [optional] |
| **partner_created** | **Boolean** |  | [optional] |
| **partner_collaboration** | **Boolean** |  | [optional] |
| **proposed_solution** | **String** |  | [optional] |
| **current_situation** | **String** |  | [optional] |
| **customer_need** | **String** |  | [optional] |
| **won_date** | **Time** |  | [optional] |
| **lost_date** | **Time** |  | [optional] |
| **expiry_date** | **Time** |  | [optional] |
| **delivered_date** | **Time** |  | [optional] |
| **closed_timestamp** | **Time** |  | [optional] |
| **expected_close_date** | **Time** |  | [optional] |
| **deal_unit_status** | **String** |  | [optional] |
| **deal_unit_purchase_process** | **String** |  | [optional] |
| **deal_unit_forecast_category** | **String** |  | [optional] |
| **deal_unit_amounts_calculation** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::DealUnitUpdateDto.new(
  closed: null,
  title: null,
  user_id: null,
  tenant_id: null,
  price_list_id: null,
  description: null,
  enrollment_id: null,
  individual_id: null,
  payment_term_id: null,
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
  billing_location_id: null,
  shipping_location_id: null,
  shipping_method_id: null,
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
  total_shipping_tax: null,
  total_shipping_tax_currency_id: null,
  total_shipping_cost: null,
  total_shipping_cost_currency_id: null,
  total_global_discounts: null,
  total_global_discounts_currency_id: null,
  total_global_surcharges: null,
  total_global_surcharges_currency_id: null,
  total_withheld_tax: null,
  total_withheld_tax_currency_id: null,
  total_tax_base: null,
  total_tax_base_currency_id: null,
  total_taxes: null,
  total_taxes_currency_id: null,
  total: null,
  total_currency_id: null,
  cost_calculation_method: null,
  tax_calculation_method: null,
  ordered: null,
  cart_id: null,
  deal_unit_feed_id: null,
  deal_unit_flow_id: null,
  deal_unit_flow_stage_id: null,
  partner_created: null,
  partner_collaboration: null,
  proposed_solution: null,
  current_situation: null,
  customer_need: null,
  won_date: null,
  lost_date: null,
  expiry_date: null,
  delivered_date: null,
  closed_timestamp: null,
  expected_close_date: null,
  deal_unit_status: null,
  deal_unit_purchase_process: null,
  deal_unit_forecast_category: null,
  deal_unit_amounts_calculation: null
)
```

