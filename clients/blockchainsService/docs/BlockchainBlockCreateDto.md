# OpenapiClient::BlockchainBlockCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **hash** | **String** |  |  |
| **data** | **String** |  | [optional] |
| **nonce** | **Integer** |  | [optional] |
| **previous_hash** | **String** |  | [optional] |
| **blockchain_id** | **String** |  |  |
| **wallet_account_id** | **String** |  |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BlockchainBlockCreateDto.new(
  id: null,
  timestamp: null,
  hash: null,
  data: null,
  nonce: null,
  previous_hash: null,
  blockchain_id: null,
  wallet_account_id: null
)
```

