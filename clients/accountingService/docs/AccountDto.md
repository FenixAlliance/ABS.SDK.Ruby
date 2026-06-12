# OpenapiClient::AccountDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **group** | **Boolean** |  | [optional] |
| **frozen** | **Boolean** |  | [optional] |
| **name** | **String** |  | [optional] |
| **code** | **String** |  | [optional] |
| **path** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **prefix** | **String** |  | [optional] |
| **balance** | **Float** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **account_type** | **String** |  | [optional] |
| **qualified_name** | **String** |  | [optional] |
| **account_type_id** | **String** |  | [optional] |
| **debits_balance** | **Float** |  | [optional] |
| **credits_balance** | **Float** |  | [optional] |
| **balance_in_usd** | **Float** |  | [optional] |
| **debits_balance_in_usd** | **Float** |  | [optional] |
| **credits_balance_in_usd** | **Float** |  | [optional] |
| **forex_rate** | **Float** |  | [optional] |
| **parent_account_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **children_accounts_count** | **Integer** |  | [optional] |
| **account_category** | **String** |  | [optional] |
| **balance_amount** | [**Money**](Money.md) |  | [optional] |
| **credits_balance_amount** | [**Money**](Money.md) |  | [optional] |
| **debits_balance_amount** | [**Money**](Money.md) |  | [optional] |
| **balance_amount_in_usd** | [**Money**](Money.md) |  | [optional] |
| **debits_balance_amount_in_usd** | [**Money**](Money.md) |  | [optional] |
| **credits_balance_amount_in_usd** | [**Money**](Money.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AccountDto.new(
  id: null,
  timestamp: null,
  group: null,
  frozen: null,
  name: null,
  code: null,
  path: null,
  title: null,
  prefix: null,
  balance: null,
  currency_id: null,
  contact_id: null,
  account_type: null,
  qualified_name: null,
  account_type_id: null,
  debits_balance: null,
  credits_balance: null,
  balance_in_usd: null,
  debits_balance_in_usd: null,
  credits_balance_in_usd: null,
  forex_rate: null,
  parent_account_id: null,
  tenant_id: null,
  enrollment_id: null,
  children_accounts_count: null,
  account_category: null,
  balance_amount: null,
  credits_balance_amount: null,
  debits_balance_amount: null,
  balance_amount_in_usd: null,
  debits_balance_amount_in_usd: null,
  credits_balance_amount_in_usd: null
)
```

