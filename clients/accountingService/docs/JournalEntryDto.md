# OpenapiClient::JournalEntryDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **journal_id** | **String** |  | [optional] |
| **journal_name** | **String** |  | [optional] |
| **journal_code** | **String** |  | [optional] |
| **fiscal_period_id** | **String** |  | [optional] |
| **financial_book_id** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **entry_type** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **posting_date** | **Time** |  | [optional] |
| **is_opening_balance** | **Boolean** |  | [optional] |
| **transaction_currency_id** | **String** |  | [optional] |
| **source_document_type** | **String** |  | [optional] |
| **source_document_id** | **String** |  | [optional] |
| **idempotency_key** | **String** |  | [optional] |
| **reversal_of_journal_entry_id** | **String** |  | [optional] |
| **posted_by** | **String** |  | [optional] |
| **forex_rate** | **Float** |  | [optional] |
| **forex_rates_snapshot** | **String** |  | [optional] |
| **debit_in_usd** | **Float** |  | [optional] |
| **credit_in_usd** | **Float** |  | [optional] |
| **accounting_entries** | [**Array&lt;AccountingEntryDto&gt;**](AccountingEntryDto.md) |  | [optional] |
| **total_debit** | **Float** |  | [optional][readonly] |
| **total_credit** | **Float** |  | [optional][readonly] |
| **total_debit_amount** | [**Money**](Money.md) |  | [optional] |
| **total_credit_amount** | [**Money**](Money.md) |  | [optional] |
| **debit_in_usd_amount** | [**Money**](Money.md) |  | [optional] |
| **credit_in_usd_amount** | [**Money**](Money.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::JournalEntryDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  enrollment_id: null,
  journal_id: null,
  journal_name: null,
  journal_code: null,
  fiscal_period_id: null,
  financial_book_id: null,
  description: null,
  entry_type: null,
  status: null,
  posting_date: null,
  is_opening_balance: null,
  transaction_currency_id: null,
  source_document_type: null,
  source_document_id: null,
  idempotency_key: null,
  reversal_of_journal_entry_id: null,
  posted_by: null,
  forex_rate: null,
  forex_rates_snapshot: null,
  debit_in_usd: null,
  credit_in_usd: null,
  accounting_entries: null,
  total_debit: null,
  total_credit: null,
  total_debit_amount: null,
  total_credit_amount: null,
  debit_in_usd_amount: null,
  credit_in_usd_amount: null
)
```

