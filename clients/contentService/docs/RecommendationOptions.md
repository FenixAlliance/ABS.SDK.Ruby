# OpenapiClient::RecommendationOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **view_weight** | **Float** |  | [optional] |
| **add_to_cart_weight** | **Float** |  | [optional] |
| **removed_from_cart_weight** | **Float** |  | [optional] |
| **added_to_wishlist_weight** | **Float** |  | [optional] |
| **already_purchased_weight** | **Float** |  | [optional] |
| **removed_to_wishlist_weight** | **Float** |  | [optional] |
| **added_to_compare_table_weight** | **Float** |  | [optional] |
| **removed_to_compare_table_weight** | **Float** |  | [optional] |
| **enable_cross_selling** | **Boolean** |  | [optional] |
| **enable_bundled_products** | **Boolean** |  | [optional] |
| **enable_recently_viewed_products** | **Boolean** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::RecommendationOptions.new(
  view_weight: null,
  add_to_cart_weight: null,
  removed_from_cart_weight: null,
  added_to_wishlist_weight: null,
  already_purchased_weight: null,
  removed_to_wishlist_weight: null,
  added_to_compare_table_weight: null,
  removed_to_compare_table_weight: null,
  enable_cross_selling: null,
  enable_bundled_products: null,
  enable_recently_viewed_products: null
)
```

