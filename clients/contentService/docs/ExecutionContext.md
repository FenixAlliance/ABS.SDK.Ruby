# OpenapiClient::ExecutionContext

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **is_authenticated** | **Boolean** |  | [optional] |
| **current_cart_id** | **String** |  | [optional][readonly] |
| **current_user_id** | **String** |  | [optional][readonly] |
| **current_tenant_id** | **String** |  | [optional][readonly] |
| **current_portal_id** | **String** |  | [optional][readonly] |
| **current_enrollment_id** | **String** |  | [optional][readonly] |
| **currency_id** | **String** |  | [optional][readonly] |
| **page_size** | **Integer** |  | [optional] |
| **date_format** | **String** |  | [optional] |
| **currency_format** | **String** |  | [optional] |
| **date_time_format** | **String** |  | [optional] |
| **to_date_data_summaries** | **Time** |  | [optional] |
| **from_date_data_summaries** | **Time** |  | [optional] |
| **authorization** | [**AuthResult**](AuthResult.md) |  | [optional] |
| **user** | [**ExtendedUserDto**](ExtendedUserDto.md) |  | [optional] |
| **current_tenant** | [**ExtendedTenantDto**](ExtendedTenantDto.md) |  | [optional] |
| **current_enrollment** | [**TenantEnrollmentDto**](TenantEnrollmentDto.md) |  | [optional] |
| **selected_tenant_mappings** | [**CrmContext**](CrmContext.md) |  | [optional] |
| **portal_owner_mappings** | [**CrmContext**](CrmContext.md) |  | [optional] |
| **root_tenant_mappings** | [**CrmContext**](CrmContext.md) |  | [optional] |
| **cart** | [**CartDto**](CartDto.md) |  | [optional] |
| **currency** | [**CurrencyDto**](CurrencyDto.md) |  | [optional] |
| **forex_rates** | [**ForexRatesDto**](ForexRatesDto.md) |  | [optional] |
| **exchange_rate** | [**Money**](Money.md) |  | [optional] |
| **country** | [**CountryDto**](CountryDto.md) |  | [optional] |
| **root_tenant** | [**TenantDto**](TenantDto.md) |  | [optional] |
| **current_portal** | [**WebPortalDto**](WebPortalDto.md) |  | [optional] |
| **tenants** | [**Array&lt;ExtendedTenantDto&gt;**](ExtendedTenantDto.md) |  | [optional] |
| **enrollments** | [**Array&lt;ExtendedTenantEnrollmentDto&gt;**](ExtendedTenantEnrollmentDto.md) |  | [optional] |
| **available_portals** | [**Array&lt;WebPortalDto&gt;**](WebPortalDto.md) |  | [optional] |
| **invitations** | [**Array&lt;ExtendedInviteDto&gt;**](ExtendedInviteDto.md) |  | [optional] |
| **granted_permissions** | **Array&lt;String&gt;** |  | [optional] |
| **accessible_features** | [**Array&lt;SuiteLicenseFeatureDto&gt;**](SuiteLicenseFeatureDto.md) |  | [optional] |
| **culture_name** | **String** |  | [optional][readonly] |
| **timezone_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ExecutionContext.new(
  is_authenticated: null,
  current_cart_id: null,
  current_user_id: null,
  current_tenant_id: null,
  current_portal_id: null,
  current_enrollment_id: null,
  currency_id: null,
  page_size: null,
  date_format: null,
  currency_format: null,
  date_time_format: null,
  to_date_data_summaries: null,
  from_date_data_summaries: null,
  authorization: null,
  user: null,
  current_tenant: null,
  current_enrollment: null,
  selected_tenant_mappings: null,
  portal_owner_mappings: null,
  root_tenant_mappings: null,
  cart: null,
  currency: null,
  forex_rates: null,
  exchange_rate: null,
  country: null,
  root_tenant: null,
  current_portal: null,
  tenants: null,
  enrollments: null,
  available_portals: null,
  invitations: null,
  granted_permissions: null,
  accessible_features: null,
  culture_name: null,
  timezone_id: null
)
```

