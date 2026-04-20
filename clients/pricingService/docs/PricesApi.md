# OpenapiClient::PricesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_final_price**](PricesApi.md#get_final_price) | **GET** /api/v2/PricingService/Prices/{itemId}/FinalPrice | Gets the final price for an item |
| [**get_price**](PricesApi.md#get_price) | **GET** /api/v2/PricingService/Prices/{itemId}/Price | Gets the calculated price for an item |
| [**get_total_savings_in_usd**](PricesApi.md#get_total_savings_in_usd) | **GET** /api/v2/PricingService/Prices/{itemId}/TotalSavings | Gets total savings for an item |
| [**get_total_taxes_in_usd**](PricesApi.md#get_total_taxes_in_usd) | **GET** /api/v2/PricingService/Prices/{itemId}/TotalTaxes | Gets total taxes for an item |


## get_final_price

> <MoneyEnvelope> get_final_price(item_id, opts)

Gets the final price for an item

Gets the final price for an item after all discounts and taxes in the specified currency.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricesApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  currency_id: 'currency_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the final price for an item
  result = api_instance.get_final_price(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricesApi->get_final_price: #{e}"
end
```

#### Using the get_final_price_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> get_final_price_with_http_info(item_id, opts)

```ruby
begin
  # Gets the final price for an item
  data, status_code, headers = api_instance.get_final_price_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricesApi->get_final_price_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **currency_id** | **String** |  | [optional][default to &#39;USD.USA&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_price

> <ItemPriceCalculationEnvelope> get_price(item_id, opts)

Gets the calculated price for an item

Calculates the price for an item considering price list, discount list, quantity, and currency.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricesApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  price_list_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  discounts_list_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  quantity: 1.2, # Float | 
  currency_id: 'currency_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets the calculated price for an item
  result = api_instance.get_price(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricesApi->get_price: #{e}"
end
```

#### Using the get_price_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPriceCalculationEnvelope>, Integer, Hash)> get_price_with_http_info(item_id, opts)

```ruby
begin
  # Gets the calculated price for an item
  data, status_code, headers = api_instance.get_price_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPriceCalculationEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricesApi->get_price_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **price_list_id** | **String** |  | [optional] |
| **discounts_list_id** | **String** |  | [optional] |
| **quantity** | **Float** |  | [optional][default to 1] |
| **currency_id** | **String** |  | [optional][default to &#39;USD.USA&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemPriceCalculationEnvelope**](ItemPriceCalculationEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_total_savings_in_usd

> <MoneyEnvelope> get_total_savings_in_usd(item_id, opts)

Gets total savings for an item

Gets the total savings amount for an item in the specified currency.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricesApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  currency_id: 'currency_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets total savings for an item
  result = api_instance.get_total_savings_in_usd(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricesApi->get_total_savings_in_usd: #{e}"
end
```

#### Using the get_total_savings_in_usd_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> get_total_savings_in_usd_with_http_info(item_id, opts)

```ruby
begin
  # Gets total savings for an item
  data, status_code, headers = api_instance.get_total_savings_in_usd_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricesApi->get_total_savings_in_usd_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **currency_id** | **String** |  | [optional][default to &#39;USD.USA&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_total_taxes_in_usd

> <MoneyEnvelope> get_total_taxes_in_usd(item_id, opts)

Gets total taxes for an item

Gets the total tax amount for an item in the specified currency.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PricesApi.new
item_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  currency_id: 'currency_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Gets total taxes for an item
  result = api_instance.get_total_taxes_in_usd(item_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricesApi->get_total_taxes_in_usd: #{e}"
end
```

#### Using the get_total_taxes_in_usd_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> get_total_taxes_in_usd_with_http_info(item_id, opts)

```ruby
begin
  # Gets total taxes for an item
  data, status_code, headers = api_instance.get_total_taxes_in_usd_with_http_info(item_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PricesApi->get_total_taxes_in_usd_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_id** | **String** |  |  |
| **currency_id** | **String** |  | [optional][default to &#39;USD.USA&#39;] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

