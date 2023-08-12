# Type definitions

> [Index](../README.md) > [CloudFront](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
    type annotations stubs module [types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## AliasICPRecordalTypeDef

```python
# AliasICPRecordalTypeDef definition

class AliasICPRecordalTypeDef(TypedDict):
    CNAME: NotRequired[str],
    ICPRecordalStatus: NotRequired[ICPRecordalStatusType],  # (1)
```

1. See [:material-code-brackets: ICPRecordalStatusType](./literals.md#icprecordalstatustype) 
## AliasesTypeDef

```python
# AliasesTypeDef definition

class AliasesTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[str]],
```

## CachedMethodsTypeDef

```python
# CachedMethodsTypeDef definition

class CachedMethodsTypeDef(TypedDict):
    Quantity: int,
    Items: List[MethodType],  # (1)
```

1. See [:material-code-brackets: MethodType](./literals.md#methodtype) 
## AssociateAliasRequestRequestTypeDef

```python
# AssociateAliasRequestRequestTypeDef definition

class AssociateAliasRequestRequestTypeDef(TypedDict):
    TargetDistributionId: str,
    Alias: str,
```

## TrustedKeyGroupsTypeDef

```python
# TrustedKeyGroupsTypeDef definition

class TrustedKeyGroupsTypeDef(TypedDict):
    Enabled: bool,
    Quantity: int,
    Items: NotRequired[List[str]],
```

## TrustedSignersTypeDef

```python
# TrustedSignersTypeDef definition

class TrustedSignersTypeDef(TypedDict):
    Enabled: bool,
    Quantity: int,
    Items: NotRequired[List[str]],
```

## CookieNamesTypeDef

```python
# CookieNamesTypeDef definition

class CookieNamesTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[str]],
```

## HeadersTypeDef

```python
# HeadersTypeDef definition

class HeadersTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[str]],
```

## QueryStringNamesTypeDef

```python
# QueryStringNamesTypeDef definition

class QueryStringNamesTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[str]],
```

## CloudFrontOriginAccessIdentityConfigTypeDef

```python
# CloudFrontOriginAccessIdentityConfigTypeDef definition

class CloudFrontOriginAccessIdentityConfigTypeDef(TypedDict):
    CallerReference: str,
    Comment: str,
```

## CloudFrontOriginAccessIdentitySummaryTypeDef

```python
# CloudFrontOriginAccessIdentitySummaryTypeDef definition

class CloudFrontOriginAccessIdentitySummaryTypeDef(TypedDict):
    Id: str,
    S3CanonicalUserId: str,
    Comment: str,
```

## ConflictingAliasTypeDef

```python
# ConflictingAliasTypeDef definition

class ConflictingAliasTypeDef(TypedDict):
    Alias: NotRequired[str],
    DistributionId: NotRequired[str],
    AccountId: NotRequired[str],
```

## ContentTypeProfileTypeDef

```python
# ContentTypeProfileTypeDef definition

class ContentTypeProfileTypeDef(TypedDict):
    Format: FormatType,  # (1)
    ContentType: str,
    ProfileId: NotRequired[str],
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## StagingDistributionDnsNamesTypeDef

```python
# StagingDistributionDnsNamesTypeDef definition

class StagingDistributionDnsNamesTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[str]],
```

## ContinuousDeploymentSingleHeaderConfigTypeDef

```python
# ContinuousDeploymentSingleHeaderConfigTypeDef definition

class ContinuousDeploymentSingleHeaderConfigTypeDef(TypedDict):
    Header: str,
    Value: str,
```

## SessionStickinessConfigTypeDef

```python
# SessionStickinessConfigTypeDef definition

class SessionStickinessConfigTypeDef(TypedDict):
    IdleTTL: int,
    MaximumTTL: int,
```

## CopyDistributionRequestRequestTypeDef

```python
# CopyDistributionRequestRequestTypeDef definition

class CopyDistributionRequestRequestTypeDef(TypedDict):
    PrimaryDistributionId: str,
    CallerReference: str,
    Staging: NotRequired[bool],
    IfMatch: NotRequired[str],
    Enabled: NotRequired[bool],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## FunctionConfigTypeDef

```python
# FunctionConfigTypeDef definition

class FunctionConfigTypeDef(TypedDict):
    Comment: str,
    Runtime: FunctionRuntimeType,  # (1)
```

1. See [:material-code-brackets: FunctionRuntimeType](./literals.md#functionruntimetype) 
## KeyGroupConfigTypeDef

```python
# KeyGroupConfigTypeDef definition

class KeyGroupConfigTypeDef(TypedDict):
    Name: str,
    Items: Sequence[str],
    Comment: NotRequired[str],
```

## OriginAccessControlConfigTypeDef

```python
# OriginAccessControlConfigTypeDef definition

class OriginAccessControlConfigTypeDef(TypedDict):
    Name: str,
    SigningProtocol: OriginAccessControlSigningProtocolsType,  # (1)
    SigningBehavior: OriginAccessControlSigningBehaviorsType,  # (2)
    OriginAccessControlOriginType: OriginAccessControlOriginTypesType,  # (3)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: OriginAccessControlSigningProtocolsType](./literals.md#originaccesscontrolsigningprotocolstype) 
2. See [:material-code-brackets: OriginAccessControlSigningBehaviorsType](./literals.md#originaccesscontrolsigningbehaviorstype) 
3. See [:material-code-brackets: OriginAccessControlOriginTypesType](./literals.md#originaccesscontrolorigintypestype) 
## PublicKeyConfigTypeDef

```python
# PublicKeyConfigTypeDef definition

class PublicKeyConfigTypeDef(TypedDict):
    CallerReference: str,
    Name: str,
    EncodedKey: str,
    Comment: NotRequired[str],
```

## CustomErrorResponseTypeDef

```python
# CustomErrorResponseTypeDef definition

class CustomErrorResponseTypeDef(TypedDict):
    ErrorCode: int,
    ResponsePagePath: NotRequired[str],
    ResponseCode: NotRequired[str],
    ErrorCachingMinTTL: NotRequired[int],
```

## OriginCustomHeaderTypeDef

```python
# OriginCustomHeaderTypeDef definition

class OriginCustomHeaderTypeDef(TypedDict):
    HeaderName: str,
    HeaderValue: str,
```

## OriginSslProtocolsTypeDef

```python
# OriginSslProtocolsTypeDef definition

class OriginSslProtocolsTypeDef(TypedDict):
    Quantity: int,
    Items: List[SslProtocolType],  # (1)
```

1. See [:material-code-brackets: SslProtocolType](./literals.md#sslprotocoltype) 
## DeleteCachePolicyRequestRequestTypeDef

```python
# DeleteCachePolicyRequestRequestTypeDef definition

class DeleteCachePolicyRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef

```python
# DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef definition

class DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteContinuousDeploymentPolicyRequestRequestTypeDef

```python
# DeleteContinuousDeploymentPolicyRequestRequestTypeDef definition

class DeleteContinuousDeploymentPolicyRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteDistributionRequestRequestTypeDef

```python
# DeleteDistributionRequestRequestTypeDef definition

class DeleteDistributionRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteFieldLevelEncryptionConfigRequestRequestTypeDef

```python
# DeleteFieldLevelEncryptionConfigRequestRequestTypeDef definition

class DeleteFieldLevelEncryptionConfigRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteFieldLevelEncryptionProfileRequestRequestTypeDef

```python
# DeleteFieldLevelEncryptionProfileRequestRequestTypeDef definition

class DeleteFieldLevelEncryptionProfileRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteFunctionRequestRequestTypeDef

```python
# DeleteFunctionRequestRequestTypeDef definition

class DeleteFunctionRequestRequestTypeDef(TypedDict):
    Name: str,
    IfMatch: str,
```

## DeleteKeyGroupRequestRequestTypeDef

```python
# DeleteKeyGroupRequestRequestTypeDef definition

class DeleteKeyGroupRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteMonitoringSubscriptionRequestRequestTypeDef

```python
# DeleteMonitoringSubscriptionRequestRequestTypeDef definition

class DeleteMonitoringSubscriptionRequestRequestTypeDef(TypedDict):
    DistributionId: str,
```

## DeleteOriginAccessControlRequestRequestTypeDef

```python
# DeleteOriginAccessControlRequestRequestTypeDef definition

class DeleteOriginAccessControlRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteOriginRequestPolicyRequestRequestTypeDef

```python
# DeleteOriginRequestPolicyRequestRequestTypeDef definition

class DeleteOriginRequestPolicyRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeletePublicKeyRequestRequestTypeDef

```python
# DeletePublicKeyRequestRequestTypeDef definition

class DeletePublicKeyRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteRealtimeLogConfigRequestRequestTypeDef

```python
# DeleteRealtimeLogConfigRequestRequestTypeDef definition

class DeleteRealtimeLogConfigRequestRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    ARN: NotRequired[str],
```

## DeleteResponseHeadersPolicyRequestRequestTypeDef

```python
# DeleteResponseHeadersPolicyRequestRequestTypeDef definition

class DeleteResponseHeadersPolicyRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DeleteStreamingDistributionRequestRequestTypeDef

```python
# DeleteStreamingDistributionRequestRequestTypeDef definition

class DeleteStreamingDistributionRequestRequestTypeDef(TypedDict):
    Id: str,
    IfMatch: NotRequired[str],
```

## DescribeFunctionRequestRequestTypeDef

```python
# DescribeFunctionRequestRequestTypeDef definition

class DescribeFunctionRequestRequestTypeDef(TypedDict):
    Name: str,
    Stage: NotRequired[FunctionStageType],  # (1)
```

1. See [:material-code-brackets: FunctionStageType](./literals.md#functionstagetype) 
## LoggingConfigTypeDef

```python
# LoggingConfigTypeDef definition

class LoggingConfigTypeDef(TypedDict):
    Enabled: bool,
    IncludeCookies: bool,
    Bucket: str,
    Prefix: str,
```

## ViewerCertificateTypeDef

```python
# ViewerCertificateTypeDef definition

class ViewerCertificateTypeDef(TypedDict):
    CloudFrontDefaultCertificate: NotRequired[bool],
    IAMCertificateId: NotRequired[str],
    ACMCertificateArn: NotRequired[str],
    SSLSupportMethod: NotRequired[SSLSupportMethodType],  # (1)
    MinimumProtocolVersion: NotRequired[MinimumProtocolVersionType],  # (2)
    Certificate: NotRequired[str],
    CertificateSource: NotRequired[CertificateSourceType],  # (3)
```

1. See [:material-code-brackets: SSLSupportMethodType](./literals.md#sslsupportmethodtype) 
2. See [:material-code-brackets: MinimumProtocolVersionType](./literals.md#minimumprotocolversiontype) 
3. See [:material-code-brackets: CertificateSourceType](./literals.md#certificatesourcetype) 
## DistributionIdListTypeDef

```python
# DistributionIdListTypeDef definition

class DistributionIdListTypeDef(TypedDict):
    Marker: str,
    MaxItems: int,
    IsTruncated: bool,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[str]],
```

## FieldPatternsTypeDef

```python
# FieldPatternsTypeDef definition

class FieldPatternsTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[str]],
```

## KinesisStreamConfigTypeDef

```python
# KinesisStreamConfigTypeDef definition

class KinesisStreamConfigTypeDef(TypedDict):
    RoleARN: str,
    StreamARN: str,
```

## QueryStringCacheKeysTypeDef

```python
# QueryStringCacheKeysTypeDef definition

class QueryStringCacheKeysTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[str]],
```

## FunctionAssociationTypeDef

```python
# FunctionAssociationTypeDef definition

class FunctionAssociationTypeDef(TypedDict):
    FunctionARN: str,
    EventType: EventTypeType,  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## FunctionMetadataTypeDef

```python
# FunctionMetadataTypeDef definition

class FunctionMetadataTypeDef(TypedDict):
    FunctionARN: str,
    LastModifiedTime: datetime,
    Stage: NotRequired[FunctionStageType],  # (1)
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: FunctionStageType](./literals.md#functionstagetype) 
## GeoRestrictionTypeDef

```python
# GeoRestrictionTypeDef definition

class GeoRestrictionTypeDef(TypedDict):
    RestrictionType: GeoRestrictionTypeType,  # (1)
    Quantity: int,
    Items: NotRequired[List[str]],
```

1. See [:material-code-brackets: GeoRestrictionTypeType](./literals.md#georestrictiontypetype) 
## GetCachePolicyConfigRequestRequestTypeDef

```python
# GetCachePolicyConfigRequestRequestTypeDef definition

class GetCachePolicyConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetCachePolicyRequestRequestTypeDef

```python
# GetCachePolicyRequestRequestTypeDef definition

class GetCachePolicyRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef

```python
# GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef definition

class GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetCloudFrontOriginAccessIdentityRequestRequestTypeDef

```python
# GetCloudFrontOriginAccessIdentityRequestRequestTypeDef definition

class GetCloudFrontOriginAccessIdentityRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetContinuousDeploymentPolicyConfigRequestRequestTypeDef

```python
# GetContinuousDeploymentPolicyConfigRequestRequestTypeDef definition

class GetContinuousDeploymentPolicyConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetContinuousDeploymentPolicyRequestRequestTypeDef

```python
# GetContinuousDeploymentPolicyRequestRequestTypeDef definition

class GetContinuousDeploymentPolicyRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetDistributionConfigRequestRequestTypeDef

```python
# GetDistributionConfigRequestRequestTypeDef definition

class GetDistributionConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetDistributionRequestRequestTypeDef

```python
# GetDistributionRequestRequestTypeDef definition

class GetDistributionRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetFieldLevelEncryptionConfigRequestRequestTypeDef

```python
# GetFieldLevelEncryptionConfigRequestRequestTypeDef definition

class GetFieldLevelEncryptionConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef

```python
# GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef definition

class GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetFieldLevelEncryptionProfileRequestRequestTypeDef

```python
# GetFieldLevelEncryptionProfileRequestRequestTypeDef definition

class GetFieldLevelEncryptionProfileRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetFieldLevelEncryptionRequestRequestTypeDef

```python
# GetFieldLevelEncryptionRequestRequestTypeDef definition

class GetFieldLevelEncryptionRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetFunctionRequestRequestTypeDef

```python
# GetFunctionRequestRequestTypeDef definition

class GetFunctionRequestRequestTypeDef(TypedDict):
    Name: str,
    Stage: NotRequired[FunctionStageType],  # (1)
```

1. See [:material-code-brackets: FunctionStageType](./literals.md#functionstagetype) 
## GetInvalidationRequestRequestTypeDef

```python
# GetInvalidationRequestRequestTypeDef definition

class GetInvalidationRequestRequestTypeDef(TypedDict):
    DistributionId: str,
    Id: str,
```

## GetKeyGroupConfigRequestRequestTypeDef

```python
# GetKeyGroupConfigRequestRequestTypeDef definition

class GetKeyGroupConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetKeyGroupRequestRequestTypeDef

```python
# GetKeyGroupRequestRequestTypeDef definition

class GetKeyGroupRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetMonitoringSubscriptionRequestRequestTypeDef

```python
# GetMonitoringSubscriptionRequestRequestTypeDef definition

class GetMonitoringSubscriptionRequestRequestTypeDef(TypedDict):
    DistributionId: str,
```

## GetOriginAccessControlConfigRequestRequestTypeDef

```python
# GetOriginAccessControlConfigRequestRequestTypeDef definition

class GetOriginAccessControlConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetOriginAccessControlRequestRequestTypeDef

```python
# GetOriginAccessControlRequestRequestTypeDef definition

class GetOriginAccessControlRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetOriginRequestPolicyConfigRequestRequestTypeDef

```python
# GetOriginRequestPolicyConfigRequestRequestTypeDef definition

class GetOriginRequestPolicyConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetOriginRequestPolicyRequestRequestTypeDef

```python
# GetOriginRequestPolicyRequestRequestTypeDef definition

class GetOriginRequestPolicyRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetPublicKeyConfigRequestRequestTypeDef

```python
# GetPublicKeyConfigRequestRequestTypeDef definition

class GetPublicKeyConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetPublicKeyRequestRequestTypeDef

```python
# GetPublicKeyRequestRequestTypeDef definition

class GetPublicKeyRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetRealtimeLogConfigRequestRequestTypeDef

```python
# GetRealtimeLogConfigRequestRequestTypeDef definition

class GetRealtimeLogConfigRequestRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    ARN: NotRequired[str],
```

## GetResponseHeadersPolicyConfigRequestRequestTypeDef

```python
# GetResponseHeadersPolicyConfigRequestRequestTypeDef definition

class GetResponseHeadersPolicyConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetResponseHeadersPolicyRequestRequestTypeDef

```python
# GetResponseHeadersPolicyRequestRequestTypeDef definition

class GetResponseHeadersPolicyRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetStreamingDistributionConfigRequestRequestTypeDef

```python
# GetStreamingDistributionConfigRequestRequestTypeDef definition

class GetStreamingDistributionConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetStreamingDistributionRequestRequestTypeDef

```python
# GetStreamingDistributionRequestRequestTypeDef definition

class GetStreamingDistributionRequestRequestTypeDef(TypedDict):
    Id: str,
```

## PathsTypeDef

```python
# PathsTypeDef definition

class PathsTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[str]],
```

## InvalidationSummaryTypeDef

```python
# InvalidationSummaryTypeDef definition

class InvalidationSummaryTypeDef(TypedDict):
    Id: str,
    CreateTime: datetime,
    Status: str,
```

## KeyPairIdsTypeDef

```python
# KeyPairIdsTypeDef definition

class KeyPairIdsTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[str]],
```

## LambdaFunctionAssociationTypeDef

```python
# LambdaFunctionAssociationTypeDef definition

class LambdaFunctionAssociationTypeDef(TypedDict):
    LambdaFunctionARN: str,
    EventType: EventTypeType,  # (1)
    IncludeBody: NotRequired[bool],
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## ListCachePoliciesRequestRequestTypeDef

```python
# ListCachePoliciesRequestRequestTypeDef definition

class ListCachePoliciesRequestRequestTypeDef(TypedDict):
    Type: NotRequired[CachePolicyTypeType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

1. See [:material-code-brackets: CachePolicyTypeType](./literals.md#cachepolicytypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef

```python
# ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef definition

class ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListConflictingAliasesRequestRequestTypeDef

```python
# ListConflictingAliasesRequestRequestTypeDef definition

class ListConflictingAliasesRequestRequestTypeDef(TypedDict):
    DistributionId: str,
    Alias: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListContinuousDeploymentPoliciesRequestRequestTypeDef

```python
# ListContinuousDeploymentPoliciesRequestRequestTypeDef definition

class ListContinuousDeploymentPoliciesRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListDistributionsByCachePolicyIdRequestRequestTypeDef

```python
# ListDistributionsByCachePolicyIdRequestRequestTypeDef definition

class ListDistributionsByCachePolicyIdRequestRequestTypeDef(TypedDict):
    CachePolicyId: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListDistributionsByKeyGroupRequestRequestTypeDef

```python
# ListDistributionsByKeyGroupRequestRequestTypeDef definition

class ListDistributionsByKeyGroupRequestRequestTypeDef(TypedDict):
    KeyGroupId: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef

```python
# ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef definition

class ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef(TypedDict):
    OriginRequestPolicyId: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListDistributionsByRealtimeLogConfigRequestRequestTypeDef

```python
# ListDistributionsByRealtimeLogConfigRequestRequestTypeDef definition

class ListDistributionsByRealtimeLogConfigRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
    RealtimeLogConfigName: NotRequired[str],
    RealtimeLogConfigArn: NotRequired[str],
```

## ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef

```python
# ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef definition

class ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef(TypedDict):
    ResponseHeadersPolicyId: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListDistributionsByWebACLIdRequestRequestTypeDef

```python
# ListDistributionsByWebACLIdRequestRequestTypeDef definition

class ListDistributionsByWebACLIdRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListDistributionsRequestRequestTypeDef

```python
# ListDistributionsRequestRequestTypeDef definition

class ListDistributionsRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListFieldLevelEncryptionConfigsRequestRequestTypeDef

```python
# ListFieldLevelEncryptionConfigsRequestRequestTypeDef definition

class ListFieldLevelEncryptionConfigsRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListFieldLevelEncryptionProfilesRequestRequestTypeDef

```python
# ListFieldLevelEncryptionProfilesRequestRequestTypeDef definition

class ListFieldLevelEncryptionProfilesRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListFunctionsRequestRequestTypeDef

```python
# ListFunctionsRequestRequestTypeDef definition

class ListFunctionsRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
    Stage: NotRequired[FunctionStageType],  # (1)
```

1. See [:material-code-brackets: FunctionStageType](./literals.md#functionstagetype) 
## ListInvalidationsRequestRequestTypeDef

```python
# ListInvalidationsRequestRequestTypeDef definition

class ListInvalidationsRequestRequestTypeDef(TypedDict):
    DistributionId: str,
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListKeyGroupsRequestRequestTypeDef

```python
# ListKeyGroupsRequestRequestTypeDef definition

class ListKeyGroupsRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListOriginAccessControlsRequestRequestTypeDef

```python
# ListOriginAccessControlsRequestRequestTypeDef definition

class ListOriginAccessControlsRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListOriginRequestPoliciesRequestRequestTypeDef

```python
# ListOriginRequestPoliciesRequestRequestTypeDef definition

class ListOriginRequestPoliciesRequestRequestTypeDef(TypedDict):
    Type: NotRequired[OriginRequestPolicyTypeType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

1. See [:material-code-brackets: OriginRequestPolicyTypeType](./literals.md#originrequestpolicytypetype) 
## ListPublicKeysRequestRequestTypeDef

```python
# ListPublicKeysRequestRequestTypeDef definition

class ListPublicKeysRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListRealtimeLogConfigsRequestRequestTypeDef

```python
# ListRealtimeLogConfigsRequestRequestTypeDef definition

class ListRealtimeLogConfigsRequestRequestTypeDef(TypedDict):
    MaxItems: NotRequired[str],
    Marker: NotRequired[str],
```

## ListResponseHeadersPoliciesRequestRequestTypeDef

```python
# ListResponseHeadersPoliciesRequestRequestTypeDef definition

class ListResponseHeadersPoliciesRequestRequestTypeDef(TypedDict):
    Type: NotRequired[ResponseHeadersPolicyTypeType],  # (1)
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

1. See [:material-code-brackets: ResponseHeadersPolicyTypeType](./literals.md#responseheaderspolicytypetype) 
## ListStreamingDistributionsRequestRequestTypeDef

```python
# ListStreamingDistributionsRequestRequestTypeDef definition

class ListStreamingDistributionsRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    Resource: str,
```

## RealtimeMetricsSubscriptionConfigTypeDef

```python
# RealtimeMetricsSubscriptionConfigTypeDef definition

class RealtimeMetricsSubscriptionConfigTypeDef(TypedDict):
    RealtimeMetricsSubscriptionStatus: RealtimeMetricsSubscriptionStatusType,  # (1)
```

1. See [:material-code-brackets: RealtimeMetricsSubscriptionStatusType](./literals.md#realtimemetricssubscriptionstatustype) 
## OriginAccessControlSummaryTypeDef

```python
# OriginAccessControlSummaryTypeDef definition

class OriginAccessControlSummaryTypeDef(TypedDict):
    Id: str,
    Description: str,
    Name: str,
    SigningProtocol: OriginAccessControlSigningProtocolsType,  # (1)
    SigningBehavior: OriginAccessControlSigningBehaviorsType,  # (2)
    OriginAccessControlOriginType: OriginAccessControlOriginTypesType,  # (3)
```

1. See [:material-code-brackets: OriginAccessControlSigningProtocolsType](./literals.md#originaccesscontrolsigningprotocolstype) 
2. See [:material-code-brackets: OriginAccessControlSigningBehaviorsType](./literals.md#originaccesscontrolsigningbehaviorstype) 
3. See [:material-code-brackets: OriginAccessControlOriginTypesType](./literals.md#originaccesscontrolorigintypestype) 
## StatusCodesTypeDef

```python
# StatusCodesTypeDef definition

class StatusCodesTypeDef(TypedDict):
    Quantity: int,
    Items: List[int],
```

## OriginGroupMemberTypeDef

```python
# OriginGroupMemberTypeDef definition

class OriginGroupMemberTypeDef(TypedDict):
    OriginId: str,
```

## OriginShieldTypeDef

```python
# OriginShieldTypeDef definition

class OriginShieldTypeDef(TypedDict):
    Enabled: bool,
    OriginShieldRegion: NotRequired[str],
```

## S3OriginConfigTypeDef

```python
# S3OriginConfigTypeDef definition

class S3OriginConfigTypeDef(TypedDict):
    OriginAccessIdentity: str,
```

## PublicKeySummaryTypeDef

```python
# PublicKeySummaryTypeDef definition

class PublicKeySummaryTypeDef(TypedDict):
    Id: str,
    Name: str,
    CreatedTime: datetime,
    EncodedKey: str,
    Comment: NotRequired[str],
```

## PublishFunctionRequestRequestTypeDef

```python
# PublishFunctionRequestRequestTypeDef definition

class PublishFunctionRequestRequestTypeDef(TypedDict):
    Name: str,
    IfMatch: str,
```

## QueryArgProfileTypeDef

```python
# QueryArgProfileTypeDef definition

class QueryArgProfileTypeDef(TypedDict):
    QueryArg: str,
    ProfileId: str,
```

## ResponseHeadersPolicyAccessControlAllowHeadersTypeDef

```python
# ResponseHeadersPolicyAccessControlAllowHeadersTypeDef definition

class ResponseHeadersPolicyAccessControlAllowHeadersTypeDef(TypedDict):
    Quantity: int,
    Items: Sequence[str],
```

## ResponseHeadersPolicyAccessControlAllowMethodsTypeDef

```python
# ResponseHeadersPolicyAccessControlAllowMethodsTypeDef definition

class ResponseHeadersPolicyAccessControlAllowMethodsTypeDef(TypedDict):
    Quantity: int,
    Items: Sequence[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],  # (1)
```

1. See [:material-code-brackets: ResponseHeadersPolicyAccessControlAllowMethodsValuesType](./literals.md#responseheaderspolicyaccesscontrolallowmethodsvaluestype) 
## ResponseHeadersPolicyAccessControlAllowOriginsTypeDef

```python
# ResponseHeadersPolicyAccessControlAllowOriginsTypeDef definition

class ResponseHeadersPolicyAccessControlAllowOriginsTypeDef(TypedDict):
    Quantity: int,
    Items: Sequence[str],
```

## ResponseHeadersPolicyAccessControlExposeHeadersTypeDef

```python
# ResponseHeadersPolicyAccessControlExposeHeadersTypeDef definition

class ResponseHeadersPolicyAccessControlExposeHeadersTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[str]],
```

## ResponseHeadersPolicyServerTimingHeadersConfigTypeDef

```python
# ResponseHeadersPolicyServerTimingHeadersConfigTypeDef definition

class ResponseHeadersPolicyServerTimingHeadersConfigTypeDef(TypedDict):
    Enabled: bool,
    SamplingRate: NotRequired[float],
```

## ResponseHeadersPolicyContentSecurityPolicyTypeDef

```python
# ResponseHeadersPolicyContentSecurityPolicyTypeDef definition

class ResponseHeadersPolicyContentSecurityPolicyTypeDef(TypedDict):
    Override: bool,
    ContentSecurityPolicy: str,
```

## ResponseHeadersPolicyContentTypeOptionsTypeDef

```python
# ResponseHeadersPolicyContentTypeOptionsTypeDef definition

class ResponseHeadersPolicyContentTypeOptionsTypeDef(TypedDict):
    Override: bool,
```

## ResponseHeadersPolicyCustomHeaderTypeDef

```python
# ResponseHeadersPolicyCustomHeaderTypeDef definition

class ResponseHeadersPolicyCustomHeaderTypeDef(TypedDict):
    Header: str,
    Value: str,
    Override: bool,
```

## ResponseHeadersPolicyFrameOptionsTypeDef

```python
# ResponseHeadersPolicyFrameOptionsTypeDef definition

class ResponseHeadersPolicyFrameOptionsTypeDef(TypedDict):
    Override: bool,
    FrameOption: FrameOptionsListType,  # (1)
```

1. See [:material-code-brackets: FrameOptionsListType](./literals.md#frameoptionslisttype) 
## ResponseHeadersPolicyReferrerPolicyTypeDef

```python
# ResponseHeadersPolicyReferrerPolicyTypeDef definition

class ResponseHeadersPolicyReferrerPolicyTypeDef(TypedDict):
    Override: bool,
    ReferrerPolicy: ReferrerPolicyListType,  # (1)
```

1. See [:material-code-brackets: ReferrerPolicyListType](./literals.md#referrerpolicylisttype) 
## ResponseHeadersPolicyRemoveHeaderTypeDef

```python
# ResponseHeadersPolicyRemoveHeaderTypeDef definition

class ResponseHeadersPolicyRemoveHeaderTypeDef(TypedDict):
    Header: str,
```

## ResponseHeadersPolicyStrictTransportSecurityTypeDef

```python
# ResponseHeadersPolicyStrictTransportSecurityTypeDef definition

class ResponseHeadersPolicyStrictTransportSecurityTypeDef(TypedDict):
    Override: bool,
    AccessControlMaxAgeSec: int,
    IncludeSubdomains: NotRequired[bool],
    Preload: NotRequired[bool],
```

## ResponseHeadersPolicyXSSProtectionTypeDef

```python
# ResponseHeadersPolicyXSSProtectionTypeDef definition

class ResponseHeadersPolicyXSSProtectionTypeDef(TypedDict):
    Override: bool,
    Protection: bool,
    ModeBlock: NotRequired[bool],
    ReportUri: NotRequired[str],
```

## S3OriginTypeDef

```python
# S3OriginTypeDef definition

class S3OriginTypeDef(TypedDict):
    DomainName: str,
    OriginAccessIdentity: str,
```

## StreamingLoggingConfigTypeDef

```python
# StreamingLoggingConfigTypeDef definition

class StreamingLoggingConfigTypeDef(TypedDict):
    Enabled: bool,
    Bucket: str,
    Prefix: str,
```

## TagKeysTypeDef

```python
# TagKeysTypeDef definition

class TagKeysTypeDef(TypedDict):
    Items: NotRequired[Sequence[str]],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## UpdateDistributionWithStagingConfigRequestRequestTypeDef

```python
# UpdateDistributionWithStagingConfigRequestRequestTypeDef definition

class UpdateDistributionWithStagingConfigRequestRequestTypeDef(TypedDict):
    Id: str,
    StagingDistributionId: NotRequired[str],
    IfMatch: NotRequired[str],
```

## AllowedMethodsTypeDef

```python
# AllowedMethodsTypeDef definition

class AllowedMethodsTypeDef(TypedDict):
    Quantity: int,
    Items: List[MethodType],  # (1)
    CachedMethods: NotRequired[CachedMethodsTypeDef],  # (2)
```

1. See [:material-code-brackets: MethodType](./literals.md#methodtype) 
2. See [:material-code-braces: CachedMethodsTypeDef](./type_defs.md#cachedmethodstypedef) 
## TestFunctionRequestRequestTypeDef

```python
# TestFunctionRequestRequestTypeDef definition

class TestFunctionRequestRequestTypeDef(TypedDict):
    Name: str,
    IfMatch: str,
    EventObject: Union[str, bytes, IO[Any], StreamingBody],
    Stage: NotRequired[FunctionStageType],  # (1)
```

1. See [:material-code-brackets: FunctionStageType](./literals.md#functionstagetype) 
## CachePolicyCookiesConfigTypeDef

```python
# CachePolicyCookiesConfigTypeDef definition

class CachePolicyCookiesConfigTypeDef(TypedDict):
    CookieBehavior: CachePolicyCookieBehaviorType,  # (1)
    Cookies: NotRequired[CookieNamesTypeDef],  # (2)
```

1. See [:material-code-brackets: CachePolicyCookieBehaviorType](./literals.md#cachepolicycookiebehaviortype) 
2. See [:material-code-braces: CookieNamesTypeDef](./type_defs.md#cookienamestypedef) 
## CookiePreferenceTypeDef

```python
# CookiePreferenceTypeDef definition

class CookiePreferenceTypeDef(TypedDict):
    Forward: ItemSelectionType,  # (1)
    WhitelistedNames: NotRequired[CookieNamesTypeDef],  # (2)
```

1. See [:material-code-brackets: ItemSelectionType](./literals.md#itemselectiontype) 
2. See [:material-code-braces: CookieNamesTypeDef](./type_defs.md#cookienamestypedef) 
## OriginRequestPolicyCookiesConfigTypeDef

```python
# OriginRequestPolicyCookiesConfigTypeDef definition

class OriginRequestPolicyCookiesConfigTypeDef(TypedDict):
    CookieBehavior: OriginRequestPolicyCookieBehaviorType,  # (1)
    Cookies: NotRequired[CookieNamesTypeDef],  # (2)
```

1. See [:material-code-brackets: OriginRequestPolicyCookieBehaviorType](./literals.md#originrequestpolicycookiebehaviortype) 
2. See [:material-code-braces: CookieNamesTypeDef](./type_defs.md#cookienamestypedef) 
## CachePolicyHeadersConfigTypeDef

```python
# CachePolicyHeadersConfigTypeDef definition

class CachePolicyHeadersConfigTypeDef(TypedDict):
    HeaderBehavior: CachePolicyHeaderBehaviorType,  # (1)
    Headers: NotRequired[HeadersTypeDef],  # (2)
```

1. See [:material-code-brackets: CachePolicyHeaderBehaviorType](./literals.md#cachepolicyheaderbehaviortype) 
2. See [:material-code-braces: HeadersTypeDef](./type_defs.md#headerstypedef) 
## OriginRequestPolicyHeadersConfigTypeDef

```python
# OriginRequestPolicyHeadersConfigTypeDef definition

class OriginRequestPolicyHeadersConfigTypeDef(TypedDict):
    HeaderBehavior: OriginRequestPolicyHeaderBehaviorType,  # (1)
    Headers: NotRequired[HeadersTypeDef],  # (2)
```

1. See [:material-code-brackets: OriginRequestPolicyHeaderBehaviorType](./literals.md#originrequestpolicyheaderbehaviortype) 
2. See [:material-code-braces: HeadersTypeDef](./type_defs.md#headerstypedef) 
## CachePolicyQueryStringsConfigTypeDef

```python
# CachePolicyQueryStringsConfigTypeDef definition

class CachePolicyQueryStringsConfigTypeDef(TypedDict):
    QueryStringBehavior: CachePolicyQueryStringBehaviorType,  # (1)
    QueryStrings: NotRequired[QueryStringNamesTypeDef],  # (2)
```

1. See [:material-code-brackets: CachePolicyQueryStringBehaviorType](./literals.md#cachepolicyquerystringbehaviortype) 
2. See [:material-code-braces: QueryStringNamesTypeDef](./type_defs.md#querystringnamestypedef) 
## OriginRequestPolicyQueryStringsConfigTypeDef

```python
# OriginRequestPolicyQueryStringsConfigTypeDef definition

class OriginRequestPolicyQueryStringsConfigTypeDef(TypedDict):
    QueryStringBehavior: OriginRequestPolicyQueryStringBehaviorType,  # (1)
    QueryStrings: NotRequired[QueryStringNamesTypeDef],  # (2)
```

1. See [:material-code-brackets: OriginRequestPolicyQueryStringBehaviorType](./literals.md#originrequestpolicyquerystringbehaviortype) 
2. See [:material-code-braces: QueryStringNamesTypeDef](./type_defs.md#querystringnamestypedef) 
## CloudFrontOriginAccessIdentityTypeDef

```python
# CloudFrontOriginAccessIdentityTypeDef definition

class CloudFrontOriginAccessIdentityTypeDef(TypedDict):
    Id: str,
    S3CanonicalUserId: str,
    CloudFrontOriginAccessIdentityConfig: NotRequired[CloudFrontOriginAccessIdentityConfigTypeDef],  # (1)
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityConfigTypeDef](./type_defs.md#cloudfrontoriginaccessidentityconfigtypedef) 
## CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef

```python
# CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef definition

class CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef(TypedDict):
    CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,  # (1)
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityConfigTypeDef](./type_defs.md#cloudfrontoriginaccessidentityconfigtypedef) 
## UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef

```python
# UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef definition

class UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef(TypedDict):
    CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityConfigTypeDef](./type_defs.md#cloudfrontoriginaccessidentityconfigtypedef) 
## CloudFrontOriginAccessIdentityListTypeDef

```python
# CloudFrontOriginAccessIdentityListTypeDef definition

class CloudFrontOriginAccessIdentityListTypeDef(TypedDict):
    Marker: str,
    MaxItems: int,
    IsTruncated: bool,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[CloudFrontOriginAccessIdentitySummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentitySummaryTypeDef](./type_defs.md#cloudfrontoriginaccessidentitysummarytypedef) 
## ConflictingAliasesListTypeDef

```python
# ConflictingAliasesListTypeDef definition

class ConflictingAliasesListTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    MaxItems: NotRequired[int],
    Quantity: NotRequired[int],
    Items: NotRequired[List[ConflictingAliasTypeDef]],  # (1)
```

1. See [:material-code-braces: ConflictingAliasTypeDef](./type_defs.md#conflictingaliastypedef) 
## ContentTypeProfilesTypeDef

```python
# ContentTypeProfilesTypeDef definition

class ContentTypeProfilesTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[ContentTypeProfileTypeDef]],  # (1)
```

1. See [:material-code-braces: ContentTypeProfileTypeDef](./type_defs.md#contenttypeprofiletypedef) 
## ContinuousDeploymentSingleWeightConfigTypeDef

```python
# ContinuousDeploymentSingleWeightConfigTypeDef definition

class ContinuousDeploymentSingleWeightConfigTypeDef(TypedDict):
    Weight: float,
    SessionStickinessConfig: NotRequired[SessionStickinessConfigTypeDef],  # (1)
```

1. See [:material-code-braces: SessionStickinessConfigTypeDef](./type_defs.md#sessionstickinessconfigtypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCloudFrontOriginAccessIdentityConfigResultTypeDef

```python
# GetCloudFrontOriginAccessIdentityConfigResultTypeDef definition

class GetCloudFrontOriginAccessIdentityConfigResultTypeDef(TypedDict):
    CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityConfigTypeDef](./type_defs.md#cloudfrontoriginaccessidentityconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFunctionResultTypeDef

```python
# GetFunctionResultTypeDef definition

class GetFunctionResultTypeDef(TypedDict):
    FunctionCode: StreamingBody,
    ETag: str,
    ContentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFunctionRequestRequestTypeDef

```python
# CreateFunctionRequestRequestTypeDef definition

class CreateFunctionRequestRequestTypeDef(TypedDict):
    Name: str,
    FunctionConfig: FunctionConfigTypeDef,  # (1)
    FunctionCode: Union[str, bytes, IO[Any], StreamingBody],
```

1. See [:material-code-braces: FunctionConfigTypeDef](./type_defs.md#functionconfigtypedef) 
## UpdateFunctionRequestRequestTypeDef

```python
# UpdateFunctionRequestRequestTypeDef definition

class UpdateFunctionRequestRequestTypeDef(TypedDict):
    Name: str,
    IfMatch: str,
    FunctionConfig: FunctionConfigTypeDef,  # (1)
    FunctionCode: Union[str, bytes, IO[Any], StreamingBody],
```

1. See [:material-code-braces: FunctionConfigTypeDef](./type_defs.md#functionconfigtypedef) 
## CreateKeyGroupRequestRequestTypeDef

```python
# CreateKeyGroupRequestRequestTypeDef definition

class CreateKeyGroupRequestRequestTypeDef(TypedDict):
    KeyGroupConfig: KeyGroupConfigTypeDef,  # (1)
```

1. See [:material-code-braces: KeyGroupConfigTypeDef](./type_defs.md#keygroupconfigtypedef) 
## GetKeyGroupConfigResultTypeDef

```python
# GetKeyGroupConfigResultTypeDef definition

class GetKeyGroupConfigResultTypeDef(TypedDict):
    KeyGroupConfig: KeyGroupConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyGroupConfigTypeDef](./type_defs.md#keygroupconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KeyGroupTypeDef

```python
# KeyGroupTypeDef definition

class KeyGroupTypeDef(TypedDict):
    Id: str,
    LastModifiedTime: datetime,
    KeyGroupConfig: KeyGroupConfigTypeDef,  # (1)
```

1. See [:material-code-braces: KeyGroupConfigTypeDef](./type_defs.md#keygroupconfigtypedef) 
## UpdateKeyGroupRequestRequestTypeDef

```python
# UpdateKeyGroupRequestRequestTypeDef definition

class UpdateKeyGroupRequestRequestTypeDef(TypedDict):
    KeyGroupConfig: KeyGroupConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: KeyGroupConfigTypeDef](./type_defs.md#keygroupconfigtypedef) 
## CreateOriginAccessControlRequestRequestTypeDef

```python
# CreateOriginAccessControlRequestRequestTypeDef definition

class CreateOriginAccessControlRequestRequestTypeDef(TypedDict):
    OriginAccessControlConfig: OriginAccessControlConfigTypeDef,  # (1)
```

1. See [:material-code-braces: OriginAccessControlConfigTypeDef](./type_defs.md#originaccesscontrolconfigtypedef) 
## GetOriginAccessControlConfigResultTypeDef

```python
# GetOriginAccessControlConfigResultTypeDef definition

class GetOriginAccessControlConfigResultTypeDef(TypedDict):
    OriginAccessControlConfig: OriginAccessControlConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginAccessControlConfigTypeDef](./type_defs.md#originaccesscontrolconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OriginAccessControlTypeDef

```python
# OriginAccessControlTypeDef definition

class OriginAccessControlTypeDef(TypedDict):
    Id: str,
    OriginAccessControlConfig: NotRequired[OriginAccessControlConfigTypeDef],  # (1)
```

1. See [:material-code-braces: OriginAccessControlConfigTypeDef](./type_defs.md#originaccesscontrolconfigtypedef) 
## UpdateOriginAccessControlRequestRequestTypeDef

```python
# UpdateOriginAccessControlRequestRequestTypeDef definition

class UpdateOriginAccessControlRequestRequestTypeDef(TypedDict):
    OriginAccessControlConfig: OriginAccessControlConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: OriginAccessControlConfigTypeDef](./type_defs.md#originaccesscontrolconfigtypedef) 
## CreatePublicKeyRequestRequestTypeDef

```python
# CreatePublicKeyRequestRequestTypeDef definition

class CreatePublicKeyRequestRequestTypeDef(TypedDict):
    PublicKeyConfig: PublicKeyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: PublicKeyConfigTypeDef](./type_defs.md#publickeyconfigtypedef) 
## GetPublicKeyConfigResultTypeDef

```python
# GetPublicKeyConfigResultTypeDef definition

class GetPublicKeyConfigResultTypeDef(TypedDict):
    PublicKeyConfig: PublicKeyConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyConfigTypeDef](./type_defs.md#publickeyconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublicKeyTypeDef

```python
# PublicKeyTypeDef definition

class PublicKeyTypeDef(TypedDict):
    Id: str,
    CreatedTime: datetime,
    PublicKeyConfig: PublicKeyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: PublicKeyConfigTypeDef](./type_defs.md#publickeyconfigtypedef) 
## UpdatePublicKeyRequestRequestTypeDef

```python
# UpdatePublicKeyRequestRequestTypeDef definition

class UpdatePublicKeyRequestRequestTypeDef(TypedDict):
    PublicKeyConfig: PublicKeyConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: PublicKeyConfigTypeDef](./type_defs.md#publickeyconfigtypedef) 
## CustomErrorResponsesTypeDef

```python
# CustomErrorResponsesTypeDef definition

class CustomErrorResponsesTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[CustomErrorResponseTypeDef]],  # (1)
```

1. See [:material-code-braces: CustomErrorResponseTypeDef](./type_defs.md#customerrorresponsetypedef) 
## CustomHeadersTypeDef

```python
# CustomHeadersTypeDef definition

class CustomHeadersTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[OriginCustomHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: OriginCustomHeaderTypeDef](./type_defs.md#origincustomheadertypedef) 
## CustomOriginConfigTypeDef

```python
# CustomOriginConfigTypeDef definition

class CustomOriginConfigTypeDef(TypedDict):
    HTTPPort: int,
    HTTPSPort: int,
    OriginProtocolPolicy: OriginProtocolPolicyType,  # (1)
    OriginSslProtocols: NotRequired[OriginSslProtocolsTypeDef],  # (2)
    OriginReadTimeout: NotRequired[int],
    OriginKeepaliveTimeout: NotRequired[int],
```

1. See [:material-code-brackets: OriginProtocolPolicyType](./literals.md#originprotocolpolicytype) 
2. See [:material-code-braces: OriginSslProtocolsTypeDef](./type_defs.md#originsslprotocolstypedef) 
## ListDistributionsByCachePolicyIdResultTypeDef

```python
# ListDistributionsByCachePolicyIdResultTypeDef definition

class ListDistributionsByCachePolicyIdResultTypeDef(TypedDict):
    DistributionIdList: DistributionIdListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionIdListTypeDef](./type_defs.md#distributionidlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDistributionsByKeyGroupResultTypeDef

```python
# ListDistributionsByKeyGroupResultTypeDef definition

class ListDistributionsByKeyGroupResultTypeDef(TypedDict):
    DistributionIdList: DistributionIdListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionIdListTypeDef](./type_defs.md#distributionidlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDistributionsByOriginRequestPolicyIdResultTypeDef

```python
# ListDistributionsByOriginRequestPolicyIdResultTypeDef definition

class ListDistributionsByOriginRequestPolicyIdResultTypeDef(TypedDict):
    DistributionIdList: DistributionIdListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionIdListTypeDef](./type_defs.md#distributionidlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDistributionsByResponseHeadersPolicyIdResultTypeDef

```python
# ListDistributionsByResponseHeadersPolicyIdResultTypeDef definition

class ListDistributionsByResponseHeadersPolicyIdResultTypeDef(TypedDict):
    DistributionIdList: DistributionIdListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionIdListTypeDef](./type_defs.md#distributionidlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EncryptionEntityTypeDef

```python
# EncryptionEntityTypeDef definition

class EncryptionEntityTypeDef(TypedDict):
    PublicKeyId: str,
    ProviderId: str,
    FieldPatterns: FieldPatternsTypeDef,  # (1)
```

1. See [:material-code-braces: FieldPatternsTypeDef](./type_defs.md#fieldpatternstypedef) 
## EndPointTypeDef

```python
# EndPointTypeDef definition

class EndPointTypeDef(TypedDict):
    StreamType: str,
    KinesisStreamConfig: NotRequired[KinesisStreamConfigTypeDef],  # (1)
```

1. See [:material-code-braces: KinesisStreamConfigTypeDef](./type_defs.md#kinesisstreamconfigtypedef) 
## FunctionAssociationsTypeDef

```python
# FunctionAssociationsTypeDef definition

class FunctionAssociationsTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[FunctionAssociationTypeDef]],  # (1)
```

1. See [:material-code-braces: FunctionAssociationTypeDef](./type_defs.md#functionassociationtypedef) 
## FunctionSummaryTypeDef

```python
# FunctionSummaryTypeDef definition

class FunctionSummaryTypeDef(TypedDict):
    Name: str,
    FunctionConfig: FunctionConfigTypeDef,  # (1)
    FunctionMetadata: FunctionMetadataTypeDef,  # (2)
    Status: NotRequired[str],
```

1. See [:material-code-braces: FunctionConfigTypeDef](./type_defs.md#functionconfigtypedef) 
2. See [:material-code-braces: FunctionMetadataTypeDef](./type_defs.md#functionmetadatatypedef) 
## RestrictionsTypeDef

```python
# RestrictionsTypeDef definition

class RestrictionsTypeDef(TypedDict):
    GeoRestriction: GeoRestrictionTypeDef,  # (1)
```

1. See [:material-code-braces: GeoRestrictionTypeDef](./type_defs.md#georestrictiontypedef) 
## GetDistributionRequestDistributionDeployedWaitTypeDef

```python
# GetDistributionRequestDistributionDeployedWaitTypeDef definition

class GetDistributionRequestDistributionDeployedWaitTypeDef(TypedDict):
    Id: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetInvalidationRequestInvalidationCompletedWaitTypeDef

```python
# GetInvalidationRequestInvalidationCompletedWaitTypeDef definition

class GetInvalidationRequestInvalidationCompletedWaitTypeDef(TypedDict):
    DistributionId: str,
    Id: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef

```python
# GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef definition

class GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef(TypedDict):
    Id: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## InvalidationBatchTypeDef

```python
# InvalidationBatchTypeDef definition

class InvalidationBatchTypeDef(TypedDict):
    Paths: PathsTypeDef,  # (1)
    CallerReference: str,
```

1. See [:material-code-braces: PathsTypeDef](./type_defs.md#pathstypedef) 
## InvalidationListTypeDef

```python
# InvalidationListTypeDef definition

class InvalidationListTypeDef(TypedDict):
    Marker: str,
    MaxItems: int,
    IsTruncated: bool,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[InvalidationSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: InvalidationSummaryTypeDef](./type_defs.md#invalidationsummarytypedef) 
## KGKeyPairIdsTypeDef

```python
# KGKeyPairIdsTypeDef definition

class KGKeyPairIdsTypeDef(TypedDict):
    KeyGroupId: NotRequired[str],
    KeyPairIds: NotRequired[KeyPairIdsTypeDef],  # (1)
```

1. See [:material-code-braces: KeyPairIdsTypeDef](./type_defs.md#keypairidstypedef) 
## SignerTypeDef

```python
# SignerTypeDef definition

class SignerTypeDef(TypedDict):
    AwsAccountNumber: NotRequired[str],
    KeyPairIds: NotRequired[KeyPairIdsTypeDef],  # (1)
```

1. See [:material-code-braces: KeyPairIdsTypeDef](./type_defs.md#keypairidstypedef) 
## LambdaFunctionAssociationsTypeDef

```python
# LambdaFunctionAssociationsTypeDef definition

class LambdaFunctionAssociationsTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[LambdaFunctionAssociationTypeDef]],  # (1)
```

1. See [:material-code-braces: LambdaFunctionAssociationTypeDef](./type_defs.md#lambdafunctionassociationtypedef) 
## ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef

```python
# ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef definition

class ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDistributionsRequestListDistributionsPaginateTypeDef

```python
# ListDistributionsRequestListDistributionsPaginateTypeDef definition

class ListDistributionsRequestListDistributionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInvalidationsRequestListInvalidationsPaginateTypeDef

```python
# ListInvalidationsRequestListInvalidationsPaginateTypeDef definition

class ListInvalidationsRequestListInvalidationsPaginateTypeDef(TypedDict):
    DistributionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef

```python
# ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef definition

class ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## MonitoringSubscriptionTypeDef

```python
# MonitoringSubscriptionTypeDef definition

class MonitoringSubscriptionTypeDef(TypedDict):
    RealtimeMetricsSubscriptionConfig: NotRequired[RealtimeMetricsSubscriptionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: RealtimeMetricsSubscriptionConfigTypeDef](./type_defs.md#realtimemetricssubscriptionconfigtypedef) 
## OriginAccessControlListTypeDef

```python
# OriginAccessControlListTypeDef definition

class OriginAccessControlListTypeDef(TypedDict):
    Marker: str,
    MaxItems: int,
    IsTruncated: bool,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[OriginAccessControlSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: OriginAccessControlSummaryTypeDef](./type_defs.md#originaccesscontrolsummarytypedef) 
## OriginGroupFailoverCriteriaTypeDef

```python
# OriginGroupFailoverCriteriaTypeDef definition

class OriginGroupFailoverCriteriaTypeDef(TypedDict):
    StatusCodes: StatusCodesTypeDef,  # (1)
```

1. See [:material-code-braces: StatusCodesTypeDef](./type_defs.md#statuscodestypedef) 
## OriginGroupMembersTypeDef

```python
# OriginGroupMembersTypeDef definition

class OriginGroupMembersTypeDef(TypedDict):
    Quantity: int,
    Items: List[OriginGroupMemberTypeDef],  # (1)
```

1. See [:material-code-braces: OriginGroupMemberTypeDef](./type_defs.md#origingroupmembertypedef) 
## PublicKeyListTypeDef

```python
# PublicKeyListTypeDef definition

class PublicKeyListTypeDef(TypedDict):
    MaxItems: int,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[PublicKeySummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: PublicKeySummaryTypeDef](./type_defs.md#publickeysummarytypedef) 
## QueryArgProfilesTypeDef

```python
# QueryArgProfilesTypeDef definition

class QueryArgProfilesTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[QueryArgProfileTypeDef]],  # (1)
```

1. See [:material-code-braces: QueryArgProfileTypeDef](./type_defs.md#queryargprofiletypedef) 
## ResponseHeadersPolicyCorsConfigTypeDef

```python
# ResponseHeadersPolicyCorsConfigTypeDef definition

class ResponseHeadersPolicyCorsConfigTypeDef(TypedDict):
    AccessControlAllowOrigins: ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,  # (1)
    AccessControlAllowHeaders: ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,  # (2)
    AccessControlAllowMethods: ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,  # (3)
    AccessControlAllowCredentials: bool,
    OriginOverride: bool,
    AccessControlExposeHeaders: NotRequired[ResponseHeadersPolicyAccessControlExposeHeadersTypeDef],  # (4)
    AccessControlMaxAgeSec: NotRequired[int],
```

1. See [:material-code-braces: ResponseHeadersPolicyAccessControlAllowOriginsTypeDef](./type_defs.md#responseheaderspolicyaccesscontrolalloworiginstypedef) 
2. See [:material-code-braces: ResponseHeadersPolicyAccessControlAllowHeadersTypeDef](./type_defs.md#responseheaderspolicyaccesscontrolallowheaderstypedef) 
3. See [:material-code-braces: ResponseHeadersPolicyAccessControlAllowMethodsTypeDef](./type_defs.md#responseheaderspolicyaccesscontrolallowmethodstypedef) 
4. See [:material-code-braces: ResponseHeadersPolicyAccessControlExposeHeadersTypeDef](./type_defs.md#responseheaderspolicyaccesscontrolexposeheaderstypedef) 
## ResponseHeadersPolicyCustomHeadersConfigTypeDef

```python
# ResponseHeadersPolicyCustomHeadersConfigTypeDef definition

class ResponseHeadersPolicyCustomHeadersConfigTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[ResponseHeadersPolicyCustomHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: ResponseHeadersPolicyCustomHeaderTypeDef](./type_defs.md#responseheaderspolicycustomheadertypedef) 
## ResponseHeadersPolicyRemoveHeadersConfigTypeDef

```python
# ResponseHeadersPolicyRemoveHeadersConfigTypeDef definition

class ResponseHeadersPolicyRemoveHeadersConfigTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[ResponseHeadersPolicyRemoveHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: ResponseHeadersPolicyRemoveHeaderTypeDef](./type_defs.md#responseheaderspolicyremoveheadertypedef) 
## ResponseHeadersPolicySecurityHeadersConfigTypeDef

```python
# ResponseHeadersPolicySecurityHeadersConfigTypeDef definition

class ResponseHeadersPolicySecurityHeadersConfigTypeDef(TypedDict):
    XSSProtection: NotRequired[ResponseHeadersPolicyXSSProtectionTypeDef],  # (1)
    FrameOptions: NotRequired[ResponseHeadersPolicyFrameOptionsTypeDef],  # (2)
    ReferrerPolicy: NotRequired[ResponseHeadersPolicyReferrerPolicyTypeDef],  # (3)
    ContentSecurityPolicy: NotRequired[ResponseHeadersPolicyContentSecurityPolicyTypeDef],  # (4)
    ContentTypeOptions: NotRequired[ResponseHeadersPolicyContentTypeOptionsTypeDef],  # (5)
    StrictTransportSecurity: NotRequired[ResponseHeadersPolicyStrictTransportSecurityTypeDef],  # (6)
```

1. See [:material-code-braces: ResponseHeadersPolicyXSSProtectionTypeDef](./type_defs.md#responseheaderspolicyxssprotectiontypedef) 
2. See [:material-code-braces: ResponseHeadersPolicyFrameOptionsTypeDef](./type_defs.md#responseheaderspolicyframeoptionstypedef) 
3. See [:material-code-braces: ResponseHeadersPolicyReferrerPolicyTypeDef](./type_defs.md#responseheaderspolicyreferrerpolicytypedef) 
4. See [:material-code-braces: ResponseHeadersPolicyContentSecurityPolicyTypeDef](./type_defs.md#responseheaderspolicycontentsecuritypolicytypedef) 
5. See [:material-code-braces: ResponseHeadersPolicyContentTypeOptionsTypeDef](./type_defs.md#responseheaderspolicycontenttypeoptionstypedef) 
6. See [:material-code-braces: ResponseHeadersPolicyStrictTransportSecurityTypeDef](./type_defs.md#responseheaderspolicystricttransportsecuritytypedef) 
## StreamingDistributionSummaryTypeDef

```python
# StreamingDistributionSummaryTypeDef definition

class StreamingDistributionSummaryTypeDef(TypedDict):
    Id: str,
    ARN: str,
    Status: str,
    LastModifiedTime: datetime,
    DomainName: str,
    S3Origin: S3OriginTypeDef,  # (1)
    Aliases: AliasesTypeDef,  # (2)
    TrustedSigners: TrustedSignersTypeDef,  # (3)
    Comment: str,
    PriceClass: PriceClassType,  # (4)
    Enabled: bool,
```

1. See [:material-code-braces: S3OriginTypeDef](./type_defs.md#s3origintypedef) 
2. See [:material-code-braces: AliasesTypeDef](./type_defs.md#aliasestypedef) 
3. See [:material-code-braces: TrustedSignersTypeDef](./type_defs.md#trustedsignerstypedef) 
4. See [:material-code-brackets: PriceClassType](./literals.md#priceclasstype) 
## StreamingDistributionConfigTypeDef

```python
# StreamingDistributionConfigTypeDef definition

class StreamingDistributionConfigTypeDef(TypedDict):
    CallerReference: str,
    S3Origin: S3OriginTypeDef,  # (1)
    Comment: str,
    TrustedSigners: TrustedSignersTypeDef,  # (4)
    Enabled: bool,
    Aliases: NotRequired[AliasesTypeDef],  # (2)
    Logging: NotRequired[StreamingLoggingConfigTypeDef],  # (3)
    PriceClass: NotRequired[PriceClassType],  # (5)
```

1. See [:material-code-braces: S3OriginTypeDef](./type_defs.md#s3origintypedef) 
2. See [:material-code-braces: AliasesTypeDef](./type_defs.md#aliasestypedef) 
3. See [:material-code-braces: StreamingLoggingConfigTypeDef](./type_defs.md#streamingloggingconfigtypedef) 
4. See [:material-code-braces: TrustedSignersTypeDef](./type_defs.md#trustedsignerstypedef) 
5. See [:material-code-brackets: PriceClassType](./literals.md#priceclasstype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    Resource: str,
    TagKeys: TagKeysTypeDef,  # (1)
```

1. See [:material-code-braces: TagKeysTypeDef](./type_defs.md#tagkeystypedef) 
## TagsTypeDef

```python
# TagsTypeDef definition

class TagsTypeDef(TypedDict):
    Items: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ForwardedValuesTypeDef

```python
# ForwardedValuesTypeDef definition

class ForwardedValuesTypeDef(TypedDict):
    QueryString: bool,
    Cookies: CookiePreferenceTypeDef,  # (1)
    Headers: NotRequired[HeadersTypeDef],  # (2)
    QueryStringCacheKeys: NotRequired[QueryStringCacheKeysTypeDef],  # (3)
```

1. See [:material-code-braces: CookiePreferenceTypeDef](./type_defs.md#cookiepreferencetypedef) 
2. See [:material-code-braces: HeadersTypeDef](./type_defs.md#headerstypedef) 
3. See [:material-code-braces: QueryStringCacheKeysTypeDef](./type_defs.md#querystringcachekeystypedef) 
## ParametersInCacheKeyAndForwardedToOriginTypeDef

```python
# ParametersInCacheKeyAndForwardedToOriginTypeDef definition

class ParametersInCacheKeyAndForwardedToOriginTypeDef(TypedDict):
    EnableAcceptEncodingGzip: bool,
    HeadersConfig: CachePolicyHeadersConfigTypeDef,  # (1)
    CookiesConfig: CachePolicyCookiesConfigTypeDef,  # (2)
    QueryStringsConfig: CachePolicyQueryStringsConfigTypeDef,  # (3)
    EnableAcceptEncodingBrotli: NotRequired[bool],
```

1. See [:material-code-braces: CachePolicyHeadersConfigTypeDef](./type_defs.md#cachepolicyheadersconfigtypedef) 
2. See [:material-code-braces: CachePolicyCookiesConfigTypeDef](./type_defs.md#cachepolicycookiesconfigtypedef) 
3. See [:material-code-braces: CachePolicyQueryStringsConfigTypeDef](./type_defs.md#cachepolicyquerystringsconfigtypedef) 
## OriginRequestPolicyConfigTypeDef

```python
# OriginRequestPolicyConfigTypeDef definition

class OriginRequestPolicyConfigTypeDef(TypedDict):
    Name: str,
    HeadersConfig: OriginRequestPolicyHeadersConfigTypeDef,  # (1)
    CookiesConfig: OriginRequestPolicyCookiesConfigTypeDef,  # (2)
    QueryStringsConfig: OriginRequestPolicyQueryStringsConfigTypeDef,  # (3)
    Comment: NotRequired[str],
```

1. See [:material-code-braces: OriginRequestPolicyHeadersConfigTypeDef](./type_defs.md#originrequestpolicyheadersconfigtypedef) 
2. See [:material-code-braces: OriginRequestPolicyCookiesConfigTypeDef](./type_defs.md#originrequestpolicycookiesconfigtypedef) 
3. See [:material-code-braces: OriginRequestPolicyQueryStringsConfigTypeDef](./type_defs.md#originrequestpolicyquerystringsconfigtypedef) 
## CreateCloudFrontOriginAccessIdentityResultTypeDef

```python
# CreateCloudFrontOriginAccessIdentityResultTypeDef definition

class CreateCloudFrontOriginAccessIdentityResultTypeDef(TypedDict):
    CloudFrontOriginAccessIdentity: CloudFrontOriginAccessIdentityTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityTypeDef](./type_defs.md#cloudfrontoriginaccessidentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCloudFrontOriginAccessIdentityResultTypeDef

```python
# GetCloudFrontOriginAccessIdentityResultTypeDef definition

class GetCloudFrontOriginAccessIdentityResultTypeDef(TypedDict):
    CloudFrontOriginAccessIdentity: CloudFrontOriginAccessIdentityTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityTypeDef](./type_defs.md#cloudfrontoriginaccessidentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCloudFrontOriginAccessIdentityResultTypeDef

```python
# UpdateCloudFrontOriginAccessIdentityResultTypeDef definition

class UpdateCloudFrontOriginAccessIdentityResultTypeDef(TypedDict):
    CloudFrontOriginAccessIdentity: CloudFrontOriginAccessIdentityTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityTypeDef](./type_defs.md#cloudfrontoriginaccessidentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCloudFrontOriginAccessIdentitiesResultTypeDef

```python
# ListCloudFrontOriginAccessIdentitiesResultTypeDef definition

class ListCloudFrontOriginAccessIdentitiesResultTypeDef(TypedDict):
    CloudFrontOriginAccessIdentityList: CloudFrontOriginAccessIdentityListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityListTypeDef](./type_defs.md#cloudfrontoriginaccessidentitylisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConflictingAliasesResultTypeDef

```python
# ListConflictingAliasesResultTypeDef definition

class ListConflictingAliasesResultTypeDef(TypedDict):
    ConflictingAliasesList: ConflictingAliasesListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConflictingAliasesListTypeDef](./type_defs.md#conflictingaliaseslisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContentTypeProfileConfigTypeDef

```python
# ContentTypeProfileConfigTypeDef definition

class ContentTypeProfileConfigTypeDef(TypedDict):
    ForwardWhenContentTypeIsUnknown: bool,
    ContentTypeProfiles: NotRequired[ContentTypeProfilesTypeDef],  # (1)
```

1. See [:material-code-braces: ContentTypeProfilesTypeDef](./type_defs.md#contenttypeprofilestypedef) 
## TrafficConfigTypeDef

```python
# TrafficConfigTypeDef definition

class TrafficConfigTypeDef(TypedDict):
    Type: ContinuousDeploymentPolicyTypeType,  # (3)
    SingleWeightConfig: NotRequired[ContinuousDeploymentSingleWeightConfigTypeDef],  # (1)
    SingleHeaderConfig: NotRequired[ContinuousDeploymentSingleHeaderConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ContinuousDeploymentSingleWeightConfigTypeDef](./type_defs.md#continuousdeploymentsingleweightconfigtypedef) 
2. See [:material-code-braces: ContinuousDeploymentSingleHeaderConfigTypeDef](./type_defs.md#continuousdeploymentsingleheaderconfigtypedef) 
3. See [:material-code-brackets: ContinuousDeploymentPolicyTypeType](./literals.md#continuousdeploymentpolicytypetype) 
## CreateKeyGroupResultTypeDef

```python
# CreateKeyGroupResultTypeDef definition

class CreateKeyGroupResultTypeDef(TypedDict):
    KeyGroup: KeyGroupTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyGroupTypeDef](./type_defs.md#keygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKeyGroupResultTypeDef

```python
# GetKeyGroupResultTypeDef definition

class GetKeyGroupResultTypeDef(TypedDict):
    KeyGroup: KeyGroupTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyGroupTypeDef](./type_defs.md#keygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KeyGroupSummaryTypeDef

```python
# KeyGroupSummaryTypeDef definition

class KeyGroupSummaryTypeDef(TypedDict):
    KeyGroup: KeyGroupTypeDef,  # (1)
```

1. See [:material-code-braces: KeyGroupTypeDef](./type_defs.md#keygrouptypedef) 
## UpdateKeyGroupResultTypeDef

```python
# UpdateKeyGroupResultTypeDef definition

class UpdateKeyGroupResultTypeDef(TypedDict):
    KeyGroup: KeyGroupTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyGroupTypeDef](./type_defs.md#keygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOriginAccessControlResultTypeDef

```python
# CreateOriginAccessControlResultTypeDef definition

class CreateOriginAccessControlResultTypeDef(TypedDict):
    OriginAccessControl: OriginAccessControlTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginAccessControlTypeDef](./type_defs.md#originaccesscontroltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOriginAccessControlResultTypeDef

```python
# GetOriginAccessControlResultTypeDef definition

class GetOriginAccessControlResultTypeDef(TypedDict):
    OriginAccessControl: OriginAccessControlTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginAccessControlTypeDef](./type_defs.md#originaccesscontroltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOriginAccessControlResultTypeDef

```python
# UpdateOriginAccessControlResultTypeDef definition

class UpdateOriginAccessControlResultTypeDef(TypedDict):
    OriginAccessControl: OriginAccessControlTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginAccessControlTypeDef](./type_defs.md#originaccesscontroltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePublicKeyResultTypeDef

```python
# CreatePublicKeyResultTypeDef definition

class CreatePublicKeyResultTypeDef(TypedDict):
    PublicKey: PublicKeyTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyTypeDef](./type_defs.md#publickeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPublicKeyResultTypeDef

```python
# GetPublicKeyResultTypeDef definition

class GetPublicKeyResultTypeDef(TypedDict):
    PublicKey: PublicKeyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyTypeDef](./type_defs.md#publickeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePublicKeyResultTypeDef

```python
# UpdatePublicKeyResultTypeDef definition

class UpdatePublicKeyResultTypeDef(TypedDict):
    PublicKey: PublicKeyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyTypeDef](./type_defs.md#publickeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OriginTypeDef

```python
# OriginTypeDef definition

class OriginTypeDef(TypedDict):
    Id: str,
    DomainName: str,
    OriginPath: NotRequired[str],
    CustomHeaders: NotRequired[CustomHeadersTypeDef],  # (1)
    S3OriginConfig: NotRequired[S3OriginConfigTypeDef],  # (2)
    CustomOriginConfig: NotRequired[CustomOriginConfigTypeDef],  # (3)
    ConnectionAttempts: NotRequired[int],
    ConnectionTimeout: NotRequired[int],
    OriginShield: NotRequired[OriginShieldTypeDef],  # (4)
    OriginAccessControlId: NotRequired[str],
```

1. See [:material-code-braces: CustomHeadersTypeDef](./type_defs.md#customheaderstypedef) 
2. See [:material-code-braces: S3OriginConfigTypeDef](./type_defs.md#s3originconfigtypedef) 
3. See [:material-code-braces: CustomOriginConfigTypeDef](./type_defs.md#customoriginconfigtypedef) 
4. See [:material-code-braces: OriginShieldTypeDef](./type_defs.md#originshieldtypedef) 
## EncryptionEntitiesTypeDef

```python
# EncryptionEntitiesTypeDef definition

class EncryptionEntitiesTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[Sequence[EncryptionEntityTypeDef]],  # (1)
```

1. See [:material-code-braces: EncryptionEntityTypeDef](./type_defs.md#encryptionentitytypedef) 
## CreateRealtimeLogConfigRequestRequestTypeDef

```python
# CreateRealtimeLogConfigRequestRequestTypeDef definition

class CreateRealtimeLogConfigRequestRequestTypeDef(TypedDict):
    EndPoints: Sequence[EndPointTypeDef],  # (1)
    Fields: Sequence[str],
    Name: str,
    SamplingRate: int,
```

1. See [:material-code-braces: EndPointTypeDef](./type_defs.md#endpointtypedef) 
## RealtimeLogConfigTypeDef

```python
# RealtimeLogConfigTypeDef definition

class RealtimeLogConfigTypeDef(TypedDict):
    ARN: str,
    Name: str,
    SamplingRate: int,
    EndPoints: List[EndPointTypeDef],  # (1)
    Fields: List[str],
```

1. See [:material-code-braces: EndPointTypeDef](./type_defs.md#endpointtypedef) 
## UpdateRealtimeLogConfigRequestRequestTypeDef

```python
# UpdateRealtimeLogConfigRequestRequestTypeDef definition

class UpdateRealtimeLogConfigRequestRequestTypeDef(TypedDict):
    EndPoints: NotRequired[Sequence[EndPointTypeDef]],  # (1)
    Fields: NotRequired[Sequence[str]],
    Name: NotRequired[str],
    ARN: NotRequired[str],
    SamplingRate: NotRequired[int],
```

1. See [:material-code-braces: EndPointTypeDef](./type_defs.md#endpointtypedef) 
## CreateFunctionResultTypeDef

```python
# CreateFunctionResultTypeDef definition

class CreateFunctionResultTypeDef(TypedDict):
    FunctionSummary: FunctionSummaryTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionSummaryTypeDef](./type_defs.md#functionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFunctionResultTypeDef

```python
# DescribeFunctionResultTypeDef definition

class DescribeFunctionResultTypeDef(TypedDict):
    FunctionSummary: FunctionSummaryTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionSummaryTypeDef](./type_defs.md#functionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionListTypeDef

```python
# FunctionListTypeDef definition

class FunctionListTypeDef(TypedDict):
    MaxItems: int,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[FunctionSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: FunctionSummaryTypeDef](./type_defs.md#functionsummarytypedef) 
## PublishFunctionResultTypeDef

```python
# PublishFunctionResultTypeDef definition

class PublishFunctionResultTypeDef(TypedDict):
    FunctionSummary: FunctionSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionSummaryTypeDef](./type_defs.md#functionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestResultTypeDef

```python
# TestResultTypeDef definition

class TestResultTypeDef(TypedDict):
    FunctionSummary: NotRequired[FunctionSummaryTypeDef],  # (1)
    ComputeUtilization: NotRequired[str],
    FunctionExecutionLogs: NotRequired[List[str]],
    FunctionErrorMessage: NotRequired[str],
    FunctionOutput: NotRequired[str],
```

1. See [:material-code-braces: FunctionSummaryTypeDef](./type_defs.md#functionsummarytypedef) 
## UpdateFunctionResultTypeDef

```python
# UpdateFunctionResultTypeDef definition

class UpdateFunctionResultTypeDef(TypedDict):
    FunctionSummary: FunctionSummaryTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionSummaryTypeDef](./type_defs.md#functionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInvalidationRequestRequestTypeDef

```python
# CreateInvalidationRequestRequestTypeDef definition

class CreateInvalidationRequestRequestTypeDef(TypedDict):
    DistributionId: str,
    InvalidationBatch: InvalidationBatchTypeDef,  # (1)
```

1. See [:material-code-braces: InvalidationBatchTypeDef](./type_defs.md#invalidationbatchtypedef) 
## InvalidationTypeDef

```python
# InvalidationTypeDef definition

class InvalidationTypeDef(TypedDict):
    Id: str,
    Status: str,
    CreateTime: datetime,
    InvalidationBatch: InvalidationBatchTypeDef,  # (1)
```

1. See [:material-code-braces: InvalidationBatchTypeDef](./type_defs.md#invalidationbatchtypedef) 
## ListInvalidationsResultTypeDef

```python
# ListInvalidationsResultTypeDef definition

class ListInvalidationsResultTypeDef(TypedDict):
    InvalidationList: InvalidationListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvalidationListTypeDef](./type_defs.md#invalidationlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActiveTrustedKeyGroupsTypeDef

```python
# ActiveTrustedKeyGroupsTypeDef definition

class ActiveTrustedKeyGroupsTypeDef(TypedDict):
    Enabled: bool,
    Quantity: int,
    Items: NotRequired[List[KGKeyPairIdsTypeDef]],  # (1)
```

1. See [:material-code-braces: KGKeyPairIdsTypeDef](./type_defs.md#kgkeypairidstypedef) 
## ActiveTrustedSignersTypeDef

```python
# ActiveTrustedSignersTypeDef definition

class ActiveTrustedSignersTypeDef(TypedDict):
    Enabled: bool,
    Quantity: int,
    Items: NotRequired[List[SignerTypeDef]],  # (1)
```

1. See [:material-code-braces: SignerTypeDef](./type_defs.md#signertypedef) 
## CreateMonitoringSubscriptionRequestRequestTypeDef

```python
# CreateMonitoringSubscriptionRequestRequestTypeDef definition

class CreateMonitoringSubscriptionRequestRequestTypeDef(TypedDict):
    DistributionId: str,
    MonitoringSubscription: MonitoringSubscriptionTypeDef,  # (1)
```

1. See [:material-code-braces: MonitoringSubscriptionTypeDef](./type_defs.md#monitoringsubscriptiontypedef) 
## CreateMonitoringSubscriptionResultTypeDef

```python
# CreateMonitoringSubscriptionResultTypeDef definition

class CreateMonitoringSubscriptionResultTypeDef(TypedDict):
    MonitoringSubscription: MonitoringSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringSubscriptionTypeDef](./type_defs.md#monitoringsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMonitoringSubscriptionResultTypeDef

```python
# GetMonitoringSubscriptionResultTypeDef definition

class GetMonitoringSubscriptionResultTypeDef(TypedDict):
    MonitoringSubscription: MonitoringSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringSubscriptionTypeDef](./type_defs.md#monitoringsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOriginAccessControlsResultTypeDef

```python
# ListOriginAccessControlsResultTypeDef definition

class ListOriginAccessControlsResultTypeDef(TypedDict):
    OriginAccessControlList: OriginAccessControlListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginAccessControlListTypeDef](./type_defs.md#originaccesscontrollisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OriginGroupTypeDef

```python
# OriginGroupTypeDef definition

class OriginGroupTypeDef(TypedDict):
    Id: str,
    FailoverCriteria: OriginGroupFailoverCriteriaTypeDef,  # (1)
    Members: OriginGroupMembersTypeDef,  # (2)
```

1. See [:material-code-braces: OriginGroupFailoverCriteriaTypeDef](./type_defs.md#origingroupfailovercriteriatypedef) 
2. See [:material-code-braces: OriginGroupMembersTypeDef](./type_defs.md#origingroupmemberstypedef) 
## ListPublicKeysResultTypeDef

```python
# ListPublicKeysResultTypeDef definition

class ListPublicKeysResultTypeDef(TypedDict):
    PublicKeyList: PublicKeyListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyListTypeDef](./type_defs.md#publickeylisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryArgProfileConfigTypeDef

```python
# QueryArgProfileConfigTypeDef definition

class QueryArgProfileConfigTypeDef(TypedDict):
    ForwardWhenQueryArgProfileIsUnknown: bool,
    QueryArgProfiles: NotRequired[QueryArgProfilesTypeDef],  # (1)
```

1. See [:material-code-braces: QueryArgProfilesTypeDef](./type_defs.md#queryargprofilestypedef) 
## ResponseHeadersPolicyConfigTypeDef

```python
# ResponseHeadersPolicyConfigTypeDef definition

class ResponseHeadersPolicyConfigTypeDef(TypedDict):
    Name: str,
    Comment: NotRequired[str],
    CorsConfig: NotRequired[ResponseHeadersPolicyCorsConfigTypeDef],  # (1)
    SecurityHeadersConfig: NotRequired[ResponseHeadersPolicySecurityHeadersConfigTypeDef],  # (2)
    ServerTimingHeadersConfig: NotRequired[ResponseHeadersPolicyServerTimingHeadersConfigTypeDef],  # (3)
    CustomHeadersConfig: NotRequired[ResponseHeadersPolicyCustomHeadersConfigTypeDef],  # (4)
    RemoveHeadersConfig: NotRequired[ResponseHeadersPolicyRemoveHeadersConfigTypeDef],  # (5)
```

1. See [:material-code-braces: ResponseHeadersPolicyCorsConfigTypeDef](./type_defs.md#responseheaderspolicycorsconfigtypedef) 
2. See [:material-code-braces: ResponseHeadersPolicySecurityHeadersConfigTypeDef](./type_defs.md#responseheaderspolicysecurityheadersconfigtypedef) 
3. See [:material-code-braces: ResponseHeadersPolicyServerTimingHeadersConfigTypeDef](./type_defs.md#responseheaderspolicyservertimingheadersconfigtypedef) 
4. See [:material-code-braces: ResponseHeadersPolicyCustomHeadersConfigTypeDef](./type_defs.md#responseheaderspolicycustomheadersconfigtypedef) 
5. See [:material-code-braces: ResponseHeadersPolicyRemoveHeadersConfigTypeDef](./type_defs.md#responseheaderspolicyremoveheadersconfigtypedef) 
## StreamingDistributionListTypeDef

```python
# StreamingDistributionListTypeDef definition

class StreamingDistributionListTypeDef(TypedDict):
    Marker: str,
    MaxItems: int,
    IsTruncated: bool,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[StreamingDistributionSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: StreamingDistributionSummaryTypeDef](./type_defs.md#streamingdistributionsummarytypedef) 
## CreateStreamingDistributionRequestRequestTypeDef

```python
# CreateStreamingDistributionRequestRequestTypeDef definition

class CreateStreamingDistributionRequestRequestTypeDef(TypedDict):
    StreamingDistributionConfig: StreamingDistributionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: StreamingDistributionConfigTypeDef](./type_defs.md#streamingdistributionconfigtypedef) 
## GetStreamingDistributionConfigResultTypeDef

```python
# GetStreamingDistributionConfigResultTypeDef definition

class GetStreamingDistributionConfigResultTypeDef(TypedDict):
    StreamingDistributionConfig: StreamingDistributionConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingDistributionConfigTypeDef](./type_defs.md#streamingdistributionconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStreamingDistributionRequestRequestTypeDef

```python
# UpdateStreamingDistributionRequestRequestTypeDef definition

class UpdateStreamingDistributionRequestRequestTypeDef(TypedDict):
    StreamingDistributionConfig: StreamingDistributionConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: StreamingDistributionConfigTypeDef](./type_defs.md#streamingdistributionconfigtypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    Tags: TagsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagsTypeDef](./type_defs.md#tagstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StreamingDistributionConfigWithTagsTypeDef

```python
# StreamingDistributionConfigWithTagsTypeDef definition

class StreamingDistributionConfigWithTagsTypeDef(TypedDict):
    StreamingDistributionConfig: StreamingDistributionConfigTypeDef,  # (1)
    Tags: TagsTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingDistributionConfigTypeDef](./type_defs.md#streamingdistributionconfigtypedef) 
2. See [:material-code-braces: TagsTypeDef](./type_defs.md#tagstypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    Resource: str,
    Tags: TagsTypeDef,  # (1)
```

1. See [:material-code-braces: TagsTypeDef](./type_defs.md#tagstypedef) 
## CacheBehaviorTypeDef

```python
# CacheBehaviorTypeDef definition

class CacheBehaviorTypeDef(TypedDict):
    PathPattern: str,
    TargetOriginId: str,
    ViewerProtocolPolicy: ViewerProtocolPolicyType,  # (3)
    TrustedSigners: NotRequired[TrustedSignersTypeDef],  # (1)
    TrustedKeyGroups: NotRequired[TrustedKeyGroupsTypeDef],  # (2)
    AllowedMethods: NotRequired[AllowedMethodsTypeDef],  # (4)
    SmoothStreaming: NotRequired[bool],
    Compress: NotRequired[bool],
    LambdaFunctionAssociations: NotRequired[LambdaFunctionAssociationsTypeDef],  # (5)
    FunctionAssociations: NotRequired[FunctionAssociationsTypeDef],  # (6)
    FieldLevelEncryptionId: NotRequired[str],
    RealtimeLogConfigArn: NotRequired[str],
    CachePolicyId: NotRequired[str],
    OriginRequestPolicyId: NotRequired[str],
    ResponseHeadersPolicyId: NotRequired[str],
    ForwardedValues: NotRequired[ForwardedValuesTypeDef],  # (7)
    MinTTL: NotRequired[int],
    DefaultTTL: NotRequired[int],
    MaxTTL: NotRequired[int],
```

1. See [:material-code-braces: TrustedSignersTypeDef](./type_defs.md#trustedsignerstypedef) 
2. See [:material-code-braces: TrustedKeyGroupsTypeDef](./type_defs.md#trustedkeygroupstypedef) 
3. See [:material-code-brackets: ViewerProtocolPolicyType](./literals.md#viewerprotocolpolicytype) 
4. See [:material-code-braces: AllowedMethodsTypeDef](./type_defs.md#allowedmethodstypedef) 
5. See [:material-code-braces: LambdaFunctionAssociationsTypeDef](./type_defs.md#lambdafunctionassociationstypedef) 
6. See [:material-code-braces: FunctionAssociationsTypeDef](./type_defs.md#functionassociationstypedef) 
7. See [:material-code-braces: ForwardedValuesTypeDef](./type_defs.md#forwardedvaluestypedef) 
## DefaultCacheBehaviorTypeDef

```python
# DefaultCacheBehaviorTypeDef definition

class DefaultCacheBehaviorTypeDef(TypedDict):
    TargetOriginId: str,
    ViewerProtocolPolicy: ViewerProtocolPolicyType,  # (3)
    TrustedSigners: NotRequired[TrustedSignersTypeDef],  # (1)
    TrustedKeyGroups: NotRequired[TrustedKeyGroupsTypeDef],  # (2)
    AllowedMethods: NotRequired[AllowedMethodsTypeDef],  # (4)
    SmoothStreaming: NotRequired[bool],
    Compress: NotRequired[bool],
    LambdaFunctionAssociations: NotRequired[LambdaFunctionAssociationsTypeDef],  # (5)
    FunctionAssociations: NotRequired[FunctionAssociationsTypeDef],  # (6)
    FieldLevelEncryptionId: NotRequired[str],
    RealtimeLogConfigArn: NotRequired[str],
    CachePolicyId: NotRequired[str],
    OriginRequestPolicyId: NotRequired[str],
    ResponseHeadersPolicyId: NotRequired[str],
    ForwardedValues: NotRequired[ForwardedValuesTypeDef],  # (7)
    MinTTL: NotRequired[int],
    DefaultTTL: NotRequired[int],
    MaxTTL: NotRequired[int],
```

1. See [:material-code-braces: TrustedSignersTypeDef](./type_defs.md#trustedsignerstypedef) 
2. See [:material-code-braces: TrustedKeyGroupsTypeDef](./type_defs.md#trustedkeygroupstypedef) 
3. See [:material-code-brackets: ViewerProtocolPolicyType](./literals.md#viewerprotocolpolicytype) 
4. See [:material-code-braces: AllowedMethodsTypeDef](./type_defs.md#allowedmethodstypedef) 
5. See [:material-code-braces: LambdaFunctionAssociationsTypeDef](./type_defs.md#lambdafunctionassociationstypedef) 
6. See [:material-code-braces: FunctionAssociationsTypeDef](./type_defs.md#functionassociationstypedef) 
7. See [:material-code-braces: ForwardedValuesTypeDef](./type_defs.md#forwardedvaluestypedef) 
## CachePolicyConfigTypeDef

```python
# CachePolicyConfigTypeDef definition

class CachePolicyConfigTypeDef(TypedDict):
    Name: str,
    MinTTL: int,
    Comment: NotRequired[str],
    DefaultTTL: NotRequired[int],
    MaxTTL: NotRequired[int],
    ParametersInCacheKeyAndForwardedToOrigin: NotRequired[ParametersInCacheKeyAndForwardedToOriginTypeDef],  # (1)
```

1. See [:material-code-braces: ParametersInCacheKeyAndForwardedToOriginTypeDef](./type_defs.md#parametersincachekeyandforwardedtoorigintypedef) 
## CreateOriginRequestPolicyRequestRequestTypeDef

```python
# CreateOriginRequestPolicyRequestRequestTypeDef definition

class CreateOriginRequestPolicyRequestRequestTypeDef(TypedDict):
    OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: OriginRequestPolicyConfigTypeDef](./type_defs.md#originrequestpolicyconfigtypedef) 
## GetOriginRequestPolicyConfigResultTypeDef

```python
# GetOriginRequestPolicyConfigResultTypeDef definition

class GetOriginRequestPolicyConfigResultTypeDef(TypedDict):
    OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginRequestPolicyConfigTypeDef](./type_defs.md#originrequestpolicyconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OriginRequestPolicyTypeDef

```python
# OriginRequestPolicyTypeDef definition

class OriginRequestPolicyTypeDef(TypedDict):
    Id: str,
    LastModifiedTime: datetime,
    OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: OriginRequestPolicyConfigTypeDef](./type_defs.md#originrequestpolicyconfigtypedef) 
## UpdateOriginRequestPolicyRequestRequestTypeDef

```python
# UpdateOriginRequestPolicyRequestRequestTypeDef definition

class UpdateOriginRequestPolicyRequestRequestTypeDef(TypedDict):
    OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: OriginRequestPolicyConfigTypeDef](./type_defs.md#originrequestpolicyconfigtypedef) 
## ContinuousDeploymentPolicyConfigTypeDef

```python
# ContinuousDeploymentPolicyConfigTypeDef definition

class ContinuousDeploymentPolicyConfigTypeDef(TypedDict):
    StagingDistributionDnsNames: StagingDistributionDnsNamesTypeDef,  # (1)
    Enabled: bool,
    TrafficConfig: NotRequired[TrafficConfigTypeDef],  # (2)
```

1. See [:material-code-braces: StagingDistributionDnsNamesTypeDef](./type_defs.md#stagingdistributiondnsnamestypedef) 
2. See [:material-code-braces: TrafficConfigTypeDef](./type_defs.md#trafficconfigtypedef) 
## KeyGroupListTypeDef

```python
# KeyGroupListTypeDef definition

class KeyGroupListTypeDef(TypedDict):
    MaxItems: int,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[KeyGroupSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: KeyGroupSummaryTypeDef](./type_defs.md#keygroupsummarytypedef) 
## OriginsTypeDef

```python
# OriginsTypeDef definition

class OriginsTypeDef(TypedDict):
    Quantity: int,
    Items: List[OriginTypeDef],  # (1)
```

1. See [:material-code-braces: OriginTypeDef](./type_defs.md#origintypedef) 
## FieldLevelEncryptionProfileConfigTypeDef

```python
# FieldLevelEncryptionProfileConfigTypeDef definition

class FieldLevelEncryptionProfileConfigTypeDef(TypedDict):
    Name: str,
    CallerReference: str,
    EncryptionEntities: EncryptionEntitiesTypeDef,  # (1)
    Comment: NotRequired[str],
```

1. See [:material-code-braces: EncryptionEntitiesTypeDef](./type_defs.md#encryptionentitiestypedef) 
## FieldLevelEncryptionProfileSummaryTypeDef

```python
# FieldLevelEncryptionProfileSummaryTypeDef definition

class FieldLevelEncryptionProfileSummaryTypeDef(TypedDict):
    Id: str,
    LastModifiedTime: datetime,
    Name: str,
    EncryptionEntities: EncryptionEntitiesTypeDef,  # (1)
    Comment: NotRequired[str],
```

1. See [:material-code-braces: EncryptionEntitiesTypeDef](./type_defs.md#encryptionentitiestypedef) 
## CreateRealtimeLogConfigResultTypeDef

```python
# CreateRealtimeLogConfigResultTypeDef definition

class CreateRealtimeLogConfigResultTypeDef(TypedDict):
    RealtimeLogConfig: RealtimeLogConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RealtimeLogConfigTypeDef](./type_defs.md#realtimelogconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRealtimeLogConfigResultTypeDef

```python
# GetRealtimeLogConfigResultTypeDef definition

class GetRealtimeLogConfigResultTypeDef(TypedDict):
    RealtimeLogConfig: RealtimeLogConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RealtimeLogConfigTypeDef](./type_defs.md#realtimelogconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RealtimeLogConfigsTypeDef

```python
# RealtimeLogConfigsTypeDef definition

class RealtimeLogConfigsTypeDef(TypedDict):
    MaxItems: int,
    IsTruncated: bool,
    Marker: str,
    Items: NotRequired[List[RealtimeLogConfigTypeDef]],  # (1)
    NextMarker: NotRequired[str],
```

1. See [:material-code-braces: RealtimeLogConfigTypeDef](./type_defs.md#realtimelogconfigtypedef) 
## UpdateRealtimeLogConfigResultTypeDef

```python
# UpdateRealtimeLogConfigResultTypeDef definition

class UpdateRealtimeLogConfigResultTypeDef(TypedDict):
    RealtimeLogConfig: RealtimeLogConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RealtimeLogConfigTypeDef](./type_defs.md#realtimelogconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFunctionsResultTypeDef

```python
# ListFunctionsResultTypeDef definition

class ListFunctionsResultTypeDef(TypedDict):
    FunctionList: FunctionListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FunctionListTypeDef](./type_defs.md#functionlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestFunctionResultTypeDef

```python
# TestFunctionResultTypeDef definition

class TestFunctionResultTypeDef(TypedDict):
    TestResult: TestResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestResultTypeDef](./type_defs.md#testresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInvalidationResultTypeDef

```python
# CreateInvalidationResultTypeDef definition

class CreateInvalidationResultTypeDef(TypedDict):
    Location: str,
    Invalidation: InvalidationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvalidationTypeDef](./type_defs.md#invalidationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInvalidationResultTypeDef

```python
# GetInvalidationResultTypeDef definition

class GetInvalidationResultTypeDef(TypedDict):
    Invalidation: InvalidationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvalidationTypeDef](./type_defs.md#invalidationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StreamingDistributionTypeDef

```python
# StreamingDistributionTypeDef definition

class StreamingDistributionTypeDef(TypedDict):
    Id: str,
    ARN: str,
    Status: str,
    DomainName: str,
    ActiveTrustedSigners: ActiveTrustedSignersTypeDef,  # (1)
    StreamingDistributionConfig: StreamingDistributionConfigTypeDef,  # (2)
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-braces: ActiveTrustedSignersTypeDef](./type_defs.md#activetrustedsignerstypedef) 
2. See [:material-code-braces: StreamingDistributionConfigTypeDef](./type_defs.md#streamingdistributionconfigtypedef) 
## OriginGroupsTypeDef

```python
# OriginGroupsTypeDef definition

class OriginGroupsTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[OriginGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: OriginGroupTypeDef](./type_defs.md#origingrouptypedef) 
## FieldLevelEncryptionConfigTypeDef

```python
# FieldLevelEncryptionConfigTypeDef definition

class FieldLevelEncryptionConfigTypeDef(TypedDict):
    CallerReference: str,
    Comment: NotRequired[str],
    QueryArgProfileConfig: NotRequired[QueryArgProfileConfigTypeDef],  # (1)
    ContentTypeProfileConfig: NotRequired[ContentTypeProfileConfigTypeDef],  # (2)
```

1. See [:material-code-braces: QueryArgProfileConfigTypeDef](./type_defs.md#queryargprofileconfigtypedef) 
2. See [:material-code-braces: ContentTypeProfileConfigTypeDef](./type_defs.md#contenttypeprofileconfigtypedef) 
## FieldLevelEncryptionSummaryTypeDef

```python
# FieldLevelEncryptionSummaryTypeDef definition

class FieldLevelEncryptionSummaryTypeDef(TypedDict):
    Id: str,
    LastModifiedTime: datetime,
    Comment: NotRequired[str],
    QueryArgProfileConfig: NotRequired[QueryArgProfileConfigTypeDef],  # (1)
    ContentTypeProfileConfig: NotRequired[ContentTypeProfileConfigTypeDef],  # (2)
```

1. See [:material-code-braces: QueryArgProfileConfigTypeDef](./type_defs.md#queryargprofileconfigtypedef) 
2. See [:material-code-braces: ContentTypeProfileConfigTypeDef](./type_defs.md#contenttypeprofileconfigtypedef) 
## CreateResponseHeadersPolicyRequestRequestTypeDef

```python
# CreateResponseHeadersPolicyRequestRequestTypeDef definition

class CreateResponseHeadersPolicyRequestRequestTypeDef(TypedDict):
    ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseHeadersPolicyConfigTypeDef](./type_defs.md#responseheaderspolicyconfigtypedef) 
## GetResponseHeadersPolicyConfigResultTypeDef

```python
# GetResponseHeadersPolicyConfigResultTypeDef definition

class GetResponseHeadersPolicyConfigResultTypeDef(TypedDict):
    ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseHeadersPolicyConfigTypeDef](./type_defs.md#responseheaderspolicyconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResponseHeadersPolicyTypeDef

```python
# ResponseHeadersPolicyTypeDef definition

class ResponseHeadersPolicyTypeDef(TypedDict):
    Id: str,
    LastModifiedTime: datetime,
    ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseHeadersPolicyConfigTypeDef](./type_defs.md#responseheaderspolicyconfigtypedef) 
## UpdateResponseHeadersPolicyRequestRequestTypeDef

```python
# UpdateResponseHeadersPolicyRequestRequestTypeDef definition

class UpdateResponseHeadersPolicyRequestRequestTypeDef(TypedDict):
    ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: ResponseHeadersPolicyConfigTypeDef](./type_defs.md#responseheaderspolicyconfigtypedef) 
## ListStreamingDistributionsResultTypeDef

```python
# ListStreamingDistributionsResultTypeDef definition

class ListStreamingDistributionsResultTypeDef(TypedDict):
    StreamingDistributionList: StreamingDistributionListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingDistributionListTypeDef](./type_defs.md#streamingdistributionlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamingDistributionWithTagsRequestRequestTypeDef

```python
# CreateStreamingDistributionWithTagsRequestRequestTypeDef definition

class CreateStreamingDistributionWithTagsRequestRequestTypeDef(TypedDict):
    StreamingDistributionConfigWithTags: StreamingDistributionConfigWithTagsTypeDef,  # (1)
```

1. See [:material-code-braces: StreamingDistributionConfigWithTagsTypeDef](./type_defs.md#streamingdistributionconfigwithtagstypedef) 
## CacheBehaviorsTypeDef

```python
# CacheBehaviorsTypeDef definition

class CacheBehaviorsTypeDef(TypedDict):
    Quantity: int,
    Items: NotRequired[List[CacheBehaviorTypeDef]],  # (1)
```

1. See [:material-code-braces: CacheBehaviorTypeDef](./type_defs.md#cachebehaviortypedef) 
## CachePolicyTypeDef

```python
# CachePolicyTypeDef definition

class CachePolicyTypeDef(TypedDict):
    Id: str,
    LastModifiedTime: datetime,
    CachePolicyConfig: CachePolicyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: CachePolicyConfigTypeDef](./type_defs.md#cachepolicyconfigtypedef) 
## CreateCachePolicyRequestRequestTypeDef

```python
# CreateCachePolicyRequestRequestTypeDef definition

class CreateCachePolicyRequestRequestTypeDef(TypedDict):
    CachePolicyConfig: CachePolicyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: CachePolicyConfigTypeDef](./type_defs.md#cachepolicyconfigtypedef) 
## GetCachePolicyConfigResultTypeDef

```python
# GetCachePolicyConfigResultTypeDef definition

class GetCachePolicyConfigResultTypeDef(TypedDict):
    CachePolicyConfig: CachePolicyConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CachePolicyConfigTypeDef](./type_defs.md#cachepolicyconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCachePolicyRequestRequestTypeDef

```python
# UpdateCachePolicyRequestRequestTypeDef definition

class UpdateCachePolicyRequestRequestTypeDef(TypedDict):
    CachePolicyConfig: CachePolicyConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: CachePolicyConfigTypeDef](./type_defs.md#cachepolicyconfigtypedef) 
## CreateOriginRequestPolicyResultTypeDef

```python
# CreateOriginRequestPolicyResultTypeDef definition

class CreateOriginRequestPolicyResultTypeDef(TypedDict):
    OriginRequestPolicy: OriginRequestPolicyTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginRequestPolicyTypeDef](./type_defs.md#originrequestpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOriginRequestPolicyResultTypeDef

```python
# GetOriginRequestPolicyResultTypeDef definition

class GetOriginRequestPolicyResultTypeDef(TypedDict):
    OriginRequestPolicy: OriginRequestPolicyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginRequestPolicyTypeDef](./type_defs.md#originrequestpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OriginRequestPolicySummaryTypeDef

```python
# OriginRequestPolicySummaryTypeDef definition

class OriginRequestPolicySummaryTypeDef(TypedDict):
    Type: OriginRequestPolicyTypeType,  # (1)
    OriginRequestPolicy: OriginRequestPolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: OriginRequestPolicyTypeType](./literals.md#originrequestpolicytypetype) 
2. See [:material-code-braces: OriginRequestPolicyTypeDef](./type_defs.md#originrequestpolicytypedef) 
## UpdateOriginRequestPolicyResultTypeDef

```python
# UpdateOriginRequestPolicyResultTypeDef definition

class UpdateOriginRequestPolicyResultTypeDef(TypedDict):
    OriginRequestPolicy: OriginRequestPolicyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginRequestPolicyTypeDef](./type_defs.md#originrequestpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContinuousDeploymentPolicyTypeDef

```python
# ContinuousDeploymentPolicyTypeDef definition

class ContinuousDeploymentPolicyTypeDef(TypedDict):
    Id: str,
    LastModifiedTime: datetime,
    ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ContinuousDeploymentPolicyConfigTypeDef](./type_defs.md#continuousdeploymentpolicyconfigtypedef) 
## CreateContinuousDeploymentPolicyRequestRequestTypeDef

```python
# CreateContinuousDeploymentPolicyRequestRequestTypeDef definition

class CreateContinuousDeploymentPolicyRequestRequestTypeDef(TypedDict):
    ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ContinuousDeploymentPolicyConfigTypeDef](./type_defs.md#continuousdeploymentpolicyconfigtypedef) 
## GetContinuousDeploymentPolicyConfigResultTypeDef

```python
# GetContinuousDeploymentPolicyConfigResultTypeDef definition

class GetContinuousDeploymentPolicyConfigResultTypeDef(TypedDict):
    ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousDeploymentPolicyConfigTypeDef](./type_defs.md#continuousdeploymentpolicyconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContinuousDeploymentPolicyRequestRequestTypeDef

```python
# UpdateContinuousDeploymentPolicyRequestRequestTypeDef definition

class UpdateContinuousDeploymentPolicyRequestRequestTypeDef(TypedDict):
    ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: ContinuousDeploymentPolicyConfigTypeDef](./type_defs.md#continuousdeploymentpolicyconfigtypedef) 
## ListKeyGroupsResultTypeDef

```python
# ListKeyGroupsResultTypeDef definition

class ListKeyGroupsResultTypeDef(TypedDict):
    KeyGroupList: KeyGroupListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyGroupListTypeDef](./type_defs.md#keygrouplisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFieldLevelEncryptionProfileRequestRequestTypeDef

```python
# CreateFieldLevelEncryptionProfileRequestRequestTypeDef definition

class CreateFieldLevelEncryptionProfileRequestRequestTypeDef(TypedDict):
    FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,  # (1)
```

1. See [:material-code-braces: FieldLevelEncryptionProfileConfigTypeDef](./type_defs.md#fieldlevelencryptionprofileconfigtypedef) 
## FieldLevelEncryptionProfileTypeDef

```python
# FieldLevelEncryptionProfileTypeDef definition

class FieldLevelEncryptionProfileTypeDef(TypedDict):
    Id: str,
    LastModifiedTime: datetime,
    FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,  # (1)
```

1. See [:material-code-braces: FieldLevelEncryptionProfileConfigTypeDef](./type_defs.md#fieldlevelencryptionprofileconfigtypedef) 
## GetFieldLevelEncryptionProfileConfigResultTypeDef

```python
# GetFieldLevelEncryptionProfileConfigResultTypeDef definition

class GetFieldLevelEncryptionProfileConfigResultTypeDef(TypedDict):
    FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionProfileConfigTypeDef](./type_defs.md#fieldlevelencryptionprofileconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFieldLevelEncryptionProfileRequestRequestTypeDef

```python
# UpdateFieldLevelEncryptionProfileRequestRequestTypeDef definition

class UpdateFieldLevelEncryptionProfileRequestRequestTypeDef(TypedDict):
    FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: FieldLevelEncryptionProfileConfigTypeDef](./type_defs.md#fieldlevelencryptionprofileconfigtypedef) 
## FieldLevelEncryptionProfileListTypeDef

```python
# FieldLevelEncryptionProfileListTypeDef definition

class FieldLevelEncryptionProfileListTypeDef(TypedDict):
    MaxItems: int,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[FieldLevelEncryptionProfileSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldLevelEncryptionProfileSummaryTypeDef](./type_defs.md#fieldlevelencryptionprofilesummarytypedef) 
## ListRealtimeLogConfigsResultTypeDef

```python
# ListRealtimeLogConfigsResultTypeDef definition

class ListRealtimeLogConfigsResultTypeDef(TypedDict):
    RealtimeLogConfigs: RealtimeLogConfigsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RealtimeLogConfigsTypeDef](./type_defs.md#realtimelogconfigstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamingDistributionResultTypeDef

```python
# CreateStreamingDistributionResultTypeDef definition

class CreateStreamingDistributionResultTypeDef(TypedDict):
    StreamingDistribution: StreamingDistributionTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingDistributionTypeDef](./type_defs.md#streamingdistributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamingDistributionWithTagsResultTypeDef

```python
# CreateStreamingDistributionWithTagsResultTypeDef definition

class CreateStreamingDistributionWithTagsResultTypeDef(TypedDict):
    StreamingDistribution: StreamingDistributionTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingDistributionTypeDef](./type_defs.md#streamingdistributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStreamingDistributionResultTypeDef

```python
# GetStreamingDistributionResultTypeDef definition

class GetStreamingDistributionResultTypeDef(TypedDict):
    StreamingDistribution: StreamingDistributionTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingDistributionTypeDef](./type_defs.md#streamingdistributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStreamingDistributionResultTypeDef

```python
# UpdateStreamingDistributionResultTypeDef definition

class UpdateStreamingDistributionResultTypeDef(TypedDict):
    StreamingDistribution: StreamingDistributionTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamingDistributionTypeDef](./type_defs.md#streamingdistributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFieldLevelEncryptionConfigRequestRequestTypeDef

```python
# CreateFieldLevelEncryptionConfigRequestRequestTypeDef definition

class CreateFieldLevelEncryptionConfigRequestRequestTypeDef(TypedDict):
    FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: FieldLevelEncryptionConfigTypeDef](./type_defs.md#fieldlevelencryptionconfigtypedef) 
## FieldLevelEncryptionTypeDef

```python
# FieldLevelEncryptionTypeDef definition

class FieldLevelEncryptionTypeDef(TypedDict):
    Id: str,
    LastModifiedTime: datetime,
    FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: FieldLevelEncryptionConfigTypeDef](./type_defs.md#fieldlevelencryptionconfigtypedef) 
## GetFieldLevelEncryptionConfigResultTypeDef

```python
# GetFieldLevelEncryptionConfigResultTypeDef definition

class GetFieldLevelEncryptionConfigResultTypeDef(TypedDict):
    FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionConfigTypeDef](./type_defs.md#fieldlevelencryptionconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFieldLevelEncryptionConfigRequestRequestTypeDef

```python
# UpdateFieldLevelEncryptionConfigRequestRequestTypeDef definition

class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(TypedDict):
    FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: FieldLevelEncryptionConfigTypeDef](./type_defs.md#fieldlevelencryptionconfigtypedef) 
## FieldLevelEncryptionListTypeDef

```python
# FieldLevelEncryptionListTypeDef definition

class FieldLevelEncryptionListTypeDef(TypedDict):
    MaxItems: int,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[FieldLevelEncryptionSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldLevelEncryptionSummaryTypeDef](./type_defs.md#fieldlevelencryptionsummarytypedef) 
## CreateResponseHeadersPolicyResultTypeDef

```python
# CreateResponseHeadersPolicyResultTypeDef definition

class CreateResponseHeadersPolicyResultTypeDef(TypedDict):
    ResponseHeadersPolicy: ResponseHeadersPolicyTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseHeadersPolicyTypeDef](./type_defs.md#responseheaderspolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResponseHeadersPolicyResultTypeDef

```python
# GetResponseHeadersPolicyResultTypeDef definition

class GetResponseHeadersPolicyResultTypeDef(TypedDict):
    ResponseHeadersPolicy: ResponseHeadersPolicyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseHeadersPolicyTypeDef](./type_defs.md#responseheaderspolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResponseHeadersPolicySummaryTypeDef

```python
# ResponseHeadersPolicySummaryTypeDef definition

class ResponseHeadersPolicySummaryTypeDef(TypedDict):
    Type: ResponseHeadersPolicyTypeType,  # (1)
    ResponseHeadersPolicy: ResponseHeadersPolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: ResponseHeadersPolicyTypeType](./literals.md#responseheaderspolicytypetype) 
2. See [:material-code-braces: ResponseHeadersPolicyTypeDef](./type_defs.md#responseheaderspolicytypedef) 
## UpdateResponseHeadersPolicyResultTypeDef

```python
# UpdateResponseHeadersPolicyResultTypeDef definition

class UpdateResponseHeadersPolicyResultTypeDef(TypedDict):
    ResponseHeadersPolicy: ResponseHeadersPolicyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseHeadersPolicyTypeDef](./type_defs.md#responseheaderspolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DistributionConfigTypeDef

```python
# DistributionConfigTypeDef definition

class DistributionConfigTypeDef(TypedDict):
    CallerReference: str,
    Origins: OriginsTypeDef,  # (2)
    DefaultCacheBehavior: DefaultCacheBehaviorTypeDef,  # (4)
    Comment: str,
    Enabled: bool,
    Aliases: NotRequired[AliasesTypeDef],  # (1)
    DefaultRootObject: NotRequired[str],
    OriginGroups: NotRequired[OriginGroupsTypeDef],  # (3)
    CacheBehaviors: NotRequired[CacheBehaviorsTypeDef],  # (5)
    CustomErrorResponses: NotRequired[CustomErrorResponsesTypeDef],  # (6)
    Logging: NotRequired[LoggingConfigTypeDef],  # (7)
    PriceClass: NotRequired[PriceClassType],  # (8)
    ViewerCertificate: NotRequired[ViewerCertificateTypeDef],  # (9)
    Restrictions: NotRequired[RestrictionsTypeDef],  # (10)
    WebACLId: NotRequired[str],
    HttpVersion: NotRequired[HttpVersionType],  # (11)
    IsIPV6Enabled: NotRequired[bool],
    ContinuousDeploymentPolicyId: NotRequired[str],
    Staging: NotRequired[bool],
```

1. See [:material-code-braces: AliasesTypeDef](./type_defs.md#aliasestypedef) 
2. See [:material-code-braces: OriginsTypeDef](./type_defs.md#originstypedef) 
3. See [:material-code-braces: OriginGroupsTypeDef](./type_defs.md#origingroupstypedef) 
4. See [:material-code-braces: DefaultCacheBehaviorTypeDef](./type_defs.md#defaultcachebehaviortypedef) 
5. See [:material-code-braces: CacheBehaviorsTypeDef](./type_defs.md#cachebehaviorstypedef) 
6. See [:material-code-braces: CustomErrorResponsesTypeDef](./type_defs.md#customerrorresponsestypedef) 
7. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
8. See [:material-code-brackets: PriceClassType](./literals.md#priceclasstype) 
9. See [:material-code-braces: ViewerCertificateTypeDef](./type_defs.md#viewercertificatetypedef) 
10. See [:material-code-braces: RestrictionsTypeDef](./type_defs.md#restrictionstypedef) 
11. See [:material-code-brackets: HttpVersionType](./literals.md#httpversiontype) 
## DistributionSummaryTypeDef

```python
# DistributionSummaryTypeDef definition

class DistributionSummaryTypeDef(TypedDict):
    Id: str,
    ARN: str,
    Status: str,
    LastModifiedTime: datetime,
    DomainName: str,
    Aliases: AliasesTypeDef,  # (1)
    Origins: OriginsTypeDef,  # (2)
    DefaultCacheBehavior: DefaultCacheBehaviorTypeDef,  # (4)
    CacheBehaviors: CacheBehaviorsTypeDef,  # (5)
    CustomErrorResponses: CustomErrorResponsesTypeDef,  # (6)
    Comment: str,
    PriceClass: PriceClassType,  # (7)
    Enabled: bool,
    ViewerCertificate: ViewerCertificateTypeDef,  # (8)
    Restrictions: RestrictionsTypeDef,  # (9)
    WebACLId: str,
    HttpVersion: HttpVersionType,  # (10)
    IsIPV6Enabled: bool,
    Staging: bool,
    OriginGroups: NotRequired[OriginGroupsTypeDef],  # (3)
    AliasICPRecordals: NotRequired[List[AliasICPRecordalTypeDef]],  # (11)
```

1. See [:material-code-braces: AliasesTypeDef](./type_defs.md#aliasestypedef) 
2. See [:material-code-braces: OriginsTypeDef](./type_defs.md#originstypedef) 
3. See [:material-code-braces: OriginGroupsTypeDef](./type_defs.md#origingroupstypedef) 
4. See [:material-code-braces: DefaultCacheBehaviorTypeDef](./type_defs.md#defaultcachebehaviortypedef) 
5. See [:material-code-braces: CacheBehaviorsTypeDef](./type_defs.md#cachebehaviorstypedef) 
6. See [:material-code-braces: CustomErrorResponsesTypeDef](./type_defs.md#customerrorresponsestypedef) 
7. See [:material-code-brackets: PriceClassType](./literals.md#priceclasstype) 
8. See [:material-code-braces: ViewerCertificateTypeDef](./type_defs.md#viewercertificatetypedef) 
9. See [:material-code-braces: RestrictionsTypeDef](./type_defs.md#restrictionstypedef) 
10. See [:material-code-brackets: HttpVersionType](./literals.md#httpversiontype) 
11. See [:material-code-braces: AliasICPRecordalTypeDef](./type_defs.md#aliasicprecordaltypedef) 
## CachePolicySummaryTypeDef

```python
# CachePolicySummaryTypeDef definition

class CachePolicySummaryTypeDef(TypedDict):
    Type: CachePolicyTypeType,  # (1)
    CachePolicy: CachePolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: CachePolicyTypeType](./literals.md#cachepolicytypetype) 
2. See [:material-code-braces: CachePolicyTypeDef](./type_defs.md#cachepolicytypedef) 
## CreateCachePolicyResultTypeDef

```python
# CreateCachePolicyResultTypeDef definition

class CreateCachePolicyResultTypeDef(TypedDict):
    CachePolicy: CachePolicyTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CachePolicyTypeDef](./type_defs.md#cachepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCachePolicyResultTypeDef

```python
# GetCachePolicyResultTypeDef definition

class GetCachePolicyResultTypeDef(TypedDict):
    CachePolicy: CachePolicyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CachePolicyTypeDef](./type_defs.md#cachepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCachePolicyResultTypeDef

```python
# UpdateCachePolicyResultTypeDef definition

class UpdateCachePolicyResultTypeDef(TypedDict):
    CachePolicy: CachePolicyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CachePolicyTypeDef](./type_defs.md#cachepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OriginRequestPolicyListTypeDef

```python
# OriginRequestPolicyListTypeDef definition

class OriginRequestPolicyListTypeDef(TypedDict):
    MaxItems: int,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[OriginRequestPolicySummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: OriginRequestPolicySummaryTypeDef](./type_defs.md#originrequestpolicysummarytypedef) 
## ContinuousDeploymentPolicySummaryTypeDef

```python
# ContinuousDeploymentPolicySummaryTypeDef definition

class ContinuousDeploymentPolicySummaryTypeDef(TypedDict):
    ContinuousDeploymentPolicy: ContinuousDeploymentPolicyTypeDef,  # (1)
```

1. See [:material-code-braces: ContinuousDeploymentPolicyTypeDef](./type_defs.md#continuousdeploymentpolicytypedef) 
## CreateContinuousDeploymentPolicyResultTypeDef

```python
# CreateContinuousDeploymentPolicyResultTypeDef definition

class CreateContinuousDeploymentPolicyResultTypeDef(TypedDict):
    ContinuousDeploymentPolicy: ContinuousDeploymentPolicyTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousDeploymentPolicyTypeDef](./type_defs.md#continuousdeploymentpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContinuousDeploymentPolicyResultTypeDef

```python
# GetContinuousDeploymentPolicyResultTypeDef definition

class GetContinuousDeploymentPolicyResultTypeDef(TypedDict):
    ContinuousDeploymentPolicy: ContinuousDeploymentPolicyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousDeploymentPolicyTypeDef](./type_defs.md#continuousdeploymentpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContinuousDeploymentPolicyResultTypeDef

```python
# UpdateContinuousDeploymentPolicyResultTypeDef definition

class UpdateContinuousDeploymentPolicyResultTypeDef(TypedDict):
    ContinuousDeploymentPolicy: ContinuousDeploymentPolicyTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousDeploymentPolicyTypeDef](./type_defs.md#continuousdeploymentpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFieldLevelEncryptionProfileResultTypeDef

```python
# CreateFieldLevelEncryptionProfileResultTypeDef definition

class CreateFieldLevelEncryptionProfileResultTypeDef(TypedDict):
    FieldLevelEncryptionProfile: FieldLevelEncryptionProfileTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionProfileTypeDef](./type_defs.md#fieldlevelencryptionprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFieldLevelEncryptionProfileResultTypeDef

```python
# GetFieldLevelEncryptionProfileResultTypeDef definition

class GetFieldLevelEncryptionProfileResultTypeDef(TypedDict):
    FieldLevelEncryptionProfile: FieldLevelEncryptionProfileTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionProfileTypeDef](./type_defs.md#fieldlevelencryptionprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFieldLevelEncryptionProfileResultTypeDef

```python
# UpdateFieldLevelEncryptionProfileResultTypeDef definition

class UpdateFieldLevelEncryptionProfileResultTypeDef(TypedDict):
    FieldLevelEncryptionProfile: FieldLevelEncryptionProfileTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionProfileTypeDef](./type_defs.md#fieldlevelencryptionprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFieldLevelEncryptionProfilesResultTypeDef

```python
# ListFieldLevelEncryptionProfilesResultTypeDef definition

class ListFieldLevelEncryptionProfilesResultTypeDef(TypedDict):
    FieldLevelEncryptionProfileList: FieldLevelEncryptionProfileListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionProfileListTypeDef](./type_defs.md#fieldlevelencryptionprofilelisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFieldLevelEncryptionConfigResultTypeDef

```python
# CreateFieldLevelEncryptionConfigResultTypeDef definition

class CreateFieldLevelEncryptionConfigResultTypeDef(TypedDict):
    FieldLevelEncryption: FieldLevelEncryptionTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionTypeDef](./type_defs.md#fieldlevelencryptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFieldLevelEncryptionResultTypeDef

```python
# GetFieldLevelEncryptionResultTypeDef definition

class GetFieldLevelEncryptionResultTypeDef(TypedDict):
    FieldLevelEncryption: FieldLevelEncryptionTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionTypeDef](./type_defs.md#fieldlevelencryptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFieldLevelEncryptionConfigResultTypeDef

```python
# UpdateFieldLevelEncryptionConfigResultTypeDef definition

class UpdateFieldLevelEncryptionConfigResultTypeDef(TypedDict):
    FieldLevelEncryption: FieldLevelEncryptionTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionTypeDef](./type_defs.md#fieldlevelencryptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFieldLevelEncryptionConfigsResultTypeDef

```python
# ListFieldLevelEncryptionConfigsResultTypeDef definition

class ListFieldLevelEncryptionConfigsResultTypeDef(TypedDict):
    FieldLevelEncryptionList: FieldLevelEncryptionListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldLevelEncryptionListTypeDef](./type_defs.md#fieldlevelencryptionlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResponseHeadersPolicyListTypeDef

```python
# ResponseHeadersPolicyListTypeDef definition

class ResponseHeadersPolicyListTypeDef(TypedDict):
    MaxItems: int,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[ResponseHeadersPolicySummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: ResponseHeadersPolicySummaryTypeDef](./type_defs.md#responseheaderspolicysummarytypedef) 
## CreateDistributionRequestRequestTypeDef

```python
# CreateDistributionRequestRequestTypeDef definition

class CreateDistributionRequestRequestTypeDef(TypedDict):
    DistributionConfig: DistributionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: DistributionConfigTypeDef](./type_defs.md#distributionconfigtypedef) 
## DistributionConfigWithTagsTypeDef

```python
# DistributionConfigWithTagsTypeDef definition

class DistributionConfigWithTagsTypeDef(TypedDict):
    DistributionConfig: DistributionConfigTypeDef,  # (1)
    Tags: TagsTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionConfigTypeDef](./type_defs.md#distributionconfigtypedef) 
2. See [:material-code-braces: TagsTypeDef](./type_defs.md#tagstypedef) 
## DistributionTypeDef

```python
# DistributionTypeDef definition

class DistributionTypeDef(TypedDict):
    Id: str,
    ARN: str,
    Status: str,
    LastModifiedTime: datetime,
    InProgressInvalidationBatches: int,
    DomainName: str,
    DistributionConfig: DistributionConfigTypeDef,  # (3)
    ActiveTrustedSigners: NotRequired[ActiveTrustedSignersTypeDef],  # (1)
    ActiveTrustedKeyGroups: NotRequired[ActiveTrustedKeyGroupsTypeDef],  # (2)
    AliasICPRecordals: NotRequired[List[AliasICPRecordalTypeDef]],  # (4)
```

1. See [:material-code-braces: ActiveTrustedSignersTypeDef](./type_defs.md#activetrustedsignerstypedef) 
2. See [:material-code-braces: ActiveTrustedKeyGroupsTypeDef](./type_defs.md#activetrustedkeygroupstypedef) 
3. See [:material-code-braces: DistributionConfigTypeDef](./type_defs.md#distributionconfigtypedef) 
4. See [:material-code-braces: AliasICPRecordalTypeDef](./type_defs.md#aliasicprecordaltypedef) 
## GetDistributionConfigResultTypeDef

```python
# GetDistributionConfigResultTypeDef definition

class GetDistributionConfigResultTypeDef(TypedDict):
    DistributionConfig: DistributionConfigTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionConfigTypeDef](./type_defs.md#distributionconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDistributionRequestRequestTypeDef

```python
# UpdateDistributionRequestRequestTypeDef definition

class UpdateDistributionRequestRequestTypeDef(TypedDict):
    DistributionConfig: DistributionConfigTypeDef,  # (1)
    Id: str,
    IfMatch: NotRequired[str],
```

1. See [:material-code-braces: DistributionConfigTypeDef](./type_defs.md#distributionconfigtypedef) 
## DistributionListTypeDef

```python
# DistributionListTypeDef definition

class DistributionListTypeDef(TypedDict):
    Marker: str,
    MaxItems: int,
    IsTruncated: bool,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[DistributionSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: DistributionSummaryTypeDef](./type_defs.md#distributionsummarytypedef) 
## CachePolicyListTypeDef

```python
# CachePolicyListTypeDef definition

class CachePolicyListTypeDef(TypedDict):
    MaxItems: int,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[CachePolicySummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: CachePolicySummaryTypeDef](./type_defs.md#cachepolicysummarytypedef) 
## ListOriginRequestPoliciesResultTypeDef

```python
# ListOriginRequestPoliciesResultTypeDef definition

class ListOriginRequestPoliciesResultTypeDef(TypedDict):
    OriginRequestPolicyList: OriginRequestPolicyListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginRequestPolicyListTypeDef](./type_defs.md#originrequestpolicylisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContinuousDeploymentPolicyListTypeDef

```python
# ContinuousDeploymentPolicyListTypeDef definition

class ContinuousDeploymentPolicyListTypeDef(TypedDict):
    MaxItems: int,
    Quantity: int,
    NextMarker: NotRequired[str],
    Items: NotRequired[List[ContinuousDeploymentPolicySummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: ContinuousDeploymentPolicySummaryTypeDef](./type_defs.md#continuousdeploymentpolicysummarytypedef) 
## ListResponseHeadersPoliciesResultTypeDef

```python
# ListResponseHeadersPoliciesResultTypeDef definition

class ListResponseHeadersPoliciesResultTypeDef(TypedDict):
    ResponseHeadersPolicyList: ResponseHeadersPolicyListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseHeadersPolicyListTypeDef](./type_defs.md#responseheaderspolicylisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDistributionWithTagsRequestRequestTypeDef

```python
# CreateDistributionWithTagsRequestRequestTypeDef definition

class CreateDistributionWithTagsRequestRequestTypeDef(TypedDict):
    DistributionConfigWithTags: DistributionConfigWithTagsTypeDef,  # (1)
```

1. See [:material-code-braces: DistributionConfigWithTagsTypeDef](./type_defs.md#distributionconfigwithtagstypedef) 
## CopyDistributionResultTypeDef

```python
# CopyDistributionResultTypeDef definition

class CopyDistributionResultTypeDef(TypedDict):
    Distribution: DistributionTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDistributionResultTypeDef

```python
# CreateDistributionResultTypeDef definition

class CreateDistributionResultTypeDef(TypedDict):
    Distribution: DistributionTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDistributionWithTagsResultTypeDef

```python
# CreateDistributionWithTagsResultTypeDef definition

class CreateDistributionWithTagsResultTypeDef(TypedDict):
    Distribution: DistributionTypeDef,  # (1)
    Location: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDistributionResultTypeDef

```python
# GetDistributionResultTypeDef definition

class GetDistributionResultTypeDef(TypedDict):
    Distribution: DistributionTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDistributionResultTypeDef

```python
# UpdateDistributionResultTypeDef definition

class UpdateDistributionResultTypeDef(TypedDict):
    Distribution: DistributionTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDistributionWithStagingConfigResultTypeDef

```python
# UpdateDistributionWithStagingConfigResultTypeDef definition

class UpdateDistributionWithStagingConfigResultTypeDef(TypedDict):
    Distribution: DistributionTypeDef,  # (1)
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDistributionsByRealtimeLogConfigResultTypeDef

```python
# ListDistributionsByRealtimeLogConfigResultTypeDef definition

class ListDistributionsByRealtimeLogConfigResultTypeDef(TypedDict):
    DistributionList: DistributionListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionListTypeDef](./type_defs.md#distributionlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDistributionsByWebACLIdResultTypeDef

```python
# ListDistributionsByWebACLIdResultTypeDef definition

class ListDistributionsByWebACLIdResultTypeDef(TypedDict):
    DistributionList: DistributionListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionListTypeDef](./type_defs.md#distributionlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDistributionsResultTypeDef

```python
# ListDistributionsResultTypeDef definition

class ListDistributionsResultTypeDef(TypedDict):
    DistributionList: DistributionListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionListTypeDef](./type_defs.md#distributionlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCachePoliciesResultTypeDef

```python
# ListCachePoliciesResultTypeDef definition

class ListCachePoliciesResultTypeDef(TypedDict):
    CachePolicyList: CachePolicyListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CachePolicyListTypeDef](./type_defs.md#cachepolicylisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContinuousDeploymentPoliciesResultTypeDef

```python
# ListContinuousDeploymentPoliciesResultTypeDef definition

class ListContinuousDeploymentPoliciesResultTypeDef(TypedDict):
    ContinuousDeploymentPolicyList: ContinuousDeploymentPolicyListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousDeploymentPolicyListTypeDef](./type_defs.md#continuousdeploymentpolicylisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
