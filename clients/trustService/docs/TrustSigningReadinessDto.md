# OpenapiClient::TrustSigningReadinessDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **can_proceed** | **Boolean** |  | [optional] |
| **blocking_reasons** | **Array&lt;String&gt;** |  | [optional] |
| **warnings** | **Array&lt;String&gt;** |  | [optional] |
| **resolved_document_title** | **String** |  | [optional] |
| **resolved_profile_display_name** | **String** |  | [optional] |
| **resolved_certificate_title** | **String** |  | [optional] |
| **expected_signature_format** | **String** |  | [optional] |
| **expected_signature_purpose** | **String** |  | [optional] |
| **expected_digest_algorithm** | **String** |  | [optional] |
| **expected_signature_algorithm** | **String** |  | [optional] |
| **expected_canonicalization_algorithm** | **String** |  | [optional] |
| **policy_identifier** | **String** |  | [optional] |
| **authority_profile** | **String** |  | [optional] |
| **requires_custody_provider** | **Boolean** |  | [optional] |
| **requires_source_artifact** | **Boolean** |  | [optional] |
| **requires_certificate** | **Boolean** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TrustSigningReadinessDto.new(
  can_proceed: null,
  blocking_reasons: null,
  warnings: null,
  resolved_document_title: null,
  resolved_profile_display_name: null,
  resolved_certificate_title: null,
  expected_signature_format: null,
  expected_signature_purpose: null,
  expected_digest_algorithm: null,
  expected_signature_algorithm: null,
  expected_canonicalization_algorithm: null,
  policy_identifier: null,
  authority_profile: null,
  requires_custody_provider: null,
  requires_source_artifact: null,
  requires_certificate: null,
  correlation_id: null
)
```

