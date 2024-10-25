# Type definitions

> [Index](../README.md) > [ElasticLoadBalancing](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
    type annotations stubs module [types-aiobotocore-elb](https://pypi.org/project/types-aiobotocore-elb/).



## AccessLogTypeDef

```python
# AccessLogTypeDef definition

class AccessLogTypeDef(TypedDict):
    Enabled: bool,
    S3BucketName: NotRequired[str],
    EmitInterval: NotRequired[int],
    S3BucketPrefix: NotRequired[str],
```

## AddAvailabilityZonesInputRequestTypeDef

```python
# AddAvailabilityZonesInputRequestTypeDef definition

class AddAvailabilityZonesInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    AvailabilityZones: Sequence[str],
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

## AdditionalAttributeTypeDef

```python
# AdditionalAttributeTypeDef definition

class AdditionalAttributeTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## AppCookieStickinessPolicyTypeDef

```python
# AppCookieStickinessPolicyTypeDef definition

class AppCookieStickinessPolicyTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    CookieName: NotRequired[str],
```

## ApplySecurityGroupsToLoadBalancerInputRequestTypeDef

```python
# ApplySecurityGroupsToLoadBalancerInputRequestTypeDef definition

class ApplySecurityGroupsToLoadBalancerInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    SecurityGroups: Sequence[str],
```

## AttachLoadBalancerToSubnetsInputRequestTypeDef

```python
# AttachLoadBalancerToSubnetsInputRequestTypeDef definition

class AttachLoadBalancerToSubnetsInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    Subnets: Sequence[str],
```

## BackendServerDescriptionTypeDef

```python
# BackendServerDescriptionTypeDef definition

class BackendServerDescriptionTypeDef(TypedDict):
    InstancePort: NotRequired[int],
    PolicyNames: NotRequired[List[str]],
```

## HealthCheckTypeDef

```python
# HealthCheckTypeDef definition

class HealthCheckTypeDef(TypedDict):
    Target: str,
    Interval: int,
    Timeout: int,
    UnhealthyThreshold: int,
    HealthyThreshold: int,
```

## ConnectionDrainingTypeDef

```python
# ConnectionDrainingTypeDef definition

class ConnectionDrainingTypeDef(TypedDict):
    Enabled: bool,
    Timeout: NotRequired[int],
```

## ConnectionSettingsTypeDef

```python
# ConnectionSettingsTypeDef definition

class ConnectionSettingsTypeDef(TypedDict):
    IdleTimeout: int,
```

## ListenerTypeDef

```python
# ListenerTypeDef definition

class ListenerTypeDef(TypedDict):
    Protocol: str,
    LoadBalancerPort: int,
    InstancePort: int,
    InstanceProtocol: NotRequired[str],
    SSLCertificateId: NotRequired[str],
```

## CreateAppCookieStickinessPolicyInputRequestTypeDef

```python
# CreateAppCookieStickinessPolicyInputRequestTypeDef definition

class CreateAppCookieStickinessPolicyInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    PolicyName: str,
    CookieName: str,
```

## CreateLBCookieStickinessPolicyInputRequestTypeDef

```python
# CreateLBCookieStickinessPolicyInputRequestTypeDef definition

class CreateLBCookieStickinessPolicyInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    PolicyName: str,
    CookieExpirationPeriod: NotRequired[int],
```

## PolicyAttributeTypeDef

```python
# PolicyAttributeTypeDef definition

class PolicyAttributeTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    AttributeValue: NotRequired[str],
```

## CrossZoneLoadBalancingTypeDef

```python
# CrossZoneLoadBalancingTypeDef definition

class CrossZoneLoadBalancingTypeDef(TypedDict):
    Enabled: bool,
```

## DeleteAccessPointInputRequestTypeDef

```python
# DeleteAccessPointInputRequestTypeDef definition

class DeleteAccessPointInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
```

## DeleteLoadBalancerListenerInputRequestTypeDef

```python
# DeleteLoadBalancerListenerInputRequestTypeDef definition

class DeleteLoadBalancerListenerInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    LoadBalancerPorts: Sequence[int],
```

## DeleteLoadBalancerPolicyInputRequestTypeDef

```python
# DeleteLoadBalancerPolicyInputRequestTypeDef definition

class DeleteLoadBalancerPolicyInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    PolicyName: str,
```

## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    InstanceId: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAccessPointsInputRequestTypeDef

```python
# DescribeAccessPointsInputRequestTypeDef definition

class DescribeAccessPointsInputRequestTypeDef(TypedDict):
    LoadBalancerNames: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    PageSize: NotRequired[int],
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

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## InstanceStateTypeDef

```python
# InstanceStateTypeDef definition

class InstanceStateTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    State: NotRequired[str],
    ReasonCode: NotRequired[str],
    Description: NotRequired[str],
```

## DescribeLoadBalancerAttributesInputRequestTypeDef

```python
# DescribeLoadBalancerAttributesInputRequestTypeDef definition

class DescribeLoadBalancerAttributesInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
```

## DescribeLoadBalancerPoliciesInputRequestTypeDef

```python
# DescribeLoadBalancerPoliciesInputRequestTypeDef definition

class DescribeLoadBalancerPoliciesInputRequestTypeDef(TypedDict):
    LoadBalancerName: NotRequired[str],
    PolicyNames: NotRequired[Sequence[str]],
```

## DescribeLoadBalancerPolicyTypesInputRequestTypeDef

```python
# DescribeLoadBalancerPolicyTypesInputRequestTypeDef definition

class DescribeLoadBalancerPolicyTypesInputRequestTypeDef(TypedDict):
    PolicyTypeNames: NotRequired[Sequence[str]],
```

## DescribeTagsInputRequestTypeDef

```python
# DescribeTagsInputRequestTypeDef definition

class DescribeTagsInputRequestTypeDef(TypedDict):
    LoadBalancerNames: Sequence[str],
```

## DetachLoadBalancerFromSubnetsInputRequestTypeDef

```python
# DetachLoadBalancerFromSubnetsInputRequestTypeDef definition

class DetachLoadBalancerFromSubnetsInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    Subnets: Sequence[str],
```

## LBCookieStickinessPolicyTypeDef

```python
# LBCookieStickinessPolicyTypeDef definition

class LBCookieStickinessPolicyTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    CookieExpirationPeriod: NotRequired[int],
```

## SourceSecurityGroupTypeDef

```python
# SourceSecurityGroupTypeDef definition

class SourceSecurityGroupTypeDef(TypedDict):
    OwnerAlias: NotRequired[str],
    GroupName: NotRequired[str],
```

## PolicyAttributeDescriptionTypeDef

```python
# PolicyAttributeDescriptionTypeDef definition

class PolicyAttributeDescriptionTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    AttributeValue: NotRequired[str],
```

## PolicyAttributeTypeDescriptionTypeDef

```python
# PolicyAttributeTypeDescriptionTypeDef definition

class PolicyAttributeTypeDescriptionTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    AttributeType: NotRequired[str],
    Description: NotRequired[str],
    DefaultValue: NotRequired[str],
    Cardinality: NotRequired[str],
```

## RemoveAvailabilityZonesInputRequestTypeDef

```python
# RemoveAvailabilityZonesInputRequestTypeDef definition

class RemoveAvailabilityZonesInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    AvailabilityZones: Sequence[str],
```

## TagKeyOnlyTypeDef

```python
# TagKeyOnlyTypeDef definition

class TagKeyOnlyTypeDef(TypedDict):
    Key: NotRequired[str],
```

## SetLoadBalancerListenerSSLCertificateInputRequestTypeDef

```python
# SetLoadBalancerListenerSSLCertificateInputRequestTypeDef definition

class SetLoadBalancerListenerSSLCertificateInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    LoadBalancerPort: int,
    SSLCertificateId: str,
```

## SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef

```python
# SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef definition

class SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    InstancePort: int,
    PolicyNames: Sequence[str],
```

## SetLoadBalancerPoliciesOfListenerInputRequestTypeDef

```python
# SetLoadBalancerPoliciesOfListenerInputRequestTypeDef definition

class SetLoadBalancerPoliciesOfListenerInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    LoadBalancerPort: int,
    PolicyNames: Sequence[str],
```

## AddAvailabilityZonesOutputTypeDef

```python
# AddAvailabilityZonesOutputTypeDef definition

class AddAvailabilityZonesOutputTypeDef(TypedDict):
    AvailabilityZones: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplySecurityGroupsToLoadBalancerOutputTypeDef

```python
# ApplySecurityGroupsToLoadBalancerOutputTypeDef definition

class ApplySecurityGroupsToLoadBalancerOutputTypeDef(TypedDict):
    SecurityGroups: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachLoadBalancerToSubnetsOutputTypeDef

```python
# AttachLoadBalancerToSubnetsOutputTypeDef definition

class AttachLoadBalancerToSubnetsOutputTypeDef(TypedDict):
    Subnets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAccessPointOutputTypeDef

```python
# CreateAccessPointOutputTypeDef definition

class CreateAccessPointOutputTypeDef(TypedDict):
    DNSName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetachLoadBalancerFromSubnetsOutputTypeDef

```python
# DetachLoadBalancerFromSubnetsOutputTypeDef definition

class DetachLoadBalancerFromSubnetsOutputTypeDef(TypedDict):
    Subnets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveAvailabilityZonesOutputTypeDef

```python
# RemoveAvailabilityZonesOutputTypeDef definition

class RemoveAvailabilityZonesOutputTypeDef(TypedDict):
    AvailabilityZones: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddTagsInputRequestTypeDef

```python
# AddTagsInputRequestTypeDef definition

class AddTagsInputRequestTypeDef(TypedDict):
    LoadBalancerNames: Sequence[str],
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagDescriptionTypeDef

```python
# TagDescriptionTypeDef definition

class TagDescriptionTypeDef(TypedDict):
    LoadBalancerName: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ConfigureHealthCheckInputRequestTypeDef

```python
# ConfigureHealthCheckInputRequestTypeDef definition

class ConfigureHealthCheckInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    HealthCheck: HealthCheckTypeDef,  # (1)
```

1. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
## ConfigureHealthCheckOutputTypeDef

```python
# ConfigureHealthCheckOutputTypeDef definition

class ConfigureHealthCheckOutputTypeDef(TypedDict):
    HealthCheck: HealthCheckTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAccessPointInputRequestTypeDef

```python
# CreateAccessPointInputRequestTypeDef definition

class CreateAccessPointInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    Listeners: Sequence[ListenerTypeDef],  # (1)
    AvailabilityZones: NotRequired[Sequence[str]],
    Subnets: NotRequired[Sequence[str]],
    SecurityGroups: NotRequired[Sequence[str]],
    Scheme: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateLoadBalancerListenerInputRequestTypeDef

```python
# CreateLoadBalancerListenerInputRequestTypeDef definition

class CreateLoadBalancerListenerInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    Listeners: Sequence[ListenerTypeDef],  # (1)
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
## ListenerDescriptionTypeDef

```python
# ListenerDescriptionTypeDef definition

class ListenerDescriptionTypeDef(TypedDict):
    Listener: NotRequired[ListenerTypeDef],  # (1)
    PolicyNames: NotRequired[List[str]],
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
## CreateLoadBalancerPolicyInputRequestTypeDef

```python
# CreateLoadBalancerPolicyInputRequestTypeDef definition

class CreateLoadBalancerPolicyInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    PolicyName: str,
    PolicyTypeName: str,
    PolicyAttributes: NotRequired[Sequence[PolicyAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyAttributeTypeDef](./type_defs.md#policyattributetypedef) 
## LoadBalancerAttributesOutputTypeDef

```python
# LoadBalancerAttributesOutputTypeDef definition

class LoadBalancerAttributesOutputTypeDef(TypedDict):
    CrossZoneLoadBalancing: NotRequired[CrossZoneLoadBalancingTypeDef],  # (1)
    AccessLog: NotRequired[AccessLogTypeDef],  # (2)
    ConnectionDraining: NotRequired[ConnectionDrainingTypeDef],  # (3)
    ConnectionSettings: NotRequired[ConnectionSettingsTypeDef],  # (4)
    AdditionalAttributes: NotRequired[List[AdditionalAttributeTypeDef]],  # (5)
```

1. See [:material-code-braces: CrossZoneLoadBalancingTypeDef](./type_defs.md#crosszoneloadbalancingtypedef) 
2. See [:material-code-braces: AccessLogTypeDef](./type_defs.md#accesslogtypedef) 
3. See [:material-code-braces: ConnectionDrainingTypeDef](./type_defs.md#connectiondrainingtypedef) 
4. See [:material-code-braces: ConnectionSettingsTypeDef](./type_defs.md#connectionsettingstypedef) 
5. See [:material-code-braces: AdditionalAttributeTypeDef](./type_defs.md#additionalattributetypedef) 
## LoadBalancerAttributesTypeDef

```python
# LoadBalancerAttributesTypeDef definition

class LoadBalancerAttributesTypeDef(TypedDict):
    CrossZoneLoadBalancing: NotRequired[CrossZoneLoadBalancingTypeDef],  # (1)
    AccessLog: NotRequired[AccessLogTypeDef],  # (2)
    ConnectionDraining: NotRequired[ConnectionDrainingTypeDef],  # (3)
    ConnectionSettings: NotRequired[ConnectionSettingsTypeDef],  # (4)
    AdditionalAttributes: NotRequired[Sequence[AdditionalAttributeTypeDef]],  # (5)
```

1. See [:material-code-braces: CrossZoneLoadBalancingTypeDef](./type_defs.md#crosszoneloadbalancingtypedef) 
2. See [:material-code-braces: AccessLogTypeDef](./type_defs.md#accesslogtypedef) 
3. See [:material-code-braces: ConnectionDrainingTypeDef](./type_defs.md#connectiondrainingtypedef) 
4. See [:material-code-braces: ConnectionSettingsTypeDef](./type_defs.md#connectionsettingstypedef) 
5. See [:material-code-braces: AdditionalAttributeTypeDef](./type_defs.md#additionalattributetypedef) 
## DeregisterEndPointsInputRequestTypeDef

```python
# DeregisterEndPointsInputRequestTypeDef definition

class DeregisterEndPointsInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    Instances: Sequence[InstanceTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
## DeregisterEndPointsOutputTypeDef

```python
# DeregisterEndPointsOutputTypeDef definition

class DeregisterEndPointsOutputTypeDef(TypedDict):
    Instances: List[InstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndPointStateInputRequestTypeDef

```python
# DescribeEndPointStateInputRequestTypeDef definition

class DescribeEndPointStateInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    Instances: NotRequired[Sequence[InstanceTypeDef]],  # (1)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
## RegisterEndPointsInputRequestTypeDef

```python
# RegisterEndPointsInputRequestTypeDef definition

class RegisterEndPointsInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    Instances: Sequence[InstanceTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
## RegisterEndPointsOutputTypeDef

```python
# RegisterEndPointsOutputTypeDef definition

class RegisterEndPointsOutputTypeDef(TypedDict):
    Instances: List[InstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef

```python
# DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef definition

class DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef(TypedDict):
    LoadBalancerNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef

```python
# DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef definition

class DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef(TypedDict):
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
## DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef

```python
# DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef definition

class DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef(TypedDict):
    LoadBalancerName: str,
    Instances: NotRequired[Sequence[InstanceTypeDef]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef

```python
# DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef definition

class DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef(TypedDict):
    LoadBalancerName: str,
    Instances: NotRequired[Sequence[InstanceTypeDef]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEndPointStateInputInstanceInServiceWaitTypeDef

```python
# DescribeEndPointStateInputInstanceInServiceWaitTypeDef definition

class DescribeEndPointStateInputInstanceInServiceWaitTypeDef(TypedDict):
    LoadBalancerName: str,
    Instances: NotRequired[Sequence[InstanceTypeDef]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEndPointStateOutputTypeDef

```python
# DescribeEndPointStateOutputTypeDef definition

class DescribeEndPointStateOutputTypeDef(TypedDict):
    InstanceStates: List[InstanceStateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceStateTypeDef](./type_defs.md#instancestatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PoliciesTypeDef

```python
# PoliciesTypeDef definition

class PoliciesTypeDef(TypedDict):
    AppCookieStickinessPolicies: NotRequired[List[AppCookieStickinessPolicyTypeDef]],  # (1)
    LBCookieStickinessPolicies: NotRequired[List[LBCookieStickinessPolicyTypeDef]],  # (2)
    OtherPolicies: NotRequired[List[str]],
```

1. See [:material-code-braces: AppCookieStickinessPolicyTypeDef](./type_defs.md#appcookiestickinesspolicytypedef) 
2. See [:material-code-braces: LBCookieStickinessPolicyTypeDef](./type_defs.md#lbcookiestickinesspolicytypedef) 
## PolicyDescriptionTypeDef

```python
# PolicyDescriptionTypeDef definition

class PolicyDescriptionTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    PolicyTypeName: NotRequired[str],
    PolicyAttributeDescriptions: NotRequired[List[PolicyAttributeDescriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyAttributeDescriptionTypeDef](./type_defs.md#policyattributedescriptiontypedef) 
## PolicyTypeDescriptionTypeDef

```python
# PolicyTypeDescriptionTypeDef definition

class PolicyTypeDescriptionTypeDef(TypedDict):
    PolicyTypeName: NotRequired[str],
    Description: NotRequired[str],
    PolicyAttributeTypeDescriptions: NotRequired[List[PolicyAttributeTypeDescriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyAttributeTypeDescriptionTypeDef](./type_defs.md#policyattributetypedescriptiontypedef) 
## RemoveTagsInputRequestTypeDef

```python
# RemoveTagsInputRequestTypeDef definition

class RemoveTagsInputRequestTypeDef(TypedDict):
    LoadBalancerNames: Sequence[str],
    Tags: Sequence[TagKeyOnlyTypeDef],  # (1)
```

1. See [:material-code-braces: TagKeyOnlyTypeDef](./type_defs.md#tagkeyonlytypedef) 
## DescribeTagsOutputTypeDef

```python
# DescribeTagsOutputTypeDef definition

class DescribeTagsOutputTypeDef(TypedDict):
    TagDescriptions: List[TagDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagDescriptionTypeDef](./type_defs.md#tagdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoadBalancerAttributesOutputTypeDef

```python
# DescribeLoadBalancerAttributesOutputTypeDef definition

class DescribeLoadBalancerAttributesOutputTypeDef(TypedDict):
    LoadBalancerAttributes: LoadBalancerAttributesOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerAttributesOutputTypeDef](./type_defs.md#loadbalancerattributesoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyLoadBalancerAttributesOutputTypeDef

```python
# ModifyLoadBalancerAttributesOutputTypeDef definition

class ModifyLoadBalancerAttributesOutputTypeDef(TypedDict):
    LoadBalancerName: str,
    LoadBalancerAttributes: LoadBalancerAttributesOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerAttributesOutputTypeDef](./type_defs.md#loadbalancerattributesoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyLoadBalancerAttributesInputRequestTypeDef

```python
# ModifyLoadBalancerAttributesInputRequestTypeDef definition

class ModifyLoadBalancerAttributesInputRequestTypeDef(TypedDict):
    LoadBalancerName: str,
    LoadBalancerAttributes: LoadBalancerAttributesTypeDef,  # (1)
```

1. See [:material-code-braces: LoadBalancerAttributesTypeDef](./type_defs.md#loadbalancerattributestypedef) 
## LoadBalancerDescriptionTypeDef

```python
# LoadBalancerDescriptionTypeDef definition

class LoadBalancerDescriptionTypeDef(TypedDict):
    LoadBalancerName: NotRequired[str],
    DNSName: NotRequired[str],
    CanonicalHostedZoneName: NotRequired[str],
    CanonicalHostedZoneNameID: NotRequired[str],
    ListenerDescriptions: NotRequired[List[ListenerDescriptionTypeDef]],  # (1)
    Policies: NotRequired[PoliciesTypeDef],  # (2)
    BackendServerDescriptions: NotRequired[List[BackendServerDescriptionTypeDef]],  # (3)
    AvailabilityZones: NotRequired[List[str]],
    Subnets: NotRequired[List[str]],
    VPCId: NotRequired[str],
    Instances: NotRequired[List[InstanceTypeDef]],  # (4)
    HealthCheck: NotRequired[HealthCheckTypeDef],  # (5)
    SourceSecurityGroup: NotRequired[SourceSecurityGroupTypeDef],  # (6)
    SecurityGroups: NotRequired[List[str]],
    CreatedTime: NotRequired[datetime],
    Scheme: NotRequired[str],
```

1. See [:material-code-braces: ListenerDescriptionTypeDef](./type_defs.md#listenerdescriptiontypedef) 
2. See [:material-code-braces: PoliciesTypeDef](./type_defs.md#policiestypedef) 
3. See [:material-code-braces: BackendServerDescriptionTypeDef](./type_defs.md#backendserverdescriptiontypedef) 
4. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
5. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
6. See [:material-code-braces: SourceSecurityGroupTypeDef](./type_defs.md#sourcesecuritygrouptypedef) 
## DescribeLoadBalancerPoliciesOutputTypeDef

```python
# DescribeLoadBalancerPoliciesOutputTypeDef definition

class DescribeLoadBalancerPoliciesOutputTypeDef(TypedDict):
    PolicyDescriptions: List[PolicyDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyDescriptionTypeDef](./type_defs.md#policydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoadBalancerPolicyTypesOutputTypeDef

```python
# DescribeLoadBalancerPolicyTypesOutputTypeDef definition

class DescribeLoadBalancerPolicyTypesOutputTypeDef(TypedDict):
    PolicyTypeDescriptions: List[PolicyTypeDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDescriptionTypeDef](./type_defs.md#policytypedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccessPointsOutputTypeDef

```python
# DescribeAccessPointsOutputTypeDef definition

class DescribeAccessPointsOutputTypeDef(TypedDict):
    LoadBalancerDescriptions: List[LoadBalancerDescriptionTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerDescriptionTypeDef](./type_defs.md#loadbalancerdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
