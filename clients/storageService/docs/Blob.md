# OpenapiClient::Blob

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **kind** | **String** |  | [optional] |
| **is_folder** | **Boolean** |  | [optional][readonly] |
| **is_file** | **Boolean** |  | [optional][readonly] |
| **folder_path** | **String** |  | [optional][readonly] |
| **name** | **String** |  | [optional][readonly] |
| **size** | **Integer** |  | [optional] |
| **md5** | **String** |  | [optional] |
| **created_time** | **Time** |  | [optional] |
| **last_modification_time** | **Time** |  | [optional] |
| **full_path** | **String** |  | [optional] |
| **properties** | **Hash&lt;String, Object&gt;** |  | [optional][readonly] |
| **metadata** | **Hash&lt;String, String&gt;** |  | [optional][readonly] |
| **is_root_folder** | **Boolean** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Blob.new(
  kind: null,
  is_folder: null,
  is_file: null,
  folder_path: null,
  name: null,
  size: null,
  md5: null,
  created_time: null,
  last_modification_time: null,
  full_path: null,
  properties: null,
  metadata: null,
  is_root_folder: null
)
```

