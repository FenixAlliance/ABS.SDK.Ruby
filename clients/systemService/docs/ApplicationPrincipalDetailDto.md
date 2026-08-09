# OpenapiClient::ApplicationPrincipalDetailDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **display_name** | **String** |  | [optional] |
| **principal_kind** | **String** |  | [optional] |
| **principal_status** | **String** |  | [optional] |
| **business_application_id** | **String** |  | [optional] |
| **business_application_name** | **String** |  | [optional] |
| **business_application_namespace** | **String** |  | [optional] |
| **business_application_disabled** | **Boolean** |  | [optional] |
| **system_locked** | **Boolean** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **enrollment_disabled** | **Boolean** |  | [optional] |
| **granted_permissions** | **Array&lt;String&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ApplicationPrincipalDetailDto.new(
  id: null,
  timestamp: null,
  display_name: null,
  principal_kind: null,
  principal_status: null,
  business_application_id: null,
  business_application_name: null,
  business_application_namespace: null,
  business_application_disabled: null,
  system_locked: null,
  tenant_id: null,
  enrollment_id: null,
  enrollment_disabled: null,
  granted_permissions: null
)
```

