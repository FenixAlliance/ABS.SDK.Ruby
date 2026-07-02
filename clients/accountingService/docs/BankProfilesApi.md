# OpenapiClient::BankProfilesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_bank_profiles**](BankProfilesApi.md#get_bank_profiles) | **GET** /api/v2/AccountingService/BankProfiles | Get all bank profiles for a tenant |
| [**get_bank_profiles_count**](BankProfilesApi.md#get_bank_profiles_count) | **GET** /api/v2/AccountingService/BankProfiles/Count | Get bank profiles count |


## get_bank_profiles

> <BankProfileDtoListEnvelope> get_bank_profiles(tenant_id, opts)

Get all bank profiles for a tenant

Retrieves all bank profiles for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all bank profiles for a tenant
  result = api_instance.get_bank_profiles(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankProfilesApi->get_bank_profiles: #{e}"
end
```

#### Using the get_bank_profiles_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BankProfileDtoListEnvelope>, Integer, Hash)> get_bank_profiles_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all bank profiles for a tenant
  data, status_code, headers = api_instance.get_bank_profiles_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BankProfileDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankProfilesApi->get_bank_profiles_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BankProfileDtoListEnvelope**](BankProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_bank_profiles_count

> <Int32Envelope> get_bank_profiles_count(tenant_id, opts)

Get bank profiles count

Returns the count of bank profiles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BankProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get bank profiles count
  result = api_instance.get_bank_profiles_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankProfilesApi->get_bank_profiles_count: #{e}"
end
```

#### Using the get_bank_profiles_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_bank_profiles_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get bank profiles count
  data, status_code, headers = api_instance.get_bank_profiles_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BankProfilesApi->get_bank_profiles_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

