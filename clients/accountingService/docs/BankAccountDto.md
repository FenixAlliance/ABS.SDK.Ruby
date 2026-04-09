# OpenapiClient::BankAccountDto

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
| **account_type** | **String** |  | [optional] |
| **account_type_id** | **String** |  | [optional] |
| **debits_balance** | **Float** |  | [optional] |
| **credits_balance** | **Float** |  | [optional] |
| **parent_account_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **children_accounts_count** | **Integer** |  | [optional] |
| **account_category** | **String** |  | [optional] |
| **balance_amount** | [**Money**](Money.md) |  | [optional] |
| **credits_balance_amount** | [**Money**](Money.md) |  | [optional] |
| **debits_balance_amount** | [**Money**](Money.md) |  | [optional] |
| **iban** | **String** |  | [optional] |
| **swift** | **String** |  | [optional] |
| **branch_code** | **String** |  | [optional] |
| **bank_account_number** | **String** |  | [optional] |
| **qualified_name** | **String** |  | [optional] |
| **bank_id** | **String** |  | [optional] |
| **bank_profile_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BankAccountDto.new(
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
  account_type: null,
  account_type_id: null,
  debits_balance: null,
  credits_balance: null,
  parent_account_id: null,
  tenant_id: null,
  enrollment_id: null,
  children_accounts_count: null,
  account_category: null,
  balance_amount: null,
  credits_balance_amount: null,
  debits_balance_amount: null,
  iban: null,
  swift: null,
  branch_code: null,
  bank_account_number: null,
  qualified_name: null,
  bank_id: null,
  bank_profile_id: null
)
```

