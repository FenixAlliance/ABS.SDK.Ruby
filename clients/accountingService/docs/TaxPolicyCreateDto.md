# OpenapiClient::TaxPolicyCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **code** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **is_free** | **Boolean** |  | [optional] |
| **reduce** | **Boolean** |  | [optional] |
| **is_enabled** | **Boolean** |  | [optional] |
| **is_default** | **Boolean** |  | [optional] |
| **allow_international** | **Boolean** |  | [optional] |
| **hours** | **Integer** |  | [optional] |
| **days** | **Integer** |  | [optional] |
| **weeks** | **Integer** |  | [optional] |
| **months** | **Integer** |  | [optional] |
| **years** | **Integer** |  | [optional] |
| **value** | **Float** |  | [optional] |
| **percentage** | **Float** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **country_id** | **String** |  | [optional] |
| **country_state_id** | **String** |  | [optional] |
| **custom_state** | **String** |  | [optional] |
| **custom_city** | **String** |  | [optional] |
| **city_id** | **String** |  | [optional] |
| **zero** | **Boolean** |  | [optional] |
| **reduced** | **Boolean** |  | [optional] |
| **withholding** | **Boolean** |  | [optional] |
| **fiscal_authority_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TaxPolicyCreateDto.new(
  id: null,
  timestamp: null,
  code: null,
  title: null,
  description: null,
  is_free: null,
  reduce: null,
  is_enabled: null,
  is_default: null,
  allow_international: null,
  hours: null,
  days: null,
  weeks: null,
  months: null,
  years: null,
  value: null,
  percentage: null,
  currency_id: null,
  country_id: null,
  country_state_id: null,
  custom_state: null,
  custom_city: null,
  city_id: null,
  zero: null,
  reduced: null,
  withholding: null,
  fiscal_authority_id: null
)
```

