# OpenapiClient::ExecutionProvenance

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **initiation** | **String** |  | [optional] |
| **on_behalf_of_actor_id** | **Object** |  | [optional] |
| **on_behalf_of_actor_kind** | **String** |  | [optional] |
| **causation_id** | **String** |  | [optional] |
| **originating_workflow_instance_id** | **String** |  | [optional] |
| **event_depth** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ExecutionProvenance.new(
  initiation: null,
  on_behalf_of_actor_id: null,
  on_behalf_of_actor_kind: null,
  causation_id: null,
  originating_workflow_instance_id: null,
  event_depth: null
)
```

