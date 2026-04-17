# OpenapiClient::ItemsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_stock_item_tags_by_item_id**](ItemsApi.md#count_stock_item_tags_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Tags/Count | Count tags for a stock item |
| [**count_stock_items_by_business**](ItemsApi.md#count_stock_items_by_business) | **GET** /api/v2/CatalogService/Items/Count | Count stock items by business |
| [**create_stock_item**](ItemsApi.md#create_stock_item) | **POST** /api/v2/CatalogService/Items | Create a new stock item |
| [**delete_stock_item**](ItemsApi.md#delete_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId} | Delete a stock item |
| [**get_extended_stock_item_by_id**](ItemsApi.md#get_extended_stock_item_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Extended | Get extended stock item by ID |
| [**get_product_primary_image_async**](ItemsApi.md#get_product_primary_image_async) | **GET** /api/v2/CatalogService/Items/{itemId}/Images/Primary | Get item primary image |
| [**get_stock_item_attachment_by_id**](ItemsApi.md#get_stock_item_attachment_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Attachments/{itemAttachmentId} | Get attachment by ID for a stock item |
| [**get_stock_item_attachments_by_item_id**](ItemsApi.md#get_stock_item_attachments_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Attachments | Get attachments for a stock item |
| [**get_stock_item_attribute_option_by_id**](ItemsApi.md#get_stock_item_attribute_option_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/AttributeOptions/{itemAttributeOptionId} | Get attribute option by ID for a stock item |
| [**get_stock_item_attribute_options_by_item_id**](ItemsApi.md#get_stock_item_attribute_options_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/AttributeOptions | Get attribute options for a stock item |
| [**get_stock_item_brand_by_id**](ItemsApi.md#get_stock_item_brand_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Brands/{itemBrandId} | Get brand by ID for a stock item |
| [**get_stock_item_brands_by_item_id**](ItemsApi.md#get_stock_item_brands_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Brands | Get brands for a stock item |
| [**get_stock_item_by_id**](ItemsApi.md#get_stock_item_by_id) | **GET** /api/v2/CatalogService/Items/{itemId} | Get stock item by ID |
| [**get_stock_item_categories_by_item_id**](ItemsApi.md#get_stock_item_categories_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Categories | Get categories for a stock item |
| [**get_stock_item_category_by_id**](ItemsApi.md#get_stock_item_category_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Categories/{itemCategoryId} | Get category by ID for a stock item |
| [**get_stock_item_google_categories_by_item_id**](ItemsApi.md#get_stock_item_google_categories_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/GoogleCategories | Get Google categories for a stock item |
| [**get_stock_item_google_category_by_id**](ItemsApi.md#get_stock_item_google_category_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/GoogleCategories/{itemGoogleCategoryId} | Get Google category by ID for a stock item |
| [**get_stock_item_image_by_id**](ItemsApi.md#get_stock_item_image_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Images/{itemImageId} | Get image by ID for a stock item |
| [**get_stock_item_images_by_item_id**](ItemsApi.md#get_stock_item_images_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Images | Get images for a stock item |
| [**get_stock_item_price_rule_by_id**](ItemsApi.md#get_stock_item_price_rule_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/PriceRules/{itemPriceRuleId} | Get price rule by ID for a stock item |
| [**get_stock_item_price_rules_by_item_id**](ItemsApi.md#get_stock_item_price_rules_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/PriceRules | Get price rules for a stock item |
| [**get_stock_item_question_by_id**](ItemsApi.md#get_stock_item_question_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Questions/{itemQuestionId} | Get question by ID for a stock item |
| [**get_stock_item_questions_by_item_id**](ItemsApi.md#get_stock_item_questions_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Questions | Get questions for a stock item |
| [**get_stock_item_refund_policies_by_item_id**](ItemsApi.md#get_stock_item_refund_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/RefundPolicies | Get refund policies for a stock item |
| [**get_stock_item_refund_policy_by_id**](ItemsApi.md#get_stock_item_refund_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/RefundPolicies/{itemRefundPolicyId} | Get refund policy by ID for a stock item |
| [**get_stock_item_return_policies_by_item_id**](ItemsApi.md#get_stock_item_return_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/ReturnPolicies | Get return policies for a stock item |
| [**get_stock_item_return_policy_by_id**](ItemsApi.md#get_stock_item_return_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/ReturnPolicies/{itemReturnPolicyId} | Get return policy by ID for a stock item |
| [**get_stock_item_review_by_id**](ItemsApi.md#get_stock_item_review_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Reviews/{itemReviewId} | Get review by ID for a stock item |
| [**get_stock_item_reviews_by_item_id**](ItemsApi.md#get_stock_item_reviews_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Reviews | Get reviews for a stock item |
| [**get_stock_item_shipping_policies_by_item_id**](ItemsApi.md#get_stock_item_shipping_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/ShippingPolicies | Get shipping policies for a stock item |
| [**get_stock_item_shipping_policy_by_id**](ItemsApi.md#get_stock_item_shipping_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/ShippingPolicies/{itemShippingPolicyId} | Get shipping policy by ID for a stock item |
| [**get_stock_item_tag_by_id**](ItemsApi.md#get_stock_item_tag_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Tags/{itemTagId} | Get tag by ID for a stock item |
| [**get_stock_item_tags_by_item_id**](ItemsApi.md#get_stock_item_tags_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Tags | Get tags for a stock item |
| [**get_stock_item_tax_policies_by_item_id**](ItemsApi.md#get_stock_item_tax_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/TaxPolicies | Get tax policies for a stock item |
| [**get_stock_item_tax_policy_by_id**](ItemsApi.md#get_stock_item_tax_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/TaxPolicies/{itemTaxPolicyId} | Get tax policy by ID for a stock item |
| [**get_stock_item_type_by_id**](ItemsApi.md#get_stock_item_type_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Types/{itemTypeId} | Get type by ID for a stock item |
| [**get_stock_item_types_by_item_id**](ItemsApi.md#get_stock_item_types_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Types | Get types for a stock item |
| [**get_stock_item_warranty_policies_by_item_id**](ItemsApi.md#get_stock_item_warranty_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/WarrantyPolicies | Get warranty policies for a stock item |
| [**get_stock_item_warranty_policy_by_id**](ItemsApi.md#get_stock_item_warranty_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/WarrantyPolicies/{itemWarrantyPolicyId} | Get warranty policy by ID for a stock item |
| [**get_stock_items_odata_max_price**](ItemsApi.md#get_stock_items_odata_max_price) | **GET** /api/v2/CatalogService/Items/MaxPrice | Get max price of stock items |
| [**get_stock_items_odata_min_price**](ItemsApi.md#get_stock_items_odata_min_price) | **GET** /api/v2/CatalogService/Items/MinPrice | Get min price of stock items |
| [**get_stock_items_query**](ItemsApi.md#get_stock_items_query) | **GET** /api/v2/CatalogService/Items | Get all stock items |
| [**relate_attachment_to_stock_item**](ItemsApi.md#relate_attachment_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Attachments/{itemAttachmentId} | Relate attachment to stock item |
| [**relate_attribute_option_to_stock_item**](ItemsApi.md#relate_attribute_option_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/AttributeOptions/{itemAttributeOptionId} | Relate attribute option to stock item |
| [**relate_brand_to_stock_item**](ItemsApi.md#relate_brand_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Brands/{itemBrandId} | Relate brand to stock item |
| [**relate_category_to_stock_item**](ItemsApi.md#relate_category_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Categories/{itemCategoryId} | Relate category to stock item |
| [**relate_google_category_to_stock_item**](ItemsApi.md#relate_google_category_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/GoogleCategories/{itemGoogleCategoryId} | Relate Google category to stock item |
| [**relate_image_to_stock_item**](ItemsApi.md#relate_image_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Images/{itemImageId} | Relate image to stock item |
| [**relate_price_rule_to_stock_item**](ItemsApi.md#relate_price_rule_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/PriceRules/{itemPriceRuleId} | Relate price rule to stock item |
| [**relate_question_to_stock_item**](ItemsApi.md#relate_question_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Questions | Create question for stock item |
| [**relate_refund_policy_to_stock_item**](ItemsApi.md#relate_refund_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/RefundPolicies/{itemRefundPolicyId} | Relate refund policy to stock item |
| [**relate_return_policy_to_stock_item**](ItemsApi.md#relate_return_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/ReturnPolicies/{itemReturnPolicyId} | Relate return policy to stock item |
| [**relate_review_to_stock_item**](ItemsApi.md#relate_review_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Reviews | Create review for stock item |
| [**relate_shipping_policy_to_stock_item**](ItemsApi.md#relate_shipping_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/ShippingPolicies/{itemShippingPolicyId} | Relate shipping policy to stock item |
| [**relate_tag_to_stock_item**](ItemsApi.md#relate_tag_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Tags/{itemTagId} | Relate tag to stock item |
| [**relate_tax_policy_to_stock_item**](ItemsApi.md#relate_tax_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/TaxPolicies/{itemTaxPolicyId} | Relate tax policy to stock item |
| [**relate_type_to_stock_item**](ItemsApi.md#relate_type_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Types/{itemTypeId} | Relate type to stock item |
| [**relate_warranty_policy_to_stock_item**](ItemsApi.md#relate_warranty_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/WarrantyPolicies/{itemWarrantyPolicyId} | Relate warranty policy to stock item |
| [**remove_attachment_from_stock_item**](ItemsApi.md#remove_attachment_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Attachments/{itemAttachmentId} | Remove attachment from stock item |
| [**remove_attribute_option_from_stock_item**](ItemsApi.md#remove_attribute_option_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/AttributeOptions/{itemAttributeOptionId} | Remove attribute option from stock item |
| [**remove_brand_from_stock_item**](ItemsApi.md#remove_brand_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Brands/{itemBrandId} | Remove brand from stock item |
| [**remove_category_from_stock_item**](ItemsApi.md#remove_category_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Categories/{itemCategoryId} | Remove category from stock item |
| [**remove_google_category_from_stock_item**](ItemsApi.md#remove_google_category_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/GoogleCategories/{itemGoogleCategoryId} | Remove Google category from stock item |
| [**remove_image_from_stock_item**](ItemsApi.md#remove_image_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Images/{itemImageId} | Remove image from stock item |
| [**remove_price_rule_from_stock_item**](ItemsApi.md#remove_price_rule_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/PriceRules/{itemPriceRuleId} | Remove price rule from stock item |
| [**remove_question_from_stock_item**](ItemsApi.md#remove_question_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Questions/{itemQuestionId} | Remove question from stock item |
| [**remove_refund_policy_from_stock_item**](ItemsApi.md#remove_refund_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/RefundPolicies/{itemRefundPolicyId} | Remove refund policy from stock item |
| [**remove_return_policy_from_stock_item**](ItemsApi.md#remove_return_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/ReturnPolicies/{itemReturnPolicyId} | Remove return policy from stock item |
| [**remove_review_from_stock_item**](ItemsApi.md#remove_review_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Reviews/{itemReviewId} | Remove review from stock item |
| [**remove_shipping_policy_from_stock_item**](ItemsApi.md#remove_shipping_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/ShippingPolicies/{itemShippingPolicyId} | Remove shipping policy from stock item |
| [**remove_tag_from_stock_item**](ItemsApi.md#remove_tag_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Tags/{itemTagId} | Remove tag from stock item |
| [**remove_tax_policy_from_stock_item**](ItemsApi.md#remove_tax_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/TaxPolicies/{itemTaxPolicyId} | Remove tax policy from stock item |
| [**remove_type_from_stock_item**](ItemsApi.md#remove_type_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Types/{itemTypeId} | Remove type from stock item |
| [**remove_warranty_policy_from_stock_item**](ItemsApi.md#remove_warranty_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/WarrantyPolicies/{itemWarrantyPolicyId} | Remove warranty policy from stock item |
| [**update_product_primary_image_async**](ItemsApi.md#update_product_primary_image_async) | **POST** /api/v2/CatalogService/Items/{itemId}/Images/Primary | Update item primary image |
| [**update_stock_item**](ItemsApi.md#update_stock_item) | **PUT** /api/v2/CatalogService/Items/{itemId} | Update a stock item |


## count_stock_item_tags_by_item_id

> <Int32Envelope> count_stock_item_tags_by_item_id(item_id, opts)

Count tags for a stock item

Counts the number of tags associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count tags for a stock item
  result = api_instance.count_stock_item_tags_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->count_stock_item_tags_by_item_id: #{e}"
end
```

#### Using the count_stock_item_tags_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_stock_item_tags_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Count tags for a stock item
  data, status_code, headers = api_instance.count_stock_item_tags_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->count_stock_item_tags_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## count_stock_items_by_business

> <Int32Envelope> count_stock_items_by_business(opts)

Count stock items by business

Counts the number of stock items for a business, optionally filtered by tenant and OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count stock items by business
  result = api_instance.count_stock_items_by_business(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->count_stock_items_by_business: #{e}"
end
```

#### Using the count_stock_items_by_business_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_stock_items_by_business_with_http_info(opts)

```ruby
begin
  # Count stock items by business
  data, status_code, headers = api_instance.count_stock_items_by_business_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->count_stock_items_by_business_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_stock_item

> create_stock_item(tenant_id, opts)

Create a new stock item

Creates a new stock item for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  catalog_item_create_dto: OpenapiClient::CatalogItemCreateDto.new # CatalogItemCreateDto | 
}

begin
  # Create a new stock item
  api_instance.create_stock_item(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->create_stock_item: #{e}"
end
```

#### Using the create_stock_item_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_stock_item_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new stock item
  data, status_code, headers = api_instance.create_stock_item_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->create_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **catalog_item_create_dto** | [**CatalogItemCreateDto**](CatalogItemCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_stock_item

> delete_stock_item(tenant_id, item_id, opts)

Delete a stock item

Deletes a stock item for the specified tenant and item ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a stock item
  api_instance.delete_stock_item(tenant_id, item_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->delete_stock_item: #{e}"
end
```

#### Using the delete_stock_item_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_stock_item_with_http_info(tenant_id, item_id, opts)

```ruby
begin
  # Delete a stock item
  data, status_code, headers = api_instance.delete_stock_item_with_http_info(tenant_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->delete_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_stock_item_by_id

> <CatalogItemDtoEnvelope> get_extended_stock_item_by_id(item_id, opts)

Get extended stock item by ID

Retrieves extended information for a stock item by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get extended stock item by ID
  result = api_instance.get_extended_stock_item_by_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_extended_stock_item_by_id: #{e}"
end
```

#### Using the get_extended_stock_item_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CatalogItemDtoEnvelope>, Integer, Hash)> get_extended_stock_item_by_id_with_http_info(item_id, opts)

```ruby
begin
  # Get extended stock item by ID
  data, status_code, headers = api_instance.get_extended_stock_item_by_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CatalogItemDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_extended_stock_item_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CatalogItemDtoEnvelope**](CatalogItemDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_product_primary_image_async

> <EmptyEnvelope> get_product_primary_image_async(item_id, opts)

Get item primary image

Retrieves the primary image for a specific catalog item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item primary image
  result = api_instance.get_product_primary_image_async(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_product_primary_image_async: #{e}"
end
```

#### Using the get_product_primary_image_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_product_primary_image_async_with_http_info(item_id, opts)

```ruby
begin
  # Get item primary image
  data, status_code, headers = api_instance.get_product_primary_image_async_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_product_primary_image_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_attachment_by_id

> <ItemAttachmentDtoEnvelope> get_stock_item_attachment_by_id(item_id, item_attachment_id, opts)

Get attachment by ID for a stock item

Retrieves a specific attachment by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get attachment by ID for a stock item
  result = api_instance.get_stock_item_attachment_by_id(item_id, item_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_attachment_by_id: #{e}"
end
```

#### Using the get_stock_item_attachment_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttachmentDtoEnvelope>, Integer, Hash)> get_stock_item_attachment_by_id_with_http_info(item_id, item_attachment_id, opts)

```ruby
begin
  # Get attachment by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_attachment_by_id_with_http_info(item_id, item_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttachmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_attachment_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_attachments_by_item_id

> <ItemAttachmentDtoListEnvelope> get_stock_item_attachments_by_item_id(item_id, opts)

Get attachments for a stock item

Retrieves all attachments associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get attachments for a stock item
  result = api_instance.get_stock_item_attachments_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_attachments_by_item_id: #{e}"
end
```

#### Using the get_stock_item_attachments_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttachmentDtoListEnvelope>, Integer, Hash)> get_stock_item_attachments_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get attachments for a stock item
  data, status_code, headers = api_instance.get_stock_item_attachments_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttachmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_attachments_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttachmentDtoListEnvelope**](ItemAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_attribute_option_by_id

> <ItemAttributeOptionDtoEnvelope> get_stock_item_attribute_option_by_id(item_id, item_attribute_option_id, opts)

Get attribute option by ID for a stock item

Retrieves a specific attribute option by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attribute_option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get attribute option by ID for a stock item
  result = api_instance.get_stock_item_attribute_option_by_id(item_id, item_attribute_option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_attribute_option_by_id: #{e}"
end
```

#### Using the get_stock_item_attribute_option_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeOptionDtoEnvelope>, Integer, Hash)> get_stock_item_attribute_option_by_id_with_http_info(item_id, item_attribute_option_id, opts)

```ruby
begin
  # Get attribute option by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_attribute_option_by_id_with_http_info(item_id, item_attribute_option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeOptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_attribute_option_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_attribute_option_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_attribute_options_by_item_id

> <ItemAttributeOptionDtoListEnvelope> get_stock_item_attribute_options_by_item_id(item_id, opts)

Get attribute options for a stock item

Retrieves all attribute options associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get attribute options for a stock item
  result = api_instance.get_stock_item_attribute_options_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_attribute_options_by_item_id: #{e}"
end
```

#### Using the get_stock_item_attribute_options_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeOptionDtoListEnvelope>, Integer, Hash)> get_stock_item_attribute_options_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get attribute options for a stock item
  data, status_code, headers = api_instance.get_stock_item_attribute_options_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeOptionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_attribute_options_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttributeOptionDtoListEnvelope**](ItemAttributeOptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_brand_by_id

> <ItemBrandDtoEnvelope> get_stock_item_brand_by_id(item_id, item_brand_id, opts)

Get brand by ID for a stock item

Retrieves a specific brand by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_brand_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get brand by ID for a stock item
  result = api_instance.get_stock_item_brand_by_id(item_id, item_brand_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_brand_by_id: #{e}"
end
```

#### Using the get_stock_item_brand_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBrandDtoEnvelope>, Integer, Hash)> get_stock_item_brand_by_id_with_http_info(item_id, item_brand_id, opts)

```ruby
begin
  # Get brand by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_brand_by_id_with_http_info(item_id, item_brand_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBrandDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_brand_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_brand_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_brands_by_item_id

> <ItemBrandDtoListEnvelope> get_stock_item_brands_by_item_id(item_id, opts)

Get brands for a stock item

Retrieves all brands associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get brands for a stock item
  result = api_instance.get_stock_item_brands_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_brands_by_item_id: #{e}"
end
```

#### Using the get_stock_item_brands_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBrandDtoListEnvelope>, Integer, Hash)> get_stock_item_brands_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get brands for a stock item
  data, status_code, headers = api_instance.get_stock_item_brands_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBrandDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_brands_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemBrandDtoListEnvelope**](ItemBrandDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_by_id

> <CatalogItemDtoEnvelope> get_stock_item_by_id(item_id, opts)

Get stock item by ID

Retrieves a stock item by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get stock item by ID
  result = api_instance.get_stock_item_by_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_by_id: #{e}"
end
```

#### Using the get_stock_item_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CatalogItemDtoEnvelope>, Integer, Hash)> get_stock_item_by_id_with_http_info(item_id, opts)

```ruby
begin
  # Get stock item by ID
  data, status_code, headers = api_instance.get_stock_item_by_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CatalogItemDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CatalogItemDtoEnvelope**](CatalogItemDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_categories_by_item_id

> <ItemCategoryDtoListEnvelope> get_stock_item_categories_by_item_id(item_id, opts)

Get categories for a stock item

Retrieves all categories associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get categories for a stock item
  result = api_instance.get_stock_item_categories_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_categories_by_item_id: #{e}"
end
```

#### Using the get_stock_item_categories_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCategoryDtoListEnvelope>, Integer, Hash)> get_stock_item_categories_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get categories for a stock item
  data, status_code, headers = api_instance.get_stock_item_categories_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_categories_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemCategoryDtoListEnvelope**](ItemCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_category_by_id

> <ItemCategoryDtoEnvelope> get_stock_item_category_by_id(item_id, item_category_id, opts)

Get category by ID for a stock item

Retrieves a specific category by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get category by ID for a stock item
  result = api_instance.get_stock_item_category_by_id(item_id, item_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_category_by_id: #{e}"
end
```

#### Using the get_stock_item_category_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCategoryDtoEnvelope>, Integer, Hash)> get_stock_item_category_by_id_with_http_info(item_id, item_category_id, opts)

```ruby
begin
  # Get category by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_category_by_id_with_http_info(item_id, item_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_category_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_google_categories_by_item_id

> <ItemGoogleCategoryDtoListEnvelope> get_stock_item_google_categories_by_item_id(item_id, opts)

Get Google categories for a stock item

Retrieves all Google categories associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Google categories for a stock item
  result = api_instance.get_stock_item_google_categories_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_google_categories_by_item_id: #{e}"
end
```

#### Using the get_stock_item_google_categories_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoListEnvelope>, Integer, Hash)> get_stock_item_google_categories_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get Google categories for a stock item
  data, status_code, headers = api_instance.get_stock_item_google_categories_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_google_categories_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_google_category_by_id

> <ItemGoogleCategoryDtoEnvelope> get_stock_item_google_category_by_id(item_id, item_google_category_id, opts)

Get Google category by ID for a stock item

Retrieves a specific Google category by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_google_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Google category by ID for a stock item
  result = api_instance.get_stock_item_google_category_by_id(item_id, item_google_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_google_category_by_id: #{e}"
end
```

#### Using the get_stock_item_google_category_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoEnvelope>, Integer, Hash)> get_stock_item_google_category_by_id_with_http_info(item_id, item_google_category_id, opts)

```ruby
begin
  # Get Google category by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_google_category_by_id_with_http_info(item_id, item_google_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_google_category_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_google_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoEnvelope**](ItemGoogleCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_image_by_id

> <ItemImageDtoEnvelope> get_stock_item_image_by_id(item_id, item_image_id, opts)

Get image by ID for a stock item

Retrieves a specific image by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_image_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get image by ID for a stock item
  result = api_instance.get_stock_item_image_by_id(item_id, item_image_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_image_by_id: #{e}"
end
```

#### Using the get_stock_item_image_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemImageDtoEnvelope>, Integer, Hash)> get_stock_item_image_by_id_with_http_info(item_id, item_image_id, opts)

```ruby
begin
  # Get image by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_image_by_id_with_http_info(item_id, item_image_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemImageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_image_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_image_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemImageDtoEnvelope**](ItemImageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_images_by_item_id

> <ItemImageDtoListEnvelope> get_stock_item_images_by_item_id(item_id, opts)

Get images for a stock item

Retrieves all images associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get images for a stock item
  result = api_instance.get_stock_item_images_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_images_by_item_id: #{e}"
end
```

#### Using the get_stock_item_images_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemImageDtoListEnvelope>, Integer, Hash)> get_stock_item_images_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get images for a stock item
  data, status_code, headers = api_instance.get_stock_item_images_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemImageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_images_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemImageDtoListEnvelope**](ItemImageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_price_rule_by_id

> <PricingRuleDtoEnvelope> get_stock_item_price_rule_by_id(item_id, item_price_rule_id, opts)

Get price rule by ID for a stock item

Retrieves a specific pricing rule by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_price_rule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get price rule by ID for a stock item
  result = api_instance.get_stock_item_price_rule_by_id(item_id, item_price_rule_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_price_rule_by_id: #{e}"
end
```

#### Using the get_stock_item_price_rule_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PricingRuleDtoEnvelope>, Integer, Hash)> get_stock_item_price_rule_by_id_with_http_info(item_id, item_price_rule_id, opts)

```ruby
begin
  # Get price rule by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_price_rule_by_id_with_http_info(item_id, item_price_rule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PricingRuleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_price_rule_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_price_rule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PricingRuleDtoEnvelope**](PricingRuleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_price_rules_by_item_id

> <PricingRuleDtoListEnvelope> get_stock_item_price_rules_by_item_id(item_id, opts)

Get price rules for a stock item

Retrieves all pricing rules associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get price rules for a stock item
  result = api_instance.get_stock_item_price_rules_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_price_rules_by_item_id: #{e}"
end
```

#### Using the get_stock_item_price_rules_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PricingRuleDtoListEnvelope>, Integer, Hash)> get_stock_item_price_rules_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get price rules for a stock item
  data, status_code, headers = api_instance.get_stock_item_price_rules_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PricingRuleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_price_rules_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PricingRuleDtoListEnvelope**](PricingRuleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_question_by_id

> <ItemQuestionDtoEnvelope> get_stock_item_question_by_id(item_id, item_question_id, opts)

Get question by ID for a stock item

Retrieves a specific question by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_question_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get question by ID for a stock item
  result = api_instance.get_stock_item_question_by_id(item_id, item_question_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_question_by_id: #{e}"
end
```

#### Using the get_stock_item_question_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemQuestionDtoEnvelope>, Integer, Hash)> get_stock_item_question_by_id_with_http_info(item_id, item_question_id, opts)

```ruby
begin
  # Get question by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_question_by_id_with_http_info(item_id, item_question_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemQuestionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_question_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_question_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemQuestionDtoEnvelope**](ItemQuestionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_questions_by_item_id

> <ItemQuestionDtoListEnvelope> get_stock_item_questions_by_item_id(item_id, opts)

Get questions for a stock item

Retrieves all questions associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get questions for a stock item
  result = api_instance.get_stock_item_questions_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_questions_by_item_id: #{e}"
end
```

#### Using the get_stock_item_questions_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemQuestionDtoListEnvelope>, Integer, Hash)> get_stock_item_questions_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get questions for a stock item
  data, status_code, headers = api_instance.get_stock_item_questions_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemQuestionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_questions_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemQuestionDtoListEnvelope**](ItemQuestionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_refund_policies_by_item_id

> <ItemRefundPolicyDtoListEnvelope> get_stock_item_refund_policies_by_item_id(item_id, opts)

Get refund policies for a stock item

Retrieves all refund policies associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get refund policies for a stock item
  result = api_instance.get_stock_item_refund_policies_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_refund_policies_by_item_id: #{e}"
end
```

#### Using the get_stock_item_refund_policies_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRefundPolicyDtoListEnvelope>, Integer, Hash)> get_stock_item_refund_policies_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get refund policies for a stock item
  data, status_code, headers = api_instance.get_stock_item_refund_policies_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRefundPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_refund_policies_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRefundPolicyDtoListEnvelope**](ItemRefundPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_refund_policy_by_id

> <ItemRefundPolicyDtoEnvelope> get_stock_item_refund_policy_by_id(item_id, item_refund_policy_id, opts)

Get refund policy by ID for a stock item

Retrieves a specific refund policy by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get refund policy by ID for a stock item
  result = api_instance.get_stock_item_refund_policy_by_id(item_id, item_refund_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_refund_policy_by_id: #{e}"
end
```

#### Using the get_stock_item_refund_policy_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRefundPolicyDtoEnvelope>, Integer, Hash)> get_stock_item_refund_policy_by_id_with_http_info(item_id, item_refund_policy_id, opts)

```ruby
begin
  # Get refund policy by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_refund_policy_by_id_with_http_info(item_id, item_refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRefundPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_refund_policy_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_refund_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRefundPolicyDtoEnvelope**](ItemRefundPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_return_policies_by_item_id

> <ItemReturnPolicyDtoListEnvelope> get_stock_item_return_policies_by_item_id(item_id, opts)

Get return policies for a stock item

Retrieves all return policies associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get return policies for a stock item
  result = api_instance.get_stock_item_return_policies_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_return_policies_by_item_id: #{e}"
end
```

#### Using the get_stock_item_return_policies_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReturnPolicyDtoListEnvelope>, Integer, Hash)> get_stock_item_return_policies_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get return policies for a stock item
  data, status_code, headers = api_instance.get_stock_item_return_policies_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReturnPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_return_policies_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReturnPolicyDtoListEnvelope**](ItemReturnPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_return_policy_by_id

> <ItemReturnPolicyDtoEnvelope> get_stock_item_return_policy_by_id(item_id, item_return_policy_id, opts)

Get return policy by ID for a stock item

Retrieves a specific return policy by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_return_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get return policy by ID for a stock item
  result = api_instance.get_stock_item_return_policy_by_id(item_id, item_return_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_return_policy_by_id: #{e}"
end
```

#### Using the get_stock_item_return_policy_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReturnPolicyDtoEnvelope>, Integer, Hash)> get_stock_item_return_policy_by_id_with_http_info(item_id, item_return_policy_id, opts)

```ruby
begin
  # Get return policy by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_return_policy_by_id_with_http_info(item_id, item_return_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReturnPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_return_policy_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_return_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReturnPolicyDtoEnvelope**](ItemReturnPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_review_by_id

> <ItemReviewDtoEnvelope> get_stock_item_review_by_id(item_id, item_review_id, opts)

Get review by ID for a stock item

Retrieves a specific review by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_review_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get review by ID for a stock item
  result = api_instance.get_stock_item_review_by_id(item_id, item_review_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_review_by_id: #{e}"
end
```

#### Using the get_stock_item_review_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReviewDtoEnvelope>, Integer, Hash)> get_stock_item_review_by_id_with_http_info(item_id, item_review_id, opts)

```ruby
begin
  # Get review by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_review_by_id_with_http_info(item_id, item_review_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReviewDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_review_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_review_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReviewDtoEnvelope**](ItemReviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_reviews_by_item_id

> <ItemReviewDtoListEnvelope> get_stock_item_reviews_by_item_id(item_id, opts)

Get reviews for a stock item

Retrieves all reviews associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get reviews for a stock item
  result = api_instance.get_stock_item_reviews_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_reviews_by_item_id: #{e}"
end
```

#### Using the get_stock_item_reviews_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReviewDtoListEnvelope>, Integer, Hash)> get_stock_item_reviews_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get reviews for a stock item
  data, status_code, headers = api_instance.get_stock_item_reviews_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReviewDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_reviews_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReviewDtoListEnvelope**](ItemReviewDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_shipping_policies_by_item_id

> <ItemShippingPolicyDtoListEnvelope> get_stock_item_shipping_policies_by_item_id(item_id, opts)

Get shipping policies for a stock item

Retrieves all shipping policies associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping policies for a stock item
  result = api_instance.get_stock_item_shipping_policies_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_shipping_policies_by_item_id: #{e}"
end
```

#### Using the get_stock_item_shipping_policies_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemShippingPolicyDtoListEnvelope>, Integer, Hash)> get_stock_item_shipping_policies_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get shipping policies for a stock item
  data, status_code, headers = api_instance.get_stock_item_shipping_policies_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemShippingPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_shipping_policies_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemShippingPolicyDtoListEnvelope**](ItemShippingPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_shipping_policy_by_id

> <ItemShippingPolicyDtoEnvelope> get_stock_item_shipping_policy_by_id(item_id, item_shipping_policy_id, opts)

Get shipping policy by ID for a stock item

Retrieves a specific shipping policy by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_shipping_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get shipping policy by ID for a stock item
  result = api_instance.get_stock_item_shipping_policy_by_id(item_id, item_shipping_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_shipping_policy_by_id: #{e}"
end
```

#### Using the get_stock_item_shipping_policy_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemShippingPolicyDtoEnvelope>, Integer, Hash)> get_stock_item_shipping_policy_by_id_with_http_info(item_id, item_shipping_policy_id, opts)

```ruby
begin
  # Get shipping policy by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_shipping_policy_by_id_with_http_info(item_id, item_shipping_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemShippingPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_shipping_policy_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_shipping_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemShippingPolicyDtoEnvelope**](ItemShippingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_tag_by_id

> <ItemTagDtoEnvelope> get_stock_item_tag_by_id(item_id, item_tag_id, opts)

Get tag by ID for a stock item

Retrieves a specific tag by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get tag by ID for a stock item
  result = api_instance.get_stock_item_tag_by_id(item_id, item_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_tag_by_id: #{e}"
end
```

#### Using the get_stock_item_tag_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTagDtoEnvelope>, Integer, Hash)> get_stock_item_tag_by_id_with_http_info(item_id, item_tag_id, opts)

```ruby
begin
  # Get tag by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_tag_by_id_with_http_info(item_id, item_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTagDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_tag_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_tags_by_item_id

> <ItemTagDtoListEnvelope> get_stock_item_tags_by_item_id(item_id, opts)

Get tags for a stock item

Retrieves all tags associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get tags for a stock item
  result = api_instance.get_stock_item_tags_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_tags_by_item_id: #{e}"
end
```

#### Using the get_stock_item_tags_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTagDtoListEnvelope>, Integer, Hash)> get_stock_item_tags_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get tags for a stock item
  data, status_code, headers = api_instance.get_stock_item_tags_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTagDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_tags_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTagDtoListEnvelope**](ItemTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_tax_policies_by_item_id

> <ItemTaxPolicyDtoListEnvelope> get_stock_item_tax_policies_by_item_id(item_id, opts)

Get tax policies for a stock item

Retrieves all tax policies associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get tax policies for a stock item
  result = api_instance.get_stock_item_tax_policies_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_tax_policies_by_item_id: #{e}"
end
```

#### Using the get_stock_item_tax_policies_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTaxPolicyDtoListEnvelope>, Integer, Hash)> get_stock_item_tax_policies_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get tax policies for a stock item
  data, status_code, headers = api_instance.get_stock_item_tax_policies_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTaxPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_tax_policies_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTaxPolicyDtoListEnvelope**](ItemTaxPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_tax_policy_by_id

> <ItemTaxPolicyDtoEnvelope> get_stock_item_tax_policy_by_id(item_id, item_tax_policy_id, opts)

Get tax policy by ID for a stock item

Retrieves a specific tax policy by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get tax policy by ID for a stock item
  result = api_instance.get_stock_item_tax_policy_by_id(item_id, item_tax_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_tax_policy_by_id: #{e}"
end
```

#### Using the get_stock_item_tax_policy_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTaxPolicyDtoEnvelope>, Integer, Hash)> get_stock_item_tax_policy_by_id_with_http_info(item_id, item_tax_policy_id, opts)

```ruby
begin
  # Get tax policy by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_tax_policy_by_id_with_http_info(item_id, item_tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTaxPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_tax_policy_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTaxPolicyDtoEnvelope**](ItemTaxPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_type_by_id

> <ItemTypeDtoEnvelope> get_stock_item_type_by_id(item_id, item_type_id, opts)

Get type by ID for a stock item

Retrieves a specific type by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get type by ID for a stock item
  result = api_instance.get_stock_item_type_by_id(item_id, item_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_type_by_id: #{e}"
end
```

#### Using the get_stock_item_type_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTypeDtoEnvelope>, Integer, Hash)> get_stock_item_type_by_id_with_http_info(item_id, item_type_id, opts)

```ruby
begin
  # Get type by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_type_by_id_with_http_info(item_id, item_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_type_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_types_by_item_id

> <ItemTypeDtoListEnvelope> get_stock_item_types_by_item_id(item_id, opts)

Get types for a stock item

Retrieves all types associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get types for a stock item
  result = api_instance.get_stock_item_types_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_types_by_item_id: #{e}"
end
```

#### Using the get_stock_item_types_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTypeDtoListEnvelope>, Integer, Hash)> get_stock_item_types_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get types for a stock item
  data, status_code, headers = api_instance.get_stock_item_types_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_types_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTypeDtoListEnvelope**](ItemTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_warranty_policies_by_item_id

> <ItemWarrantyPolicyDtoListEnvelope> get_stock_item_warranty_policies_by_item_id(item_id, opts)

Get warranty policies for a stock item

Retrieves all warranty policies associated with a specific stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get warranty policies for a stock item
  result = api_instance.get_stock_item_warranty_policies_by_item_id(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_warranty_policies_by_item_id: #{e}"
end
```

#### Using the get_stock_item_warranty_policies_by_item_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemWarrantyPolicyDtoListEnvelope>, Integer, Hash)> get_stock_item_warranty_policies_by_item_id_with_http_info(item_id, opts)

```ruby
begin
  # Get warranty policies for a stock item
  data, status_code, headers = api_instance.get_stock_item_warranty_policies_by_item_id_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemWarrantyPolicyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_warranty_policies_by_item_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemWarrantyPolicyDtoListEnvelope**](ItemWarrantyPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_item_warranty_policy_by_id

> <ItemWarrantyPolicyDtoEnvelope> get_stock_item_warranty_policy_by_id(item_id, item_warranty_policy_id, opts)

Get warranty policy by ID for a stock item

Retrieves a specific warranty policy by ID for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_warranty_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get warranty policy by ID for a stock item
  result = api_instance.get_stock_item_warranty_policy_by_id(item_id, item_warranty_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_warranty_policy_by_id: #{e}"
end
```

#### Using the get_stock_item_warranty_policy_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemWarrantyPolicyDtoEnvelope>, Integer, Hash)> get_stock_item_warranty_policy_by_id_with_http_info(item_id, item_warranty_policy_id, opts)

```ruby
begin
  # Get warranty policy by ID for a stock item
  data, status_code, headers = api_instance.get_stock_item_warranty_policy_by_id_with_http_info(item_id, item_warranty_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemWarrantyPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_item_warranty_policy_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_warranty_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemWarrantyPolicyDtoEnvelope**](ItemWarrantyPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_items_odata_max_price

> <MoneyEnvelope> get_stock_items_odata_max_price(opts)

Get max price of stock items

Retrieves the maximum price among all stock items, optionally filtered by tenant and OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get max price of stock items
  result = api_instance.get_stock_items_odata_max_price(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_items_odata_max_price: #{e}"
end
```

#### Using the get_stock_items_odata_max_price_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> get_stock_items_odata_max_price_with_http_info(opts)

```ruby
begin
  # Get max price of stock items
  data, status_code, headers = api_instance.get_stock_items_odata_max_price_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_items_odata_max_price_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_items_odata_min_price

> <MoneyEnvelope> get_stock_items_odata_min_price(opts)

Get min price of stock items

Retrieves the minimum price among all stock items, optionally filtered by tenant and OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get min price of stock items
  result = api_instance.get_stock_items_odata_min_price(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_items_odata_min_price: #{e}"
end
```

#### Using the get_stock_items_odata_min_price_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> get_stock_items_odata_min_price_with_http_info(opts)

```ruby
begin
  # Get min price of stock items
  data, status_code, headers = api_instance.get_stock_items_odata_min_price_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_items_odata_min_price_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stock_items_query

> <CatalogItemDtoListEnvelope> get_stock_items_query(opts)

Get all stock items

Retrieves all stock items, optionally filtered by tenant and OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all stock items
  result = api_instance.get_stock_items_query(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_items_query: #{e}"
end
```

#### Using the get_stock_items_query_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CatalogItemDtoListEnvelope>, Integer, Hash)> get_stock_items_query_with_http_info(opts)

```ruby
begin
  # Get all stock items
  data, status_code, headers = api_instance.get_stock_items_query_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CatalogItemDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->get_stock_items_query_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CatalogItemDtoListEnvelope**](CatalogItemDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_attachment_to_stock_item

> <ItemAttachmentDtoEnvelope> relate_attachment_to_stock_item(tenant_id, item_id, item_attachment_id, opts)

Relate attachment to stock item

Associates an attachment with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attachment_id = 'item_attachment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_attachment_create_dto: OpenapiClient::ItemAttachmentCreateDto.new # ItemAttachmentCreateDto | 
}

begin
  # Relate attachment to stock item
  result = api_instance.relate_attachment_to_stock_item(tenant_id, item_id, item_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_attachment_to_stock_item: #{e}"
end
```

#### Using the relate_attachment_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttachmentDtoEnvelope>, Integer, Hash)> relate_attachment_to_stock_item_with_http_info(tenant_id, item_id, item_attachment_id, opts)

```ruby
begin
  # Relate attachment to stock item
  data, status_code, headers = api_instance.relate_attachment_to_stock_item_with_http_info(tenant_id, item_id, item_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttachmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_attachment_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_attachment_create_dto** | [**ItemAttachmentCreateDto**](ItemAttachmentCreateDto.md) |  | [optional] |

### Return type

[**ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## relate_attribute_option_to_stock_item

> <ItemAttributeOptionDtoEnvelope> relate_attribute_option_to_stock_item(item_id, item_attribute_option_id, opts)

Relate attribute option to stock item

Associates an attribute option with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attribute_option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate attribute option to stock item
  result = api_instance.relate_attribute_option_to_stock_item(item_id, item_attribute_option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_attribute_option_to_stock_item: #{e}"
end
```

#### Using the relate_attribute_option_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeOptionDtoEnvelope>, Integer, Hash)> relate_attribute_option_to_stock_item_with_http_info(item_id, item_attribute_option_id, opts)

```ruby
begin
  # Relate attribute option to stock item
  data, status_code, headers = api_instance.relate_attribute_option_to_stock_item_with_http_info(item_id, item_attribute_option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeOptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_attribute_option_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_attribute_option_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_brand_to_stock_item

> <ItemBrandDtoEnvelope> relate_brand_to_stock_item(tenant_id, item_id, item_brand_id, opts)

Relate brand to stock item

Associates a brand with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_brand_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate brand to stock item
  result = api_instance.relate_brand_to_stock_item(tenant_id, item_id, item_brand_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_brand_to_stock_item: #{e}"
end
```

#### Using the relate_brand_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBrandDtoEnvelope>, Integer, Hash)> relate_brand_to_stock_item_with_http_info(tenant_id, item_id, item_brand_id, opts)

```ruby
begin
  # Relate brand to stock item
  data, status_code, headers = api_instance.relate_brand_to_stock_item_with_http_info(tenant_id, item_id, item_brand_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBrandDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_brand_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_brand_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_category_to_stock_item

> <ItemCategoryDtoEnvelope> relate_category_to_stock_item(tenant_id, item_id, item_category_id, opts)

Relate category to stock item

Associates a category with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate category to stock item
  result = api_instance.relate_category_to_stock_item(tenant_id, item_id, item_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_category_to_stock_item: #{e}"
end
```

#### Using the relate_category_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCategoryDtoEnvelope>, Integer, Hash)> relate_category_to_stock_item_with_http_info(tenant_id, item_id, item_category_id, opts)

```ruby
begin
  # Relate category to stock item
  data, status_code, headers = api_instance.relate_category_to_stock_item_with_http_info(tenant_id, item_id, item_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_category_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_google_category_to_stock_item

> <ItemGoogleCategoryDtoEnvelope> relate_google_category_to_stock_item(tenant_id, item_id, item_google_category_id, opts)

Relate Google category to stock item

Associates a Google category with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_google_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate Google category to stock item
  result = api_instance.relate_google_category_to_stock_item(tenant_id, item_id, item_google_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_google_category_to_stock_item: #{e}"
end
```

#### Using the relate_google_category_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoEnvelope>, Integer, Hash)> relate_google_category_to_stock_item_with_http_info(tenant_id, item_id, item_google_category_id, opts)

```ruby
begin
  # Relate Google category to stock item
  data, status_code, headers = api_instance.relate_google_category_to_stock_item_with_http_info(tenant_id, item_id, item_google_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_google_category_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_google_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoEnvelope**](ItemGoogleCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_image_to_stock_item

> <ItemImageDtoEnvelope> relate_image_to_stock_item(tenant_id, item_id, item_image_id, opts)

Relate image to stock item

Associates an image with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_image_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate image to stock item
  result = api_instance.relate_image_to_stock_item(tenant_id, item_id, item_image_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_image_to_stock_item: #{e}"
end
```

#### Using the relate_image_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemImageDtoEnvelope>, Integer, Hash)> relate_image_to_stock_item_with_http_info(tenant_id, item_id, item_image_id, opts)

```ruby
begin
  # Relate image to stock item
  data, status_code, headers = api_instance.relate_image_to_stock_item_with_http_info(tenant_id, item_id, item_image_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemImageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_image_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_image_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemImageDtoEnvelope**](ItemImageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_price_rule_to_stock_item

> <PricingRuleDtoEnvelope> relate_price_rule_to_stock_item(item_id, item_price_rule_id, opts)

Relate price rule to stock item

Associates a pricing rule with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_price_rule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate price rule to stock item
  result = api_instance.relate_price_rule_to_stock_item(item_id, item_price_rule_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_price_rule_to_stock_item: #{e}"
end
```

#### Using the relate_price_rule_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PricingRuleDtoEnvelope>, Integer, Hash)> relate_price_rule_to_stock_item_with_http_info(item_id, item_price_rule_id, opts)

```ruby
begin
  # Relate price rule to stock item
  data, status_code, headers = api_instance.relate_price_rule_to_stock_item_with_http_info(item_id, item_price_rule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PricingRuleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_price_rule_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_price_rule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PricingRuleDtoEnvelope**](PricingRuleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_question_to_stock_item

> <ItemQuestionDtoEnvelope> relate_question_to_stock_item(tenant_id, item_id, opts)

Create question for stock item

Creates a new question for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_question_record_create_dto: OpenapiClient::ItemQuestionRecordCreateDto.new({title: 'title_example', needs_revision: false, question: 'question_example'}) # ItemQuestionRecordCreateDto | 
}

begin
  # Create question for stock item
  result = api_instance.relate_question_to_stock_item(tenant_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_question_to_stock_item: #{e}"
end
```

#### Using the relate_question_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemQuestionDtoEnvelope>, Integer, Hash)> relate_question_to_stock_item_with_http_info(tenant_id, item_id, opts)

```ruby
begin
  # Create question for stock item
  data, status_code, headers = api_instance.relate_question_to_stock_item_with_http_info(tenant_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemQuestionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_question_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_question_record_create_dto** | [**ItemQuestionRecordCreateDto**](ItemQuestionRecordCreateDto.md) |  | [optional] |

### Return type

[**ItemQuestionDtoEnvelope**](ItemQuestionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## relate_refund_policy_to_stock_item

> <ItemRefundPolicyDtoEnvelope> relate_refund_policy_to_stock_item(tenant_id, item_id, item_refund_policy_id, opts)

Relate refund policy to stock item

Associates a refund policy with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate refund policy to stock item
  result = api_instance.relate_refund_policy_to_stock_item(tenant_id, item_id, item_refund_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_refund_policy_to_stock_item: #{e}"
end
```

#### Using the relate_refund_policy_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRefundPolicyDtoEnvelope>, Integer, Hash)> relate_refund_policy_to_stock_item_with_http_info(tenant_id, item_id, item_refund_policy_id, opts)

```ruby
begin
  # Relate refund policy to stock item
  data, status_code, headers = api_instance.relate_refund_policy_to_stock_item_with_http_info(tenant_id, item_id, item_refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRefundPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_refund_policy_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_refund_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRefundPolicyDtoEnvelope**](ItemRefundPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_return_policy_to_stock_item

> <ItemReturnPolicyDtoEnvelope> relate_return_policy_to_stock_item(tenant_id, item_id, item_return_policy_id, opts)

Relate return policy to stock item

Associates a return policy with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_return_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate return policy to stock item
  result = api_instance.relate_return_policy_to_stock_item(tenant_id, item_id, item_return_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_return_policy_to_stock_item: #{e}"
end
```

#### Using the relate_return_policy_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReturnPolicyDtoEnvelope>, Integer, Hash)> relate_return_policy_to_stock_item_with_http_info(tenant_id, item_id, item_return_policy_id, opts)

```ruby
begin
  # Relate return policy to stock item
  data, status_code, headers = api_instance.relate_return_policy_to_stock_item_with_http_info(tenant_id, item_id, item_return_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReturnPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_return_policy_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_return_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReturnPolicyDtoEnvelope**](ItemReturnPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_review_to_stock_item

> <ItemReviewDtoEnvelope> relate_review_to_stock_item(tenant_id, item_id, opts)

Create review for stock item

Creates a new review for a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_review_record_create_dto: OpenapiClient::ItemReviewRecordCreateDto.new # ItemReviewRecordCreateDto | 
}

begin
  # Create review for stock item
  result = api_instance.relate_review_to_stock_item(tenant_id, item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_review_to_stock_item: #{e}"
end
```

#### Using the relate_review_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReviewDtoEnvelope>, Integer, Hash)> relate_review_to_stock_item_with_http_info(tenant_id, item_id, opts)

```ruby
begin
  # Create review for stock item
  data, status_code, headers = api_instance.relate_review_to_stock_item_with_http_info(tenant_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReviewDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_review_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_review_record_create_dto** | [**ItemReviewRecordCreateDto**](ItemReviewRecordCreateDto.md) |  | [optional] |

### Return type

[**ItemReviewDtoEnvelope**](ItemReviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## relate_shipping_policy_to_stock_item

> <ItemShippingPolicyDtoEnvelope> relate_shipping_policy_to_stock_item(tenant_id, item_id, item_shipping_policy_id, opts)

Relate shipping policy to stock item

Associates a shipping policy with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_shipping_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate shipping policy to stock item
  result = api_instance.relate_shipping_policy_to_stock_item(tenant_id, item_id, item_shipping_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_shipping_policy_to_stock_item: #{e}"
end
```

#### Using the relate_shipping_policy_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemShippingPolicyDtoEnvelope>, Integer, Hash)> relate_shipping_policy_to_stock_item_with_http_info(tenant_id, item_id, item_shipping_policy_id, opts)

```ruby
begin
  # Relate shipping policy to stock item
  data, status_code, headers = api_instance.relate_shipping_policy_to_stock_item_with_http_info(tenant_id, item_id, item_shipping_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemShippingPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_shipping_policy_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_shipping_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemShippingPolicyDtoEnvelope**](ItemShippingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_tag_to_stock_item

> <ItemTagDtoEnvelope> relate_tag_to_stock_item(tenant_id, item_id, item_tag_id, opts)

Relate tag to stock item

Associates a tag with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate tag to stock item
  result = api_instance.relate_tag_to_stock_item(tenant_id, item_id, item_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_tag_to_stock_item: #{e}"
end
```

#### Using the relate_tag_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTagDtoEnvelope>, Integer, Hash)> relate_tag_to_stock_item_with_http_info(tenant_id, item_id, item_tag_id, opts)

```ruby
begin
  # Relate tag to stock item
  data, status_code, headers = api_instance.relate_tag_to_stock_item_with_http_info(tenant_id, item_id, item_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTagDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_tag_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_tax_policy_to_stock_item

> <ItemTaxPolicyDtoEnvelope> relate_tax_policy_to_stock_item(tenant_id, item_id, item_tax_policy_id, opts)

Relate tax policy to stock item

Associates a tax policy with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate tax policy to stock item
  result = api_instance.relate_tax_policy_to_stock_item(tenant_id, item_id, item_tax_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_tax_policy_to_stock_item: #{e}"
end
```

#### Using the relate_tax_policy_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTaxPolicyDtoEnvelope>, Integer, Hash)> relate_tax_policy_to_stock_item_with_http_info(tenant_id, item_id, item_tax_policy_id, opts)

```ruby
begin
  # Relate tax policy to stock item
  data, status_code, headers = api_instance.relate_tax_policy_to_stock_item_with_http_info(tenant_id, item_id, item_tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTaxPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_tax_policy_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTaxPolicyDtoEnvelope**](ItemTaxPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_type_to_stock_item

> <ItemTypeDtoEnvelope> relate_type_to_stock_item(tenant_id, item_id, item_type_id, opts)

Relate type to stock item

Associates a type with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate type to stock item
  result = api_instance.relate_type_to_stock_item(tenant_id, item_id, item_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_type_to_stock_item: #{e}"
end
```

#### Using the relate_type_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTypeDtoEnvelope>, Integer, Hash)> relate_type_to_stock_item_with_http_info(tenant_id, item_id, item_type_id, opts)

```ruby
begin
  # Relate type to stock item
  data, status_code, headers = api_instance.relate_type_to_stock_item_with_http_info(tenant_id, item_id, item_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_type_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## relate_warranty_policy_to_stock_item

> <ItemWarrantyPolicyDtoEnvelope> relate_warranty_policy_to_stock_item(tenant_id, item_id, item_warranty_policy_id, opts)

Relate warranty policy to stock item

Associates a warranty policy with a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_warranty_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Relate warranty policy to stock item
  result = api_instance.relate_warranty_policy_to_stock_item(tenant_id, item_id, item_warranty_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_warranty_policy_to_stock_item: #{e}"
end
```

#### Using the relate_warranty_policy_to_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemWarrantyPolicyDtoEnvelope>, Integer, Hash)> relate_warranty_policy_to_stock_item_with_http_info(tenant_id, item_id, item_warranty_policy_id, opts)

```ruby
begin
  # Relate warranty policy to stock item
  data, status_code, headers = api_instance.relate_warranty_policy_to_stock_item_with_http_info(tenant_id, item_id, item_warranty_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemWarrantyPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->relate_warranty_policy_to_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_warranty_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemWarrantyPolicyDtoEnvelope**](ItemWarrantyPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_attachment_from_stock_item

> <ItemAttachmentDtoEnvelope> remove_attachment_from_stock_item(tenant_id, item_id, item_attachment_id, opts)

Remove attachment from stock item

Removes an attachment from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove attachment from stock item
  result = api_instance.remove_attachment_from_stock_item(tenant_id, item_id, item_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_attachment_from_stock_item: #{e}"
end
```

#### Using the remove_attachment_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttachmentDtoEnvelope>, Integer, Hash)> remove_attachment_from_stock_item_with_http_info(tenant_id, item_id, item_attachment_id, opts)

```ruby
begin
  # Remove attachment from stock item
  data, status_code, headers = api_instance.remove_attachment_from_stock_item_with_http_info(tenant_id, item_id, item_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttachmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_attachment_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_attribute_option_from_stock_item

> <ItemAttributeOptionDtoEnvelope> remove_attribute_option_from_stock_item(item_id, item_attribute_option_id, opts)

Remove attribute option from stock item

Removes an attribute option from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attribute_option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove attribute option from stock item
  result = api_instance.remove_attribute_option_from_stock_item(item_id, item_attribute_option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_attribute_option_from_stock_item: #{e}"
end
```

#### Using the remove_attribute_option_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeOptionDtoEnvelope>, Integer, Hash)> remove_attribute_option_from_stock_item_with_http_info(item_id, item_attribute_option_id, opts)

```ruby
begin
  # Remove attribute option from stock item
  data, status_code, headers = api_instance.remove_attribute_option_from_stock_item_with_http_info(item_id, item_attribute_option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeOptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_attribute_option_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_attribute_option_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_brand_from_stock_item

> <ItemBrandDtoEnvelope> remove_brand_from_stock_item(tenant_id, item_id, item_brand_id, opts)

Remove brand from stock item

Removes a brand association from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_brand_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove brand from stock item
  result = api_instance.remove_brand_from_stock_item(tenant_id, item_id, item_brand_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_brand_from_stock_item: #{e}"
end
```

#### Using the remove_brand_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBrandDtoEnvelope>, Integer, Hash)> remove_brand_from_stock_item_with_http_info(tenant_id, item_id, item_brand_id, opts)

```ruby
begin
  # Remove brand from stock item
  data, status_code, headers = api_instance.remove_brand_from_stock_item_with_http_info(tenant_id, item_id, item_brand_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBrandDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_brand_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_brand_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_category_from_stock_item

> <ItemCategoryDtoEnvelope> remove_category_from_stock_item(tenant_id, item_id, item_category_id, opts)

Remove category from stock item

Removes a category association from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove category from stock item
  result = api_instance.remove_category_from_stock_item(tenant_id, item_id, item_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_category_from_stock_item: #{e}"
end
```

#### Using the remove_category_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCategoryDtoEnvelope>, Integer, Hash)> remove_category_from_stock_item_with_http_info(tenant_id, item_id, item_category_id, opts)

```ruby
begin
  # Remove category from stock item
  data, status_code, headers = api_instance.remove_category_from_stock_item_with_http_info(tenant_id, item_id, item_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_category_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_google_category_from_stock_item

> <ItemGoogleCategoryDtoEnvelope> remove_google_category_from_stock_item(tenant_id, item_id, item_google_category_id, opts)

Remove Google category from stock item

Removes a Google category from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_google_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove Google category from stock item
  result = api_instance.remove_google_category_from_stock_item(tenant_id, item_id, item_google_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_google_category_from_stock_item: #{e}"
end
```

#### Using the remove_google_category_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoEnvelope>, Integer, Hash)> remove_google_category_from_stock_item_with_http_info(tenant_id, item_id, item_google_category_id, opts)

```ruby
begin
  # Remove Google category from stock item
  data, status_code, headers = api_instance.remove_google_category_from_stock_item_with_http_info(tenant_id, item_id, item_google_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_google_category_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_google_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoEnvelope**](ItemGoogleCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_image_from_stock_item

> <ItemImageDtoEnvelope> remove_image_from_stock_item(tenant_id, item_id, item_image_id, opts)

Remove image from stock item

Removes an image association from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_image_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove image from stock item
  result = api_instance.remove_image_from_stock_item(tenant_id, item_id, item_image_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_image_from_stock_item: #{e}"
end
```

#### Using the remove_image_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemImageDtoEnvelope>, Integer, Hash)> remove_image_from_stock_item_with_http_info(tenant_id, item_id, item_image_id, opts)

```ruby
begin
  # Remove image from stock item
  data, status_code, headers = api_instance.remove_image_from_stock_item_with_http_info(tenant_id, item_id, item_image_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemImageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_image_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_image_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemImageDtoEnvelope**](ItemImageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_price_rule_from_stock_item

> <PricingRuleDtoEnvelope> remove_price_rule_from_stock_item(item_id, item_price_rule_id, opts)

Remove price rule from stock item

Removes a pricing rule from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_price_rule_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove price rule from stock item
  result = api_instance.remove_price_rule_from_stock_item(item_id, item_price_rule_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_price_rule_from_stock_item: #{e}"
end
```

#### Using the remove_price_rule_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PricingRuleDtoEnvelope>, Integer, Hash)> remove_price_rule_from_stock_item_with_http_info(item_id, item_price_rule_id, opts)

```ruby
begin
  # Remove price rule from stock item
  data, status_code, headers = api_instance.remove_price_rule_from_stock_item_with_http_info(item_id, item_price_rule_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PricingRuleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_price_rule_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **item_price_rule_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**PricingRuleDtoEnvelope**](PricingRuleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_question_from_stock_item

> <ItemQuestionDtoEnvelope> remove_question_from_stock_item(tenant_id, item_id, item_question_id, opts)

Remove question from stock item

Removes a question from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_question_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove question from stock item
  result = api_instance.remove_question_from_stock_item(tenant_id, item_id, item_question_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_question_from_stock_item: #{e}"
end
```

#### Using the remove_question_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemQuestionDtoEnvelope>, Integer, Hash)> remove_question_from_stock_item_with_http_info(tenant_id, item_id, item_question_id, opts)

```ruby
begin
  # Remove question from stock item
  data, status_code, headers = api_instance.remove_question_from_stock_item_with_http_info(tenant_id, item_id, item_question_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemQuestionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_question_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_question_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemQuestionDtoEnvelope**](ItemQuestionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_refund_policy_from_stock_item

> <ItemRefundPolicyDtoEnvelope> remove_refund_policy_from_stock_item(tenant_id, item_id, item_refund_policy_id, opts)

Remove refund policy from stock item

Removes a refund policy from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_refund_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove refund policy from stock item
  result = api_instance.remove_refund_policy_from_stock_item(tenant_id, item_id, item_refund_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_refund_policy_from_stock_item: #{e}"
end
```

#### Using the remove_refund_policy_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRefundPolicyDtoEnvelope>, Integer, Hash)> remove_refund_policy_from_stock_item_with_http_info(tenant_id, item_id, item_refund_policy_id, opts)

```ruby
begin
  # Remove refund policy from stock item
  data, status_code, headers = api_instance.remove_refund_policy_from_stock_item_with_http_info(tenant_id, item_id, item_refund_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRefundPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_refund_policy_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_refund_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRefundPolicyDtoEnvelope**](ItemRefundPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_return_policy_from_stock_item

> <ItemReturnPolicyDtoEnvelope> remove_return_policy_from_stock_item(tenant_id, item_id, item_return_policy_id, opts)

Remove return policy from stock item

Removes a return policy from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_return_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove return policy from stock item
  result = api_instance.remove_return_policy_from_stock_item(tenant_id, item_id, item_return_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_return_policy_from_stock_item: #{e}"
end
```

#### Using the remove_return_policy_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReturnPolicyDtoEnvelope>, Integer, Hash)> remove_return_policy_from_stock_item_with_http_info(tenant_id, item_id, item_return_policy_id, opts)

```ruby
begin
  # Remove return policy from stock item
  data, status_code, headers = api_instance.remove_return_policy_from_stock_item_with_http_info(tenant_id, item_id, item_return_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReturnPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_return_policy_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_return_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReturnPolicyDtoEnvelope**](ItemReturnPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_review_from_stock_item

> <ItemReviewDtoEnvelope> remove_review_from_stock_item(tenant_id, item_id, item_review_id, opts)

Remove review from stock item

Removes a review from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_review_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove review from stock item
  result = api_instance.remove_review_from_stock_item(tenant_id, item_id, item_review_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_review_from_stock_item: #{e}"
end
```

#### Using the remove_review_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemReviewDtoEnvelope>, Integer, Hash)> remove_review_from_stock_item_with_http_info(tenant_id, item_id, item_review_id, opts)

```ruby
begin
  # Remove review from stock item
  data, status_code, headers = api_instance.remove_review_from_stock_item_with_http_info(tenant_id, item_id, item_review_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemReviewDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_review_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_review_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemReviewDtoEnvelope**](ItemReviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_shipping_policy_from_stock_item

> <ItemShippingPolicyDtoEnvelope> remove_shipping_policy_from_stock_item(tenant_id, item_id, item_shipping_policy_id, opts)

Remove shipping policy from stock item

Removes a shipping policy from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_shipping_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove shipping policy from stock item
  result = api_instance.remove_shipping_policy_from_stock_item(tenant_id, item_id, item_shipping_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_shipping_policy_from_stock_item: #{e}"
end
```

#### Using the remove_shipping_policy_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemShippingPolicyDtoEnvelope>, Integer, Hash)> remove_shipping_policy_from_stock_item_with_http_info(tenant_id, item_id, item_shipping_policy_id, opts)

```ruby
begin
  # Remove shipping policy from stock item
  data, status_code, headers = api_instance.remove_shipping_policy_from_stock_item_with_http_info(tenant_id, item_id, item_shipping_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemShippingPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_shipping_policy_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_shipping_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemShippingPolicyDtoEnvelope**](ItemShippingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_tag_from_stock_item

> <ItemTagDtoEnvelope> remove_tag_from_stock_item(tenant_id, item_id, item_tag_id, opts)

Remove tag from stock item

Removes a tag association from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove tag from stock item
  result = api_instance.remove_tag_from_stock_item(tenant_id, item_id, item_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_tag_from_stock_item: #{e}"
end
```

#### Using the remove_tag_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTagDtoEnvelope>, Integer, Hash)> remove_tag_from_stock_item_with_http_info(tenant_id, item_id, item_tag_id, opts)

```ruby
begin
  # Remove tag from stock item
  data, status_code, headers = api_instance.remove_tag_from_stock_item_with_http_info(tenant_id, item_id, item_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTagDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_tag_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_tax_policy_from_stock_item

> <ItemTaxPolicyDtoEnvelope> remove_tax_policy_from_stock_item(tenant_id, item_id, item_tax_policy_id, opts)

Remove tax policy from stock item

Removes a tax policy from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tax_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove tax policy from stock item
  result = api_instance.remove_tax_policy_from_stock_item(tenant_id, item_id, item_tax_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_tax_policy_from_stock_item: #{e}"
end
```

#### Using the remove_tax_policy_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTaxPolicyDtoEnvelope>, Integer, Hash)> remove_tax_policy_from_stock_item_with_http_info(tenant_id, item_id, item_tax_policy_id, opts)

```ruby
begin
  # Remove tax policy from stock item
  data, status_code, headers = api_instance.remove_tax_policy_from_stock_item_with_http_info(tenant_id, item_id, item_tax_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTaxPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_tax_policy_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_tax_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTaxPolicyDtoEnvelope**](ItemTaxPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_type_from_stock_item

> <ItemTypeDtoEnvelope> remove_type_from_stock_item(tenant_id, item_id, item_type_id, opts)

Remove type from stock item

Removes a type association from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove type from stock item
  result = api_instance.remove_type_from_stock_item(tenant_id, item_id, item_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_type_from_stock_item: #{e}"
end
```

#### Using the remove_type_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTypeDtoEnvelope>, Integer, Hash)> remove_type_from_stock_item_with_http_info(tenant_id, item_id, item_type_id, opts)

```ruby
begin
  # Remove type from stock item
  data, status_code, headers = api_instance.remove_type_from_stock_item_with_http_info(tenant_id, item_id, item_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_type_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_warranty_policy_from_stock_item

> <ItemWarrantyPolicyDtoEnvelope> remove_warranty_policy_from_stock_item(tenant_id, item_id, item_warranty_policy_id, opts)

Remove warranty policy from stock item

Removes a warranty policy from a stock item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_warranty_policy_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove warranty policy from stock item
  result = api_instance.remove_warranty_policy_from_stock_item(tenant_id, item_id, item_warranty_policy_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_warranty_policy_from_stock_item: #{e}"
end
```

#### Using the remove_warranty_policy_from_stock_item_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemWarrantyPolicyDtoEnvelope>, Integer, Hash)> remove_warranty_policy_from_stock_item_with_http_info(tenant_id, item_id, item_warranty_policy_id, opts)

```ruby
begin
  # Remove warranty policy from stock item
  data, status_code, headers = api_instance.remove_warranty_policy_from_stock_item_with_http_info(tenant_id, item_id, item_warranty_policy_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemWarrantyPolicyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->remove_warranty_policy_from_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **item_warranty_policy_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemWarrantyPolicyDtoEnvelope**](ItemWarrantyPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_product_primary_image_async

> <EmptyEnvelope> update_product_primary_image_async(item_id, opts)

Update item primary image

Updates the primary image for a specific catalog item.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  data: File.new('/path/to/some/file') # File | 
}

begin
  # Update item primary image
  result = api_instance.update_product_primary_image_async(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->update_product_primary_image_async: #{e}"
end
```

#### Using the update_product_primary_image_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_product_primary_image_async_with_http_info(item_id, opts)

```ruby
begin
  # Update item primary image
  data, status_code, headers = api_instance.update_product_primary_image_async_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->update_product_primary_image_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **data** | **File** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml


## update_stock_item

> update_stock_item(tenant_id, item_id, opts)

Update a stock item

Updates an existing stock item for the specified tenant and item ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  catalog_item_update_dto: OpenapiClient::CatalogItemUpdateDto.new # CatalogItemUpdateDto | 
}

begin
  # Update a stock item
  api_instance.update_stock_item(tenant_id, item_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->update_stock_item: #{e}"
end
```

#### Using the update_stock_item_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_stock_item_with_http_info(tenant_id, item_id, opts)

```ruby
begin
  # Update a stock item
  data, status_code, headers = api_instance.update_stock_item_with_http_info(tenant_id, item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemsApi->update_stock_item_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **catalog_item_update_dto** | [**CatalogItemUpdateDto**](CatalogItemUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

