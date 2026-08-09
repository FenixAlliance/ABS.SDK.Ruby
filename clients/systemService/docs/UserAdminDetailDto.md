# OpenapiClient::UserAdminDetailDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **orders** | [**Array&lt;UserOrderSummaryDto&gt;**](UserOrderSummaryDto.md) |  | [optional] |
| **logins** | [**Array&lt;UserExternalLoginDto&gt;**](UserExternalLoginDto.md) |  | [optional] |
| **enrollment** | [**TenantEnrollmentDto**](TenantEnrollmentDto.md) |  | [optional] |
| **granted_roles** | [**Array&lt;SecurityRoleDto&gt;**](SecurityRoleDto.md) |  | [optional] |
| **granted_permissions** | [**Array&lt;SecurityPermissionDto&gt;**](SecurityPermissionDto.md) |  | [optional] |
| **role_catalog** | [**Array&lt;SecurityRoleDto&gt;**](SecurityRoleDto.md) |  | [optional] |
| **permission_catalog** | [**Array&lt;SecurityPermissionDto&gt;**](SecurityPermissionDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::UserAdminDetailDto.new(
  orders: null,
  logins: null,
  enrollment: null,
  granted_roles: null,
  granted_permissions: null,
  role_catalog: null,
  permission_catalog: null
)
```

