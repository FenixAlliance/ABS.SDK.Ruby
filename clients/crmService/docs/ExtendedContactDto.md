# OpenapiClient::ExtendedContactDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **qualified_name** | **String** |  | [optional][readonly] |
| **tenant_id** | **String** |  | [optional] |
| **type** | **String** |  | [optional] |
| **email** | **String** |  | [optional] |
| **phone** | **String** |  | [optional] |
| **public_name** | **String** |  | [optional] |
| **first_name** | **String** |  | [optional] |
| **last_name** | **String** |  | [optional] |
| **job_title** | **String** |  | [optional] |
| **cover_url** | **String** |  | [optional] |
| **avatar_url** | **String** |  | [optional] |
| **country_id** | **String** |  | [optional] |
| **timezone_id** | **String** |  | [optional] |
| **language_id** | **String** |  | [optional] |
| **social_profile_id** | **String** |  | [optional] |
| **web_url** | **String** |  | [optional] |
| **git_hub_url** | **String** |  | [optional] |
| **twitch_url** | **String** |  | [optional] |
| **reddit_url** | **String** |  | [optional] |
| **tik_tok_url** | **String** |  | [optional] |
| **website_url** | **String** |  | [optional] |
| **twitter_url** | **String** |  | [optional] |
| **facebook_url** | **String** |  | [optional] |
| **you_tube_url** | **String** |  | [optional] |
| **linked_in_url** | **String** |  | [optional] |
| **instagram_url** | **String** |  | [optional] |
| **github_username** | **String** |  | [optional] |
| **duns** | **String** |  | [optional] |
| **tax_id** | **String** |  | [optional] |
| **about** | **String** |  | [optional] |
| **street** | **String** |  | [optional] |
| **cart_id** | **String** |  | [optional] |
| **city_id** | **String** |  | [optional] |
| **zip_code** | **String** |  | [optional] |
| **state_id** | **String** |  | [optional] |
| **wallet_id** | **String** |  | [optional] |
| **fax_number** | **String** |  | [optional] |
| **postal_code** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **street_line1** | **String** |  | [optional] |
| **street_line2** | **String** |  | [optional] |
| **territory_id** | **String** |  | [optional] |
| **mobile_phone** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **annual_revenue** | **String** |  | [optional] |
| **related_user_id** | **String** |  | [optional] |
| **business_phone** | **String** |  | [optional] |
| **owner_contact_id** | **String** |  | [optional] |
| **related_tenant_id** | **String** |  | [optional] |
| **activity_feed_id** | **String** |  | [optional] |
| **parent_contact_id** | **String** |  | [optional] |
| **identity_provider** | **String** |  | [optional] |
| **partner_profile_id** | **String** |  | [optional] |
| **primary_contact_id** | **String** |  | [optional] |
| **active_directory_id** | **String** |  | [optional] |
| **identity_provider_access_token** | **String** |  | [optional] |
| **birthday** | **Time** |  | [optional] |
| **cart** | [**CartDto**](CartDto.md) |  | [optional] |
| **wallet** | [**WalletDto**](WalletDto.md) |  | [optional] |
| **social_profile** | [**SocialProfileDto**](SocialProfileDto.md) |  | [optional] |
| **parent_contact** | [**SimpleContactDto**](SimpleContactDto.md) |  | [optional] |
| **primary_contact** | [**SimpleContactDto**](SimpleContactDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ExtendedContactDto.new(
  id: null,
  timestamp: null,
  qualified_name: null,
  tenant_id: null,
  type: null,
  email: null,
  phone: null,
  public_name: null,
  first_name: null,
  last_name: null,
  job_title: null,
  cover_url: null,
  avatar_url: null,
  country_id: null,
  timezone_id: null,
  language_id: null,
  social_profile_id: null,
  web_url: null,
  git_hub_url: null,
  twitch_url: null,
  reddit_url: null,
  tik_tok_url: null,
  website_url: null,
  twitter_url: null,
  facebook_url: null,
  you_tube_url: null,
  linked_in_url: null,
  instagram_url: null,
  github_username: null,
  duns: null,
  tax_id: null,
  about: null,
  street: null,
  cart_id: null,
  city_id: null,
  zip_code: null,
  state_id: null,
  wallet_id: null,
  fax_number: null,
  postal_code: null,
  currency_id: null,
  street_line1: null,
  street_line2: null,
  territory_id: null,
  mobile_phone: null,
  enrollment_id: null,
  annual_revenue: null,
  related_user_id: null,
  business_phone: null,
  owner_contact_id: null,
  related_tenant_id: null,
  activity_feed_id: null,
  parent_contact_id: null,
  identity_provider: null,
  partner_profile_id: null,
  primary_contact_id: null,
  active_directory_id: null,
  identity_provider_access_token: null,
  birthday: null,
  cart: null,
  wallet: null,
  social_profile: null,
  parent_contact: null,
  primary_contact: null
)
```

