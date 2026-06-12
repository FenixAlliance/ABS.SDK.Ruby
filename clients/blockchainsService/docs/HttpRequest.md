# OpenapiClient::HttpRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **http_context** | [**HttpContext**](HttpContext.md) |  | [optional] |
| **method** | **String** |  | [optional] |
| **scheme** | **String** |  | [optional] |
| **is_https** | **Boolean** |  | [optional] |
| **host** | [**HostString**](HostString.md) |  | [optional] |
| **path_base** | [**PathString**](PathString.md) |  | [optional] |
| **path** | [**PathString**](PathString.md) |  | [optional] |
| **query_string** | [**QueryString**](QueryString.md) |  | [optional] |
| **query** | [**Array&lt;StringStringValuesKeyValuePair&gt;**](StringStringValuesKeyValuePair.md) |  | [optional] |
| **protocol** | **String** |  | [optional] |
| **headers** | **Hash&lt;String, Array&lt;String&gt;&gt;** |  | [optional][readonly] |
| **cookies** | [**Array&lt;StringStringKeyValuePair&gt;**](StringStringKeyValuePair.md) |  | [optional] |
| **content_length** | **Integer** |  | [optional] |
| **content_type** | **String** |  | [optional] |
| **body** | **File** |  | [optional] |
| **body_reader** | **File** |  | [optional][readonly] |
| **has_form_content_type** | **Boolean** |  | [optional][readonly] |
| **form** | [**Array&lt;StringStringValuesKeyValuePair&gt;**](StringStringValuesKeyValuePair.md) |  | [optional] |
| **route_values** | **Hash&lt;String, Object&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::HttpRequest.new(
  http_context: null,
  method: null,
  scheme: null,
  is_https: null,
  host: null,
  path_base: null,
  path: null,
  query_string: null,
  query: null,
  protocol: null,
  headers: null,
  cookies: null,
  content_length: null,
  content_type: null,
  body: null,
  body_reader: null,
  has_form_content_type: null,
  form: null,
  route_values: null
)
```

