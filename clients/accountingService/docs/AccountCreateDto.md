# OpenapiClient::AccountCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **group** | **Boolean** |  | [optional] |
| **frozen** | **Boolean** |  | [optional] |
| **name** | **String** |  |  |
| **code** | **String** |  | [optional] |
| **path** | **String** |  | [optional] |
| **prefix** | **String** |  | [optional] |
| **currency_id** | **String** |  |  |
| **contact_id** | **String** |  | [optional] |
| **account_type_id** | **String** |  | [optional] |
| **parent_account_id** | **String** |  | [optional] |
| **account_category** | **String** |  |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AccountCreateDto.new(
  id: null,
  timestamp: null,
  group: null,
  frozen: null,
  name: null,
  code: null,
  path: null,
  prefix: null,
  currency_id: null,
  contact_id: null,
  account_type_id: null,
  parent_account_id: null,
  account_category: null
)
```

