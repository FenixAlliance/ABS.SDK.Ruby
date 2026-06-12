# OpenapiClient::ActivityFeedsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_activity_types_async**](ActivityFeedsApi.md#count_activity_types_async) | **GET** /api/v2/ActivitiesService/ActivityTypes/Count | Count Activity Types |
| [**create_activity_async**](ActivityFeedsApi.md#create_activity_async) | **POST** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities | Create an activity |
| [**create_activity_type_async**](ActivityFeedsApi.md#create_activity_type_async) | **POST** /api/v2/ActivitiesService/ActivityTypes | Create Activity Type |
| [**delete_activity_async**](ActivityFeedsApi.md#delete_activity_async) | **DELETE** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/{activityId} | Delete an activity |
| [**delete_activity_type_async**](ActivityFeedsApi.md#delete_activity_type_async) | **DELETE** /api/v2/ActivitiesService/ActivityTypes/{activityTypeId} | Delete Activity Type |
| [**get_activities_async**](ActivityFeedsApi.md#get_activities_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities | Get activities |
| [**get_activities_count_async**](ActivityFeedsApi.md#get_activities_count_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/Count | Count activities |
| [**get_activity_async**](ActivityFeedsApi.md#get_activity_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/{activityId} | Get activity by ID |
| [**get_activity_feed_async**](ActivityFeedsApi.md#get_activity_feed_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId} | Get activity feed by ID |
| [**get_activity_feeds_async**](ActivityFeedsApi.md#get_activity_feeds_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds | Get activity feeds |
| [**get_activity_feeds_count_async**](ActivityFeedsApi.md#get_activity_feeds_count_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/Count | Count activity feeds |
| [**get_activity_type_by_id_async**](ActivityFeedsApi.md#get_activity_type_by_id_async) | **GET** /api/v2/ActivitiesService/ActivityTypes/{activityTypeId} | Get Activity Type |
| [**get_activity_types_async**](ActivityFeedsApi.md#get_activity_types_async) | **GET** /api/v2/ActivitiesService/ActivityTypes | Get Activity Types |
| [**patch_activity_async**](ActivityFeedsApi.md#patch_activity_async) | **PATCH** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/{activityId} | Patch an activity |
| [**patch_activity_type_async**](ActivityFeedsApi.md#patch_activity_type_async) | **PATCH** /api/v2/ActivitiesService/ActivityTypes/{activityTypeId} | Patch Activity Type |
| [**update_activity_async**](ActivityFeedsApi.md#update_activity_async) | **PUT** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/{activityId} | Update an activity |
| [**update_activity_type_async**](ActivityFeedsApi.md#update_activity_type_async) | **PUT** /api/v2/ActivitiesService/ActivityTypes/{activityTypeId} | Update Activity Type |


## count_activity_types_async

> <Int32Envelope> count_activity_types_async(tenant_id, opts)

Count Activity Types

Count activity types for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count Activity Types
  result = api_instance.count_activity_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->count_activity_types_async: #{e}"
end
```

#### Using the count_activity_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_activity_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count Activity Types
  data, status_code, headers = api_instance.count_activity_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->count_activity_types_async_with_http_info: #{e}"
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


## create_activity_async

> <ActivityRecordDtoEnvelope> create_activity_async(tenant_id, activity_feed_id, opts)

Create an activity

Creates a new activity in a specific activity feed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  activity_record_create_dto: OpenapiClient::ActivityRecordCreateDto.new # ActivityRecordCreateDto | 
}

begin
  # Create an activity
  result = api_instance.create_activity_async(tenant_id, activity_feed_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->create_activity_async: #{e}"
end
```

#### Using the create_activity_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ActivityRecordDtoEnvelope>, Integer, Hash)> create_activity_async_with_http_info(tenant_id, activity_feed_id, opts)

```ruby
begin
  # Create an activity
  data, status_code, headers = api_instance.create_activity_async_with_http_info(tenant_id, activity_feed_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ActivityRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->create_activity_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_feed_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **activity_record_create_dto** | [**ActivityRecordCreateDto**](ActivityRecordCreateDto.md) |  | [optional] |

### Return type

[**ActivityRecordDtoEnvelope**](ActivityRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_activity_type_async

> <Envelope> create_activity_type_async(tenant_id, opts)

Create Activity Type

Create a new activity type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  activity_type_create_dto: OpenapiClient::ActivityTypeCreateDto.new # ActivityTypeCreateDto | 
}

begin
  # Create Activity Type
  result = api_instance.create_activity_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->create_activity_type_async: #{e}"
end
```

#### Using the create_activity_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> create_activity_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create Activity Type
  data, status_code, headers = api_instance.create_activity_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->create_activity_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **activity_type_create_dto** | [**ActivityTypeCreateDto**](ActivityTypeCreateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_activity_async

> <EmptyEnvelope> delete_activity_async(tenant_id, activity_feed_id, activity_id, opts)

Delete an activity

Deletes an activity from an activity feed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an activity
  result = api_instance.delete_activity_async(tenant_id, activity_feed_id, activity_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->delete_activity_async: #{e}"
end
```

#### Using the delete_activity_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_activity_async_with_http_info(tenant_id, activity_feed_id, activity_id, opts)

```ruby
begin
  # Delete an activity
  data, status_code, headers = api_instance.delete_activity_async_with_http_info(tenant_id, activity_feed_id, activity_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->delete_activity_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_feed_id** | **String** |  |  |
| **activity_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_activity_type_async

> <Envelope> delete_activity_type_async(tenant_id, activity_type_id, opts)

Delete Activity Type

Delete an activity type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete Activity Type
  result = api_instance.delete_activity_type_async(tenant_id, activity_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->delete_activity_type_async: #{e}"
end
```

#### Using the delete_activity_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> delete_activity_type_async_with_http_info(tenant_id, activity_type_id, opts)

```ruby
begin
  # Delete Activity Type
  data, status_code, headers = api_instance.delete_activity_type_async_with_http_info(tenant_id, activity_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->delete_activity_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_activities_async

> <ActivityRecordDtoListEnvelope> get_activities_async(tenant_id, activity_feed_id, opts)

Get activities

Retrieves activities for a specific activity feed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get activities
  result = api_instance.get_activities_async(tenant_id, activity_feed_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activities_async: #{e}"
end
```

#### Using the get_activities_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ActivityRecordDtoListEnvelope>, Integer, Hash)> get_activities_async_with_http_info(tenant_id, activity_feed_id, opts)

```ruby
begin
  # Get activities
  data, status_code, headers = api_instance.get_activities_async_with_http_info(tenant_id, activity_feed_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ActivityRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activities_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_feed_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ActivityRecordDtoListEnvelope**](ActivityRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_activities_count_async

> <Int32Envelope> get_activities_count_async(tenant_id, activity_feed_id, opts)

Count activities

Returns the count of activities for a specific activity feed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count activities
  result = api_instance.get_activities_count_async(tenant_id, activity_feed_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activities_count_async: #{e}"
end
```

#### Using the get_activities_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_activities_count_async_with_http_info(tenant_id, activity_feed_id, opts)

```ruby
begin
  # Count activities
  data, status_code, headers = api_instance.get_activities_count_async_with_http_info(tenant_id, activity_feed_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activities_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_feed_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_activity_async

> <ActivityRecordDtoEnvelope> get_activity_async(tenant_id, activity_feed_id, activity_id, opts)

Get activity by ID

Retrieves a specific activity by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get activity by ID
  result = api_instance.get_activity_async(tenant_id, activity_feed_id, activity_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_async: #{e}"
end
```

#### Using the get_activity_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ActivityRecordDtoEnvelope>, Integer, Hash)> get_activity_async_with_http_info(tenant_id, activity_feed_id, activity_id, opts)

```ruby
begin
  # Get activity by ID
  data, status_code, headers = api_instance.get_activity_async_with_http_info(tenant_id, activity_feed_id, activity_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ActivityRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_feed_id** | **String** |  |  |
| **activity_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ActivityRecordDtoEnvelope**](ActivityRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_activity_feed_async

> <ActivityFeedDtoEnvelope> get_activity_feed_async(tenant_id, activity_feed_id, opts)

Get activity feed by ID

Retrieves a specific activity feed by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get activity feed by ID
  result = api_instance.get_activity_feed_async(tenant_id, activity_feed_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_feed_async: #{e}"
end
```

#### Using the get_activity_feed_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ActivityFeedDtoEnvelope>, Integer, Hash)> get_activity_feed_async_with_http_info(tenant_id, activity_feed_id, opts)

```ruby
begin
  # Get activity feed by ID
  data, status_code, headers = api_instance.get_activity_feed_async_with_http_info(tenant_id, activity_feed_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ActivityFeedDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_feed_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_feed_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ActivityFeedDtoEnvelope**](ActivityFeedDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_activity_feeds_async

> <ActivityFeedDtoListEnvelope> get_activity_feeds_async(tenant_id, opts)

Get activity feeds

Retrieves a list of activity feeds for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get activity feeds
  result = api_instance.get_activity_feeds_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_feeds_async: #{e}"
end
```

#### Using the get_activity_feeds_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ActivityFeedDtoListEnvelope>, Integer, Hash)> get_activity_feeds_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get activity feeds
  data, status_code, headers = api_instance.get_activity_feeds_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ActivityFeedDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_feeds_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ActivityFeedDtoListEnvelope**](ActivityFeedDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_activity_feeds_count_async

> <Int32Envelope> get_activity_feeds_count_async(tenant_id, opts)

Count activity feeds

Returns the count of activity feeds for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count activity feeds
  result = api_instance.get_activity_feeds_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_feeds_count_async: #{e}"
end
```

#### Using the get_activity_feeds_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_activity_feeds_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count activity feeds
  data, status_code, headers = api_instance.get_activity_feeds_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_feeds_count_async_with_http_info: #{e}"
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


## get_activity_type_by_id_async

> <ActivityTypeDtoEnvelope> get_activity_type_by_id_async(tenant_id, activity_type_id, opts)

Get Activity Type

Get an activity type by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Activity Type
  result = api_instance.get_activity_type_by_id_async(tenant_id, activity_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_type_by_id_async: #{e}"
end
```

#### Using the get_activity_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ActivityTypeDtoEnvelope>, Integer, Hash)> get_activity_type_by_id_async_with_http_info(tenant_id, activity_type_id, opts)

```ruby
begin
  # Get Activity Type
  data, status_code, headers = api_instance.get_activity_type_by_id_async_with_http_info(tenant_id, activity_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ActivityTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_type_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ActivityTypeDtoEnvelope**](ActivityTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_activity_types_async

> <ActivityTypeDtoListEnvelope> get_activity_types_async(tenant_id, opts)

Get Activity Types

Get a list of activity types for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Activity Types
  result = api_instance.get_activity_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_types_async: #{e}"
end
```

#### Using the get_activity_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ActivityTypeDtoListEnvelope>, Integer, Hash)> get_activity_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get Activity Types
  data, status_code, headers = api_instance.get_activity_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ActivityTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->get_activity_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ActivityTypeDtoListEnvelope**](ActivityTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_activity_async

> <EmptyEnvelope> patch_activity_async(tenant_id, activity_feed_id, activity_id, opts)

Patch an activity

Patch an activity

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an activity
  result = api_instance.patch_activity_async(tenant_id, activity_feed_id, activity_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->patch_activity_async: #{e}"
end
```

#### Using the patch_activity_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_activity_async_with_http_info(tenant_id, activity_feed_id, activity_id, opts)

```ruby
begin
  # Patch an activity
  data, status_code, headers = api_instance.patch_activity_async_with_http_info(tenant_id, activity_feed_id, activity_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->patch_activity_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_feed_id** | **String** |  |  |
| **activity_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_activity_type_async

> <EmptyEnvelope> patch_activity_type_async(tenant_id, activity_type_id, opts)

Patch Activity Type

Patch an activity type

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch Activity Type
  result = api_instance.patch_activity_type_async(tenant_id, activity_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->patch_activity_type_async: #{e}"
end
```

#### Using the patch_activity_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_activity_type_async_with_http_info(tenant_id, activity_type_id, opts)

```ruby
begin
  # Patch Activity Type
  data, status_code, headers = api_instance.patch_activity_type_async_with_http_info(tenant_id, activity_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->patch_activity_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_activity_async

> <ActivityRecordDtoEnvelope> update_activity_async(tenant_id, activity_feed_id, activity_id, opts)

Update an activity

Updates an existing activity.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_feed_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  activity_record_update_dto: OpenapiClient::ActivityRecordUpdateDto.new # ActivityRecordUpdateDto | 
}

begin
  # Update an activity
  result = api_instance.update_activity_async(tenant_id, activity_feed_id, activity_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->update_activity_async: #{e}"
end
```

#### Using the update_activity_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ActivityRecordDtoEnvelope>, Integer, Hash)> update_activity_async_with_http_info(tenant_id, activity_feed_id, activity_id, opts)

```ruby
begin
  # Update an activity
  data, status_code, headers = api_instance.update_activity_async_with_http_info(tenant_id, activity_feed_id, activity_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ActivityRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->update_activity_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_feed_id** | **String** |  |  |
| **activity_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **activity_record_update_dto** | [**ActivityRecordUpdateDto**](ActivityRecordUpdateDto.md) |  | [optional] |

### Return type

[**ActivityRecordDtoEnvelope**](ActivityRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_activity_type_async

> <Envelope> update_activity_type_async(tenant_id, activity_type_id, opts)

Update Activity Type

Update an existing activity type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ActivityFeedsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
activity_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  activity_type_update_dto: OpenapiClient::ActivityTypeUpdateDto.new # ActivityTypeUpdateDto | 
}

begin
  # Update Activity Type
  result = api_instance.update_activity_type_async(tenant_id, activity_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->update_activity_type_async: #{e}"
end
```

#### Using the update_activity_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> update_activity_type_async_with_http_info(tenant_id, activity_type_id, opts)

```ruby
begin
  # Update Activity Type
  data, status_code, headers = api_instance.update_activity_type_async_with_http_info(tenant_id, activity_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ActivityFeedsApi->update_activity_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **activity_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **activity_type_update_dto** | [**ActivityTypeUpdateDto**](ActivityTypeUpdateDto.md) |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

