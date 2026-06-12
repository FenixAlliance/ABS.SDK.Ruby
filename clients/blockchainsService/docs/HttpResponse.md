# OpenapiClient::HttpResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **http_context** | [**HttpContext**](HttpContext.md) |  | [optional] |
| **status_code** | **Integer** |  | [optional] |
| **headers** | **Hash&lt;String, Array&lt;String&gt;&gt;** |  | [optional][readonly] |
| **body** | **File** |  | [optional] |
| **body_writer** | [**PipeWriter**](PipeWriter.md) |  | [optional] |
| **content_length** | **Integer** |  | [optional] |
| **content_type** | **String** |  | [optional] |
| **cookies** | **Object** |  | [optional] |
| **has_started** | **Boolean** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::HttpResponse.new(
  http_context: null,
  status_code: null,
  headers: null,
  body: null,
  body_writer: null,
  content_length: null,
  content_type: null,
  cookies: null,
  has_started: null
)
```

