# Type definitions

> [Index](../README.md) > [ElasticLoadBalancingv2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#elasticloadbalancingv2)
    type annotations stubs module [types-aiobotocore-elbv2](https://pypi.org/project/types-aiobotocore-elbv2/).

## AuthenticateCognitoActionConfigUnionTypeDef

```python
# AuthenticateCognitoActionConfigUnionTypeDef definition

AuthenticateCognitoActionConfigUnionTypeDef = Union[
    AuthenticateCognitoActionConfigTypeDef,  # (1)
    AuthenticateCognitoActionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AuthenticateCognitoActionConfigTypeDef](./type_defs.md#authenticatecognitoactionconfigtypedef) 
2. See [:material-code-braces: AuthenticateCognitoActionConfigOutputTypeDef](./type_defs.md#authenticatecognitoactionconfigoutputtypedef) 

## AuthenticateOidcActionConfigUnionTypeDef

```python
# AuthenticateOidcActionConfigUnionTypeDef definition

AuthenticateOidcActionConfigUnionTypeDef = Union[
    AuthenticateOidcActionConfigTypeDef,  # (1)
    AuthenticateOidcActionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AuthenticateOidcActionConfigTypeDef](./type_defs.md#authenticateoidcactionconfigtypedef) 
2. See [:material-code-braces: AuthenticateOidcActionConfigOutputTypeDef](./type_defs.md#authenticateoidcactionconfigoutputtypedef) 

## HostHeaderConditionConfigUnionTypeDef

```python
# HostHeaderConditionConfigUnionTypeDef definition

HostHeaderConditionConfigUnionTypeDef = Union[
    HostHeaderConditionConfigTypeDef,  # (1)
    HostHeaderConditionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HostHeaderConditionConfigTypeDef](./type_defs.md#hostheaderconditionconfigtypedef) 
2. See [:material-code-braces: HostHeaderConditionConfigOutputTypeDef](./type_defs.md#hostheaderconditionconfigoutputtypedef) 

## HttpHeaderConditionConfigUnionTypeDef

```python
# HttpHeaderConditionConfigUnionTypeDef definition

HttpHeaderConditionConfigUnionTypeDef = Union[
    HttpHeaderConditionConfigTypeDef,  # (1)
    HttpHeaderConditionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HttpHeaderConditionConfigTypeDef](./type_defs.md#httpheaderconditionconfigtypedef) 
2. See [:material-code-braces: HttpHeaderConditionConfigOutputTypeDef](./type_defs.md#httpheaderconditionconfigoutputtypedef) 

## HttpRequestMethodConditionConfigUnionTypeDef

```python
# HttpRequestMethodConditionConfigUnionTypeDef definition

HttpRequestMethodConditionConfigUnionTypeDef = Union[
    HttpRequestMethodConditionConfigTypeDef,  # (1)
    HttpRequestMethodConditionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HttpRequestMethodConditionConfigTypeDef](./type_defs.md#httprequestmethodconditionconfigtypedef) 
2. See [:material-code-braces: HttpRequestMethodConditionConfigOutputTypeDef](./type_defs.md#httprequestmethodconditionconfigoutputtypedef) 

## PathPatternConditionConfigUnionTypeDef

```python
# PathPatternConditionConfigUnionTypeDef definition

PathPatternConditionConfigUnionTypeDef = Union[
    PathPatternConditionConfigTypeDef,  # (1)
    PathPatternConditionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PathPatternConditionConfigTypeDef](./type_defs.md#pathpatternconditionconfigtypedef) 
2. See [:material-code-braces: PathPatternConditionConfigOutputTypeDef](./type_defs.md#pathpatternconditionconfigoutputtypedef) 

## SourceIpConditionConfigUnionTypeDef

```python
# SourceIpConditionConfigUnionTypeDef definition

SourceIpConditionConfigUnionTypeDef = Union[
    SourceIpConditionConfigTypeDef,  # (1)
    SourceIpConditionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SourceIpConditionConfigTypeDef](./type_defs.md#sourceipconditionconfigtypedef) 
2. See [:material-code-braces: SourceIpConditionConfigOutputTypeDef](./type_defs.md#sourceipconditionconfigoutputtypedef) 

## ForwardActionConfigUnionTypeDef

```python
# ForwardActionConfigUnionTypeDef definition

ForwardActionConfigUnionTypeDef = Union[
    ForwardActionConfigTypeDef,  # (1)
    ForwardActionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ForwardActionConfigTypeDef](./type_defs.md#forwardactionconfigtypedef) 
2. See [:material-code-braces: ForwardActionConfigOutputTypeDef](./type_defs.md#forwardactionconfigoutputtypedef) 

## QueryStringConditionConfigUnionTypeDef

```python
# QueryStringConditionConfigUnionTypeDef definition

QueryStringConditionConfigUnionTypeDef = Union[
    QueryStringConditionConfigTypeDef,  # (1)
    QueryStringConditionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: QueryStringConditionConfigTypeDef](./type_defs.md#querystringconditionconfigtypedef) 
2. See [:material-code-braces: QueryStringConditionConfigOutputTypeDef](./type_defs.md#querystringconditionconfigoutputtypedef) 

## ActionUnionTypeDef

```python
# ActionUnionTypeDef definition

ActionUnionTypeDef = Union[
    ActionTypeDef,  # (1)
    ActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 

## RuleConditionUnionTypeDef

```python
# RuleConditionUnionTypeDef definition

RuleConditionUnionTypeDef = Union[
    RuleConditionTypeDef,  # (1)
    RuleConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) 
2. See [:material-code-braces: RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef) 



## AuthenticateCognitoActionConfigOutputTypeDef

```python
# AuthenticateCognitoActionConfigOutputTypeDef definition

class AuthenticateCognitoActionConfigOutputTypeDef(TypedDict):
    UserPoolArn: str,
    UserPoolClientId: str,
    UserPoolDomain: str,
    SessionCookieName: NotRequired[str],
    Scope: NotRequired[str],
    SessionTimeout: NotRequired[int],
    AuthenticationRequestExtraParams: NotRequired[Dict[str, str]],
    OnUnauthenticatedRequest: NotRequired[AuthenticateCognitoActionConditionalBehaviorEnumType],  # (1)
```

1. See [:material-code-brackets: AuthenticateCognitoActionConditionalBehaviorEnumType](./literals.md#authenticatecognitoactionconditionalbehaviorenumtype) 
## AuthenticateOidcActionConfigOutputTypeDef

```python
# AuthenticateOidcActionConfigOutputTypeDef definition

class AuthenticateOidcActionConfigOutputTypeDef(TypedDict):
    Issuer: str,
    AuthorizationEndpoint: str,
    TokenEndpoint: str,
    UserInfoEndpoint: str,
    ClientId: str,
    ClientSecret: NotRequired[str],
    SessionCookieName: NotRequired[str],
    Scope: NotRequired[str],
    SessionTimeout: NotRequired[int],
    AuthenticationRequestExtraParams: NotRequired[Dict[str, str]],
    OnUnauthenticatedRequest: NotRequired[AuthenticateOidcActionConditionalBehaviorEnumType],  # (1)
    UseExistingClientSecret: NotRequired[bool],
```

1. See [:material-code-brackets: AuthenticateOidcActionConditionalBehaviorEnumType](./literals.md#authenticateoidcactionconditionalbehaviorenumtype) 
## FixedResponseActionConfigTypeDef

```python
# FixedResponseActionConfigTypeDef definition

class FixedResponseActionConfigTypeDef(TypedDict):
    StatusCode: str,
    MessageBody: NotRequired[str],
    ContentType: NotRequired[str],
```

## RedirectActionConfigTypeDef

```python
# RedirectActionConfigTypeDef definition

class RedirectActionConfigTypeDef(TypedDict):
    StatusCode: RedirectActionStatusCodeEnumType,  # (1)
    Protocol: NotRequired[str],
    Port: NotRequired[str],
    Host: NotRequired[str],
    Path: NotRequired[str],
    Query: NotRequired[str],
```

1. See [:material-code-brackets: RedirectActionStatusCodeEnumType](./literals.md#redirectactionstatuscodeenumtype) 
## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    IsDefault: NotRequired[bool],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## RevocationContentTypeDef

```python
# RevocationContentTypeDef definition

class RevocationContentTypeDef(TypedDict):
    S3Bucket: NotRequired[str],
    S3Key: NotRequired[str],
    S3ObjectVersion: NotRequired[str],
    RevocationType: NotRequired[RevocationTypeType],  # (1)
```

1. See [:material-code-brackets: RevocationTypeType](./literals.md#revocationtypetype) 
## TrustStoreRevocationTypeDef

```python
# TrustStoreRevocationTypeDef definition

class TrustStoreRevocationTypeDef(TypedDict):
    TrustStoreArn: NotRequired[str],
    RevocationId: NotRequired[int],
    RevocationType: NotRequired[RevocationTypeType],  # (1)
    NumberOfRevokedEntries: NotRequired[int],
```

1. See [:material-code-brackets: RevocationTypeType](./literals.md#revocationtypetype) 
## AdministrativeOverrideTypeDef

```python
# AdministrativeOverrideTypeDef definition

class AdministrativeOverrideTypeDef(TypedDict):
    State: NotRequired[TargetAdministrativeOverrideStateEnumType],  # (1)
    Reason: NotRequired[TargetAdministrativeOverrideReasonEnumType],  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: TargetAdministrativeOverrideStateEnumType](./literals.md#targetadministrativeoverridestateenumtype) 
2. See [:material-code-brackets: TargetAdministrativeOverrideReasonEnumType](./literals.md#targetadministrativeoverridereasonenumtype) 
## AnomalyDetectionTypeDef

```python
# AnomalyDetectionTypeDef definition

class AnomalyDetectionTypeDef(TypedDict):
    Result: NotRequired[AnomalyResultEnumType],  # (1)
    MitigationInEffect: NotRequired[MitigationInEffectEnumType],  # (2)
```

1. See [:material-code-brackets: AnomalyResultEnumType](./literals.md#anomalyresultenumtype) 
2. See [:material-code-brackets: MitigationInEffectEnumType](./literals.md#mitigationineffectenumtype) 
## AuthenticateCognitoActionConfigTypeDef

```python
# AuthenticateCognitoActionConfigTypeDef definition

class AuthenticateCognitoActionConfigTypeDef(TypedDict):
    UserPoolArn: str,
    UserPoolClientId: str,
    UserPoolDomain: str,
    SessionCookieName: NotRequired[str],
    Scope: NotRequired[str],
    SessionTimeout: NotRequired[int],
    AuthenticationRequestExtraParams: NotRequired[Mapping[str, str]],
    OnUnauthenticatedRequest: NotRequired[AuthenticateCognitoActionConditionalBehaviorEnumType],  # (1)
```

1. See [:material-code-brackets: AuthenticateCognitoActionConditionalBehaviorEnumType](./literals.md#authenticatecognitoactionconditionalbehaviorenumtype) 
## AuthenticateOidcActionConfigTypeDef

```python
# AuthenticateOidcActionConfigTypeDef definition

class AuthenticateOidcActionConfigTypeDef(TypedDict):
    Issuer: str,
    AuthorizationEndpoint: str,
    TokenEndpoint: str,
    UserInfoEndpoint: str,
    ClientId: str,
    ClientSecret: NotRequired[str],
    SessionCookieName: NotRequired[str],
    Scope: NotRequired[str],
    SessionTimeout: NotRequired[int],
    AuthenticationRequestExtraParams: NotRequired[Mapping[str, str]],
    OnUnauthenticatedRequest: NotRequired[AuthenticateOidcActionConditionalBehaviorEnumType],  # (1)
    UseExistingClientSecret: NotRequired[bool],
```

1. See [:material-code-brackets: AuthenticateOidcActionConditionalBehaviorEnumType](./literals.md#authenticateoidcactionconditionalbehaviorenumtype) 
## LoadBalancerAddressTypeDef

```python
# LoadBalancerAddressTypeDef definition

class LoadBalancerAddressTypeDef(TypedDict):
    IpAddress: NotRequired[str],
    AllocationId: NotRequired[str],
    PrivateIPv4Address: NotRequired[str],
    IPv6Address: NotRequired[str],
```

## CapacityReservationStatusTypeDef

```python
# CapacityReservationStatusTypeDef definition

class CapacityReservationStatusTypeDef(TypedDict):
    Code: NotRequired[CapacityReservationStateEnumType],  # (1)
    Reason: NotRequired[str],
```

1. See [:material-code-brackets: CapacityReservationStateEnumType](./literals.md#capacityreservationstateenumtype) 
## CipherTypeDef

```python
# CipherTypeDef definition

class CipherTypeDef(TypedDict):
    Name: NotRequired[str],
    Priority: NotRequired[int],
```

## MutualAuthenticationAttributesTypeDef

```python
# MutualAuthenticationAttributesTypeDef definition

class MutualAuthenticationAttributesTypeDef(TypedDict):
    Mode: NotRequired[str],
    TrustStoreArn: NotRequired[str],
    IgnoreClientCertificateExpiry: NotRequired[bool],
    TrustStoreAssociationStatus: NotRequired[TrustStoreAssociationStatusEnumType],  # (1)
    AdvertiseTrustStoreCaNames: NotRequired[AdvertiseTrustStoreCaNamesEnumType],  # (2)
```

1. See [:material-code-brackets: TrustStoreAssociationStatusEnumType](./literals.md#truststoreassociationstatusenumtype) 
2. See [:material-code-brackets: AdvertiseTrustStoreCaNamesEnumType](./literals.md#advertisetruststorecanamesenumtype) 
## SubnetMappingTypeDef

```python
# SubnetMappingTypeDef definition

class SubnetMappingTypeDef(TypedDict):
    SubnetId: NotRequired[str],
    AllocationId: NotRequired[str],
    PrivateIPv4Address: NotRequired[str],
    IPv6Address: NotRequired[str],
    SourceNatIpv6Prefix: NotRequired[str],
```

## MatcherTypeDef

```python
# MatcherTypeDef definition

class MatcherTypeDef(TypedDict):
    HttpCode: NotRequired[str],
    GrpcCode: NotRequired[str],
```

## TrustStoreTypeDef

```python
# TrustStoreTypeDef definition

class TrustStoreTypeDef(TypedDict):
    Name: NotRequired[str],
    TrustStoreArn: NotRequired[str],
    Status: NotRequired[TrustStoreStatusType],  # (1)
    NumberOfCaCertificates: NotRequired[int],
    TotalRevokedEntries: NotRequired[int],
```

1. See [:material-code-brackets: TrustStoreStatusType](./literals.md#truststorestatustype) 
## DeleteListenerInputRequestTypeDef

```python
# DeleteListenerInputRequestTypeDef definition

class DeleteListenerInputRequestTypeDef(TypedDict):
    ListenerArn: str,
```

## DeleteLoadBalancerInputRequestTypeDef

```python
# DeleteLoadBalancerInputRequestTypeDef definition

class DeleteLoadBalancerInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
```

## DeleteRuleInputRequestTypeDef

```python
# DeleteRuleInputRequestTypeDef definition

class DeleteRuleInputRequestTypeDef(TypedDict):
    RuleArn: str,
```

## DeleteSharedTrustStoreAssociationInputRequestTypeDef

```python
# DeleteSharedTrustStoreAssociationInputRequestTypeDef definition

class DeleteSharedTrustStoreAssociationInputRequestTypeDef(TypedDict):
    TrustStoreArn: str,
    ResourceArn: str,
```

## DeleteTargetGroupInputRequestTypeDef

```python
# DeleteTargetGroupInputRequestTypeDef definition

class DeleteTargetGroupInputRequestTypeDef(TypedDict):
    TargetGroupArn: str,
```

## DeleteTrustStoreInputRequestTypeDef

```python
# DeleteTrustStoreInputRequestTypeDef definition

class DeleteTrustStoreInputRequestTypeDef(TypedDict):
    TrustStoreArn: str,
```

## TargetDescriptionTypeDef

```python
# TargetDescriptionTypeDef definition

class TargetDescriptionTypeDef(TypedDict):
    Id: str,
    Port: NotRequired[int],
    AvailabilityZone: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAccountLimitsInputRequestTypeDef

```python
# DescribeAccountLimitsInputRequestTypeDef definition

class DescribeAccountLimitsInputRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
```

## LimitTypeDef

```python
# LimitTypeDef definition

class LimitTypeDef(TypedDict):
    Name: NotRequired[str],
    Max: NotRequired[str],
```

## DescribeCapacityReservationInputRequestTypeDef

```python
# DescribeCapacityReservationInputRequestTypeDef definition

class DescribeCapacityReservationInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
```

## MinimumLoadBalancerCapacityTypeDef

```python
# MinimumLoadBalancerCapacityTypeDef definition

class MinimumLoadBalancerCapacityTypeDef(TypedDict):
    CapacityUnits: NotRequired[int],
```

## DescribeListenerAttributesInputRequestTypeDef

```python
# DescribeListenerAttributesInputRequestTypeDef definition

class DescribeListenerAttributesInputRequestTypeDef(TypedDict):
    ListenerArn: str,
```

## ListenerAttributeTypeDef

```python
# ListenerAttributeTypeDef definition

class ListenerAttributeTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## DescribeListenerCertificatesInputRequestTypeDef

```python
# DescribeListenerCertificatesInputRequestTypeDef definition

class DescribeListenerCertificatesInputRequestTypeDef(TypedDict):
    ListenerArn: str,
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
```

## DescribeListenersInputRequestTypeDef

```python
# DescribeListenersInputRequestTypeDef definition

class DescribeListenersInputRequestTypeDef(TypedDict):
    LoadBalancerArn: NotRequired[str],
    ListenerArns: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
```

## DescribeLoadBalancerAttributesInputRequestTypeDef

```python
# DescribeLoadBalancerAttributesInputRequestTypeDef definition

class DescribeLoadBalancerAttributesInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
```

## LoadBalancerAttributeTypeDef

```python
# LoadBalancerAttributeTypeDef definition

class LoadBalancerAttributeTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## DescribeLoadBalancersInputRequestTypeDef

```python
# DescribeLoadBalancersInputRequestTypeDef definition

class DescribeLoadBalancersInputRequestTypeDef(TypedDict):
    LoadBalancerArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeRulesInputRequestTypeDef

```python
# DescribeRulesInputRequestTypeDef definition

class DescribeRulesInputRequestTypeDef(TypedDict):
    ListenerArn: NotRequired[str],
    RuleArns: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
```

## DescribeSSLPoliciesInputRequestTypeDef

```python
# DescribeSSLPoliciesInputRequestTypeDef definition

class DescribeSSLPoliciesInputRequestTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
    LoadBalancerType: NotRequired[LoadBalancerTypeEnumType],  # (1)
```

1. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
## DescribeTagsInputRequestTypeDef

```python
# DescribeTagsInputRequestTypeDef definition

class DescribeTagsInputRequestTypeDef(TypedDict):
    ResourceArns: Sequence[str],
```

## DescribeTargetGroupAttributesInputRequestTypeDef

```python
# DescribeTargetGroupAttributesInputRequestTypeDef definition

class DescribeTargetGroupAttributesInputRequestTypeDef(TypedDict):
    TargetGroupArn: str,
```

## TargetGroupAttributeTypeDef

```python
# TargetGroupAttributeTypeDef definition

class TargetGroupAttributeTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## DescribeTargetGroupsInputRequestTypeDef

```python
# DescribeTargetGroupsInputRequestTypeDef definition

class DescribeTargetGroupsInputRequestTypeDef(TypedDict):
    LoadBalancerArn: NotRequired[str],
    TargetGroupArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
```

## DescribeTrustStoreAssociationsInputRequestTypeDef

```python
# DescribeTrustStoreAssociationsInputRequestTypeDef definition

class DescribeTrustStoreAssociationsInputRequestTypeDef(TypedDict):
    TrustStoreArn: str,
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
```

## TrustStoreAssociationTypeDef

```python
# TrustStoreAssociationTypeDef definition

class TrustStoreAssociationTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
```

## DescribeTrustStoreRevocationTypeDef

```python
# DescribeTrustStoreRevocationTypeDef definition

class DescribeTrustStoreRevocationTypeDef(TypedDict):
    TrustStoreArn: NotRequired[str],
    RevocationId: NotRequired[int],
    RevocationType: NotRequired[RevocationTypeType],  # (1)
    NumberOfRevokedEntries: NotRequired[int],
```

1. See [:material-code-brackets: RevocationTypeType](./literals.md#revocationtypetype) 
## DescribeTrustStoreRevocationsInputRequestTypeDef

```python
# DescribeTrustStoreRevocationsInputRequestTypeDef definition

class DescribeTrustStoreRevocationsInputRequestTypeDef(TypedDict):
    TrustStoreArn: str,
    RevocationIds: NotRequired[Sequence[int]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
```

## DescribeTrustStoresInputRequestTypeDef

```python
# DescribeTrustStoresInputRequestTypeDef definition

class DescribeTrustStoresInputRequestTypeDef(TypedDict):
    TrustStoreArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
```

## TargetGroupStickinessConfigTypeDef

```python
# TargetGroupStickinessConfigTypeDef definition

class TargetGroupStickinessConfigTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    DurationSeconds: NotRequired[int],
```

## TargetGroupTupleTypeDef

```python
# TargetGroupTupleTypeDef definition

class TargetGroupTupleTypeDef(TypedDict):
    TargetGroupArn: NotRequired[str],
    Weight: NotRequired[int],
```

## GetResourcePolicyInputRequestTypeDef

```python
# GetResourcePolicyInputRequestTypeDef definition

class GetResourcePolicyInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetTrustStoreCaCertificatesBundleInputRequestTypeDef

```python
# GetTrustStoreCaCertificatesBundleInputRequestTypeDef definition

class GetTrustStoreCaCertificatesBundleInputRequestTypeDef(TypedDict):
    TrustStoreArn: str,
```

## GetTrustStoreRevocationContentInputRequestTypeDef

```python
# GetTrustStoreRevocationContentInputRequestTypeDef definition

class GetTrustStoreRevocationContentInputRequestTypeDef(TypedDict):
    TrustStoreArn: str,
    RevocationId: int,
```

## HostHeaderConditionConfigOutputTypeDef

```python
# HostHeaderConditionConfigOutputTypeDef definition

class HostHeaderConditionConfigOutputTypeDef(TypedDict):
    Values: NotRequired[List[str]],
```

## HostHeaderConditionConfigTypeDef

```python
# HostHeaderConditionConfigTypeDef definition

class HostHeaderConditionConfigTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
```

## HttpHeaderConditionConfigOutputTypeDef

```python
# HttpHeaderConditionConfigOutputTypeDef definition

class HttpHeaderConditionConfigOutputTypeDef(TypedDict):
    HttpHeaderName: NotRequired[str],
    Values: NotRequired[List[str]],
```

## HttpHeaderConditionConfigTypeDef

```python
# HttpHeaderConditionConfigTypeDef definition

class HttpHeaderConditionConfigTypeDef(TypedDict):
    HttpHeaderName: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## HttpRequestMethodConditionConfigOutputTypeDef

```python
# HttpRequestMethodConditionConfigOutputTypeDef definition

class HttpRequestMethodConditionConfigOutputTypeDef(TypedDict):
    Values: NotRequired[List[str]],
```

## HttpRequestMethodConditionConfigTypeDef

```python
# HttpRequestMethodConditionConfigTypeDef definition

class HttpRequestMethodConditionConfigTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
```

## LoadBalancerStateTypeDef

```python
# LoadBalancerStateTypeDef definition

class LoadBalancerStateTypeDef(TypedDict):
    Code: NotRequired[LoadBalancerStateEnumType],  # (1)
    Reason: NotRequired[str],
```

1. See [:material-code-brackets: LoadBalancerStateEnumType](./literals.md#loadbalancerstateenumtype) 
## ModifyTrustStoreInputRequestTypeDef

```python
# ModifyTrustStoreInputRequestTypeDef definition

class ModifyTrustStoreInputRequestTypeDef(TypedDict):
    TrustStoreArn: str,
    CaCertificatesBundleS3Bucket: str,
    CaCertificatesBundleS3Key: str,
    CaCertificatesBundleS3ObjectVersion: NotRequired[str],
```

## PathPatternConditionConfigOutputTypeDef

```python
# PathPatternConditionConfigOutputTypeDef definition

class PathPatternConditionConfigOutputTypeDef(TypedDict):
    Values: NotRequired[List[str]],
```

## PathPatternConditionConfigTypeDef

```python
# PathPatternConditionConfigTypeDef definition

class PathPatternConditionConfigTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
```

## QueryStringKeyValuePairTypeDef

```python
# QueryStringKeyValuePairTypeDef definition

class QueryStringKeyValuePairTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## RemoveTagsInputRequestTypeDef

```python
# RemoveTagsInputRequestTypeDef definition

class RemoveTagsInputRequestTypeDef(TypedDict):
    ResourceArns: Sequence[str],
    TagKeys: Sequence[str],
```

## RemoveTrustStoreRevocationsInputRequestTypeDef

```python
# RemoveTrustStoreRevocationsInputRequestTypeDef definition

class RemoveTrustStoreRevocationsInputRequestTypeDef(TypedDict):
    TrustStoreArn: str,
    RevocationIds: Sequence[int],
```

## SourceIpConditionConfigOutputTypeDef

```python
# SourceIpConditionConfigOutputTypeDef definition

class SourceIpConditionConfigOutputTypeDef(TypedDict):
    Values: NotRequired[List[str]],
```

## RulePriorityPairTypeDef

```python
# RulePriorityPairTypeDef definition

class RulePriorityPairTypeDef(TypedDict):
    RuleArn: NotRequired[str],
    Priority: NotRequired[int],
```

## SetIpAddressTypeInputRequestTypeDef

```python
# SetIpAddressTypeInputRequestTypeDef definition

class SetIpAddressTypeInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
    IpAddressType: IpAddressTypeType,  # (1)
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## SetSecurityGroupsInputRequestTypeDef

```python
# SetSecurityGroupsInputRequestTypeDef definition

class SetSecurityGroupsInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
    SecurityGroups: Sequence[str],
    EnforceSecurityGroupInboundRulesOnPrivateLinkTraffic: NotRequired[EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType],  # (1)
```

1. See [:material-code-brackets: EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType](./literals.md#enforcesecuritygroupinboundrulesonprivatelinktrafficenumtype) 
## SourceIpConditionConfigTypeDef

```python
# SourceIpConditionConfigTypeDef definition

class SourceIpConditionConfigTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
```

## TargetHealthTypeDef

```python
# TargetHealthTypeDef definition

class TargetHealthTypeDef(TypedDict):
    State: NotRequired[TargetHealthStateEnumType],  # (1)
    Reason: NotRequired[TargetHealthReasonEnumType],  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: TargetHealthStateEnumType](./literals.md#targethealthstateenumtype) 
2. See [:material-code-brackets: TargetHealthReasonEnumType](./literals.md#targethealthreasonenumtype) 
## AddListenerCertificatesInputRequestTypeDef

```python
# AddListenerCertificatesInputRequestTypeDef definition

class AddListenerCertificatesInputRequestTypeDef(TypedDict):
    ListenerArn: str,
    Certificates: Sequence[CertificateTypeDef],  # (1)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
## RemoveListenerCertificatesInputRequestTypeDef

```python
# RemoveListenerCertificatesInputRequestTypeDef definition

class RemoveListenerCertificatesInputRequestTypeDef(TypedDict):
    ListenerArn: str,
    Certificates: Sequence[CertificateTypeDef],  # (1)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
## AddListenerCertificatesOutputTypeDef

```python
# AddListenerCertificatesOutputTypeDef definition

class AddListenerCertificatesOutputTypeDef(TypedDict):
    Certificates: List[CertificateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeListenerCertificatesOutputTypeDef

```python
# DescribeListenerCertificatesOutputTypeDef definition

class DescribeListenerCertificatesOutputTypeDef(TypedDict):
    Certificates: List[CertificateTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyOutputTypeDef

```python
# GetResourcePolicyOutputTypeDef definition

class GetResourcePolicyOutputTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrustStoreCaCertificatesBundleOutputTypeDef

```python
# GetTrustStoreCaCertificatesBundleOutputTypeDef definition

class GetTrustStoreCaCertificatesBundleOutputTypeDef(TypedDict):
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrustStoreRevocationContentOutputTypeDef

```python
# GetTrustStoreRevocationContentOutputTypeDef definition

class GetTrustStoreRevocationContentOutputTypeDef(TypedDict):
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetIpAddressTypeOutputTypeDef

```python
# SetIpAddressTypeOutputTypeDef definition

class SetIpAddressTypeOutputTypeDef(TypedDict):
    IpAddressType: IpAddressTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetSecurityGroupsOutputTypeDef

```python
# SetSecurityGroupsOutputTypeDef definition

class SetSecurityGroupsOutputTypeDef(TypedDict):
    SecurityGroupIds: List[str],
    EnforceSecurityGroupInboundRulesOnPrivateLinkTraffic: EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType](./literals.md#enforcesecuritygroupinboundrulesonprivatelinktrafficenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddTagsInputRequestTypeDef

```python
# AddTagsInputRequestTypeDef definition

class AddTagsInputRequestTypeDef(TypedDict):
    ResourceArns: Sequence[str],
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTrustStoreInputRequestTypeDef

```python
# CreateTrustStoreInputRequestTypeDef definition

class CreateTrustStoreInputRequestTypeDef(TypedDict):
    Name: str,
    CaCertificatesBundleS3Bucket: str,
    CaCertificatesBundleS3Key: str,
    CaCertificatesBundleS3ObjectVersion: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagDescriptionTypeDef

```python
# TagDescriptionTypeDef definition

class TagDescriptionTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AddTrustStoreRevocationsInputRequestTypeDef

```python
# AddTrustStoreRevocationsInputRequestTypeDef definition

class AddTrustStoreRevocationsInputRequestTypeDef(TypedDict):
    TrustStoreArn: str,
    RevocationContents: NotRequired[Sequence[RevocationContentTypeDef]],  # (1)
```

1. See [:material-code-braces: RevocationContentTypeDef](./type_defs.md#revocationcontenttypedef) 
## AddTrustStoreRevocationsOutputTypeDef

```python
# AddTrustStoreRevocationsOutputTypeDef definition

class AddTrustStoreRevocationsOutputTypeDef(TypedDict):
    TrustStoreRevocations: List[TrustStoreRevocationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustStoreRevocationTypeDef](./type_defs.md#truststorerevocationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    ZoneName: NotRequired[str],
    SubnetId: NotRequired[str],
    OutpostId: NotRequired[str],
    LoadBalancerAddresses: NotRequired[List[LoadBalancerAddressTypeDef]],  # (1)
    SourceNatIpv6Prefixes: NotRequired[List[str]],
```

1. See [:material-code-braces: LoadBalancerAddressTypeDef](./type_defs.md#loadbalanceraddresstypedef) 
## ZonalCapacityReservationStateTypeDef

```python
# ZonalCapacityReservationStateTypeDef definition

class ZonalCapacityReservationStateTypeDef(TypedDict):
    State: NotRequired[CapacityReservationStatusTypeDef],  # (1)
    AvailabilityZone: NotRequired[str],
    EffectiveCapacityUnits: NotRequired[float],
```

1. See [:material-code-braces: CapacityReservationStatusTypeDef](./type_defs.md#capacityreservationstatustypedef) 
## SslPolicyTypeDef

```python
# SslPolicyTypeDef definition

class SslPolicyTypeDef(TypedDict):
    SslProtocols: NotRequired[List[str]],
    Ciphers: NotRequired[List[CipherTypeDef]],  # (1)
    Name: NotRequired[str],
    SupportedLoadBalancerTypes: NotRequired[List[str]],
```

1. See [:material-code-braces: CipherTypeDef](./type_defs.md#ciphertypedef) 
## CreateLoadBalancerInputRequestTypeDef

```python
# CreateLoadBalancerInputRequestTypeDef definition

class CreateLoadBalancerInputRequestTypeDef(TypedDict):
    Name: str,
    Subnets: NotRequired[Sequence[str]],
    SubnetMappings: NotRequired[Sequence[SubnetMappingTypeDef]],  # (1)
    SecurityGroups: NotRequired[Sequence[str]],
    Scheme: NotRequired[LoadBalancerSchemeEnumType],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    Type: NotRequired[LoadBalancerTypeEnumType],  # (4)
    IpAddressType: NotRequired[IpAddressTypeType],  # (5)
    CustomerOwnedIpv4Pool: NotRequired[str],
    EnablePrefixForIpv6SourceNat: NotRequired[EnablePrefixForIpv6SourceNatEnumType],  # (6)
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-brackets: LoadBalancerSchemeEnumType](./literals.md#loadbalancerschemeenumtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
5. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
6. See [:material-code-brackets: EnablePrefixForIpv6SourceNatEnumType](./literals.md#enableprefixforipv6sourcenatenumtype) 
## SetSubnetsInputRequestTypeDef

```python
# SetSubnetsInputRequestTypeDef definition

class SetSubnetsInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
    Subnets: NotRequired[Sequence[str]],
    SubnetMappings: NotRequired[Sequence[SubnetMappingTypeDef]],  # (1)
    IpAddressType: NotRequired[IpAddressTypeType],  # (2)
    EnablePrefixForIpv6SourceNat: NotRequired[EnablePrefixForIpv6SourceNatEnumType],  # (3)
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
3. See [:material-code-brackets: EnablePrefixForIpv6SourceNatEnumType](./literals.md#enableprefixforipv6sourcenatenumtype) 
## CreateTargetGroupInputRequestTypeDef

```python
# CreateTargetGroupInputRequestTypeDef definition

class CreateTargetGroupInputRequestTypeDef(TypedDict):
    Name: str,
    Protocol: NotRequired[ProtocolEnumType],  # (1)
    ProtocolVersion: NotRequired[str],
    Port: NotRequired[int],
    VpcId: NotRequired[str],
    HealthCheckProtocol: NotRequired[ProtocolEnumType],  # (1)
    HealthCheckPort: NotRequired[str],
    HealthCheckEnabled: NotRequired[bool],
    HealthCheckPath: NotRequired[str],
    HealthCheckIntervalSeconds: NotRequired[int],
    HealthCheckTimeoutSeconds: NotRequired[int],
    HealthyThresholdCount: NotRequired[int],
    UnhealthyThresholdCount: NotRequired[int],
    Matcher: NotRequired[MatcherTypeDef],  # (3)
    TargetType: NotRequired[TargetTypeEnumType],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    IpAddressType: NotRequired[TargetGroupIpAddressTypeEnumType],  # (6)
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
3. See [:material-code-braces: MatcherTypeDef](./type_defs.md#matchertypedef) 
4. See [:material-code-brackets: TargetTypeEnumType](./literals.md#targettypeenumtype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-brackets: TargetGroupIpAddressTypeEnumType](./literals.md#targetgroupipaddresstypeenumtype) 
## ModifyTargetGroupInputRequestTypeDef

```python
# ModifyTargetGroupInputRequestTypeDef definition

class ModifyTargetGroupInputRequestTypeDef(TypedDict):
    TargetGroupArn: str,
    HealthCheckProtocol: NotRequired[ProtocolEnumType],  # (1)
    HealthCheckPort: NotRequired[str],
    HealthCheckPath: NotRequired[str],
    HealthCheckEnabled: NotRequired[bool],
    HealthCheckIntervalSeconds: NotRequired[int],
    HealthCheckTimeoutSeconds: NotRequired[int],
    HealthyThresholdCount: NotRequired[int],
    UnhealthyThresholdCount: NotRequired[int],
    Matcher: NotRequired[MatcherTypeDef],  # (2)
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-braces: MatcherTypeDef](./type_defs.md#matchertypedef) 
## TargetGroupTypeDef

```python
# TargetGroupTypeDef definition

class TargetGroupTypeDef(TypedDict):
    TargetGroupArn: NotRequired[str],
    TargetGroupName: NotRequired[str],
    Protocol: NotRequired[ProtocolEnumType],  # (1)
    Port: NotRequired[int],
    VpcId: NotRequired[str],
    HealthCheckProtocol: NotRequired[ProtocolEnumType],  # (1)
    HealthCheckPort: NotRequired[str],
    HealthCheckEnabled: NotRequired[bool],
    HealthCheckIntervalSeconds: NotRequired[int],
    HealthCheckTimeoutSeconds: NotRequired[int],
    HealthyThresholdCount: NotRequired[int],
    UnhealthyThresholdCount: NotRequired[int],
    HealthCheckPath: NotRequired[str],
    Matcher: NotRequired[MatcherTypeDef],  # (3)
    LoadBalancerArns: NotRequired[List[str]],
    TargetType: NotRequired[TargetTypeEnumType],  # (4)
    ProtocolVersion: NotRequired[str],
    IpAddressType: NotRequired[TargetGroupIpAddressTypeEnumType],  # (5)
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
3. See [:material-code-braces: MatcherTypeDef](./type_defs.md#matchertypedef) 
4. See [:material-code-brackets: TargetTypeEnumType](./literals.md#targettypeenumtype) 
5. See [:material-code-brackets: TargetGroupIpAddressTypeEnumType](./literals.md#targetgroupipaddresstypeenumtype) 
## CreateTrustStoreOutputTypeDef

```python
# CreateTrustStoreOutputTypeDef definition

class CreateTrustStoreOutputTypeDef(TypedDict):
    TrustStores: List[TrustStoreTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustStoreTypeDef](./type_defs.md#truststoretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrustStoresOutputTypeDef

```python
# DescribeTrustStoresOutputTypeDef definition

class DescribeTrustStoresOutputTypeDef(TypedDict):
    TrustStores: List[TrustStoreTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustStoreTypeDef](./type_defs.md#truststoretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyTrustStoreOutputTypeDef

```python
# ModifyTrustStoreOutputTypeDef definition

class ModifyTrustStoreOutputTypeDef(TypedDict):
    TrustStores: List[TrustStoreTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustStoreTypeDef](./type_defs.md#truststoretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterTargetsInputRequestTypeDef

```python
# DeregisterTargetsInputRequestTypeDef definition

class DeregisterTargetsInputRequestTypeDef(TypedDict):
    TargetGroupArn: str,
    Targets: Sequence[TargetDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
## DescribeTargetHealthInputRequestTypeDef

```python
# DescribeTargetHealthInputRequestTypeDef definition

class DescribeTargetHealthInputRequestTypeDef(TypedDict):
    TargetGroupArn: str,
    Targets: NotRequired[Sequence[TargetDescriptionTypeDef]],  # (1)
    Include: NotRequired[Sequence[DescribeTargetHealthInputIncludeEnumType]],  # (2)
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
2. See [:material-code-brackets: DescribeTargetHealthInputIncludeEnumType](./literals.md#describetargethealthinputincludeenumtype) 
## RegisterTargetsInputRequestTypeDef

```python
# RegisterTargetsInputRequestTypeDef definition

class RegisterTargetsInputRequestTypeDef(TypedDict):
    TargetGroupArn: str,
    Targets: Sequence[TargetDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
## DescribeAccountLimitsInputPaginateTypeDef

```python
# DescribeAccountLimitsInputPaginateTypeDef definition

class DescribeAccountLimitsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeListenerCertificatesInputPaginateTypeDef

```python
# DescribeListenerCertificatesInputPaginateTypeDef definition

class DescribeListenerCertificatesInputPaginateTypeDef(TypedDict):
    ListenerArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeListenersInputPaginateTypeDef

```python
# DescribeListenersInputPaginateTypeDef definition

class DescribeListenersInputPaginateTypeDef(TypedDict):
    LoadBalancerArn: NotRequired[str],
    ListenerArns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeLoadBalancersInputPaginateTypeDef

```python
# DescribeLoadBalancersInputPaginateTypeDef definition

class DescribeLoadBalancersInputPaginateTypeDef(TypedDict):
    LoadBalancerArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRulesInputPaginateTypeDef

```python
# DescribeRulesInputPaginateTypeDef definition

class DescribeRulesInputPaginateTypeDef(TypedDict):
    ListenerArn: NotRequired[str],
    RuleArns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSSLPoliciesInputPaginateTypeDef

```python
# DescribeSSLPoliciesInputPaginateTypeDef definition

class DescribeSSLPoliciesInputPaginateTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    LoadBalancerType: NotRequired[LoadBalancerTypeEnumType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTargetGroupsInputPaginateTypeDef

```python
# DescribeTargetGroupsInputPaginateTypeDef definition

class DescribeTargetGroupsInputPaginateTypeDef(TypedDict):
    LoadBalancerArn: NotRequired[str],
    TargetGroupArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAccountLimitsOutputTypeDef

```python
# DescribeAccountLimitsOutputTypeDef definition

class DescribeAccountLimitsOutputTypeDef(TypedDict):
    Limits: List[LimitTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LimitTypeDef](./type_defs.md#limittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyCapacityReservationInputRequestTypeDef

```python
# ModifyCapacityReservationInputRequestTypeDef definition

class ModifyCapacityReservationInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
    MinimumLoadBalancerCapacity: NotRequired[MinimumLoadBalancerCapacityTypeDef],  # (1)
    ResetCapacityReservation: NotRequired[bool],
```

1. See [:material-code-braces: MinimumLoadBalancerCapacityTypeDef](./type_defs.md#minimumloadbalancercapacitytypedef) 
## DescribeListenerAttributesOutputTypeDef

```python
# DescribeListenerAttributesOutputTypeDef definition

class DescribeListenerAttributesOutputTypeDef(TypedDict):
    Attributes: List[ListenerAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListenerAttributeTypeDef](./type_defs.md#listenerattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyListenerAttributesInputRequestTypeDef

```python
# ModifyListenerAttributesInputRequestTypeDef definition

class ModifyListenerAttributesInputRequestTypeDef(TypedDict):
    ListenerArn: str,
    Attributes: Sequence[ListenerAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: ListenerAttributeTypeDef](./type_defs.md#listenerattributetypedef) 
## ModifyListenerAttributesOutputTypeDef

```python
# ModifyListenerAttributesOutputTypeDef definition

class ModifyListenerAttributesOutputTypeDef(TypedDict):
    Attributes: List[ListenerAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListenerAttributeTypeDef](./type_defs.md#listenerattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoadBalancerAttributesOutputTypeDef

```python
# DescribeLoadBalancerAttributesOutputTypeDef definition

class DescribeLoadBalancerAttributesOutputTypeDef(TypedDict):
    Attributes: List[LoadBalancerAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerAttributeTypeDef](./type_defs.md#loadbalancerattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyLoadBalancerAttributesInputRequestTypeDef

```python
# ModifyLoadBalancerAttributesInputRequestTypeDef definition

class ModifyLoadBalancerAttributesInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
    Attributes: Sequence[LoadBalancerAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: LoadBalancerAttributeTypeDef](./type_defs.md#loadbalancerattributetypedef) 
## ModifyLoadBalancerAttributesOutputTypeDef

```python
# ModifyLoadBalancerAttributesOutputTypeDef definition

class ModifyLoadBalancerAttributesOutputTypeDef(TypedDict):
    Attributes: List[LoadBalancerAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerAttributeTypeDef](./type_defs.md#loadbalancerattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoadBalancersInputWaitTypeDef

```python
# DescribeLoadBalancersInputWaitTypeDef definition

class DescribeLoadBalancersInputWaitTypeDef(TypedDict):
    LoadBalancerArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTargetHealthInputWaitTypeDef

```python
# DescribeTargetHealthInputWaitTypeDef definition

class DescribeTargetHealthInputWaitTypeDef(TypedDict):
    TargetGroupArn: str,
    Targets: NotRequired[Sequence[TargetDescriptionTypeDef]],  # (1)
    Include: NotRequired[Sequence[DescribeTargetHealthInputIncludeEnumType]],  # (2)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
2. See [:material-code-brackets: DescribeTargetHealthInputIncludeEnumType](./literals.md#describetargethealthinputincludeenumtype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTargetGroupAttributesOutputTypeDef

```python
# DescribeTargetGroupAttributesOutputTypeDef definition

class DescribeTargetGroupAttributesOutputTypeDef(TypedDict):
    Attributes: List[TargetGroupAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetGroupAttributeTypeDef](./type_defs.md#targetgroupattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyTargetGroupAttributesInputRequestTypeDef

```python
# ModifyTargetGroupAttributesInputRequestTypeDef definition

class ModifyTargetGroupAttributesInputRequestTypeDef(TypedDict):
    TargetGroupArn: str,
    Attributes: Sequence[TargetGroupAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: TargetGroupAttributeTypeDef](./type_defs.md#targetgroupattributetypedef) 
## ModifyTargetGroupAttributesOutputTypeDef

```python
# ModifyTargetGroupAttributesOutputTypeDef definition

class ModifyTargetGroupAttributesOutputTypeDef(TypedDict):
    Attributes: List[TargetGroupAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetGroupAttributeTypeDef](./type_defs.md#targetgroupattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrustStoreAssociationsOutputTypeDef

```python
# DescribeTrustStoreAssociationsOutputTypeDef definition

class DescribeTrustStoreAssociationsOutputTypeDef(TypedDict):
    TrustStoreAssociations: List[TrustStoreAssociationTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustStoreAssociationTypeDef](./type_defs.md#truststoreassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrustStoreRevocationsOutputTypeDef

```python
# DescribeTrustStoreRevocationsOutputTypeDef definition

class DescribeTrustStoreRevocationsOutputTypeDef(TypedDict):
    TrustStoreRevocations: List[DescribeTrustStoreRevocationTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DescribeTrustStoreRevocationTypeDef](./type_defs.md#describetruststorerevocationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ForwardActionConfigOutputTypeDef

```python
# ForwardActionConfigOutputTypeDef definition

class ForwardActionConfigOutputTypeDef(TypedDict):
    TargetGroups: NotRequired[List[TargetGroupTupleTypeDef]],  # (1)
    TargetGroupStickinessConfig: NotRequired[TargetGroupStickinessConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TargetGroupTupleTypeDef](./type_defs.md#targetgrouptupletypedef) 
2. See [:material-code-braces: TargetGroupStickinessConfigTypeDef](./type_defs.md#targetgroupstickinessconfigtypedef) 
## ForwardActionConfigTypeDef

```python
# ForwardActionConfigTypeDef definition

class ForwardActionConfigTypeDef(TypedDict):
    TargetGroups: NotRequired[Sequence[TargetGroupTupleTypeDef]],  # (1)
    TargetGroupStickinessConfig: NotRequired[TargetGroupStickinessConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TargetGroupTupleTypeDef](./type_defs.md#targetgrouptupletypedef) 
2. See [:material-code-braces: TargetGroupStickinessConfigTypeDef](./type_defs.md#targetgroupstickinessconfigtypedef) 
## QueryStringConditionConfigOutputTypeDef

```python
# QueryStringConditionConfigOutputTypeDef definition

class QueryStringConditionConfigOutputTypeDef(TypedDict):
    Values: NotRequired[List[QueryStringKeyValuePairTypeDef]],  # (1)
```

1. See [:material-code-braces: QueryStringKeyValuePairTypeDef](./type_defs.md#querystringkeyvaluepairtypedef) 
## QueryStringConditionConfigTypeDef

```python
# QueryStringConditionConfigTypeDef definition

class QueryStringConditionConfigTypeDef(TypedDict):
    Values: NotRequired[Sequence[QueryStringKeyValuePairTypeDef]],  # (1)
```

1. See [:material-code-braces: QueryStringKeyValuePairTypeDef](./type_defs.md#querystringkeyvaluepairtypedef) 
## SetRulePrioritiesInputRequestTypeDef

```python
# SetRulePrioritiesInputRequestTypeDef definition

class SetRulePrioritiesInputRequestTypeDef(TypedDict):
    RulePriorities: Sequence[RulePriorityPairTypeDef],  # (1)
```

1. See [:material-code-braces: RulePriorityPairTypeDef](./type_defs.md#ruleprioritypairtypedef) 
## TargetHealthDescriptionTypeDef

```python
# TargetHealthDescriptionTypeDef definition

class TargetHealthDescriptionTypeDef(TypedDict):
    Target: NotRequired[TargetDescriptionTypeDef],  # (1)
    HealthCheckPort: NotRequired[str],
    TargetHealth: NotRequired[TargetHealthTypeDef],  # (2)
    AnomalyDetection: NotRequired[AnomalyDetectionTypeDef],  # (3)
    AdministrativeOverride: NotRequired[AdministrativeOverrideTypeDef],  # (4)
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
2. See [:material-code-braces: TargetHealthTypeDef](./type_defs.md#targethealthtypedef) 
3. See [:material-code-braces: AnomalyDetectionTypeDef](./type_defs.md#anomalydetectiontypedef) 
4. See [:material-code-braces: AdministrativeOverrideTypeDef](./type_defs.md#administrativeoverridetypedef) 
## DescribeTagsOutputTypeDef

```python
# DescribeTagsOutputTypeDef definition

class DescribeTagsOutputTypeDef(TypedDict):
    TagDescriptions: List[TagDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagDescriptionTypeDef](./type_defs.md#tagdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoadBalancerTypeDef

```python
# LoadBalancerTypeDef definition

class LoadBalancerTypeDef(TypedDict):
    LoadBalancerArn: NotRequired[str],
    DNSName: NotRequired[str],
    CanonicalHostedZoneId: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LoadBalancerName: NotRequired[str],
    Scheme: NotRequired[LoadBalancerSchemeEnumType],  # (1)
    VpcId: NotRequired[str],
    State: NotRequired[LoadBalancerStateTypeDef],  # (2)
    Type: NotRequired[LoadBalancerTypeEnumType],  # (3)
    AvailabilityZones: NotRequired[List[AvailabilityZoneTypeDef]],  # (4)
    SecurityGroups: NotRequired[List[str]],
    IpAddressType: NotRequired[IpAddressTypeType],  # (5)
    CustomerOwnedIpv4Pool: NotRequired[str],
    EnforceSecurityGroupInboundRulesOnPrivateLinkTraffic: NotRequired[str],
    EnablePrefixForIpv6SourceNat: NotRequired[EnablePrefixForIpv6SourceNatEnumType],  # (6)
```

1. See [:material-code-brackets: LoadBalancerSchemeEnumType](./literals.md#loadbalancerschemeenumtype) 
2. See [:material-code-braces: LoadBalancerStateTypeDef](./type_defs.md#loadbalancerstatetypedef) 
3. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
4. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
5. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
6. See [:material-code-brackets: EnablePrefixForIpv6SourceNatEnumType](./literals.md#enableprefixforipv6sourcenatenumtype) 
## SetSubnetsOutputTypeDef

```python
# SetSubnetsOutputTypeDef definition

class SetSubnetsOutputTypeDef(TypedDict):
    AvailabilityZones: List[AvailabilityZoneTypeDef],  # (1)
    IpAddressType: IpAddressTypeType,  # (2)
    EnablePrefixForIpv6SourceNat: EnablePrefixForIpv6SourceNatEnumType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
2. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
3. See [:material-code-brackets: EnablePrefixForIpv6SourceNatEnumType](./literals.md#enableprefixforipv6sourcenatenumtype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCapacityReservationOutputTypeDef

```python
# DescribeCapacityReservationOutputTypeDef definition

class DescribeCapacityReservationOutputTypeDef(TypedDict):
    LastModifiedTime: datetime,
    DecreaseRequestsRemaining: int,
    MinimumLoadBalancerCapacity: MinimumLoadBalancerCapacityTypeDef,  # (1)
    CapacityReservationState: List[ZonalCapacityReservationStateTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MinimumLoadBalancerCapacityTypeDef](./type_defs.md#minimumloadbalancercapacitytypedef) 
2. See [:material-code-braces: ZonalCapacityReservationStateTypeDef](./type_defs.md#zonalcapacityreservationstatetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyCapacityReservationOutputTypeDef

```python
# ModifyCapacityReservationOutputTypeDef definition

class ModifyCapacityReservationOutputTypeDef(TypedDict):
    LastModifiedTime: datetime,
    DecreaseRequestsRemaining: int,
    MinimumLoadBalancerCapacity: MinimumLoadBalancerCapacityTypeDef,  # (1)
    CapacityReservationState: List[ZonalCapacityReservationStateTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MinimumLoadBalancerCapacityTypeDef](./type_defs.md#minimumloadbalancercapacitytypedef) 
2. See [:material-code-braces: ZonalCapacityReservationStateTypeDef](./type_defs.md#zonalcapacityreservationstatetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSSLPoliciesOutputTypeDef

```python
# DescribeSSLPoliciesOutputTypeDef definition

class DescribeSSLPoliciesOutputTypeDef(TypedDict):
    SslPolicies: List[SslPolicyTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SslPolicyTypeDef](./type_defs.md#sslpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTargetGroupOutputTypeDef

```python
# CreateTargetGroupOutputTypeDef definition

class CreateTargetGroupOutputTypeDef(TypedDict):
    TargetGroups: List[TargetGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetGroupTypeDef](./type_defs.md#targetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTargetGroupsOutputTypeDef

```python
# DescribeTargetGroupsOutputTypeDef definition

class DescribeTargetGroupsOutputTypeDef(TypedDict):
    TargetGroups: List[TargetGroupTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetGroupTypeDef](./type_defs.md#targetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyTargetGroupOutputTypeDef

```python
# ModifyTargetGroupOutputTypeDef definition

class ModifyTargetGroupOutputTypeDef(TypedDict):
    TargetGroups: List[TargetGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetGroupTypeDef](./type_defs.md#targetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActionOutputTypeDef

```python
# ActionOutputTypeDef definition

class ActionOutputTypeDef(TypedDict):
    Type: ActionTypeEnumType,  # (1)
    TargetGroupArn: NotRequired[str],
    AuthenticateOidcConfig: NotRequired[AuthenticateOidcActionConfigOutputTypeDef],  # (2)
    AuthenticateCognitoConfig: NotRequired[AuthenticateCognitoActionConfigOutputTypeDef],  # (3)
    Order: NotRequired[int],
    RedirectConfig: NotRequired[RedirectActionConfigTypeDef],  # (4)
    FixedResponseConfig: NotRequired[FixedResponseActionConfigTypeDef],  # (5)
    ForwardConfig: NotRequired[ForwardActionConfigOutputTypeDef],  # (6)
```

1. See [:material-code-brackets: ActionTypeEnumType](./literals.md#actiontypeenumtype) 
2. See [:material-code-braces: AuthenticateOidcActionConfigOutputTypeDef](./type_defs.md#authenticateoidcactionconfigoutputtypedef) 
3. See [:material-code-braces: AuthenticateCognitoActionConfigOutputTypeDef](./type_defs.md#authenticatecognitoactionconfigoutputtypedef) 
4. See [:material-code-braces: RedirectActionConfigTypeDef](./type_defs.md#redirectactionconfigtypedef) 
5. See [:material-code-braces: FixedResponseActionConfigTypeDef](./type_defs.md#fixedresponseactionconfigtypedef) 
6. See [:material-code-braces: ForwardActionConfigOutputTypeDef](./type_defs.md#forwardactionconfigoutputtypedef) 
## RuleConditionOutputTypeDef

```python
# RuleConditionOutputTypeDef definition

class RuleConditionOutputTypeDef(TypedDict):
    Field: NotRequired[str],
    Values: NotRequired[List[str]],
    HostHeaderConfig: NotRequired[HostHeaderConditionConfigOutputTypeDef],  # (1)
    PathPatternConfig: NotRequired[PathPatternConditionConfigOutputTypeDef],  # (2)
    HttpHeaderConfig: NotRequired[HttpHeaderConditionConfigOutputTypeDef],  # (3)
    QueryStringConfig: NotRequired[QueryStringConditionConfigOutputTypeDef],  # (4)
    HttpRequestMethodConfig: NotRequired[HttpRequestMethodConditionConfigOutputTypeDef],  # (5)
    SourceIpConfig: NotRequired[SourceIpConditionConfigOutputTypeDef],  # (6)
```

1. See [:material-code-braces: HostHeaderConditionConfigOutputTypeDef](./type_defs.md#hostheaderconditionconfigoutputtypedef) 
2. See [:material-code-braces: PathPatternConditionConfigOutputTypeDef](./type_defs.md#pathpatternconditionconfigoutputtypedef) 
3. See [:material-code-braces: HttpHeaderConditionConfigOutputTypeDef](./type_defs.md#httpheaderconditionconfigoutputtypedef) 
4. See [:material-code-braces: QueryStringConditionConfigOutputTypeDef](./type_defs.md#querystringconditionconfigoutputtypedef) 
5. See [:material-code-braces: HttpRequestMethodConditionConfigOutputTypeDef](./type_defs.md#httprequestmethodconditionconfigoutputtypedef) 
6. See [:material-code-braces: SourceIpConditionConfigOutputTypeDef](./type_defs.md#sourceipconditionconfigoutputtypedef) 
## DescribeTargetHealthOutputTypeDef

```python
# DescribeTargetHealthOutputTypeDef definition

class DescribeTargetHealthOutputTypeDef(TypedDict):
    TargetHealthDescriptions: List[TargetHealthDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetHealthDescriptionTypeDef](./type_defs.md#targethealthdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoadBalancerOutputTypeDef

```python
# CreateLoadBalancerOutputTypeDef definition

class CreateLoadBalancerOutputTypeDef(TypedDict):
    LoadBalancers: List[LoadBalancerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoadBalancersOutputTypeDef

```python
# DescribeLoadBalancersOutputTypeDef definition

class DescribeLoadBalancersOutputTypeDef(TypedDict):
    LoadBalancers: List[LoadBalancerTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListenerTypeDef

```python
# ListenerTypeDef definition

class ListenerTypeDef(TypedDict):
    ListenerArn: NotRequired[str],
    LoadBalancerArn: NotRequired[str],
    Port: NotRequired[int],
    Protocol: NotRequired[ProtocolEnumType],  # (1)
    Certificates: NotRequired[List[CertificateTypeDef]],  # (2)
    SslPolicy: NotRequired[str],
    DefaultActions: NotRequired[List[ActionOutputTypeDef]],  # (3)
    AlpnPolicy: NotRequired[List[str]],
    MutualAuthentication: NotRequired[MutualAuthenticationAttributesTypeDef],  # (4)
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
3. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
4. See [:material-code-braces: MutualAuthenticationAttributesTypeDef](./type_defs.md#mutualauthenticationattributestypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    Type: ActionTypeEnumType,  # (1)
    TargetGroupArn: NotRequired[str],
    AuthenticateOidcConfig: NotRequired[AuthenticateOidcActionConfigUnionTypeDef],  # (2)
    AuthenticateCognitoConfig: NotRequired[AuthenticateCognitoActionConfigUnionTypeDef],  # (3)
    Order: NotRequired[int],
    RedirectConfig: NotRequired[RedirectActionConfigTypeDef],  # (4)
    FixedResponseConfig: NotRequired[FixedResponseActionConfigTypeDef],  # (5)
    ForwardConfig: NotRequired[ForwardActionConfigUnionTypeDef],  # (6)
```

1. See [:material-code-brackets: ActionTypeEnumType](./literals.md#actiontypeenumtype) 
2. See [:material-code-braces: AuthenticateOidcActionConfigTypeDef](./type_defs.md#authenticateoidcactionconfigtypedef) [:material-code-braces: AuthenticateOidcActionConfigOutputTypeDef](./type_defs.md#authenticateoidcactionconfigoutputtypedef) 
3. See [:material-code-braces: AuthenticateCognitoActionConfigTypeDef](./type_defs.md#authenticatecognitoactionconfigtypedef) [:material-code-braces: AuthenticateCognitoActionConfigOutputTypeDef](./type_defs.md#authenticatecognitoactionconfigoutputtypedef) 
4. See [:material-code-braces: RedirectActionConfigTypeDef](./type_defs.md#redirectactionconfigtypedef) 
5. See [:material-code-braces: FixedResponseActionConfigTypeDef](./type_defs.md#fixedresponseactionconfigtypedef) 
6. See [:material-code-braces: ForwardActionConfigTypeDef](./type_defs.md#forwardactionconfigtypedef) [:material-code-braces: ForwardActionConfigOutputTypeDef](./type_defs.md#forwardactionconfigoutputtypedef) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    RuleArn: NotRequired[str],
    Priority: NotRequired[str],
    Conditions: NotRequired[List[RuleConditionOutputTypeDef]],  # (1)
    Actions: NotRequired[List[ActionOutputTypeDef]],  # (2)
    IsDefault: NotRequired[bool],
```

1. See [:material-code-braces: RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef) 
2. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
## RuleConditionTypeDef

```python
# RuleConditionTypeDef definition

class RuleConditionTypeDef(TypedDict):
    Field: NotRequired[str],
    Values: NotRequired[Sequence[str]],
    HostHeaderConfig: NotRequired[HostHeaderConditionConfigUnionTypeDef],  # (1)
    PathPatternConfig: NotRequired[PathPatternConditionConfigUnionTypeDef],  # (2)
    HttpHeaderConfig: NotRequired[HttpHeaderConditionConfigUnionTypeDef],  # (3)
    QueryStringConfig: NotRequired[QueryStringConditionConfigUnionTypeDef],  # (4)
    HttpRequestMethodConfig: NotRequired[HttpRequestMethodConditionConfigUnionTypeDef],  # (5)
    SourceIpConfig: NotRequired[SourceIpConditionConfigUnionTypeDef],  # (6)
```

1. See [:material-code-braces: HostHeaderConditionConfigTypeDef](./type_defs.md#hostheaderconditionconfigtypedef) [:material-code-braces: HostHeaderConditionConfigOutputTypeDef](./type_defs.md#hostheaderconditionconfigoutputtypedef) 
2. See [:material-code-braces: PathPatternConditionConfigTypeDef](./type_defs.md#pathpatternconditionconfigtypedef) [:material-code-braces: PathPatternConditionConfigOutputTypeDef](./type_defs.md#pathpatternconditionconfigoutputtypedef) 
3. See [:material-code-braces: HttpHeaderConditionConfigTypeDef](./type_defs.md#httpheaderconditionconfigtypedef) [:material-code-braces: HttpHeaderConditionConfigOutputTypeDef](./type_defs.md#httpheaderconditionconfigoutputtypedef) 
4. See [:material-code-braces: QueryStringConditionConfigTypeDef](./type_defs.md#querystringconditionconfigtypedef) [:material-code-braces: QueryStringConditionConfigOutputTypeDef](./type_defs.md#querystringconditionconfigoutputtypedef) 
5. See [:material-code-braces: HttpRequestMethodConditionConfigTypeDef](./type_defs.md#httprequestmethodconditionconfigtypedef) [:material-code-braces: HttpRequestMethodConditionConfigOutputTypeDef](./type_defs.md#httprequestmethodconditionconfigoutputtypedef) 
6. See [:material-code-braces: SourceIpConditionConfigTypeDef](./type_defs.md#sourceipconditionconfigtypedef) [:material-code-braces: SourceIpConditionConfigOutputTypeDef](./type_defs.md#sourceipconditionconfigoutputtypedef) 
## CreateListenerOutputTypeDef

```python
# CreateListenerOutputTypeDef definition

class CreateListenerOutputTypeDef(TypedDict):
    Listeners: List[ListenerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeListenersOutputTypeDef

```python
# DescribeListenersOutputTypeDef definition

class DescribeListenersOutputTypeDef(TypedDict):
    Listeners: List[ListenerTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyListenerOutputTypeDef

```python
# ModifyListenerOutputTypeDef definition

class ModifyListenerOutputTypeDef(TypedDict):
    Listeners: List[ListenerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyListenerInputRequestTypeDef

```python
# ModifyListenerInputRequestTypeDef definition

class ModifyListenerInputRequestTypeDef(TypedDict):
    ListenerArn: str,
    Port: NotRequired[int],
    Protocol: NotRequired[ProtocolEnumType],  # (1)
    SslPolicy: NotRequired[str],
    Certificates: NotRequired[Sequence[CertificateTypeDef]],  # (2)
    DefaultActions: NotRequired[Sequence[ActionTypeDef]],  # (3)
    AlpnPolicy: NotRequired[Sequence[str]],
    MutualAuthentication: NotRequired[MutualAuthenticationAttributesTypeDef],  # (4)
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
3. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
4. See [:material-code-braces: MutualAuthenticationAttributesTypeDef](./type_defs.md#mutualauthenticationattributestypedef) 
## CreateRuleOutputTypeDef

```python
# CreateRuleOutputTypeDef definition

class CreateRuleOutputTypeDef(TypedDict):
    Rules: List[RuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRulesOutputTypeDef

```python
# DescribeRulesOutputTypeDef definition

class DescribeRulesOutputTypeDef(TypedDict):
    Rules: List[RuleTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyRuleOutputTypeDef

```python
# ModifyRuleOutputTypeDef definition

class ModifyRuleOutputTypeDef(TypedDict):
    Rules: List[RuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetRulePrioritiesOutputTypeDef

```python
# SetRulePrioritiesOutputTypeDef definition

class SetRulePrioritiesOutputTypeDef(TypedDict):
    Rules: List[RuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyRuleInputRequestTypeDef

```python
# ModifyRuleInputRequestTypeDef definition

class ModifyRuleInputRequestTypeDef(TypedDict):
    RuleArn: str,
    Conditions: NotRequired[Sequence[RuleConditionTypeDef]],  # (1)
    Actions: NotRequired[Sequence[ActionTypeDef]],  # (2)
```

1. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## CreateListenerInputRequestTypeDef

```python
# CreateListenerInputRequestTypeDef definition

class CreateListenerInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
    DefaultActions: Sequence[ActionUnionTypeDef],  # (1)
    Protocol: NotRequired[ProtocolEnumType],  # (2)
    Port: NotRequired[int],
    SslPolicy: NotRequired[str],
    Certificates: NotRequired[Sequence[CertificateTypeDef]],  # (3)
    AlpnPolicy: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    MutualAuthentication: NotRequired[MutualAuthenticationAttributesTypeDef],  # (5)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
2. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
3. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: MutualAuthenticationAttributesTypeDef](./type_defs.md#mutualauthenticationattributestypedef) 
## CreateRuleInputRequestTypeDef

```python
# CreateRuleInputRequestTypeDef definition

class CreateRuleInputRequestTypeDef(TypedDict):
    ListenerArn: str,
    Conditions: Sequence[RuleConditionUnionTypeDef],  # (1)
    Priority: int,
    Actions: Sequence[ActionTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) [:material-code-braces: RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
