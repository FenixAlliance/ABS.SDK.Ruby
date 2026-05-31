# OpenapiClient::BillingProfileDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **type** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **about** | **String** |  | [optional] |
| **verified** | **Boolean** |  | [optional] |
| **submitted** | **Boolean** |  | [optional] |
| **avatar_url** | **String** |  | [optional] |
| **contact** | [**ContactDto**](ContactDto.md) |  | [optional] |
| **qualified_name** | **String** |  | [optional][readonly] |
| **verification_timestamp** | **Time** |  | [optional] |
| **data** | **String** |  | [optional] |
| **data_label** | **String** |  | [optional] |
| **data1** | **String** |  | [optional] |
| **data1_label** | **String** |  | [optional] |
| **data2** | **String** |  | [optional] |
| **data2_label** | **String** |  | [optional] |
| **data3** | **String** |  | [optional] |
| **data3_label** | **String** |  | [optional] |
| **data4** | **String** |  | [optional] |
| **data4_label** | **String** |  | [optional] |
| **data5** | **String** |  | [optional] |
| **data5_label** | **String** |  | [optional] |
| **data6** | **String** |  | [optional] |
| **data6_label** | **String** |  | [optional] |
| **data7** | **String** |  | [optional] |
| **data7_label** | **String** |  | [optional] |
| **data8** | **String** |  | [optional] |
| **data8_label** | **String** |  | [optional] |
| **data9** | **String** |  | [optional] |
| **data9_label** | **String** |  | [optional] |
| **tax_id** | **String** |  |  |
| **email** | **String** |  |  |
| **phone** | **String** |  | [optional] |
| **address** | **String** |  | [optional] |
| **address1** | **String** |  | [optional] |
| **address2** | **String** |  | [optional] |
| **postal_code** | **String** |  | [optional] |
| **business_name** | **String** |  | [optional] |
| **commercial_name** | **String** |  | [optional] |
| **ticker** | **String** |  | [optional] |
| **duns** | **String** |  | [optional] |
| **is_public_company** | **Boolean** |  | [optional] |
| **is_facta_customer** | **Boolean** |  | [optional] |
| **tax_payer_type** | **String** |  | [optional] |
| **country_id** | **String** |  |  |
| **state_id** | **String** |  | [optional] |
| **city_id** | **String** |  | [optional] |
| **fiscal_identification_type_id** | **String** |  | [optional] |
| **fiscal_authority_id** | **String** |  | [optional] |
| **fiscal_regime_id** | **String** |  | [optional] |
| **contact_name** | **String** |  | [optional] |
| **fiscal_authority_name** | **String** |  | [optional] |
| **country_name** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BillingProfileDto.new(
  id: null,
  timestamp: null,
  contact_id: null,
  tenant_id: null,
  type: null,
  enrollment_id: null,
  about: null,
  verified: null,
  submitted: null,
  avatar_url: null,
  contact: null,
  qualified_name: null,
  verification_timestamp: null,
  data: null,
  data_label: null,
  data1: null,
  data1_label: null,
  data2: null,
  data2_label: null,
  data3: null,
  data3_label: null,
  data4: null,
  data4_label: null,
  data5: null,
  data5_label: null,
  data6: null,
  data6_label: null,
  data7: null,
  data7_label: null,
  data8: null,
  data8_label: null,
  data9: null,
  data9_label: null,
  tax_id: null,
  email: null,
  phone: null,
  address: null,
  address1: null,
  address2: null,
  postal_code: null,
  business_name: null,
  commercial_name: null,
  ticker: null,
  duns: null,
  is_public_company: null,
  is_facta_customer: null,
  tax_payer_type: null,
  country_id: null,
  state_id: null,
  city_id: null,
  fiscal_identification_type_id: null,
  fiscal_authority_id: null,
  fiscal_regime_id: null,
  contact_name: null,
  fiscal_authority_name: null,
  country_name: null
)
```

