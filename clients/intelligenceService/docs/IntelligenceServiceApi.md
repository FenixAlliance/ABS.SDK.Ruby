# OpenapiClient::IntelligenceServiceApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**invoke_agent_surface_async**](IntelligenceServiceApi.md#invoke_agent_surface_async) | **POST** /api/v2/IntelligenceService/Agents/{agentId}/agui | Run a governed agent over the AG-UI protocol |


## invoke_agent_surface_async

> invoke_agent_surface_async(agent_id)

Run a governed agent over the AG-UI protocol

Streams a governed agent run as AG-UI server-sent events. Feature-flagged on ABP.Cognitive.AgentSurface.Enable; returns 503 when disabled, 401 when unauthorized and 404 when the agent cannot be resolved. An optional ?projectId= binds the run to a project (resolved tenant-scoped): the project id + name are surfaced to the model as context so it can call the governed project-storage tools; it is never auto-filled into a tool's arguments.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::IntelligenceServiceApi.new
agent_id = 'agent_id_example' # String | 

begin
  # Run a governed agent over the AG-UI protocol
  api_instance.invoke_agent_surface_async(agent_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling IntelligenceServiceApi->invoke_agent_surface_async: #{e}"
end
```

#### Using the invoke_agent_surface_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> invoke_agent_surface_async_with_http_info(agent_id)

```ruby
begin
  # Run a governed agent over the AG-UI protocol
  data, status_code, headers = api_instance.invoke_agent_surface_async_with_http_info(agent_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling IntelligenceServiceApi->invoke_agent_surface_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **agent_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

