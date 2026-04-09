# OpenapiClient::CountriesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_countries**](CountriesApi.md#count_countries) | **GET** /api/v2/GlobeService/Countries/Count | Count countries |
| [**get_all_countries**](CountriesApi.md#get_all_countries) | **GET** /api/v2/GlobeService/Countries | Get all countries |
| [**get_calling_codes_by_country_id_async**](CountriesApi.md#get_calling_codes_by_country_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/CallingCodes | Get calling codes for a country |
| [**get_cities_by_country_state_id_async**](CountriesApi.md#get_cities_by_country_state_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/States/{countryStateId}/Cities | Get cities for a state |
| [**get_country_by_id**](CountriesApi.md#get_country_by_id) | **GET** /api/v2/GlobeService/Countries/{countryId} | Get country by ID |
| [**get_country_state_by_id_async**](CountriesApi.md#get_country_state_by_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/States/{countryStateId} | Get state by ID |
| [**get_country_states_async**](CountriesApi.md#get_country_states_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/States | Get states for a country |
| [**get_enabled_currencies_by_country_id_async**](CountriesApi.md#get_enabled_currencies_by_country_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/Currencies | Get currencies for a country |
| [**get_time_zones_by_country_id_async**](CountriesApi.md#get_time_zones_by_country_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/Timezones | Get timezones for a country |
| [**get_top_level_domains_by_country_id_async**](CountriesApi.md#get_top_level_domains_by_country_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/TopLevelDomains | Get top-level domains for a country |
| [**search_countries_by_name_async**](CountriesApi.md#search_countries_by_name_async) | **GET** /api/v2/GlobeService/Countries/Search | Search countries by name |


## count_countries

> <Int32Envelope> count_countries(opts)

Count countries

Returns the total number of countries, with optional OData filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count countries
  result = api_instance.count_countries(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->count_countries: #{e}"
end
```

#### Using the count_countries_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_countries_with_http_info(opts)

```ruby
begin
  # Count countries
  data, status_code, headers = api_instance.count_countries_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->count_countries_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_all_countries

> <CountryDtoListEnvelope> get_all_countries(opts)

Get all countries

Retrieves a list of all countries with optional OData pagination and filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all countries
  result = api_instance.get_all_countries(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_all_countries: #{e}"
end
```

#### Using the get_all_countries_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryDtoListEnvelope>, Integer, Hash)> get_all_countries_with_http_info(opts)

```ruby
begin
  # Get all countries
  data, status_code, headers = api_instance.get_all_countries_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_all_countries_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountryDtoListEnvelope**](CountryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_calling_codes_by_country_id_async

> <CountryCallingCodeDtoListEnvelope> get_calling_codes_by_country_id_async(country_id, opts)

Get calling codes for a country

Retrieves the list of international telephone calling codes associated with the specified country.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
country_id = 'country_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get calling codes for a country
  result = api_instance.get_calling_codes_by_country_id_async(country_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_calling_codes_by_country_id_async: #{e}"
end
```

#### Using the get_calling_codes_by_country_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryCallingCodeDtoListEnvelope>, Integer, Hash)> get_calling_codes_by_country_id_async_with_http_info(country_id, opts)

```ruby
begin
  # Get calling codes for a country
  data, status_code, headers = api_instance.get_calling_codes_by_country_id_async_with_http_info(country_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryCallingCodeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_calling_codes_by_country_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **country_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountryCallingCodeDtoListEnvelope**](CountryCallingCodeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_cities_by_country_state_id_async

> <CityDtoListEnvelope> get_cities_by_country_state_id_async(country_state_id, country_id, opts)

Get cities for a state

Retrieves the list of cities belonging to the specified state or province.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
country_state_id = 'country_state_id_example' # String | 
country_id = 'country_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get cities for a state
  result = api_instance.get_cities_by_country_state_id_async(country_state_id, country_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_cities_by_country_state_id_async: #{e}"
end
```

#### Using the get_cities_by_country_state_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CityDtoListEnvelope>, Integer, Hash)> get_cities_by_country_state_id_async_with_http_info(country_state_id, country_id, opts)

```ruby
begin
  # Get cities for a state
  data, status_code, headers = api_instance.get_cities_by_country_state_id_async_with_http_info(country_state_id, country_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CityDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_cities_by_country_state_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **country_state_id** | **String** |  |  |
| **country_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CityDtoListEnvelope**](CityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_country_by_id

> <CountryDtoEnvelope> get_country_by_id(country_id, opts)

Get country by ID

Retrieves a single country by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
country_id = 'country_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get country by ID
  result = api_instance.get_country_by_id(country_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_country_by_id: #{e}"
end
```

#### Using the get_country_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryDtoEnvelope>, Integer, Hash)> get_country_by_id_with_http_info(country_id, opts)

```ruby
begin
  # Get country by ID
  data, status_code, headers = api_instance.get_country_by_id_with_http_info(country_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_country_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **country_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountryDtoEnvelope**](CountryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_country_state_by_id_async

> <CountryStateDtoEnvelope> get_country_state_by_id_async(country_state_id, country_id, opts)

Get state by ID

Retrieves a single state or province by its unique identifier within a country.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
country_state_id = 'country_state_id_example' # String | 
country_id = 'country_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get state by ID
  result = api_instance.get_country_state_by_id_async(country_state_id, country_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_country_state_by_id_async: #{e}"
end
```

#### Using the get_country_state_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryStateDtoEnvelope>, Integer, Hash)> get_country_state_by_id_async_with_http_info(country_state_id, country_id, opts)

```ruby
begin
  # Get state by ID
  data, status_code, headers = api_instance.get_country_state_by_id_async_with_http_info(country_state_id, country_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryStateDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_country_state_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **country_state_id** | **String** |  |  |
| **country_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountryStateDtoEnvelope**](CountryStateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_country_states_async

> <CountryStateDtoListEnvelope> get_country_states_async(country_id, opts)

Get states for a country

Retrieves the list of states or provinces belonging to the specified country.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
country_id = 'country_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get states for a country
  result = api_instance.get_country_states_async(country_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_country_states_async: #{e}"
end
```

#### Using the get_country_states_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryStateDtoListEnvelope>, Integer, Hash)> get_country_states_async_with_http_info(country_id, opts)

```ruby
begin
  # Get states for a country
  data, status_code, headers = api_instance.get_country_states_async_with_http_info(country_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryStateDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_country_states_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **country_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountryStateDtoListEnvelope**](CountryStateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_enabled_currencies_by_country_id_async

> <CurrencyDtoListEnvelope> get_enabled_currencies_by_country_id_async(country_id, opts)

Get currencies for a country

Retrieves the list of enabled currencies for the specified country.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
country_id = 'country_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get currencies for a country
  result = api_instance.get_enabled_currencies_by_country_id_async(country_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_enabled_currencies_by_country_id_async: #{e}"
end
```

#### Using the get_enabled_currencies_by_country_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CurrencyDtoListEnvelope>, Integer, Hash)> get_enabled_currencies_by_country_id_async_with_http_info(country_id, opts)

```ruby
begin
  # Get currencies for a country
  data, status_code, headers = api_instance.get_enabled_currencies_by_country_id_async_with_http_info(country_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CurrencyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_enabled_currencies_by_country_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **country_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CurrencyDtoListEnvelope**](CurrencyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_time_zones_by_country_id_async

> <TimezoneDtoListEnvelope> get_time_zones_by_country_id_async(country_id, opts)

Get timezones for a country

Retrieves the list of timezones associated with the specified country.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
country_id = 'country_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get timezones for a country
  result = api_instance.get_time_zones_by_country_id_async(country_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_time_zones_by_country_id_async: #{e}"
end
```

#### Using the get_time_zones_by_country_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TimezoneDtoListEnvelope>, Integer, Hash)> get_time_zones_by_country_id_async_with_http_info(country_id, opts)

```ruby
begin
  # Get timezones for a country
  data, status_code, headers = api_instance.get_time_zones_by_country_id_async_with_http_info(country_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TimezoneDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_time_zones_by_country_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **country_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TimezoneDtoListEnvelope**](TimezoneDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_top_level_domains_by_country_id_async

> <CountryTopLevelDomainDtoListEnvelope> get_top_level_domains_by_country_id_async(country_id, opts)

Get top-level domains for a country

Retrieves the list of internet top-level domains (TLDs) associated with the specified country.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
country_id = 'country_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get top-level domains for a country
  result = api_instance.get_top_level_domains_by_country_id_async(country_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_top_level_domains_by_country_id_async: #{e}"
end
```

#### Using the get_top_level_domains_by_country_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryTopLevelDomainDtoListEnvelope>, Integer, Hash)> get_top_level_domains_by_country_id_async_with_http_info(country_id, opts)

```ruby
begin
  # Get top-level domains for a country
  data, status_code, headers = api_instance.get_top_level_domains_by_country_id_async_with_http_info(country_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryTopLevelDomainDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->get_top_level_domains_by_country_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **country_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountryTopLevelDomainDtoListEnvelope**](CountryTopLevelDomainDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## search_countries_by_name_async

> <CountryDtoListEnvelope> search_countries_by_name_async(country_name, opts)

Search countries by name

Searches for countries whose name matches the specified search term.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CountriesApi.new
country_name = 'country_name_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Search countries by name
  result = api_instance.search_countries_by_name_async(country_name, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->search_countries_by_name_async: #{e}"
end
```

#### Using the search_countries_by_name_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountryDtoListEnvelope>, Integer, Hash)> search_countries_by_name_async_with_http_info(country_name, opts)

```ruby
begin
  # Search countries by name
  data, status_code, headers = api_instance.search_countries_by_name_async_with_http_info(country_name, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CountriesApi->search_countries_by_name_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **country_name** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountryDtoListEnvelope**](CountryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

