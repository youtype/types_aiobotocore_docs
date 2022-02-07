<a id="cloudfrontclient-for-aiobotocore-cloudfront-module"></a>

# CloudFrontClient for aiobotocore CloudFront module

> [Index](..) > [CloudFront](.) > CloudFrontClient

Auto-generated documentation for
[CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
type annotations stubs module
[types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

- [CloudFrontClient for aiobotocore CloudFront module](#cloudfrontclient-for-aiobotocore-cloudfront-module)
  - [CloudFrontClient](#cloudfrontclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_alias](#associate_alias)
    - [can_paginate](#can_paginate)
    - [create_cache_policy](#create_cache_policy)
    - [create_cloud_front_origin_access_identity](#create_cloud_front_origin_access_identity)
    - [create_distribution](#create_distribution)
    - [create_distribution_with_tags](#create_distribution_with_tags)
    - [create_field_level_encryption_config](#create_field_level_encryption_config)
    - [create_field_level_encryption_profile](#create_field_level_encryption_profile)
    - [create_function](#create_function)
    - [create_invalidation](#create_invalidation)
    - [create_key_group](#create_key_group)
    - [create_monitoring_subscription](#create_monitoring_subscription)
    - [create_origin_request_policy](#create_origin_request_policy)
    - [create_public_key](#create_public_key)
    - [create_realtime_log_config](#create_realtime_log_config)
    - [create_response_headers_policy](#create_response_headers_policy)
    - [create_streaming_distribution](#create_streaming_distribution)
    - [create_streaming_distribution_with_tags](#create_streaming_distribution_with_tags)
    - [delete_cache_policy](#delete_cache_policy)
    - [delete_cloud_front_origin_access_identity](#delete_cloud_front_origin_access_identity)
    - [delete_distribution](#delete_distribution)
    - [delete_field_level_encryption_config](#delete_field_level_encryption_config)
    - [delete_field_level_encryption_profile](#delete_field_level_encryption_profile)
    - [delete_function](#delete_function)
    - [delete_key_group](#delete_key_group)
    - [delete_monitoring_subscription](#delete_monitoring_subscription)
    - [delete_origin_request_policy](#delete_origin_request_policy)
    - [delete_public_key](#delete_public_key)
    - [delete_realtime_log_config](#delete_realtime_log_config)
    - [delete_response_headers_policy](#delete_response_headers_policy)
    - [delete_streaming_distribution](#delete_streaming_distribution)
    - [describe_function](#describe_function)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_cache_policy](#get_cache_policy)
    - [get_cache_policy_config](#get_cache_policy_config)
    - [get_cloud_front_origin_access_identity](#get_cloud_front_origin_access_identity)
    - [get_cloud_front_origin_access_identity_config](#get_cloud_front_origin_access_identity_config)
    - [get_distribution](#get_distribution)
    - [get_distribution_config](#get_distribution_config)
    - [get_field_level_encryption](#get_field_level_encryption)
    - [get_field_level_encryption_config](#get_field_level_encryption_config)
    - [get_field_level_encryption_profile](#get_field_level_encryption_profile)
    - [get_field_level_encryption_profile_config](#get_field_level_encryption_profile_config)
    - [get_function](#get_function)
    - [get_invalidation](#get_invalidation)
    - [get_key_group](#get_key_group)
    - [get_key_group_config](#get_key_group_config)
    - [get_monitoring_subscription](#get_monitoring_subscription)
    - [get_origin_request_policy](#get_origin_request_policy)
    - [get_origin_request_policy_config](#get_origin_request_policy_config)
    - [get_public_key](#get_public_key)
    - [get_public_key_config](#get_public_key_config)
    - [get_realtime_log_config](#get_realtime_log_config)
    - [get_response_headers_policy](#get_response_headers_policy)
    - [get_response_headers_policy_config](#get_response_headers_policy_config)
    - [get_streaming_distribution](#get_streaming_distribution)
    - [get_streaming_distribution_config](#get_streaming_distribution_config)
    - [list_cache_policies](#list_cache_policies)
    - [list_cloud_front_origin_access_identities](#list_cloud_front_origin_access_identities)
    - [list_conflicting_aliases](#list_conflicting_aliases)
    - [list_distributions](#list_distributions)
    - [list_distributions_by_cache_policy_id](#list_distributions_by_cache_policy_id)
    - [list_distributions_by_key_group](#list_distributions_by_key_group)
    - [list_distributions_by_origin_request_policy_id](#list_distributions_by_origin_request_policy_id)
    - [list_distributions_by_realtime_log_config](#list_distributions_by_realtime_log_config)
    - [list_distributions_by_response_headers_policy_id](#list_distributions_by_response_headers_policy_id)
    - [list_distributions_by_web_acl_id](#list_distributions_by_web_acl_id)
    - [list_field_level_encryption_configs](#list_field_level_encryption_configs)
    - [list_field_level_encryption_profiles](#list_field_level_encryption_profiles)
    - [list_functions](#list_functions)
    - [list_invalidations](#list_invalidations)
    - [list_key_groups](#list_key_groups)
    - [list_origin_request_policies](#list_origin_request_policies)
    - [list_public_keys](#list_public_keys)
    - [list_realtime_log_configs](#list_realtime_log_configs)
    - [list_response_headers_policies](#list_response_headers_policies)
    - [list_streaming_distributions](#list_streaming_distributions)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [publish_function](#publish_function)
    - [tag_resource](#tag_resource)
    - [test_function](#test_function)
    - [untag_resource](#untag_resource)
    - [update_cache_policy](#update_cache_policy)
    - [update_cloud_front_origin_access_identity](#update_cloud_front_origin_access_identity)
    - [update_distribution](#update_distribution)
    - [update_field_level_encryption_config](#update_field_level_encryption_config)
    - [update_field_level_encryption_profile](#update_field_level_encryption_profile)
    - [update_function](#update_function)
    - [update_key_group](#update_key_group)
    - [update_origin_request_policy](#update_origin_request_policy)
    - [update_public_key](#update_public_key)
    - [update_realtime_log_config](#update_realtime_log_config)
    - [update_response_headers_policy](#update_response_headers_policy)
    - [update_streaming_distribution](#update_streaming_distribution)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="cloudfrontclient"></a>

## CloudFrontClient

Type annotations for `session.create_client("cloudfront")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_cloudfront.client import CloudFrontClient

session = get_session()
async with session.create_client("cloudfront") as client:
    client: CloudFrontClient
```

Boto3 documentation:
[CloudFront.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_cloudfront.client import Exceptions

def handle_error(exc: Exceptions.AccessDenied) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDenied`
- `Exceptions.BatchTooLarge`
- `Exceptions.CNAMEAlreadyExists`
- `Exceptions.CachePolicyAlreadyExists`
- `Exceptions.CachePolicyInUse`
- `Exceptions.CannotChangeImmutablePublicKeyFields`
- `Exceptions.ClientError`
- `Exceptions.CloudFrontOriginAccessIdentityAlreadyExists`
- `Exceptions.CloudFrontOriginAccessIdentityInUse`
- `Exceptions.DistributionAlreadyExists`
- `Exceptions.DistributionNotDisabled`
- `Exceptions.FieldLevelEncryptionConfigAlreadyExists`
- `Exceptions.FieldLevelEncryptionConfigInUse`
- `Exceptions.FieldLevelEncryptionProfileAlreadyExists`
- `Exceptions.FieldLevelEncryptionProfileInUse`
- `Exceptions.FieldLevelEncryptionProfileSizeExceeded`
- `Exceptions.FunctionAlreadyExists`
- `Exceptions.FunctionInUse`
- `Exceptions.FunctionSizeLimitExceeded`
- `Exceptions.IllegalDelete`
- `Exceptions.IllegalFieldLevelEncryptionConfigAssociationWithCacheBehavior`
- `Exceptions.IllegalUpdate`
- `Exceptions.InconsistentQuantities`
- `Exceptions.InvalidArgument`
- `Exceptions.InvalidDefaultRootObject`
- `Exceptions.InvalidErrorCode`
- `Exceptions.InvalidForwardCookies`
- `Exceptions.InvalidFunctionAssociation`
- `Exceptions.InvalidGeoRestrictionParameter`
- `Exceptions.InvalidHeadersForS3Origin`
- `Exceptions.InvalidIfMatchVersion`
- `Exceptions.InvalidLambdaFunctionAssociation`
- `Exceptions.InvalidLocationCode`
- `Exceptions.InvalidMinimumProtocolVersion`
- `Exceptions.InvalidOrigin`
- `Exceptions.InvalidOriginAccessIdentity`
- `Exceptions.InvalidOriginKeepaliveTimeout`
- `Exceptions.InvalidOriginReadTimeout`
- `Exceptions.InvalidProtocolSettings`
- `Exceptions.InvalidQueryStringParameters`
- `Exceptions.InvalidRelativePath`
- `Exceptions.InvalidRequiredProtocol`
- `Exceptions.InvalidResponseCode`
- `Exceptions.InvalidTTLOrder`
- `Exceptions.InvalidTagging`
- `Exceptions.InvalidViewerCertificate`
- `Exceptions.InvalidWebACLId`
- `Exceptions.KeyGroupAlreadyExists`
- `Exceptions.MissingBody`
- `Exceptions.NoSuchCachePolicy`
- `Exceptions.NoSuchCloudFrontOriginAccessIdentity`
- `Exceptions.NoSuchDistribution`
- `Exceptions.NoSuchFieldLevelEncryptionConfig`
- `Exceptions.NoSuchFieldLevelEncryptionProfile`
- `Exceptions.NoSuchFunctionExists`
- `Exceptions.NoSuchInvalidation`
- `Exceptions.NoSuchOrigin`
- `Exceptions.NoSuchOriginRequestPolicy`
- `Exceptions.NoSuchPublicKey`
- `Exceptions.NoSuchRealtimeLogConfig`
- `Exceptions.NoSuchResource`
- `Exceptions.NoSuchResponseHeadersPolicy`
- `Exceptions.NoSuchStreamingDistribution`
- `Exceptions.OriginRequestPolicyAlreadyExists`
- `Exceptions.OriginRequestPolicyInUse`
- `Exceptions.PreconditionFailed`
- `Exceptions.PublicKeyAlreadyExists`
- `Exceptions.PublicKeyInUse`
- `Exceptions.QueryArgProfileEmpty`
- `Exceptions.RealtimeLogConfigAlreadyExists`
- `Exceptions.RealtimeLogConfigInUse`
- `Exceptions.RealtimeLogConfigOwnerMismatch`
- `Exceptions.ResourceInUse`
- `Exceptions.ResponseHeadersPolicyAlreadyExists`
- `Exceptions.ResponseHeadersPolicyInUse`
- `Exceptions.StreamingDistributionAlreadyExists`
- `Exceptions.StreamingDistributionNotDisabled`
- `Exceptions.TestFunctionFailed`
- `Exceptions.TooManyCacheBehaviors`
- `Exceptions.TooManyCachePolicies`
- `Exceptions.TooManyCertificates`
- `Exceptions.TooManyCloudFrontOriginAccessIdentities`
- `Exceptions.TooManyCookieNamesInWhiteList`
- `Exceptions.TooManyCookiesInCachePolicy`
- `Exceptions.TooManyCookiesInOriginRequestPolicy`
- `Exceptions.TooManyCustomHeadersInResponseHeadersPolicy`
- `Exceptions.TooManyDistributionCNAMEs`
- `Exceptions.TooManyDistributions`
- `Exceptions.TooManyDistributionsAssociatedToCachePolicy`
- `Exceptions.TooManyDistributionsAssociatedToFieldLevelEncryptionConfig`
- `Exceptions.TooManyDistributionsAssociatedToKeyGroup`
- `Exceptions.TooManyDistributionsAssociatedToOriginRequestPolicy`
- `Exceptions.TooManyDistributionsAssociatedToResponseHeadersPolicy`
- `Exceptions.TooManyDistributionsWithFunctionAssociations`
- `Exceptions.TooManyDistributionsWithLambdaAssociations`
- `Exceptions.TooManyDistributionsWithSingleFunctionARN`
- `Exceptions.TooManyFieldLevelEncryptionConfigs`
- `Exceptions.TooManyFieldLevelEncryptionContentTypeProfiles`
- `Exceptions.TooManyFieldLevelEncryptionEncryptionEntities`
- `Exceptions.TooManyFieldLevelEncryptionFieldPatterns`
- `Exceptions.TooManyFieldLevelEncryptionProfiles`
- `Exceptions.TooManyFieldLevelEncryptionQueryArgProfiles`
- `Exceptions.TooManyFunctionAssociations`
- `Exceptions.TooManyFunctions`
- `Exceptions.TooManyHeadersInCachePolicy`
- `Exceptions.TooManyHeadersInForwardedValues`
- `Exceptions.TooManyHeadersInOriginRequestPolicy`
- `Exceptions.TooManyInvalidationsInProgress`
- `Exceptions.TooManyKeyGroups`
- `Exceptions.TooManyKeyGroupsAssociatedToDistribution`
- `Exceptions.TooManyLambdaFunctionAssociations`
- `Exceptions.TooManyOriginCustomHeaders`
- `Exceptions.TooManyOriginGroupsPerDistribution`
- `Exceptions.TooManyOriginRequestPolicies`
- `Exceptions.TooManyOrigins`
- `Exceptions.TooManyPublicKeys`
- `Exceptions.TooManyPublicKeysInKeyGroup`
- `Exceptions.TooManyQueryStringParameters`
- `Exceptions.TooManyQueryStringsInCachePolicy`
- `Exceptions.TooManyQueryStringsInOriginRequestPolicy`
- `Exceptions.TooManyRealtimeLogConfigs`
- `Exceptions.TooManyResponseHeadersPolicies`
- `Exceptions.TooManyStreamingDistributionCNAMEs`
- `Exceptions.TooManyStreamingDistributions`
- `Exceptions.TooManyTrustedSigners`
- `Exceptions.TrustedKeyGroupDoesNotExist`
- `Exceptions.TrustedSignerDoesNotExist`
- `Exceptions.UnsupportedOperation`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CloudFrontClient exceptions.

Type annotations for `session.create_client("cloudfront").exceptions` method.

Boto3 documentation:
[CloudFront.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate_alias"></a>

### associate_alias

Associates an alias (also known as a CNAME or an alternate domain name) with a
CloudFront distribution.

Type annotations for `session.create_client("cloudfront").associate_alias`
method.

Boto3 documentation:
[CloudFront.Client.associate_alias](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.associate_alias)

Asynchronous method. Use `await associate_alias(...)` for a synchronous call.

Arguments mapping described in
[AssociateAliasRequestRequestTypeDef](./type_defs.md#associatealiasrequestrequesttypedef).

Keyword-only arguments:

- `TargetDistributionId`: `str` *(required)*
- `Alias`: `str` *(required)*

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("cloudfront").can_paginate` method.

Boto3 documentation:
[CloudFront.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_cache_policy"></a>

### create_cache_policy

Creates a cache policy.

Type annotations for `session.create_client("cloudfront").create_cache_policy`
method.

Boto3 documentation:
[CloudFront.Client.create_cache_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)

Asynchronous method. Use `await create_cache_policy(...)` for a synchronous
call.

Arguments mapping described in
[CreateCachePolicyRequestRequestTypeDef](./type_defs.md#createcachepolicyrequestrequesttypedef).

Keyword-only arguments:

- `CachePolicyConfig`:
  [CachePolicyConfigTypeDef](./type_defs.md#cachepolicyconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateCachePolicyResultTypeDef](./type_defs.md#createcachepolicyresulttypedef).

<a id="create_cloud_front_origin_access_identity"></a>

### create_cloud_front_origin_access_identity

Creates a new origin access identity.

Type annotations for
`session.create_client("cloudfront").create_cloud_front_origin_access_identity`
method.

Boto3 documentation:
[CloudFront.Client.create_cloud_front_origin_access_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)

Asynchronous method. Use `await create_cloud_front_origin_access_identity(...)`
for a synchronous call.

Arguments mapping described in
[CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef](./type_defs.md#createcloudfrontoriginaccessidentityrequestrequesttypedef).

Keyword-only arguments:

- `CloudFrontOriginAccessIdentityConfig`:
  [CloudFrontOriginAccessIdentityConfigTypeDef](./type_defs.md#cloudfrontoriginaccessidentityconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateCloudFrontOriginAccessIdentityResultTypeDef](./type_defs.md#createcloudfrontoriginaccessidentityresulttypedef).

<a id="create_distribution"></a>

### create_distribution

Creates a new web distribution.

Type annotations for `session.create_client("cloudfront").create_distribution`
method.

Boto3 documentation:
[CloudFront.Client.create_distribution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)

Asynchronous method. Use `await create_distribution(...)` for a synchronous
call.

Arguments mapping described in
[CreateDistributionRequestRequestTypeDef](./type_defs.md#createdistributionrequestrequesttypedef).

Keyword-only arguments:

- `DistributionConfig`:
  [DistributionConfigTypeDef](./type_defs.md#distributionconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateDistributionResultTypeDef](./type_defs.md#createdistributionresulttypedef).

<a id="create_distribution_with_tags"></a>

### create_distribution_with_tags

Create a new distribution with tags.

Type annotations for
`session.create_client("cloudfront").create_distribution_with_tags` method.

Boto3 documentation:
[CloudFront.Client.create_distribution_with_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)

Asynchronous method. Use `await create_distribution_with_tags(...)` for a
synchronous call.

Arguments mapping described in
[CreateDistributionWithTagsRequestRequestTypeDef](./type_defs.md#createdistributionwithtagsrequestrequesttypedef).

Keyword-only arguments:

- `DistributionConfigWithTags`:
  [DistributionConfigWithTagsTypeDef](./type_defs.md#distributionconfigwithtagstypedef)
  *(required)*

Returns a `Coroutine` for
[CreateDistributionWithTagsResultTypeDef](./type_defs.md#createdistributionwithtagsresulttypedef).

<a id="create_field_level_encryption_config"></a>

### create_field_level_encryption_config

Create a new field-level encryption configuration.

Type annotations for
`session.create_client("cloudfront").create_field_level_encryption_config`
method.

Boto3 documentation:
[CloudFront.Client.create_field_level_encryption_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)

Asynchronous method. Use `await create_field_level_encryption_config(...)` for
a synchronous call.

Arguments mapping described in
[CreateFieldLevelEncryptionConfigRequestRequestTypeDef](./type_defs.md#createfieldlevelencryptionconfigrequestrequesttypedef).

Keyword-only arguments:

- `FieldLevelEncryptionConfig`:
  [FieldLevelEncryptionConfigTypeDef](./type_defs.md#fieldlevelencryptionconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateFieldLevelEncryptionConfigResultTypeDef](./type_defs.md#createfieldlevelencryptionconfigresulttypedef).

<a id="create_field_level_encryption_profile"></a>

### create_field_level_encryption_profile

Create a field-level encryption profile.

Type annotations for
`session.create_client("cloudfront").create_field_level_encryption_profile`
method.

Boto3 documentation:
[CloudFront.Client.create_field_level_encryption_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)

Asynchronous method. Use `await create_field_level_encryption_profile(...)` for
a synchronous call.

Arguments mapping described in
[CreateFieldLevelEncryptionProfileRequestRequestTypeDef](./type_defs.md#createfieldlevelencryptionprofilerequestrequesttypedef).

Keyword-only arguments:

- `FieldLevelEncryptionProfileConfig`:
  [FieldLevelEncryptionProfileConfigTypeDef](./type_defs.md#fieldlevelencryptionprofileconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateFieldLevelEncryptionProfileResultTypeDef](./type_defs.md#createfieldlevelencryptionprofileresulttypedef).

<a id="create_function"></a>

### create_function

Creates a CloudFront function.

Type annotations for `session.create_client("cloudfront").create_function`
method.

Boto3 documentation:
[CloudFront.Client.create_function](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)

Asynchronous method. Use `await create_function(...)` for a synchronous call.

Arguments mapping described in
[CreateFunctionRequestRequestTypeDef](./type_defs.md#createfunctionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `FunctionConfig`:
  [FunctionConfigTypeDef](./type_defs.md#functionconfigtypedef) *(required)*
- `FunctionCode`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*

Returns a `Coroutine` for
[CreateFunctionResultTypeDef](./type_defs.md#createfunctionresulttypedef).

<a id="create_invalidation"></a>

### create_invalidation

Create a new invalidation.

Type annotations for `session.create_client("cloudfront").create_invalidation`
method.

Boto3 documentation:
[CloudFront.Client.create_invalidation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)

Asynchronous method. Use `await create_invalidation(...)` for a synchronous
call.

Arguments mapping described in
[CreateInvalidationRequestRequestTypeDef](./type_defs.md#createinvalidationrequestrequesttypedef).

Keyword-only arguments:

- `DistributionId`: `str` *(required)*
- `InvalidationBatch`:
  [InvalidationBatchTypeDef](./type_defs.md#invalidationbatchtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateInvalidationResultTypeDef](./type_defs.md#createinvalidationresulttypedef).

<a id="create_key_group"></a>

### create_key_group

Creates a key group that you can use with
[CloudFront signed URLs and signed cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)\_
.

Type annotations for `session.create_client("cloudfront").create_key_group`
method.

Boto3 documentation:
[CloudFront.Client.create_key_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)

Asynchronous method. Use `await create_key_group(...)` for a synchronous call.

Arguments mapping described in
[CreateKeyGroupRequestRequestTypeDef](./type_defs.md#createkeygrouprequestrequesttypedef).

Keyword-only arguments:

- `KeyGroupConfig`:
  [KeyGroupConfigTypeDef](./type_defs.md#keygroupconfigtypedef) *(required)*

Returns a `Coroutine` for
[CreateKeyGroupResultTypeDef](./type_defs.md#createkeygroupresulttypedef).

<a id="create_monitoring_subscription"></a>

### create_monitoring_subscription

Enables additional CloudWatch metrics for the specified CloudFront
distribution.

Type annotations for
`session.create_client("cloudfront").create_monitoring_subscription` method.

Boto3 documentation:
[CloudFront.Client.create_monitoring_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_monitoring_subscription)

Asynchronous method. Use `await create_monitoring_subscription(...)` for a
synchronous call.

Arguments mapping described in
[CreateMonitoringSubscriptionRequestRequestTypeDef](./type_defs.md#createmonitoringsubscriptionrequestrequesttypedef).

Keyword-only arguments:

- `DistributionId`: `str` *(required)*
- `MonitoringSubscription`:
  [MonitoringSubscriptionTypeDef](./type_defs.md#monitoringsubscriptiontypedef)
  *(required)*

Returns a `Coroutine` for
[CreateMonitoringSubscriptionResultTypeDef](./type_defs.md#createmonitoringsubscriptionresulttypedef).

<a id="create_origin_request_policy"></a>

### create_origin_request_policy

Creates an origin request policy.

Type annotations for
`session.create_client("cloudfront").create_origin_request_policy` method.

Boto3 documentation:
[CloudFront.Client.create_origin_request_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)

Asynchronous method. Use `await create_origin_request_policy(...)` for a
synchronous call.

Arguments mapping described in
[CreateOriginRequestPolicyRequestRequestTypeDef](./type_defs.md#createoriginrequestpolicyrequestrequesttypedef).

Keyword-only arguments:

- `OriginRequestPolicyConfig`:
  [OriginRequestPolicyConfigTypeDef](./type_defs.md#originrequestpolicyconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateOriginRequestPolicyResultTypeDef](./type_defs.md#createoriginrequestpolicyresulttypedef).

<a id="create_public_key"></a>

### create_public_key

Uploads a public key to CloudFront that you can use with
[signed URLs and signed cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)\_
, or with
`field-level encryption <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level- en...`.

Type annotations for `session.create_client("cloudfront").create_public_key`
method.

Boto3 documentation:
[CloudFront.Client.create_public_key](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_public_key)

Asynchronous method. Use `await create_public_key(...)` for a synchronous call.

Arguments mapping described in
[CreatePublicKeyRequestRequestTypeDef](./type_defs.md#createpublickeyrequestrequesttypedef).

Keyword-only arguments:

- `PublicKeyConfig`:
  [PublicKeyConfigTypeDef](./type_defs.md#publickeyconfigtypedef) *(required)*

Returns a `Coroutine` for
[CreatePublicKeyResultTypeDef](./type_defs.md#createpublickeyresulttypedef).

<a id="create_realtime_log_config"></a>

### create_realtime_log_config

Creates a real-time log configuration.

Type annotations for
`session.create_client("cloudfront").create_realtime_log_config` method.

Boto3 documentation:
[CloudFront.Client.create_realtime_log_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)

Asynchronous method. Use `await create_realtime_log_config(...)` for a
synchronous call.

Arguments mapping described in
[CreateRealtimeLogConfigRequestRequestTypeDef](./type_defs.md#createrealtimelogconfigrequestrequesttypedef).

Keyword-only arguments:

- `EndPoints`: `Sequence`\[[EndPointTypeDef](./type_defs.md#endpointtypedef)\]
  *(required)*
- `Fields`: `Sequence`\[`str`\] *(required)*
- `Name`: `str` *(required)*
- `SamplingRate`: `int` *(required)*

Returns a `Coroutine` for
[CreateRealtimeLogConfigResultTypeDef](./type_defs.md#createrealtimelogconfigresulttypedef).

<a id="create_response_headers_policy"></a>

### create_response_headers_policy

Creates a response headers policy.

Type annotations for
`session.create_client("cloudfront").create_response_headers_policy` method.

Boto3 documentation:
[CloudFront.Client.create_response_headers_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)

Asynchronous method. Use `await create_response_headers_policy(...)` for a
synchronous call.

Arguments mapping described in
[CreateResponseHeadersPolicyRequestRequestTypeDef](./type_defs.md#createresponseheaderspolicyrequestrequesttypedef).

Keyword-only arguments:

- `ResponseHeadersPolicyConfig`:
  [ResponseHeadersPolicyConfigTypeDef](./type_defs.md#responseheaderspolicyconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateResponseHeadersPolicyResultTypeDef](./type_defs.md#createresponseheaderspolicyresulttypedef).

<a id="create_streaming_distribution"></a>

### create_streaming_distribution

This API is deprecated.

Type annotations for
`session.create_client("cloudfront").create_streaming_distribution` method.

Boto3 documentation:
[CloudFront.Client.create_streaming_distribution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)

Asynchronous method. Use `await create_streaming_distribution(...)` for a
synchronous call.

Arguments mapping described in
[CreateStreamingDistributionRequestRequestTypeDef](./type_defs.md#createstreamingdistributionrequestrequesttypedef).

Keyword-only arguments:

- `StreamingDistributionConfig`:
  [StreamingDistributionConfigTypeDef](./type_defs.md#streamingdistributionconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateStreamingDistributionResultTypeDef](./type_defs.md#createstreamingdistributionresulttypedef).

<a id="create_streaming_distribution_with_tags"></a>

### create_streaming_distribution_with_tags

This API is deprecated.

Type annotations for
`session.create_client("cloudfront").create_streaming_distribution_with_tags`
method.

Boto3 documentation:
[CloudFront.Client.create_streaming_distribution_with_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution_with_tags)

Asynchronous method. Use `await create_streaming_distribution_with_tags(...)`
for a synchronous call.

Arguments mapping described in
[CreateStreamingDistributionWithTagsRequestRequestTypeDef](./type_defs.md#createstreamingdistributionwithtagsrequestrequesttypedef).

Keyword-only arguments:

- `StreamingDistributionConfigWithTags`:
  [StreamingDistributionConfigWithTagsTypeDef](./type_defs.md#streamingdistributionconfigwithtagstypedef)
  *(required)*

Returns a `Coroutine` for
[CreateStreamingDistributionWithTagsResultTypeDef](./type_defs.md#createstreamingdistributionwithtagsresulttypedef).

<a id="delete_cache_policy"></a>

### delete_cache_policy

Deletes a cache policy.

Type annotations for `session.create_client("cloudfront").delete_cache_policy`
method.

Boto3 documentation:
[CloudFront.Client.delete_cache_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_cache_policy)

Asynchronous method. Use `await delete_cache_policy(...)` for a synchronous
call.

Arguments mapping described in
[DeleteCachePolicyRequestRequestTypeDef](./type_defs.md#deletecachepolicyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="delete_cloud_front_origin_access_identity"></a>

### delete_cloud_front_origin_access_identity

Delete an origin access identity.

Type annotations for
`session.create_client("cloudfront").delete_cloud_front_origin_access_identity`
method.

Boto3 documentation:
[CloudFront.Client.delete_cloud_front_origin_access_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_cloud_front_origin_access_identity)

Asynchronous method. Use `await delete_cloud_front_origin_access_identity(...)`
for a synchronous call.

Arguments mapping described in
[DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef](./type_defs.md#deletecloudfrontoriginaccessidentityrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="delete_distribution"></a>

### delete_distribution

Delete a distribution.

Type annotations for `session.create_client("cloudfront").delete_distribution`
method.

Boto3 documentation:
[CloudFront.Client.delete_distribution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_distribution)

Asynchronous method. Use `await delete_distribution(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDistributionRequestRequestTypeDef](./type_defs.md#deletedistributionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="delete_field_level_encryption_config"></a>

### delete_field_level_encryption_config

Remove a field-level encryption configuration.

Type annotations for
`session.create_client("cloudfront").delete_field_level_encryption_config`
method.

Boto3 documentation:
[CloudFront.Client.delete_field_level_encryption_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_field_level_encryption_config)

Asynchronous method. Use `await delete_field_level_encryption_config(...)` for
a synchronous call.

Arguments mapping described in
[DeleteFieldLevelEncryptionConfigRequestRequestTypeDef](./type_defs.md#deletefieldlevelencryptionconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="delete_field_level_encryption_profile"></a>

### delete_field_level_encryption_profile

Remove a field-level encryption profile.

Type annotations for
`session.create_client("cloudfront").delete_field_level_encryption_profile`
method.

Boto3 documentation:
[CloudFront.Client.delete_field_level_encryption_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_field_level_encryption_profile)

Asynchronous method. Use `await delete_field_level_encryption_profile(...)` for
a synchronous call.

Arguments mapping described in
[DeleteFieldLevelEncryptionProfileRequestRequestTypeDef](./type_defs.md#deletefieldlevelencryptionprofilerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="delete_function"></a>

### delete_function

Deletes a CloudFront function.

Type annotations for `session.create_client("cloudfront").delete_function`
method.

Boto3 documentation:
[CloudFront.Client.delete_function](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_function)

Asynchronous method. Use `await delete_function(...)` for a synchronous call.

Arguments mapping described in
[DeleteFunctionRequestRequestTypeDef](./type_defs.md#deletefunctionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `IfMatch`: `str` *(required)*

<a id="delete_key_group"></a>

### delete_key_group

Deletes a key group.

Type annotations for `session.create_client("cloudfront").delete_key_group`
method.

Boto3 documentation:
[CloudFront.Client.delete_key_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_key_group)

Asynchronous method. Use `await delete_key_group(...)` for a synchronous call.

Arguments mapping described in
[DeleteKeyGroupRequestRequestTypeDef](./type_defs.md#deletekeygrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="delete_monitoring_subscription"></a>

### delete_monitoring_subscription

Disables additional CloudWatch metrics for the specified CloudFront
distribution.

Type annotations for
`session.create_client("cloudfront").delete_monitoring_subscription` method.

Boto3 documentation:
[CloudFront.Client.delete_monitoring_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_monitoring_subscription)

Asynchronous method. Use `await delete_monitoring_subscription(...)` for a
synchronous call.

Arguments mapping described in
[DeleteMonitoringSubscriptionRequestRequestTypeDef](./type_defs.md#deletemonitoringsubscriptionrequestrequesttypedef).

Keyword-only arguments:

- `DistributionId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_origin_request_policy"></a>

### delete_origin_request_policy

Deletes an origin request policy.

Type annotations for
`session.create_client("cloudfront").delete_origin_request_policy` method.

Boto3 documentation:
[CloudFront.Client.delete_origin_request_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_origin_request_policy)

Asynchronous method. Use `await delete_origin_request_policy(...)` for a
synchronous call.

Arguments mapping described in
[DeleteOriginRequestPolicyRequestRequestTypeDef](./type_defs.md#deleteoriginrequestpolicyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="delete_public_key"></a>

### delete_public_key

Remove a public key you previously added to CloudFront.

Type annotations for `session.create_client("cloudfront").delete_public_key`
method.

Boto3 documentation:
[CloudFront.Client.delete_public_key](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_public_key)

Asynchronous method. Use `await delete_public_key(...)` for a synchronous call.

Arguments mapping described in
[DeletePublicKeyRequestRequestTypeDef](./type_defs.md#deletepublickeyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="delete_realtime_log_config"></a>

### delete_realtime_log_config

Deletes a real-time log configuration.

Type annotations for
`session.create_client("cloudfront").delete_realtime_log_config` method.

Boto3 documentation:
[CloudFront.Client.delete_realtime_log_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_realtime_log_config)

Asynchronous method. Use `await delete_realtime_log_config(...)` for a
synchronous call.

Arguments mapping described in
[DeleteRealtimeLogConfigRequestRequestTypeDef](./type_defs.md#deleterealtimelogconfigrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str`
- `ARN`: `str`

<a id="delete_response_headers_policy"></a>

### delete_response_headers_policy

Deletes a response headers policy.

Type annotations for
`session.create_client("cloudfront").delete_response_headers_policy` method.

Boto3 documentation:
[CloudFront.Client.delete_response_headers_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_response_headers_policy)

Asynchronous method. Use `await delete_response_headers_policy(...)` for a
synchronous call.

Arguments mapping described in
[DeleteResponseHeadersPolicyRequestRequestTypeDef](./type_defs.md#deleteresponseheaderspolicyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="delete_streaming_distribution"></a>

### delete_streaming_distribution

Delete a streaming distribution.

Type annotations for
`session.create_client("cloudfront").delete_streaming_distribution` method.

Boto3 documentation:
[CloudFront.Client.delete_streaming_distribution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_streaming_distribution)

Asynchronous method. Use `await delete_streaming_distribution(...)` for a
synchronous call.

Arguments mapping described in
[DeleteStreamingDistributionRequestRequestTypeDef](./type_defs.md#deletestreamingdistributionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IfMatch`: `str`

<a id="describe_function"></a>

### describe_function

Gets configuration information and metadata about a CloudFront function, but
not the function’s code.

Type annotations for `session.create_client("cloudfront").describe_function`
method.

Boto3 documentation:
[CloudFront.Client.describe_function](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.describe_function)

Asynchronous method. Use `await describe_function(...)` for a synchronous call.

Arguments mapping described in
[DescribeFunctionRequestRequestTypeDef](./type_defs.md#describefunctionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Stage`: [FunctionStageType](./literals.md#functionstagetype)

Returns a `Coroutine` for
[DescribeFunctionResultTypeDef](./type_defs.md#describefunctionresulttypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("cloudfront").generate_presigned_url` method.

Boto3 documentation:
[CloudFront.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_cache_policy"></a>

### get_cache_policy

Gets a cache policy, including the following metadata * The policy’s
identifier.

Type annotations for `session.create_client("cloudfront").get_cache_policy`
method.

Boto3 documentation:
[CloudFront.Client.get_cache_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cache_policy)

Asynchronous method. Use `await get_cache_policy(...)` for a synchronous call.

Arguments mapping described in
[GetCachePolicyRequestRequestTypeDef](./type_defs.md#getcachepolicyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetCachePolicyResultTypeDef](./type_defs.md#getcachepolicyresulttypedef).

<a id="get_cache_policy_config"></a>

### get_cache_policy_config

Gets a cache policy configuration.

Type annotations for
`session.create_client("cloudfront").get_cache_policy_config` method.

Boto3 documentation:
[CloudFront.Client.get_cache_policy_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cache_policy_config)

Asynchronous method. Use `await get_cache_policy_config(...)` for a synchronous
call.

Arguments mapping described in
[GetCachePolicyConfigRequestRequestTypeDef](./type_defs.md#getcachepolicyconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetCachePolicyConfigResultTypeDef](./type_defs.md#getcachepolicyconfigresulttypedef).

<a id="get_cloud_front_origin_access_identity"></a>

### get_cloud_front_origin_access_identity

Get the information about an origin access identity.

Type annotations for
`session.create_client("cloudfront").get_cloud_front_origin_access_identity`
method.

Boto3 documentation:
[CloudFront.Client.get_cloud_front_origin_access_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cloud_front_origin_access_identity)

Asynchronous method. Use `await get_cloud_front_origin_access_identity(...)`
for a synchronous call.

Arguments mapping described in
[GetCloudFrontOriginAccessIdentityRequestRequestTypeDef](./type_defs.md#getcloudfrontoriginaccessidentityrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetCloudFrontOriginAccessIdentityResultTypeDef](./type_defs.md#getcloudfrontoriginaccessidentityresulttypedef).

<a id="get_cloud_front_origin_access_identity_config"></a>

### get_cloud_front_origin_access_identity_config

Get the configuration information about an origin access identity.

Type annotations for
`session.create_client("cloudfront").get_cloud_front_origin_access_identity_config`
method.

Boto3 documentation:
[CloudFront.Client.get_cloud_front_origin_access_identity_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cloud_front_origin_access_identity_config)

Asynchronous method. Use
`await get_cloud_front_origin_access_identity_config(...)` for a synchronous
call.

Arguments mapping described in
[GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef](./type_defs.md#getcloudfrontoriginaccessidentityconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetCloudFrontOriginAccessIdentityConfigResultTypeDef](./type_defs.md#getcloudfrontoriginaccessidentityconfigresulttypedef).

<a id="get_distribution"></a>

### get_distribution

Get the information about a distribution.

Type annotations for `session.create_client("cloudfront").get_distribution`
method.

Boto3 documentation:
[CloudFront.Client.get_distribution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_distribution)

Asynchronous method. Use `await get_distribution(...)` for a synchronous call.

Arguments mapping described in
[GetDistributionRequestRequestTypeDef](./type_defs.md#getdistributionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetDistributionResultTypeDef](./type_defs.md#getdistributionresulttypedef).

<a id="get_distribution_config"></a>

### get_distribution_config

Get the configuration information about a distribution.

Type annotations for
`session.create_client("cloudfront").get_distribution_config` method.

Boto3 documentation:
[CloudFront.Client.get_distribution_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_distribution_config)

Asynchronous method. Use `await get_distribution_config(...)` for a synchronous
call.

Arguments mapping described in
[GetDistributionConfigRequestRequestTypeDef](./type_defs.md#getdistributionconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetDistributionConfigResultTypeDef](./type_defs.md#getdistributionconfigresulttypedef).

<a id="get_field_level_encryption"></a>

### get_field_level_encryption

Get the field-level encryption configuration information.

Type annotations for
`session.create_client("cloudfront").get_field_level_encryption` method.

Boto3 documentation:
[CloudFront.Client.get_field_level_encryption](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption)

Asynchronous method. Use `await get_field_level_encryption(...)` for a
synchronous call.

Arguments mapping described in
[GetFieldLevelEncryptionRequestRequestTypeDef](./type_defs.md#getfieldlevelencryptionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetFieldLevelEncryptionResultTypeDef](./type_defs.md#getfieldlevelencryptionresulttypedef).

<a id="get_field_level_encryption_config"></a>

### get_field_level_encryption_config

Get the field-level encryption configuration information.

Type annotations for
`session.create_client("cloudfront").get_field_level_encryption_config` method.

Boto3 documentation:
[CloudFront.Client.get_field_level_encryption_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption_config)

Asynchronous method. Use `await get_field_level_encryption_config(...)` for a
synchronous call.

Arguments mapping described in
[GetFieldLevelEncryptionConfigRequestRequestTypeDef](./type_defs.md#getfieldlevelencryptionconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetFieldLevelEncryptionConfigResultTypeDef](./type_defs.md#getfieldlevelencryptionconfigresulttypedef).

<a id="get_field_level_encryption_profile"></a>

### get_field_level_encryption_profile

Get the field-level encryption profile information.

Type annotations for
`session.create_client("cloudfront").get_field_level_encryption_profile`
method.

Boto3 documentation:
[CloudFront.Client.get_field_level_encryption_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption_profile)

Asynchronous method. Use `await get_field_level_encryption_profile(...)` for a
synchronous call.

Arguments mapping described in
[GetFieldLevelEncryptionProfileRequestRequestTypeDef](./type_defs.md#getfieldlevelencryptionprofilerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetFieldLevelEncryptionProfileResultTypeDef](./type_defs.md#getfieldlevelencryptionprofileresulttypedef).

<a id="get_field_level_encryption_profile_config"></a>

### get_field_level_encryption_profile_config

Get the field-level encryption profile configuration information.

Type annotations for
`session.create_client("cloudfront").get_field_level_encryption_profile_config`
method.

Boto3 documentation:
[CloudFront.Client.get_field_level_encryption_profile_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption_profile_config)

Asynchronous method. Use `await get_field_level_encryption_profile_config(...)`
for a synchronous call.

Arguments mapping described in
[GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef](./type_defs.md#getfieldlevelencryptionprofileconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetFieldLevelEncryptionProfileConfigResultTypeDef](./type_defs.md#getfieldlevelencryptionprofileconfigresulttypedef).

<a id="get_function"></a>

### get_function

Gets the code of a CloudFront function.

Type annotations for `session.create_client("cloudfront").get_function` method.

Boto3 documentation:
[CloudFront.Client.get_function](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_function)

Asynchronous method. Use `await get_function(...)` for a synchronous call.

Arguments mapping described in
[GetFunctionRequestRequestTypeDef](./type_defs.md#getfunctionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Stage`: [FunctionStageType](./literals.md#functionstagetype)

Returns a `Coroutine` for
[GetFunctionResultTypeDef](./type_defs.md#getfunctionresulttypedef).

<a id="get_invalidation"></a>

### get_invalidation

Get the information about an invalidation.

Type annotations for `session.create_client("cloudfront").get_invalidation`
method.

Boto3 documentation:
[CloudFront.Client.get_invalidation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_invalidation)

Asynchronous method. Use `await get_invalidation(...)` for a synchronous call.

Arguments mapping described in
[GetInvalidationRequestRequestTypeDef](./type_defs.md#getinvalidationrequestrequesttypedef).

Keyword-only arguments:

- `DistributionId`: `str` *(required)*
- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetInvalidationResultTypeDef](./type_defs.md#getinvalidationresulttypedef).

<a id="get_key_group"></a>

### get_key_group

Gets a key group, including the date and time when the key group was last
modified.

Type annotations for `session.create_client("cloudfront").get_key_group`
method.

Boto3 documentation:
[CloudFront.Client.get_key_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_key_group)

Asynchronous method. Use `await get_key_group(...)` for a synchronous call.

Arguments mapping described in
[GetKeyGroupRequestRequestTypeDef](./type_defs.md#getkeygrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetKeyGroupResultTypeDef](./type_defs.md#getkeygroupresulttypedef).

<a id="get_key_group_config"></a>

### get_key_group_config

Gets a key group configuration.

Type annotations for `session.create_client("cloudfront").get_key_group_config`
method.

Boto3 documentation:
[CloudFront.Client.get_key_group_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_key_group_config)

Asynchronous method. Use `await get_key_group_config(...)` for a synchronous
call.

Arguments mapping described in
[GetKeyGroupConfigRequestRequestTypeDef](./type_defs.md#getkeygroupconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetKeyGroupConfigResultTypeDef](./type_defs.md#getkeygroupconfigresulttypedef).

<a id="get_monitoring_subscription"></a>

### get_monitoring_subscription

Gets information about whether additional CloudWatch metrics are enabled for
the specified CloudFront distribution.

Type annotations for
`session.create_client("cloudfront").get_monitoring_subscription` method.

Boto3 documentation:
[CloudFront.Client.get_monitoring_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_monitoring_subscription)

Asynchronous method. Use `await get_monitoring_subscription(...)` for a
synchronous call.

Arguments mapping described in
[GetMonitoringSubscriptionRequestRequestTypeDef](./type_defs.md#getmonitoringsubscriptionrequestrequesttypedef).

Keyword-only arguments:

- `DistributionId`: `str` *(required)*

Returns a `Coroutine` for
[GetMonitoringSubscriptionResultTypeDef](./type_defs.md#getmonitoringsubscriptionresulttypedef).

<a id="get_origin_request_policy"></a>

### get_origin_request_policy

Gets an origin request policy, including the following metadata * The policy’s
identifier.

Type annotations for
`session.create_client("cloudfront").get_origin_request_policy` method.

Boto3 documentation:
[CloudFront.Client.get_origin_request_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_request_policy)

Asynchronous method. Use `await get_origin_request_policy(...)` for a
synchronous call.

Arguments mapping described in
[GetOriginRequestPolicyRequestRequestTypeDef](./type_defs.md#getoriginrequestpolicyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetOriginRequestPolicyResultTypeDef](./type_defs.md#getoriginrequestpolicyresulttypedef).

<a id="get_origin_request_policy_config"></a>

### get_origin_request_policy_config

Gets an origin request policy configuration.

Type annotations for
`session.create_client("cloudfront").get_origin_request_policy_config` method.

Boto3 documentation:
[CloudFront.Client.get_origin_request_policy_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_request_policy_config)

Asynchronous method. Use `await get_origin_request_policy_config(...)` for a
synchronous call.

Arguments mapping described in
[GetOriginRequestPolicyConfigRequestRequestTypeDef](./type_defs.md#getoriginrequestpolicyconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetOriginRequestPolicyConfigResultTypeDef](./type_defs.md#getoriginrequestpolicyconfigresulttypedef).

<a id="get_public_key"></a>

### get_public_key

Gets a public key.

Type annotations for `session.create_client("cloudfront").get_public_key`
method.

Boto3 documentation:
[CloudFront.Client.get_public_key](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_public_key)

Asynchronous method. Use `await get_public_key(...)` for a synchronous call.

Arguments mapping described in
[GetPublicKeyRequestRequestTypeDef](./type_defs.md#getpublickeyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetPublicKeyResultTypeDef](./type_defs.md#getpublickeyresulttypedef).

<a id="get_public_key_config"></a>

### get_public_key_config

Gets a public key configuration.

Type annotations for
`session.create_client("cloudfront").get_public_key_config` method.

Boto3 documentation:
[CloudFront.Client.get_public_key_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_public_key_config)

Asynchronous method. Use `await get_public_key_config(...)` for a synchronous
call.

Arguments mapping described in
[GetPublicKeyConfigRequestRequestTypeDef](./type_defs.md#getpublickeyconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetPublicKeyConfigResultTypeDef](./type_defs.md#getpublickeyconfigresulttypedef).

<a id="get_realtime_log_config"></a>

### get_realtime_log_config

Gets a real-time log configuration.

Type annotations for
`session.create_client("cloudfront").get_realtime_log_config` method.

Boto3 documentation:
[CloudFront.Client.get_realtime_log_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_realtime_log_config)

Asynchronous method. Use `await get_realtime_log_config(...)` for a synchronous
call.

Arguments mapping described in
[GetRealtimeLogConfigRequestRequestTypeDef](./type_defs.md#getrealtimelogconfigrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str`
- `ARN`: `str`

Returns a `Coroutine` for
[GetRealtimeLogConfigResultTypeDef](./type_defs.md#getrealtimelogconfigresulttypedef).

<a id="get_response_headers_policy"></a>

### get_response_headers_policy

Gets a response headers policy, including metadata (the policy’s identifier and
the date and time when the policy was last modified).

Type annotations for
`session.create_client("cloudfront").get_response_headers_policy` method.

Boto3 documentation:
[CloudFront.Client.get_response_headers_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_response_headers_policy)

Asynchronous method. Use `await get_response_headers_policy(...)` for a
synchronous call.

Arguments mapping described in
[GetResponseHeadersPolicyRequestRequestTypeDef](./type_defs.md#getresponseheaderspolicyrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetResponseHeadersPolicyResultTypeDef](./type_defs.md#getresponseheaderspolicyresulttypedef).

<a id="get_response_headers_policy_config"></a>

### get_response_headers_policy_config

Gets a response headers policy configuration.

Type annotations for
`session.create_client("cloudfront").get_response_headers_policy_config`
method.

Boto3 documentation:
[CloudFront.Client.get_response_headers_policy_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_response_headers_policy_config)

Asynchronous method. Use `await get_response_headers_policy_config(...)` for a
synchronous call.

Arguments mapping described in
[GetResponseHeadersPolicyConfigRequestRequestTypeDef](./type_defs.md#getresponseheaderspolicyconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetResponseHeadersPolicyConfigResultTypeDef](./type_defs.md#getresponseheaderspolicyconfigresulttypedef).

<a id="get_streaming_distribution"></a>

### get_streaming_distribution

Gets information about a specified RTMP distribution, including the
distribution configuration.

Type annotations for
`session.create_client("cloudfront").get_streaming_distribution` method.

Boto3 documentation:
[CloudFront.Client.get_streaming_distribution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_streaming_distribution)

Asynchronous method. Use `await get_streaming_distribution(...)` for a
synchronous call.

Arguments mapping described in
[GetStreamingDistributionRequestRequestTypeDef](./type_defs.md#getstreamingdistributionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetStreamingDistributionResultTypeDef](./type_defs.md#getstreamingdistributionresulttypedef).

<a id="get_streaming_distribution_config"></a>

### get_streaming_distribution_config

Get the configuration information about a streaming distribution.

Type annotations for
`session.create_client("cloudfront").get_streaming_distribution_config` method.

Boto3 documentation:
[CloudFront.Client.get_streaming_distribution_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_streaming_distribution_config)

Asynchronous method. Use `await get_streaming_distribution_config(...)` for a
synchronous call.

Arguments mapping described in
[GetStreamingDistributionConfigRequestRequestTypeDef](./type_defs.md#getstreamingdistributionconfigrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetStreamingDistributionConfigResultTypeDef](./type_defs.md#getstreamingdistributionconfigresulttypedef).

<a id="list_cache_policies"></a>

### list_cache_policies

Gets a list of cache policies.

Type annotations for `session.create_client("cloudfront").list_cache_policies`
method.

Boto3 documentation:
[CloudFront.Client.list_cache_policies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_cache_policies)

Asynchronous method. Use `await list_cache_policies(...)` for a synchronous
call.

Arguments mapping described in
[ListCachePoliciesRequestRequestTypeDef](./type_defs.md#listcachepoliciesrequestrequesttypedef).

Keyword-only arguments:

- `Type`: [CachePolicyTypeType](./literals.md#cachepolicytypetype)
- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListCachePoliciesResultTypeDef](./type_defs.md#listcachepoliciesresulttypedef).

<a id="list_cloud_front_origin_access_identities"></a>

### list_cloud_front_origin_access_identities

Lists origin access identities.

Type annotations for
`session.create_client("cloudfront").list_cloud_front_origin_access_identities`
method.

Boto3 documentation:
[CloudFront.Client.list_cloud_front_origin_access_identities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_cloud_front_origin_access_identities)

Asynchronous method. Use `await list_cloud_front_origin_access_identities(...)`
for a synchronous call.

Arguments mapping described in
[ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListCloudFrontOriginAccessIdentitiesResultTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesresulttypedef).

<a id="list_conflicting_aliases"></a>

### list_conflicting_aliases

Gets a list of aliases (also called CNAMEs or alternate domain names) that
conflict or overlap with the provided alias, and the associated CloudFront
distributions and Amazon Web Services accounts for each conflicting alias.

Type annotations for
`session.create_client("cloudfront").list_conflicting_aliases` method.

Boto3 documentation:
[CloudFront.Client.list_conflicting_aliases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_conflicting_aliases)

Asynchronous method. Use `await list_conflicting_aliases(...)` for a
synchronous call.

Arguments mapping described in
[ListConflictingAliasesRequestRequestTypeDef](./type_defs.md#listconflictingaliasesrequestrequesttypedef).

Keyword-only arguments:

- `DistributionId`: `str` *(required)*
- `Alias`: `str` *(required)*
- `Marker`: `str`
- `MaxItems`: `int`

Returns a `Coroutine` for
[ListConflictingAliasesResultTypeDef](./type_defs.md#listconflictingaliasesresulttypedef).

<a id="list_distributions"></a>

### list_distributions

List CloudFront distributions.

Type annotations for `session.create_client("cloudfront").list_distributions`
method.

Boto3 documentation:
[CloudFront.Client.list_distributions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions)

Asynchronous method. Use `await list_distributions(...)` for a synchronous
call.

Arguments mapping described in
[ListDistributionsRequestRequestTypeDef](./type_defs.md#listdistributionsrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListDistributionsResultTypeDef](./type_defs.md#listdistributionsresulttypedef).

<a id="list_distributions_by_cache_policy_id"></a>

### list_distributions_by_cache_policy_id

Gets a list of distribution IDs for distributions that have a cache behavior
that’s associated with the specified cache policy.

Type annotations for
`session.create_client("cloudfront").list_distributions_by_cache_policy_id`
method.

Boto3 documentation:
[CloudFront.Client.list_distributions_by_cache_policy_id](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_cache_policy_id)

Asynchronous method. Use `await list_distributions_by_cache_policy_id(...)` for
a synchronous call.

Arguments mapping described in
[ListDistributionsByCachePolicyIdRequestRequestTypeDef](./type_defs.md#listdistributionsbycachepolicyidrequestrequesttypedef).

Keyword-only arguments:

- `CachePolicyId`: `str` *(required)*
- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListDistributionsByCachePolicyIdResultTypeDef](./type_defs.md#listdistributionsbycachepolicyidresulttypedef).

<a id="list_distributions_by_key_group"></a>

### list_distributions_by_key_group

Gets a list of distribution IDs for distributions that have a cache behavior
that references the specified key group.

Type annotations for
`session.create_client("cloudfront").list_distributions_by_key_group` method.

Boto3 documentation:
[CloudFront.Client.list_distributions_by_key_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_key_group)

Asynchronous method. Use `await list_distributions_by_key_group(...)` for a
synchronous call.

Arguments mapping described in
[ListDistributionsByKeyGroupRequestRequestTypeDef](./type_defs.md#listdistributionsbykeygrouprequestrequesttypedef).

Keyword-only arguments:

- `KeyGroupId`: `str` *(required)*
- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListDistributionsByKeyGroupResultTypeDef](./type_defs.md#listdistributionsbykeygroupresulttypedef).

<a id="list_distributions_by_origin_request_policy_id"></a>

### list_distributions_by_origin_request_policy_id

Gets a list of distribution IDs for distributions that have a cache behavior
that’s associated with the specified origin request policy.

Type annotations for
`session.create_client("cloudfront").list_distributions_by_origin_request_policy_id`
method.

Boto3 documentation:
[CloudFront.Client.list_distributions_by_origin_request_policy_id](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_origin_request_policy_id)

Asynchronous method. Use
`await list_distributions_by_origin_request_policy_id(...)` for a synchronous
call.

Arguments mapping described in
[ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef](./type_defs.md#listdistributionsbyoriginrequestpolicyidrequestrequesttypedef).

Keyword-only arguments:

- `OriginRequestPolicyId`: `str` *(required)*
- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListDistributionsByOriginRequestPolicyIdResultTypeDef](./type_defs.md#listdistributionsbyoriginrequestpolicyidresulttypedef).

<a id="list_distributions_by_realtime_log_config"></a>

### list_distributions_by_realtime_log_config

Gets a list of distributions that have a cache behavior that’s associated with
the specified real-time log configuration.

Type annotations for
`session.create_client("cloudfront").list_distributions_by_realtime_log_config`
method.

Boto3 documentation:
[CloudFront.Client.list_distributions_by_realtime_log_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_realtime_log_config)

Asynchronous method. Use `await list_distributions_by_realtime_log_config(...)`
for a synchronous call.

Arguments mapping described in
[ListDistributionsByRealtimeLogConfigRequestRequestTypeDef](./type_defs.md#listdistributionsbyrealtimelogconfigrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`
- `RealtimeLogConfigName`: `str`
- `RealtimeLogConfigArn`: `str`

Returns a `Coroutine` for
[ListDistributionsByRealtimeLogConfigResultTypeDef](./type_defs.md#listdistributionsbyrealtimelogconfigresulttypedef).

<a id="list_distributions_by_response_headers_policy_id"></a>

### list_distributions_by_response_headers_policy_id

Gets a list of distribution IDs for distributions that have a cache behavior
that’s associated with the specified response headers policy.

Type annotations for
`session.create_client("cloudfront").list_distributions_by_response_headers_policy_id`
method.

Boto3 documentation:
[CloudFront.Client.list_distributions_by_response_headers_policy_id](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_response_headers_policy_id)

Asynchronous method. Use
`await list_distributions_by_response_headers_policy_id(...)` for a synchronous
call.

Arguments mapping described in
[ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef](./type_defs.md#listdistributionsbyresponseheaderspolicyidrequestrequesttypedef).

Keyword-only arguments:

- `ResponseHeadersPolicyId`: `str` *(required)*
- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListDistributionsByResponseHeadersPolicyIdResultTypeDef](./type_defs.md#listdistributionsbyresponseheaderspolicyidresulttypedef).

<a id="list_distributions_by_web_acl_id"></a>

### list_distributions_by_web_acl_id

List the distributions that are associated with a specified WAF web ACL.

Type annotations for
`session.create_client("cloudfront").list_distributions_by_web_acl_id` method.

Boto3 documentation:
[CloudFront.Client.list_distributions_by_web_acl_id](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_web_acl_id)

Asynchronous method. Use `await list_distributions_by_web_acl_id(...)` for a
synchronous call.

Arguments mapping described in
[ListDistributionsByWebACLIdRequestRequestTypeDef](./type_defs.md#listdistributionsbywebaclidrequestrequesttypedef).

Keyword-only arguments:

- `WebACLId`: `str` *(required)*
- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListDistributionsByWebACLIdResultTypeDef](./type_defs.md#listdistributionsbywebaclidresulttypedef).

<a id="list_field_level_encryption_configs"></a>

### list_field_level_encryption_configs

List all field-level encryption configurations that have been created in
CloudFront for this account.

Type annotations for
`session.create_client("cloudfront").list_field_level_encryption_configs`
method.

Boto3 documentation:
[CloudFront.Client.list_field_level_encryption_configs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_field_level_encryption_configs)

Asynchronous method. Use `await list_field_level_encryption_configs(...)` for a
synchronous call.

Arguments mapping described in
[ListFieldLevelEncryptionConfigsRequestRequestTypeDef](./type_defs.md#listfieldlevelencryptionconfigsrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListFieldLevelEncryptionConfigsResultTypeDef](./type_defs.md#listfieldlevelencryptionconfigsresulttypedef).

<a id="list_field_level_encryption_profiles"></a>

### list_field_level_encryption_profiles

Request a list of field-level encryption profiles that have been created in
CloudFront for this account.

Type annotations for
`session.create_client("cloudfront").list_field_level_encryption_profiles`
method.

Boto3 documentation:
[CloudFront.Client.list_field_level_encryption_profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_field_level_encryption_profiles)

Asynchronous method. Use `await list_field_level_encryption_profiles(...)` for
a synchronous call.

Arguments mapping described in
[ListFieldLevelEncryptionProfilesRequestRequestTypeDef](./type_defs.md#listfieldlevelencryptionprofilesrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListFieldLevelEncryptionProfilesResultTypeDef](./type_defs.md#listfieldlevelencryptionprofilesresulttypedef).

<a id="list_functions"></a>

### list_functions

Gets a list of all CloudFront functions in your Amazon Web Services account.

Type annotations for `session.create_client("cloudfront").list_functions`
method.

Boto3 documentation:
[CloudFront.Client.list_functions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_functions)

Asynchronous method. Use `await list_functions(...)` for a synchronous call.

Arguments mapping described in
[ListFunctionsRequestRequestTypeDef](./type_defs.md#listfunctionsrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`
- `Stage`: [FunctionStageType](./literals.md#functionstagetype)

Returns a `Coroutine` for
[ListFunctionsResultTypeDef](./type_defs.md#listfunctionsresulttypedef).

<a id="list_invalidations"></a>

### list_invalidations

Lists invalidation batches.

Type annotations for `session.create_client("cloudfront").list_invalidations`
method.

Boto3 documentation:
[CloudFront.Client.list_invalidations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_invalidations)

Asynchronous method. Use `await list_invalidations(...)` for a synchronous
call.

Arguments mapping described in
[ListInvalidationsRequestRequestTypeDef](./type_defs.md#listinvalidationsrequestrequesttypedef).

Keyword-only arguments:

- `DistributionId`: `str` *(required)*
- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListInvalidationsResultTypeDef](./type_defs.md#listinvalidationsresulttypedef).

<a id="list_key_groups"></a>

### list_key_groups

Gets a list of key groups.

Type annotations for `session.create_client("cloudfront").list_key_groups`
method.

Boto3 documentation:
[CloudFront.Client.list_key_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_key_groups)

Asynchronous method. Use `await list_key_groups(...)` for a synchronous call.

Arguments mapping described in
[ListKeyGroupsRequestRequestTypeDef](./type_defs.md#listkeygroupsrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListKeyGroupsResultTypeDef](./type_defs.md#listkeygroupsresulttypedef).

<a id="list_origin_request_policies"></a>

### list_origin_request_policies

Gets a list of origin request policies.

Type annotations for
`session.create_client("cloudfront").list_origin_request_policies` method.

Boto3 documentation:
[CloudFront.Client.list_origin_request_policies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_origin_request_policies)

Asynchronous method. Use `await list_origin_request_policies(...)` for a
synchronous call.

Arguments mapping described in
[ListOriginRequestPoliciesRequestRequestTypeDef](./type_defs.md#listoriginrequestpoliciesrequestrequesttypedef).

Keyword-only arguments:

- `Type`:
  [OriginRequestPolicyTypeType](./literals.md#originrequestpolicytypetype)
- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListOriginRequestPoliciesResultTypeDef](./type_defs.md#listoriginrequestpoliciesresulttypedef).

<a id="list_public_keys"></a>

### list_public_keys

List all public keys that have been added to CloudFront for this account.

Type annotations for `session.create_client("cloudfront").list_public_keys`
method.

Boto3 documentation:
[CloudFront.Client.list_public_keys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_public_keys)

Asynchronous method. Use `await list_public_keys(...)` for a synchronous call.

Arguments mapping described in
[ListPublicKeysRequestRequestTypeDef](./type_defs.md#listpublickeysrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListPublicKeysResultTypeDef](./type_defs.md#listpublickeysresulttypedef).

<a id="list_realtime_log_configs"></a>

### list_realtime_log_configs

Gets a list of real-time log configurations.

Type annotations for
`session.create_client("cloudfront").list_realtime_log_configs` method.

Boto3 documentation:
[CloudFront.Client.list_realtime_log_configs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_realtime_log_configs)

Asynchronous method. Use `await list_realtime_log_configs(...)` for a
synchronous call.

Arguments mapping described in
[ListRealtimeLogConfigsRequestRequestTypeDef](./type_defs.md#listrealtimelogconfigsrequestrequesttypedef).

Keyword-only arguments:

- `MaxItems`: `str`
- `Marker`: `str`

Returns a `Coroutine` for
[ListRealtimeLogConfigsResultTypeDef](./type_defs.md#listrealtimelogconfigsresulttypedef).

<a id="list_response_headers_policies"></a>

### list_response_headers_policies

Gets a list of response headers policies.

Type annotations for
`session.create_client("cloudfront").list_response_headers_policies` method.

Boto3 documentation:
[CloudFront.Client.list_response_headers_policies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_response_headers_policies)

Asynchronous method. Use `await list_response_headers_policies(...)` for a
synchronous call.

Arguments mapping described in
[ListResponseHeadersPoliciesRequestRequestTypeDef](./type_defs.md#listresponseheaderspoliciesrequestrequesttypedef).

Keyword-only arguments:

- `Type`:
  [ResponseHeadersPolicyTypeType](./literals.md#responseheaderspolicytypetype)
- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListResponseHeadersPoliciesResultTypeDef](./type_defs.md#listresponseheaderspoliciesresulttypedef).

<a id="list_streaming_distributions"></a>

### list_streaming_distributions

List streaming distributions.

Type annotations for
`session.create_client("cloudfront").list_streaming_distributions` method.

Boto3 documentation:
[CloudFront.Client.list_streaming_distributions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_streaming_distributions)

Asynchronous method. Use `await list_streaming_distributions(...)` for a
synchronous call.

Arguments mapping described in
[ListStreamingDistributionsRequestRequestTypeDef](./type_defs.md#liststreamingdistributionsrequestrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`
- `MaxItems`: `str`

Returns a `Coroutine` for
[ListStreamingDistributionsResultTypeDef](./type_defs.md#liststreamingdistributionsresulttypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

List tags for a CloudFront resource.

Type annotations for
`session.create_client("cloudfront").list_tags_for_resource` method.

Boto3 documentation:
[CloudFront.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `Resource`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef).

<a id="publish_function"></a>

### publish_function

Publishes a CloudFront function by copying the function code from the
`DEVELOPMENT` stage to `LIVE`.

Type annotations for `session.create_client("cloudfront").publish_function`
method.

Boto3 documentation:
[CloudFront.Client.publish_function](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)

Asynchronous method. Use `await publish_function(...)` for a synchronous call.

Arguments mapping described in
[PublishFunctionRequestRequestTypeDef](./type_defs.md#publishfunctionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `IfMatch`: `str` *(required)*

Returns a `Coroutine` for
[PublishFunctionResultTypeDef](./type_defs.md#publishfunctionresulttypedef).

<a id="tag_resource"></a>

### tag_resource

Add tags to a CloudFront resource.

Type annotations for `session.create_client("cloudfront").tag_resource` method.

Boto3 documentation:
[CloudFront.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `Resource`: `str` *(required)*
- `Tags`: [TagsTypeDef](./type_defs.md#tagstypedef) *(required)*

<a id="test_function"></a>

### test_function

Tests a CloudFront function.

Type annotations for `session.create_client("cloudfront").test_function`
method.

Boto3 documentation:
[CloudFront.Client.test_function](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.test_function)

Asynchronous method. Use `await test_function(...)` for a synchronous call.

Arguments mapping described in
[TestFunctionRequestRequestTypeDef](./type_defs.md#testfunctionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `IfMatch`: `str` *(required)*
- `EventObject`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*
- `Stage`: [FunctionStageType](./literals.md#functionstagetype)

Returns a `Coroutine` for
[TestFunctionResultTypeDef](./type_defs.md#testfunctionresulttypedef).

<a id="untag_resource"></a>

### untag_resource

Remove tags from a CloudFront resource.

Type annotations for `session.create_client("cloudfront").untag_resource`
method.

Boto3 documentation:
[CloudFront.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `Resource`: `str` *(required)*
- `TagKeys`: [TagKeysTypeDef](./type_defs.md#tagkeystypedef) *(required)*

<a id="update_cache_policy"></a>

### update_cache_policy

Updates a cache policy configuration.

Type annotations for `session.create_client("cloudfront").update_cache_policy`
method.

Boto3 documentation:
[CloudFront.Client.update_cache_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)

Asynchronous method. Use `await update_cache_policy(...)` for a synchronous
call.

Arguments mapping described in
[UpdateCachePolicyRequestRequestTypeDef](./type_defs.md#updatecachepolicyrequestrequesttypedef).

Keyword-only arguments:

- `CachePolicyConfig`:
  [CachePolicyConfigTypeDef](./type_defs.md#cachepolicyconfigtypedef)
  *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdateCachePolicyResultTypeDef](./type_defs.md#updatecachepolicyresulttypedef).

<a id="update_cloud_front_origin_access_identity"></a>

### update_cloud_front_origin_access_identity

Update an origin access identity.

Type annotations for
`session.create_client("cloudfront").update_cloud_front_origin_access_identity`
method.

Boto3 documentation:
[CloudFront.Client.update_cloud_front_origin_access_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)

Asynchronous method. Use `await update_cloud_front_origin_access_identity(...)`
for a synchronous call.

Arguments mapping described in
[UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef](./type_defs.md#updatecloudfrontoriginaccessidentityrequestrequesttypedef).

Keyword-only arguments:

- `CloudFrontOriginAccessIdentityConfig`:
  [CloudFrontOriginAccessIdentityConfigTypeDef](./type_defs.md#cloudfrontoriginaccessidentityconfigtypedef)
  *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdateCloudFrontOriginAccessIdentityResultTypeDef](./type_defs.md#updatecloudfrontoriginaccessidentityresulttypedef).

<a id="update_distribution"></a>

### update_distribution

Updates the configuration for a web distribution.

Type annotations for `session.create_client("cloudfront").update_distribution`
method.

Boto3 documentation:
[CloudFront.Client.update_distribution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)

Asynchronous method. Use `await update_distribution(...)` for a synchronous
call.

Arguments mapping described in
[UpdateDistributionRequestRequestTypeDef](./type_defs.md#updatedistributionrequestrequesttypedef).

Keyword-only arguments:

- `DistributionConfig`:
  [DistributionConfigTypeDef](./type_defs.md#distributionconfigtypedef)
  *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdateDistributionResultTypeDef](./type_defs.md#updatedistributionresulttypedef).

<a id="update_field_level_encryption_config"></a>

### update_field_level_encryption_config

Update a field-level encryption configuration.

Type annotations for
`session.create_client("cloudfront").update_field_level_encryption_config`
method.

Boto3 documentation:
[CloudFront.Client.update_field_level_encryption_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)

Asynchronous method. Use `await update_field_level_encryption_config(...)` for
a synchronous call.

Arguments mapping described in
[UpdateFieldLevelEncryptionConfigRequestRequestTypeDef](./type_defs.md#updatefieldlevelencryptionconfigrequestrequesttypedef).

Keyword-only arguments:

- `FieldLevelEncryptionConfig`:
  [FieldLevelEncryptionConfigTypeDef](./type_defs.md#fieldlevelencryptionconfigtypedef)
  *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdateFieldLevelEncryptionConfigResultTypeDef](./type_defs.md#updatefieldlevelencryptionconfigresulttypedef).

<a id="update_field_level_encryption_profile"></a>

### update_field_level_encryption_profile

Update a field-level encryption profile.

Type annotations for
`session.create_client("cloudfront").update_field_level_encryption_profile`
method.

Boto3 documentation:
[CloudFront.Client.update_field_level_encryption_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)

Asynchronous method. Use `await update_field_level_encryption_profile(...)` for
a synchronous call.

Arguments mapping described in
[UpdateFieldLevelEncryptionProfileRequestRequestTypeDef](./type_defs.md#updatefieldlevelencryptionprofilerequestrequesttypedef).

Keyword-only arguments:

- `FieldLevelEncryptionProfileConfig`:
  [FieldLevelEncryptionProfileConfigTypeDef](./type_defs.md#fieldlevelencryptionprofileconfigtypedef)
  *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdateFieldLevelEncryptionProfileResultTypeDef](./type_defs.md#updatefieldlevelencryptionprofileresulttypedef).

<a id="update_function"></a>

### update_function

Updates a CloudFront function.

Type annotations for `session.create_client("cloudfront").update_function`
method.

Boto3 documentation:
[CloudFront.Client.update_function](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)

Asynchronous method. Use `await update_function(...)` for a synchronous call.

Arguments mapping described in
[UpdateFunctionRequestRequestTypeDef](./type_defs.md#updatefunctionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `IfMatch`: `str` *(required)*
- `FunctionConfig`:
  [FunctionConfigTypeDef](./type_defs.md#functionconfigtypedef) *(required)*
- `FunctionCode`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*

Returns a `Coroutine` for
[UpdateFunctionResultTypeDef](./type_defs.md#updatefunctionresulttypedef).

<a id="update_key_group"></a>

### update_key_group

Updates a key group.

Type annotations for `session.create_client("cloudfront").update_key_group`
method.

Boto3 documentation:
[CloudFront.Client.update_key_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)

Asynchronous method. Use `await update_key_group(...)` for a synchronous call.

Arguments mapping described in
[UpdateKeyGroupRequestRequestTypeDef](./type_defs.md#updatekeygrouprequestrequesttypedef).

Keyword-only arguments:

- `KeyGroupConfig`:
  [KeyGroupConfigTypeDef](./type_defs.md#keygroupconfigtypedef) *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdateKeyGroupResultTypeDef](./type_defs.md#updatekeygroupresulttypedef).

<a id="update_origin_request_policy"></a>

### update_origin_request_policy

Updates an origin request policy configuration.

Type annotations for
`session.create_client("cloudfront").update_origin_request_policy` method.

Boto3 documentation:
[CloudFront.Client.update_origin_request_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)

Asynchronous method. Use `await update_origin_request_policy(...)` for a
synchronous call.

Arguments mapping described in
[UpdateOriginRequestPolicyRequestRequestTypeDef](./type_defs.md#updateoriginrequestpolicyrequestrequesttypedef).

Keyword-only arguments:

- `OriginRequestPolicyConfig`:
  [OriginRequestPolicyConfigTypeDef](./type_defs.md#originrequestpolicyconfigtypedef)
  *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdateOriginRequestPolicyResultTypeDef](./type_defs.md#updateoriginrequestpolicyresulttypedef).

<a id="update_public_key"></a>

### update_public_key

Update public key information.

Type annotations for `session.create_client("cloudfront").update_public_key`
method.

Boto3 documentation:
[CloudFront.Client.update_public_key](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_public_key)

Asynchronous method. Use `await update_public_key(...)` for a synchronous call.

Arguments mapping described in
[UpdatePublicKeyRequestRequestTypeDef](./type_defs.md#updatepublickeyrequestrequesttypedef).

Keyword-only arguments:

- `PublicKeyConfig`:
  [PublicKeyConfigTypeDef](./type_defs.md#publickeyconfigtypedef) *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdatePublicKeyResultTypeDef](./type_defs.md#updatepublickeyresulttypedef).

<a id="update_realtime_log_config"></a>

### update_realtime_log_config

Updates a real-time log configuration.

Type annotations for
`session.create_client("cloudfront").update_realtime_log_config` method.

Boto3 documentation:
[CloudFront.Client.update_realtime_log_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)

Asynchronous method. Use `await update_realtime_log_config(...)` for a
synchronous call.

Arguments mapping described in
[UpdateRealtimeLogConfigRequestRequestTypeDef](./type_defs.md#updaterealtimelogconfigrequestrequesttypedef).

Keyword-only arguments:

- `EndPoints`: `Sequence`\[[EndPointTypeDef](./type_defs.md#endpointtypedef)\]
- `Fields`: `Sequence`\[`str`\]
- `Name`: `str`
- `ARN`: `str`
- `SamplingRate`: `int`

Returns a `Coroutine` for
[UpdateRealtimeLogConfigResultTypeDef](./type_defs.md#updaterealtimelogconfigresulttypedef).

<a id="update_response_headers_policy"></a>

### update_response_headers_policy

Updates a response headers policy.

Type annotations for
`session.create_client("cloudfront").update_response_headers_policy` method.

Boto3 documentation:
[CloudFront.Client.update_response_headers_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)

Asynchronous method. Use `await update_response_headers_policy(...)` for a
synchronous call.

Arguments mapping described in
[UpdateResponseHeadersPolicyRequestRequestTypeDef](./type_defs.md#updateresponseheaderspolicyrequestrequesttypedef).

Keyword-only arguments:

- `ResponseHeadersPolicyConfig`:
  [ResponseHeadersPolicyConfigTypeDef](./type_defs.md#responseheaderspolicyconfigtypedef)
  *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdateResponseHeadersPolicyResultTypeDef](./type_defs.md#updateresponseheaderspolicyresulttypedef).

<a id="update_streaming_distribution"></a>

### update_streaming_distribution

Update a streaming distribution.

Type annotations for
`session.create_client("cloudfront").update_streaming_distribution` method.

Boto3 documentation:
[CloudFront.Client.update_streaming_distribution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)

Asynchronous method. Use `await update_streaming_distribution(...)` for a
synchronous call.

Arguments mapping described in
[UpdateStreamingDistributionRequestRequestTypeDef](./type_defs.md#updatestreamingdistributionrequestrequesttypedef).

Keyword-only arguments:

- `StreamingDistributionConfig`:
  [StreamingDistributionConfigTypeDef](./type_defs.md#streamingdistributionconfigtypedef)
  *(required)*
- `Id`: `str` *(required)*
- `IfMatch`: `str`

Returns a `Coroutine` for
[UpdateStreamingDistributionResultTypeDef](./type_defs.md#updatestreamingdistributionresulttypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("cloudfront").__aenter__` method.

Boto3 documentation:
[CloudFront.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [CloudFrontClient](#cloudfrontclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("cloudfront").__aexit__` method.

Boto3 documentation:
[CloudFront.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("cloudfront").get_paginator` method
with overloads.

- `client.get_paginator("list_cloud_front_origin_access_identities")` ->
  [ListCloudFrontOriginAccessIdentitiesPaginator](./paginators.md#listcloudfrontoriginaccessidentitiespaginator)
- `client.get_paginator("list_distributions")` ->
  [ListDistributionsPaginator](./paginators.md#listdistributionspaginator)
- `client.get_paginator("list_invalidations")` ->
  [ListInvalidationsPaginator](./paginators.md#listinvalidationspaginator)
- `client.get_paginator("list_streaming_distributions")` ->
  [ListStreamingDistributionsPaginator](./paginators.md#liststreamingdistributionspaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("cloudfront").get_waiter` method
with overloads.

- `client.get_waiter("distribution_deployed")` ->
  [DistributionDeployedWaiter](./waiters.md#distributiondeployedwaiter)
- `client.get_waiter("invalidation_completed")` ->
  [InvalidationCompletedWaiter](./waiters.md#invalidationcompletedwaiter)
- `client.get_waiter("streaming_distribution_deployed")` ->
  [StreamingDistributionDeployedWaiter](./waiters.md#streamingdistributiondeployedwaiter)
