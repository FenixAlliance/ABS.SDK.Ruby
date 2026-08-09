# OpenapiClient::CompletionsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**api_v2_ai_service_completions_complete_get**](CompletionsApi.md#api_v2_ai_service_completions_complete_get) | **GET** /api/v2/IntelligenceService/Completions/Complete |  |


## api_v2_ai_service_completions_complete_get

> api_v2_ai_service_completions_complete_get(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CompletionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  conversation_id: 'conversation_id_example', # String | 
  message: 'message_example' # String | 
}

begin
  
  api_instance.api_v2_ai_service_completions_complete_get(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompletionsApi->api_v2_ai_service_completions_complete_get: #{e}"
end
```

#### Using the api_v2_ai_service_completions_complete_get_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> api_v2_ai_service_completions_complete_get_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_ai_service_completions_complete_get_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompletionsApi->api_v2_ai_service_completions_complete_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **conversation_id** | **String** |  | [optional] |
| **message** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json;odata.metadata=minimal;odata.streaming=true, application/json;odata.metadata=minimal;odata.streaming=false, application/json;odata.metadata=minimal, application/json;odata.metadata=full;odata.streaming=true, application/json;odata.metadata=full;odata.streaming=false, application/json;odata.metadata=full, application/json;odata.metadata=none;odata.streaming=true, application/json;odata.metadata=none;odata.streaming=false, application/json;odata.metadata=none, application/json;odata.streaming=true, application/json;odata.streaming=false, application/json, application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false, application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=true, application/json;odata.metadata=minimal;odata.streaming=false;IEEE754Compatible=false, application/json;odata.metadata=minimal;odata.streaming=false;IEEE754Compatible=true, application/json;odata.metadata=minimal;IEEE754Compatible=false, application/json;odata.metadata=minimal;IEEE754Compatible=true, application/json;odata.metadata=full;odata.streaming=true;IEEE754Compatible=false, application/json;odata.metadata=full;odata.streaming=true;IEEE754Compatible=true, application/json;odata.metadata=full;odata.streaming=false;IEEE754Compatible=false, application/json;odata.metadata=full;odata.streaming=false;IEEE754Compatible=true, application/json;odata.metadata=full;IEEE754Compatible=false, application/json;odata.metadata=full;IEEE754Compatible=true, application/json;odata.metadata=none;odata.streaming=true;IEEE754Compatible=false, application/json;odata.metadata=none;odata.streaming=true;IEEE754Compatible=true, application/json;odata.metadata=none;odata.streaming=false;IEEE754Compatible=true, application/json;odata.metadata=none;odata.streaming=false;IEEE754Compatible=false, application/json;odata.metadata=none;IEEE754Compatible=false, application/json;odata.metadata=none;IEEE754Compatible=true, application/json;odata.streaming=true;IEEE754Compatible=false, application/json;odata.streaming=true;IEEE754Compatible=true, application/json;odata.streaming=false;IEEE754Compatible=false, application/json;odata.streaming=false;IEEE754Compatible=true, application/json;IEEE754Compatible=false, application/json;IEEE754Compatible=true, application/xml, text/plain, application/octet-stream, text/json, text/xml

