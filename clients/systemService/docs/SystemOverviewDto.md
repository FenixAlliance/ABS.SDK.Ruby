# OpenapiClient::SystemOverviewDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **uptime** | **String** |  | [optional] |
| **os_description** | **String** |  | [optional] |
| **machine_name** | **String** |  | [optional] |
| **process_name** | **String** |  | [optional] |
| **product_version** | **String** |  | [optional] |
| **private_memory_mb** | **Integer** |  | [optional] |
| **paged_memory_mb** | **Integer** |  | [optional] |
| **memory_working_set_mb** | **Integer** |  | [optional] |
| **is_debug_mode** | **Boolean** |  | [optional] |
| **is_dev_mode** | **Boolean** |  | [optional] |
| **framework_description** | **String** |  | [optional] |
| **runtime_identifier** | **String** |  | [optional] |
| **os_architecture** | **String** |  | [optional] |
| **os_platform** | **String** |  | [optional] |
| **process_architecture** | **String** |  | [optional] |
| **users_count** | **Integer** |  | [optional] |
| **orders_count** | **Integer** |  | [optional] |
| **contacts_count** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SystemOverviewDto.new(
  uptime: null,
  os_description: null,
  machine_name: null,
  process_name: null,
  product_version: null,
  private_memory_mb: null,
  paged_memory_mb: null,
  memory_working_set_mb: null,
  is_debug_mode: null,
  is_dev_mode: null,
  framework_description: null,
  runtime_identifier: null,
  os_architecture: null,
  os_platform: null,
  process_architecture: null,
  users_count: null,
  orders_count: null,
  contacts_count: null
)
```

