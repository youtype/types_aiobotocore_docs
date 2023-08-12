# Type definitions

> [Index](../README.md) > [ElasticLoadBalancingv2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
    type annotations stubs module [types-aiobotocore-elbv2](https://pypi.org/project/types-aiobotocore-elbv2/).



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
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## LoadBalancerAddressTypeDef

```python
# LoadBalancerAddressTypeDef definition

class LoadBalancerAddressTypeDef(TypedDict):
    IpAddress: NotRequired[str],
    AllocationId: NotRequired[str],
    PrivateIPv4Address: NotRequired[str],
    IPv6Address: NotRequired[str],
```

## CipherTypeDef

```python
# CipherTypeDef definition

class CipherTypeDef(TypedDict):
    Name: NotRequired[str],
    Priority: NotRequired[int],
```

## SubnetMappingTypeDef

```python
# SubnetMappingTypeDef definition

class SubnetMappingTypeDef(TypedDict):
    SubnetId: NotRequired[str],
    AllocationId: NotRequired[str],
    PrivateIPv4Address: NotRequired[str],
    IPv6Address: NotRequired[str],
```

## MatcherTypeDef

```python
# MatcherTypeDef definition

class MatcherTypeDef(TypedDict):
    HttpCode: NotRequired[str],
    GrpcCode: NotRequired[str],
```

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

## DeleteTargetGroupInputRequestTypeDef

```python
# DeleteTargetGroupInputRequestTypeDef definition

class DeleteTargetGroupInputRequestTypeDef(TypedDict):
    TargetGroupArn: str,
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

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
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

## HostHeaderConditionConfigTypeDef

```python
# HostHeaderConditionConfigTypeDef definition

class HostHeaderConditionConfigTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
```

## HttpHeaderConditionConfigTypeDef

```python
# HttpHeaderConditionConfigTypeDef definition

class HttpHeaderConditionConfigTypeDef(TypedDict):
    HttpHeaderName: NotRequired[str],
    Values: NotRequired[Sequence[str]],
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

## SourceIpConditionConfigTypeDef

```python
# SourceIpConditionConfigTypeDef definition

class SourceIpConditionConfigTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
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
## TagDescriptionTypeDef

```python
# TagDescriptionTypeDef definition

class TagDescriptionTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    ZoneName: NotRequired[str],
    SubnetId: NotRequired[str],
    OutpostId: NotRequired[str],
    LoadBalancerAddresses: NotRequired[List[LoadBalancerAddressTypeDef]],  # (1)
```

1. See [:material-code-braces: LoadBalancerAddressTypeDef](./type_defs.md#loadbalanceraddresstypedef) 
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
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-brackets: LoadBalancerSchemeEnumType](./literals.md#loadbalancerschemeenumtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
5. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## SetSubnetsInputRequestTypeDef

```python
# SetSubnetsInputRequestTypeDef definition

class SetSubnetsInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
    Subnets: NotRequired[Sequence[str]],
    SubnetMappings: NotRequired[Sequence[SubnetMappingTypeDef]],  # (1)
    IpAddressType: NotRequired[IpAddressTypeType],  # (2)
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
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
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
## RegisterTargetsInputRequestTypeDef

```python
# RegisterTargetsInputRequestTypeDef definition

class RegisterTargetsInputRequestTypeDef(TypedDict):
    TargetGroupArn: str,
    Targets: Sequence[TargetDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
## DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef

```python
# DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef definition

class DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef

```python
# DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef definition

class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(TypedDict):
    ListenerArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeListenersInputDescribeListenersPaginateTypeDef

```python
# DescribeListenersInputDescribeListenersPaginateTypeDef definition

class DescribeListenersInputDescribeListenersPaginateTypeDef(TypedDict):
    LoadBalancerArn: NotRequired[str],
    ListenerArns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef

```python
# DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef definition

class DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef(TypedDict):
    LoadBalancerArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRulesInputDescribeRulesPaginateTypeDef

```python
# DescribeRulesInputDescribeRulesPaginateTypeDef definition

class DescribeRulesInputDescribeRulesPaginateTypeDef(TypedDict):
    ListenerArn: NotRequired[str],
    RuleArns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef

```python
# DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef definition

class DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    LoadBalancerType: NotRequired[LoadBalancerTypeEnumType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef

```python
# DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef definition

class DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef(TypedDict):
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
## DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef

```python
# DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef definition

class DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef(TypedDict):
    LoadBalancerArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef

```python
# DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef definition

class DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef(TypedDict):
    LoadBalancerArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef

```python
# DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef definition

class DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef(TypedDict):
    LoadBalancerArns: NotRequired[Sequence[str]],
    Names: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTargetHealthInputTargetDeregisteredWaitTypeDef

```python
# DescribeTargetHealthInputTargetDeregisteredWaitTypeDef definition

class DescribeTargetHealthInputTargetDeregisteredWaitTypeDef(TypedDict):
    TargetGroupArn: str,
    Targets: NotRequired[Sequence[TargetDescriptionTypeDef]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTargetHealthInputTargetInServiceWaitTypeDef

```python
# DescribeTargetHealthInputTargetInServiceWaitTypeDef definition

class DescribeTargetHealthInputTargetInServiceWaitTypeDef(TypedDict):
    TargetGroupArn: str,
    Targets: NotRequired[Sequence[TargetDescriptionTypeDef]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
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
## ForwardActionConfigTypeDef

```python
# ForwardActionConfigTypeDef definition

class ForwardActionConfigTypeDef(TypedDict):
    TargetGroups: NotRequired[Sequence[TargetGroupTupleTypeDef]],  # (1)
    TargetGroupStickinessConfig: NotRequired[TargetGroupStickinessConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TargetGroupTupleTypeDef](./type_defs.md#targetgrouptupletypedef) 
2. See [:material-code-braces: TargetGroupStickinessConfigTypeDef](./type_defs.md#targetgroupstickinessconfigtypedef) 
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
```

1. See [:material-code-braces: TargetDescriptionTypeDef](./type_defs.md#targetdescriptiontypedef) 
2. See [:material-code-braces: TargetHealthTypeDef](./type_defs.md#targethealthtypedef) 
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
```

1. See [:material-code-brackets: LoadBalancerSchemeEnumType](./literals.md#loadbalancerschemeenumtype) 
2. See [:material-code-braces: LoadBalancerStateTypeDef](./type_defs.md#loadbalancerstatetypedef) 
3. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
4. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
5. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## SetSubnetsOutputTypeDef

```python
# SetSubnetsOutputTypeDef definition

class SetSubnetsOutputTypeDef(TypedDict):
    AvailabilityZones: List[AvailabilityZoneTypeDef],  # (1)
    IpAddressType: IpAddressTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
2. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
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
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    Type: ActionTypeEnumType,  # (1)
    TargetGroupArn: NotRequired[str],
    AuthenticateOidcConfig: NotRequired[AuthenticateOidcActionConfigTypeDef],  # (2)
    AuthenticateCognitoConfig: NotRequired[AuthenticateCognitoActionConfigTypeDef],  # (3)
    Order: NotRequired[int],
    RedirectConfig: NotRequired[RedirectActionConfigTypeDef],  # (4)
    FixedResponseConfig: NotRequired[FixedResponseActionConfigTypeDef],  # (5)
    ForwardConfig: NotRequired[ForwardActionConfigTypeDef],  # (6)
```

1. See [:material-code-brackets: ActionTypeEnumType](./literals.md#actiontypeenumtype) 
2. See [:material-code-braces: AuthenticateOidcActionConfigTypeDef](./type_defs.md#authenticateoidcactionconfigtypedef) 
3. See [:material-code-braces: AuthenticateCognitoActionConfigTypeDef](./type_defs.md#authenticatecognitoactionconfigtypedef) 
4. See [:material-code-braces: RedirectActionConfigTypeDef](./type_defs.md#redirectactionconfigtypedef) 
5. See [:material-code-braces: FixedResponseActionConfigTypeDef](./type_defs.md#fixedresponseactionconfigtypedef) 
6. See [:material-code-braces: ForwardActionConfigTypeDef](./type_defs.md#forwardactionconfigtypedef) 
## RuleConditionTypeDef

```python
# RuleConditionTypeDef definition

class RuleConditionTypeDef(TypedDict):
    Field: NotRequired[str],
    Values: NotRequired[Sequence[str]],
    HostHeaderConfig: NotRequired[HostHeaderConditionConfigTypeDef],  # (1)
    PathPatternConfig: NotRequired[PathPatternConditionConfigTypeDef],  # (2)
    HttpHeaderConfig: NotRequired[HttpHeaderConditionConfigTypeDef],  # (3)
    QueryStringConfig: NotRequired[QueryStringConditionConfigTypeDef],  # (4)
    HttpRequestMethodConfig: NotRequired[HttpRequestMethodConditionConfigTypeDef],  # (5)
    SourceIpConfig: NotRequired[SourceIpConditionConfigTypeDef],  # (6)
```

1. See [:material-code-braces: HostHeaderConditionConfigTypeDef](./type_defs.md#hostheaderconditionconfigtypedef) 
2. See [:material-code-braces: PathPatternConditionConfigTypeDef](./type_defs.md#pathpatternconditionconfigtypedef) 
3. See [:material-code-braces: HttpHeaderConditionConfigTypeDef](./type_defs.md#httpheaderconditionconfigtypedef) 
4. See [:material-code-braces: QueryStringConditionConfigTypeDef](./type_defs.md#querystringconditionconfigtypedef) 
5. See [:material-code-braces: HttpRequestMethodConditionConfigTypeDef](./type_defs.md#httprequestmethodconditionconfigtypedef) 
6. See [:material-code-braces: SourceIpConditionConfigTypeDef](./type_defs.md#sourceipconditionconfigtypedef) 
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
## CreateListenerInputRequestTypeDef

```python
# CreateListenerInputRequestTypeDef definition

class CreateListenerInputRequestTypeDef(TypedDict):
    LoadBalancerArn: str,
    DefaultActions: Sequence[ActionTypeDef],  # (1)
    Protocol: NotRequired[ProtocolEnumType],  # (2)
    Port: NotRequired[int],
    SslPolicy: NotRequired[str],
    Certificates: NotRequired[Sequence[CertificateTypeDef]],  # (3)
    AlpnPolicy: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
3. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
    DefaultActions: NotRequired[List[ActionTypeDef]],  # (3)
    AlpnPolicy: NotRequired[List[str]],
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
3. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
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
```

1. See [:material-code-brackets: ProtocolEnumType](./literals.md#protocolenumtype) 
2. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
3. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## CreateRuleInputRequestTypeDef

```python
# CreateRuleInputRequestTypeDef definition

class CreateRuleInputRequestTypeDef(TypedDict):
    ListenerArn: str,
    Conditions: Sequence[RuleConditionTypeDef],  # (1)
    Priority: int,
    Actions: Sequence[ActionTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    RuleArn: NotRequired[str],
    Priority: NotRequired[str],
    Conditions: NotRequired[List[RuleConditionTypeDef]],  # (1)
    Actions: NotRequired[List[ActionTypeDef]],  # (2)
    IsDefault: NotRequired[bool],
```

1. See [:material-code-braces: RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
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
