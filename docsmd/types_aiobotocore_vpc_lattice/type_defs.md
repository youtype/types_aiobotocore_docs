# Type definitions

> [Index](../README.md) > [VPCLattice](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [VPCLattice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
    type annotations stubs module [types-aiobotocore-vpc-lattice](https://pypi.org/project/types-aiobotocore-vpc-lattice/).

## ForwardActionUnionTypeDef

```python
# ForwardActionUnionTypeDef definition

ForwardActionUnionTypeDef = Union[
    ForwardActionTypeDef,  # (1)
    ForwardActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ForwardActionTypeDef](./type_defs.md#forwardactiontypedef) 
2. See [:material-code-braces: ForwardActionOutputTypeDef](./type_defs.md#forwardactionoutputtypedef) 

## HttpMatchUnionTypeDef

```python
# HttpMatchUnionTypeDef definition

HttpMatchUnionTypeDef = Union[
    HttpMatchTypeDef,  # (1)
    HttpMatchOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HttpMatchTypeDef](./type_defs.md#httpmatchtypedef) 
2. See [:material-code-braces: HttpMatchOutputTypeDef](./type_defs.md#httpmatchoutputtypedef) 

## RuleActionUnionTypeDef

```python
# RuleActionUnionTypeDef definition

RuleActionUnionTypeDef = Union[
    RuleActionTypeDef,  # (1)
    RuleActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 

## RuleMatchUnionTypeDef

```python
# RuleMatchUnionTypeDef definition

RuleMatchUnionTypeDef = Union[
    RuleMatchTypeDef,  # (1)
    RuleMatchOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleMatchTypeDef](./type_defs.md#rulematchtypedef) 
2. See [:material-code-braces: RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef) 



## AccessLogSubscriptionSummaryTypeDef

```python
# AccessLogSubscriptionSummaryTypeDef definition

class AccessLogSubscriptionSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    destinationArn: str,
    id: str,
    lastUpdatedAt: datetime,
    resourceArn: str,
    resourceId: str,
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

## RuleUpdateFailureTypeDef

```python
# RuleUpdateFailureTypeDef definition

class RuleUpdateFailureTypeDef(TypedDict):
    failureCode: NotRequired[str],
    failureMessage: NotRequired[str],
    ruleIdentifier: NotRequired[str],
```

## CreateAccessLogSubscriptionRequestRequestTypeDef

```python
# CreateAccessLogSubscriptionRequestRequestTypeDef definition

class CreateAccessLogSubscriptionRequestRequestTypeDef(TypedDict):
    destinationArn: str,
    resourceIdentifier: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateServiceNetworkRequestRequestTypeDef

```python
# CreateServiceNetworkRequestRequestTypeDef definition

class CreateServiceNetworkRequestRequestTypeDef(TypedDict):
    name: str,
    authType: NotRequired[AuthTypeType],  # (1)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
## CreateServiceNetworkServiceAssociationRequestRequestTypeDef

```python
# CreateServiceNetworkServiceAssociationRequestRequestTypeDef definition

class CreateServiceNetworkServiceAssociationRequestRequestTypeDef(TypedDict):
    serviceIdentifier: str,
    serviceNetworkIdentifier: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## DnsEntryTypeDef

```python
# DnsEntryTypeDef definition

class DnsEntryTypeDef(TypedDict):
    domainName: NotRequired[str],
    hostedZoneId: NotRequired[str],
```

## CreateServiceNetworkVpcAssociationRequestRequestTypeDef

```python
# CreateServiceNetworkVpcAssociationRequestRequestTypeDef definition

class CreateServiceNetworkVpcAssociationRequestRequestTypeDef(TypedDict):
    serviceNetworkIdentifier: str,
    vpcIdentifier: str,
    clientToken: NotRequired[str],
    securityGroupIds: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
```

## CreateServiceRequestRequestTypeDef

```python
# CreateServiceRequestRequestTypeDef definition

class CreateServiceRequestRequestTypeDef(TypedDict):
    name: str,
    authType: NotRequired[AuthTypeType],  # (1)
    certificateArn: NotRequired[str],
    clientToken: NotRequired[str],
    customDomainName: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
## DeleteAccessLogSubscriptionRequestRequestTypeDef

```python
# DeleteAccessLogSubscriptionRequestRequestTypeDef definition

class DeleteAccessLogSubscriptionRequestRequestTypeDef(TypedDict):
    accessLogSubscriptionIdentifier: str,
```

## DeleteAuthPolicyRequestRequestTypeDef

```python
# DeleteAuthPolicyRequestRequestTypeDef definition

class DeleteAuthPolicyRequestRequestTypeDef(TypedDict):
    resourceIdentifier: str,
```

## DeleteListenerRequestRequestTypeDef

```python
# DeleteListenerRequestRequestTypeDef definition

class DeleteListenerRequestRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    serviceIdentifier: str,
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## DeleteRuleRequestRequestTypeDef

```python
# DeleteRuleRequestRequestTypeDef definition

class DeleteRuleRequestRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    ruleIdentifier: str,
    serviceIdentifier: str,
```

## DeleteServiceNetworkRequestRequestTypeDef

```python
# DeleteServiceNetworkRequestRequestTypeDef definition

class DeleteServiceNetworkRequestRequestTypeDef(TypedDict):
    serviceNetworkIdentifier: str,
```

## DeleteServiceNetworkServiceAssociationRequestRequestTypeDef

```python
# DeleteServiceNetworkServiceAssociationRequestRequestTypeDef definition

class DeleteServiceNetworkServiceAssociationRequestRequestTypeDef(TypedDict):
    serviceNetworkServiceAssociationIdentifier: str,
```

## DeleteServiceNetworkVpcAssociationRequestRequestTypeDef

```python
# DeleteServiceNetworkVpcAssociationRequestRequestTypeDef definition

class DeleteServiceNetworkVpcAssociationRequestRequestTypeDef(TypedDict):
    serviceNetworkVpcAssociationIdentifier: str,
```

## DeleteServiceRequestRequestTypeDef

```python
# DeleteServiceRequestRequestTypeDef definition

class DeleteServiceRequestRequestTypeDef(TypedDict):
    serviceIdentifier: str,
```

## DeleteTargetGroupRequestRequestTypeDef

```python
# DeleteTargetGroupRequestRequestTypeDef definition

class DeleteTargetGroupRequestRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
```

## TargetTypeDef

```python
# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    id: str,
    port: NotRequired[int],
```

## TargetFailureTypeDef

```python
# TargetFailureTypeDef definition

class TargetFailureTypeDef(TypedDict):
    failureCode: NotRequired[str],
    failureMessage: NotRequired[str],
    id: NotRequired[str],
    port: NotRequired[int],
```

## FixedResponseActionTypeDef

```python
# FixedResponseActionTypeDef definition

class FixedResponseActionTypeDef(TypedDict):
    statusCode: int,
```

## WeightedTargetGroupTypeDef

```python
# WeightedTargetGroupTypeDef definition

class WeightedTargetGroupTypeDef(TypedDict):
    targetGroupIdentifier: str,
    weight: NotRequired[int],
```

## GetAccessLogSubscriptionRequestRequestTypeDef

```python
# GetAccessLogSubscriptionRequestRequestTypeDef definition

class GetAccessLogSubscriptionRequestRequestTypeDef(TypedDict):
    accessLogSubscriptionIdentifier: str,
```

## GetAuthPolicyRequestRequestTypeDef

```python
# GetAuthPolicyRequestRequestTypeDef definition

class GetAuthPolicyRequestRequestTypeDef(TypedDict):
    resourceIdentifier: str,
```

## GetListenerRequestRequestTypeDef

```python
# GetListenerRequestRequestTypeDef definition

class GetListenerRequestRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    serviceIdentifier: str,
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## GetRuleRequestRequestTypeDef

```python
# GetRuleRequestRequestTypeDef definition

class GetRuleRequestRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    ruleIdentifier: str,
    serviceIdentifier: str,
```

## GetServiceNetworkRequestRequestTypeDef

```python
# GetServiceNetworkRequestRequestTypeDef definition

class GetServiceNetworkRequestRequestTypeDef(TypedDict):
    serviceNetworkIdentifier: str,
```

## GetServiceNetworkServiceAssociationRequestRequestTypeDef

```python
# GetServiceNetworkServiceAssociationRequestRequestTypeDef definition

class GetServiceNetworkServiceAssociationRequestRequestTypeDef(TypedDict):
    serviceNetworkServiceAssociationIdentifier: str,
```

## GetServiceNetworkVpcAssociationRequestRequestTypeDef

```python
# GetServiceNetworkVpcAssociationRequestRequestTypeDef definition

class GetServiceNetworkVpcAssociationRequestRequestTypeDef(TypedDict):
    serviceNetworkVpcAssociationIdentifier: str,
```

## GetServiceRequestRequestTypeDef

```python
# GetServiceRequestRequestTypeDef definition

class GetServiceRequestRequestTypeDef(TypedDict):
    serviceIdentifier: str,
```

## GetTargetGroupRequestRequestTypeDef

```python
# GetTargetGroupRequestRequestTypeDef definition

class GetTargetGroupRequestRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
```

## HeaderMatchTypeTypeDef

```python
# HeaderMatchTypeTypeDef definition

class HeaderMatchTypeTypeDef(TypedDict):
    contains: NotRequired[str],
    exact: NotRequired[str],
    prefix: NotRequired[str],
```

## MatcherTypeDef

```python
# MatcherTypeDef definition

class MatcherTypeDef(TypedDict):
    httpCode: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccessLogSubscriptionsRequestRequestTypeDef

```python
# ListAccessLogSubscriptionsRequestRequestTypeDef definition

class ListAccessLogSubscriptionsRequestRequestTypeDef(TypedDict):
    resourceIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListListenersRequestRequestTypeDef

```python
# ListListenersRequestRequestTypeDef definition

class ListListenersRequestRequestTypeDef(TypedDict):
    serviceIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListenerSummaryTypeDef

```python
# ListenerSummaryTypeDef definition

class ListenerSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    id: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    port: NotRequired[int],
    protocol: NotRequired[ListenerProtocolType],  # (1)
```

1. See [:material-code-brackets: ListenerProtocolType](./literals.md#listenerprotocoltype) 
## ListRulesRequestRequestTypeDef

```python
# ListRulesRequestRequestTypeDef definition

class ListRulesRequestRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    serviceIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## RuleSummaryTypeDef

```python
# RuleSummaryTypeDef definition

class RuleSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    id: NotRequired[str],
    isDefault: NotRequired[bool],
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    priority: NotRequired[int],
```

## ListServiceNetworkServiceAssociationsRequestRequestTypeDef

```python
# ListServiceNetworkServiceAssociationsRequestRequestTypeDef definition

class ListServiceNetworkServiceAssociationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    serviceIdentifier: NotRequired[str],
    serviceNetworkIdentifier: NotRequired[str],
```

## ListServiceNetworkVpcAssociationsRequestRequestTypeDef

```python
# ListServiceNetworkVpcAssociationsRequestRequestTypeDef definition

class ListServiceNetworkVpcAssociationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    serviceNetworkIdentifier: NotRequired[str],
    vpcIdentifier: NotRequired[str],
```

## ServiceNetworkVpcAssociationSummaryTypeDef

```python
# ServiceNetworkVpcAssociationSummaryTypeDef definition

class ServiceNetworkVpcAssociationSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    id: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    serviceNetworkArn: NotRequired[str],
    serviceNetworkId: NotRequired[str],
    serviceNetworkName: NotRequired[str],
    status: NotRequired[ServiceNetworkVpcAssociationStatusType],  # (1)
    vpcId: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNetworkVpcAssociationStatusType](./literals.md#servicenetworkvpcassociationstatustype) 
## ListServiceNetworksRequestRequestTypeDef

```python
# ListServiceNetworksRequestRequestTypeDef definition

class ListServiceNetworksRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceNetworkSummaryTypeDef

```python
# ServiceNetworkSummaryTypeDef definition

class ServiceNetworkSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    id: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    numberOfAssociatedServices: NotRequired[int],
    numberOfAssociatedVPCs: NotRequired[int],
```

## ListServicesRequestRequestTypeDef

```python
# ListServicesRequestRequestTypeDef definition

class ListServicesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTargetGroupsRequestRequestTypeDef

```python
# ListTargetGroupsRequestRequestTypeDef definition

class ListTargetGroupsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    targetGroupType: NotRequired[TargetGroupTypeType],  # (1)
    vpcIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
## TargetGroupSummaryTypeDef

```python
# TargetGroupSummaryTypeDef definition

class TargetGroupSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    id: NotRequired[str],
    ipAddressType: NotRequired[IpAddressTypeType],  # (1)
    lambdaEventStructureVersion: NotRequired[LambdaEventStructureVersionType],  # (2)
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    port: NotRequired[int],
    protocol: NotRequired[TargetGroupProtocolType],  # (3)
    serviceArns: NotRequired[List[str]],
    status: NotRequired[TargetGroupStatusType],  # (4)
    type: NotRequired[TargetGroupTypeType],  # (5)
    vpcIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
2. See [:material-code-brackets: LambdaEventStructureVersionType](./literals.md#lambdaeventstructureversiontype) 
3. See [:material-code-brackets: TargetGroupProtocolType](./literals.md#targetgroupprotocoltype) 
4. See [:material-code-brackets: TargetGroupStatusType](./literals.md#targetgroupstatustype) 
5. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
## TargetSummaryTypeDef

```python
# TargetSummaryTypeDef definition

class TargetSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    port: NotRequired[int],
    reasonCode: NotRequired[str],
    status: NotRequired[TargetStatusType],  # (1)
```

1. See [:material-code-brackets: TargetStatusType](./literals.md#targetstatustype) 
## PathMatchTypeTypeDef

```python
# PathMatchTypeTypeDef definition

class PathMatchTypeTypeDef(TypedDict):
    exact: NotRequired[str],
    prefix: NotRequired[str],
```

## PutAuthPolicyRequestRequestTypeDef

```python
# PutAuthPolicyRequestRequestTypeDef definition

class PutAuthPolicyRequestRequestTypeDef(TypedDict):
    policy: str,
    resourceIdentifier: str,
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    policy: str,
    resourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAccessLogSubscriptionRequestRequestTypeDef

```python
# UpdateAccessLogSubscriptionRequestRequestTypeDef definition

class UpdateAccessLogSubscriptionRequestRequestTypeDef(TypedDict):
    accessLogSubscriptionIdentifier: str,
    destinationArn: str,
```

## UpdateServiceNetworkRequestRequestTypeDef

```python
# UpdateServiceNetworkRequestRequestTypeDef definition

class UpdateServiceNetworkRequestRequestTypeDef(TypedDict):
    authType: AuthTypeType,  # (1)
    serviceNetworkIdentifier: str,
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
## UpdateServiceNetworkVpcAssociationRequestRequestTypeDef

```python
# UpdateServiceNetworkVpcAssociationRequestRequestTypeDef definition

class UpdateServiceNetworkVpcAssociationRequestRequestTypeDef(TypedDict):
    securityGroupIds: Sequence[str],
    serviceNetworkVpcAssociationIdentifier: str,
```

## UpdateServiceRequestRequestTypeDef

```python
# UpdateServiceRequestRequestTypeDef definition

class UpdateServiceRequestRequestTypeDef(TypedDict):
    serviceIdentifier: str,
    authType: NotRequired[AuthTypeType],  # (1)
    certificateArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
## CreateAccessLogSubscriptionResponseTypeDef

```python
# CreateAccessLogSubscriptionResponseTypeDef definition

class CreateAccessLogSubscriptionResponseTypeDef(TypedDict):
    arn: str,
    destinationArn: str,
    id: str,
    resourceArn: str,
    resourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceNetworkResponseTypeDef

```python
# CreateServiceNetworkResponseTypeDef definition

class CreateServiceNetworkResponseTypeDef(TypedDict):
    arn: str,
    authType: AuthTypeType,  # (1)
    id: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceNetworkVpcAssociationResponseTypeDef

```python
# CreateServiceNetworkVpcAssociationResponseTypeDef definition

class CreateServiceNetworkVpcAssociationResponseTypeDef(TypedDict):
    arn: str,
    createdBy: str,
    id: str,
    securityGroupIds: List[str],
    status: ServiceNetworkVpcAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceNetworkVpcAssociationStatusType](./literals.md#servicenetworkvpcassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceNetworkServiceAssociationResponseTypeDef

```python
# DeleteServiceNetworkServiceAssociationResponseTypeDef definition

class DeleteServiceNetworkServiceAssociationResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    status: ServiceNetworkServiceAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceNetworkServiceAssociationStatusType](./literals.md#servicenetworkserviceassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceNetworkVpcAssociationResponseTypeDef

```python
# DeleteServiceNetworkVpcAssociationResponseTypeDef definition

class DeleteServiceNetworkVpcAssociationResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    status: ServiceNetworkVpcAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceNetworkVpcAssociationStatusType](./literals.md#servicenetworkvpcassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceResponseTypeDef

```python
# DeleteServiceResponseTypeDef definition

class DeleteServiceResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    status: ServiceStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceStatusType](./literals.md#servicestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTargetGroupResponseTypeDef

```python
# DeleteTargetGroupResponseTypeDef definition

class DeleteTargetGroupResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    status: TargetGroupStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TargetGroupStatusType](./literals.md#targetgroupstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccessLogSubscriptionResponseTypeDef

```python
# GetAccessLogSubscriptionResponseTypeDef definition

class GetAccessLogSubscriptionResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    destinationArn: str,
    id: str,
    lastUpdatedAt: datetime,
    resourceArn: str,
    resourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAuthPolicyResponseTypeDef

```python
# GetAuthPolicyResponseTypeDef definition

class GetAuthPolicyResponseTypeDef(TypedDict):
    createdAt: datetime,
    lastUpdatedAt: datetime,
    policy: str,
    state: AuthPolicyStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuthPolicyStateType](./literals.md#authpolicystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceNetworkResponseTypeDef

```python
# GetServiceNetworkResponseTypeDef definition

class GetServiceNetworkResponseTypeDef(TypedDict):
    arn: str,
    authType: AuthTypeType,  # (1)
    createdAt: datetime,
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    numberOfAssociatedServices: int,
    numberOfAssociatedVPCs: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceNetworkVpcAssociationResponseTypeDef

```python
# GetServiceNetworkVpcAssociationResponseTypeDef definition

class GetServiceNetworkVpcAssociationResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    createdBy: str,
    failureCode: str,
    failureMessage: str,
    id: str,
    lastUpdatedAt: datetime,
    securityGroupIds: List[str],
    serviceNetworkArn: str,
    serviceNetworkId: str,
    serviceNetworkName: str,
    status: ServiceNetworkVpcAssociationStatusType,  # (1)
    vpcId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceNetworkVpcAssociationStatusType](./literals.md#servicenetworkvpcassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessLogSubscriptionsResponseTypeDef

```python
# ListAccessLogSubscriptionsResponseTypeDef definition

class ListAccessLogSubscriptionsResponseTypeDef(TypedDict):
    items: List[AccessLogSubscriptionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccessLogSubscriptionSummaryTypeDef](./type_defs.md#accesslogsubscriptionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAuthPolicyResponseTypeDef

```python
# PutAuthPolicyResponseTypeDef definition

class PutAuthPolicyResponseTypeDef(TypedDict):
    policy: str,
    state: AuthPolicyStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuthPolicyStateType](./literals.md#authpolicystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccessLogSubscriptionResponseTypeDef

```python
# UpdateAccessLogSubscriptionResponseTypeDef definition

class UpdateAccessLogSubscriptionResponseTypeDef(TypedDict):
    arn: str,
    destinationArn: str,
    id: str,
    resourceArn: str,
    resourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceNetworkResponseTypeDef

```python
# UpdateServiceNetworkResponseTypeDef definition

class UpdateServiceNetworkResponseTypeDef(TypedDict):
    arn: str,
    authType: AuthTypeType,  # (1)
    id: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceNetworkVpcAssociationResponseTypeDef

```python
# UpdateServiceNetworkVpcAssociationResponseTypeDef definition

class UpdateServiceNetworkVpcAssociationResponseTypeDef(TypedDict):
    arn: str,
    createdBy: str,
    id: str,
    securityGroupIds: List[str],
    status: ServiceNetworkVpcAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceNetworkVpcAssociationStatusType](./literals.md#servicenetworkvpcassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceResponseTypeDef

```python
# UpdateServiceResponseTypeDef definition

class UpdateServiceResponseTypeDef(TypedDict):
    arn: str,
    authType: AuthTypeType,  # (1)
    certificateArn: str,
    customDomainName: str,
    id: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceNetworkServiceAssociationResponseTypeDef

```python
# CreateServiceNetworkServiceAssociationResponseTypeDef definition

class CreateServiceNetworkServiceAssociationResponseTypeDef(TypedDict):
    arn: str,
    createdBy: str,
    customDomainName: str,
    dnsEntry: DnsEntryTypeDef,  # (1)
    id: str,
    status: ServiceNetworkServiceAssociationStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
2. See [:material-code-brackets: ServiceNetworkServiceAssociationStatusType](./literals.md#servicenetworkserviceassociationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceResponseTypeDef

```python
# CreateServiceResponseTypeDef definition

class CreateServiceResponseTypeDef(TypedDict):
    arn: str,
    authType: AuthTypeType,  # (1)
    certificateArn: str,
    customDomainName: str,
    dnsEntry: DnsEntryTypeDef,  # (2)
    id: str,
    name: str,
    status: ServiceStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
3. See [:material-code-brackets: ServiceStatusType](./literals.md#servicestatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceNetworkServiceAssociationResponseTypeDef

```python
# GetServiceNetworkServiceAssociationResponseTypeDef definition

class GetServiceNetworkServiceAssociationResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    createdBy: str,
    customDomainName: str,
    dnsEntry: DnsEntryTypeDef,  # (1)
    failureCode: str,
    failureMessage: str,
    id: str,
    serviceArn: str,
    serviceId: str,
    serviceName: str,
    serviceNetworkArn: str,
    serviceNetworkId: str,
    serviceNetworkName: str,
    status: ServiceNetworkServiceAssociationStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
2. See [:material-code-brackets: ServiceNetworkServiceAssociationStatusType](./literals.md#servicenetworkserviceassociationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceResponseTypeDef

```python
# GetServiceResponseTypeDef definition

class GetServiceResponseTypeDef(TypedDict):
    arn: str,
    authType: AuthTypeType,  # (1)
    certificateArn: str,
    createdAt: datetime,
    customDomainName: str,
    dnsEntry: DnsEntryTypeDef,  # (2)
    failureCode: str,
    failureMessage: str,
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    status: ServiceStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
3. See [:material-code-brackets: ServiceStatusType](./literals.md#servicestatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceNetworkServiceAssociationSummaryTypeDef

```python
# ServiceNetworkServiceAssociationSummaryTypeDef definition

class ServiceNetworkServiceAssociationSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    customDomainName: NotRequired[str],
    dnsEntry: NotRequired[DnsEntryTypeDef],  # (1)
    id: NotRequired[str],
    serviceArn: NotRequired[str],
    serviceId: NotRequired[str],
    serviceName: NotRequired[str],
    serviceNetworkArn: NotRequired[str],
    serviceNetworkId: NotRequired[str],
    serviceNetworkName: NotRequired[str],
    status: NotRequired[ServiceNetworkServiceAssociationStatusType],  # (2)
```

1. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
2. See [:material-code-brackets: ServiceNetworkServiceAssociationStatusType](./literals.md#servicenetworkserviceassociationstatustype) 
## ServiceSummaryTypeDef

```python
# ServiceSummaryTypeDef definition

class ServiceSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    customDomainName: NotRequired[str],
    dnsEntry: NotRequired[DnsEntryTypeDef],  # (1)
    id: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    status: NotRequired[ServiceStatusType],  # (2)
```

1. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
2. See [:material-code-brackets: ServiceStatusType](./literals.md#servicestatustype) 
## DeregisterTargetsRequestRequestTypeDef

```python
# DeregisterTargetsRequestRequestTypeDef definition

class DeregisterTargetsRequestRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
    targets: Sequence[TargetTypeDef],  # (1)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## ListTargetsRequestRequestTypeDef

```python
# ListTargetsRequestRequestTypeDef definition

class ListTargetsRequestRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    targets: NotRequired[Sequence[TargetTypeDef]],  # (1)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## RegisterTargetsRequestRequestTypeDef

```python
# RegisterTargetsRequestRequestTypeDef definition

class RegisterTargetsRequestRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
    targets: Sequence[TargetTypeDef],  # (1)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## DeregisterTargetsResponseTypeDef

```python
# DeregisterTargetsResponseTypeDef definition

class DeregisterTargetsResponseTypeDef(TypedDict):
    successful: List[TargetTypeDef],  # (1)
    unsuccessful: List[TargetFailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: TargetFailureTypeDef](./type_defs.md#targetfailuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterTargetsResponseTypeDef

```python
# RegisterTargetsResponseTypeDef definition

class RegisterTargetsResponseTypeDef(TypedDict):
    successful: List[TargetTypeDef],  # (1)
    unsuccessful: List[TargetFailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: TargetFailureTypeDef](./type_defs.md#targetfailuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ForwardActionOutputTypeDef

```python
# ForwardActionOutputTypeDef definition

class ForwardActionOutputTypeDef(TypedDict):
    targetGroups: List[WeightedTargetGroupTypeDef],  # (1)
```

1. See [:material-code-braces: WeightedTargetGroupTypeDef](./type_defs.md#weightedtargetgrouptypedef) 
## ForwardActionTypeDef

```python
# ForwardActionTypeDef definition

class ForwardActionTypeDef(TypedDict):
    targetGroups: Sequence[WeightedTargetGroupTypeDef],  # (1)
```

1. See [:material-code-braces: WeightedTargetGroupTypeDef](./type_defs.md#weightedtargetgrouptypedef) 
## HeaderMatchTypeDef

```python
# HeaderMatchTypeDef definition

class HeaderMatchTypeDef(TypedDict):
    match: HeaderMatchTypeTypeDef,  # (1)
    name: str,
    caseSensitive: NotRequired[bool],
```

1. See [:material-code-braces: HeaderMatchTypeTypeDef](./type_defs.md#headermatchtypetypedef) 
## HealthCheckConfigTypeDef

```python
# HealthCheckConfigTypeDef definition

class HealthCheckConfigTypeDef(TypedDict):
    enabled: NotRequired[bool],
    healthCheckIntervalSeconds: NotRequired[int],
    healthCheckTimeoutSeconds: NotRequired[int],
    healthyThresholdCount: NotRequired[int],
    matcher: NotRequired[MatcherTypeDef],  # (1)
    path: NotRequired[str],
    port: NotRequired[int],
    protocol: NotRequired[TargetGroupProtocolType],  # (2)
    protocolVersion: NotRequired[HealthCheckProtocolVersionType],  # (3)
    unhealthyThresholdCount: NotRequired[int],
```

1. See [:material-code-braces: MatcherTypeDef](./type_defs.md#matchertypedef) 
2. See [:material-code-brackets: TargetGroupProtocolType](./literals.md#targetgroupprotocoltype) 
3. See [:material-code-brackets: HealthCheckProtocolVersionType](./literals.md#healthcheckprotocolversiontype) 
## ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef

```python
# ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef definition

class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(TypedDict):
    resourceIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListListenersRequestListListenersPaginateTypeDef

```python
# ListListenersRequestListListenersPaginateTypeDef definition

class ListListenersRequestListListenersPaginateTypeDef(TypedDict):
    serviceIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesRequestListRulesPaginateTypeDef

```python
# ListRulesRequestListRulesPaginateTypeDef definition

class ListRulesRequestListRulesPaginateTypeDef(TypedDict):
    listenerIdentifier: str,
    serviceIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef

```python
# ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef definition

class ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef(TypedDict):
    serviceIdentifier: NotRequired[str],
    serviceNetworkIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef

```python
# ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef definition

class ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef(TypedDict):
    serviceNetworkIdentifier: NotRequired[str],
    vpcIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceNetworksRequestListServiceNetworksPaginateTypeDef

```python
# ListServiceNetworksRequestListServiceNetworksPaginateTypeDef definition

class ListServiceNetworksRequestListServiceNetworksPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesRequestListServicesPaginateTypeDef

```python
# ListServicesRequestListServicesPaginateTypeDef definition

class ListServicesRequestListServicesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTargetGroupsRequestListTargetGroupsPaginateTypeDef

```python
# ListTargetGroupsRequestListTargetGroupsPaginateTypeDef definition

class ListTargetGroupsRequestListTargetGroupsPaginateTypeDef(TypedDict):
    targetGroupType: NotRequired[TargetGroupTypeType],  # (1)
    vpcIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTargetsRequestListTargetsPaginateTypeDef

```python
# ListTargetsRequestListTargetsPaginateTypeDef definition

class ListTargetsRequestListTargetsPaginateTypeDef(TypedDict):
    targetGroupIdentifier: str,
    targets: NotRequired[Sequence[TargetTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListListenersResponseTypeDef

```python
# ListListenersResponseTypeDef definition

class ListListenersResponseTypeDef(TypedDict):
    items: List[ListenerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListenerSummaryTypeDef](./type_defs.md#listenersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRulesResponseTypeDef

```python
# ListRulesResponseTypeDef definition

class ListRulesResponseTypeDef(TypedDict):
    items: List[RuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceNetworkVpcAssociationsResponseTypeDef

```python
# ListServiceNetworkVpcAssociationsResponseTypeDef definition

class ListServiceNetworkVpcAssociationsResponseTypeDef(TypedDict):
    items: List[ServiceNetworkVpcAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceNetworkVpcAssociationSummaryTypeDef](./type_defs.md#servicenetworkvpcassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceNetworksResponseTypeDef

```python
# ListServiceNetworksResponseTypeDef definition

class ListServiceNetworksResponseTypeDef(TypedDict):
    items: List[ServiceNetworkSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceNetworkSummaryTypeDef](./type_defs.md#servicenetworksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetGroupsResponseTypeDef

```python
# ListTargetGroupsResponseTypeDef definition

class ListTargetGroupsResponseTypeDef(TypedDict):
    items: List[TargetGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetGroupSummaryTypeDef](./type_defs.md#targetgroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetsResponseTypeDef

```python
# ListTargetsResponseTypeDef definition

class ListTargetsResponseTypeDef(TypedDict):
    items: List[TargetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetSummaryTypeDef](./type_defs.md#targetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PathMatchTypeDef

```python
# PathMatchTypeDef definition

class PathMatchTypeDef(TypedDict):
    match: PathMatchTypeTypeDef,  # (1)
    caseSensitive: NotRequired[bool],
```

1. See [:material-code-braces: PathMatchTypeTypeDef](./type_defs.md#pathmatchtypetypedef) 
## ListServiceNetworkServiceAssociationsResponseTypeDef

```python
# ListServiceNetworkServiceAssociationsResponseTypeDef definition

class ListServiceNetworkServiceAssociationsResponseTypeDef(TypedDict):
    items: List[ServiceNetworkServiceAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceNetworkServiceAssociationSummaryTypeDef](./type_defs.md#servicenetworkserviceassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicesResponseTypeDef

```python
# ListServicesResponseTypeDef definition

class ListServicesResponseTypeDef(TypedDict):
    items: List[ServiceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleActionOutputTypeDef

```python
# RuleActionOutputTypeDef definition

class RuleActionOutputTypeDef(TypedDict):
    fixedResponse: NotRequired[FixedResponseActionTypeDef],  # (1)
    forward: NotRequired[ForwardActionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: FixedResponseActionTypeDef](./type_defs.md#fixedresponseactiontypedef) 
2. See [:material-code-braces: ForwardActionOutputTypeDef](./type_defs.md#forwardactionoutputtypedef) 
## TargetGroupConfigTypeDef

```python
# TargetGroupConfigTypeDef definition

class TargetGroupConfigTypeDef(TypedDict):
    healthCheck: NotRequired[HealthCheckConfigTypeDef],  # (1)
    ipAddressType: NotRequired[IpAddressTypeType],  # (2)
    lambdaEventStructureVersion: NotRequired[LambdaEventStructureVersionType],  # (3)
    port: NotRequired[int],
    protocol: NotRequired[TargetGroupProtocolType],  # (4)
    protocolVersion: NotRequired[TargetGroupProtocolVersionType],  # (5)
    vpcIdentifier: NotRequired[str],
```

1. See [:material-code-braces: HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef) 
2. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
3. See [:material-code-brackets: LambdaEventStructureVersionType](./literals.md#lambdaeventstructureversiontype) 
4. See [:material-code-brackets: TargetGroupProtocolType](./literals.md#targetgroupprotocoltype) 
5. See [:material-code-brackets: TargetGroupProtocolVersionType](./literals.md#targetgroupprotocolversiontype) 
## UpdateTargetGroupRequestRequestTypeDef

```python
# UpdateTargetGroupRequestRequestTypeDef definition

class UpdateTargetGroupRequestRequestTypeDef(TypedDict):
    healthCheck: HealthCheckConfigTypeDef,  # (1)
    targetGroupIdentifier: str,
```

1. See [:material-code-braces: HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef) 
## HttpMatchOutputTypeDef

```python
# HttpMatchOutputTypeDef definition

class HttpMatchOutputTypeDef(TypedDict):
    headerMatches: NotRequired[List[HeaderMatchTypeDef]],  # (1)
    method: NotRequired[str],
    pathMatch: NotRequired[PathMatchTypeDef],  # (2)
```

1. See [:material-code-braces: HeaderMatchTypeDef](./type_defs.md#headermatchtypedef) 
2. See [:material-code-braces: PathMatchTypeDef](./type_defs.md#pathmatchtypedef) 
## HttpMatchTypeDef

```python
# HttpMatchTypeDef definition

class HttpMatchTypeDef(TypedDict):
    headerMatches: NotRequired[Sequence[HeaderMatchTypeDef]],  # (1)
    method: NotRequired[str],
    pathMatch: NotRequired[PathMatchTypeDef],  # (2)
```

1. See [:material-code-braces: HeaderMatchTypeDef](./type_defs.md#headermatchtypedef) 
2. See [:material-code-braces: PathMatchTypeDef](./type_defs.md#pathmatchtypedef) 
## CreateListenerResponseTypeDef

```python
# CreateListenerResponseTypeDef definition

class CreateListenerResponseTypeDef(TypedDict):
    arn: str,
    defaultAction: RuleActionOutputTypeDef,  # (1)
    id: str,
    name: str,
    port: int,
    protocol: ListenerProtocolType,  # (2)
    serviceArn: str,
    serviceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-brackets: ListenerProtocolType](./literals.md#listenerprotocoltype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetListenerResponseTypeDef

```python
# GetListenerResponseTypeDef definition

class GetListenerResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    defaultAction: RuleActionOutputTypeDef,  # (1)
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    port: int,
    protocol: ListenerProtocolType,  # (2)
    serviceArn: str,
    serviceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-brackets: ListenerProtocolType](./literals.md#listenerprotocoltype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateListenerResponseTypeDef

```python
# UpdateListenerResponseTypeDef definition

class UpdateListenerResponseTypeDef(TypedDict):
    arn: str,
    defaultAction: RuleActionOutputTypeDef,  # (1)
    id: str,
    name: str,
    port: int,
    protocol: ListenerProtocolType,  # (2)
    serviceArn: str,
    serviceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-brackets: ListenerProtocolType](./literals.md#listenerprotocoltype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleActionTypeDef

```python
# RuleActionTypeDef definition

class RuleActionTypeDef(TypedDict):
    fixedResponse: NotRequired[FixedResponseActionTypeDef],  # (1)
    forward: NotRequired[ForwardActionUnionTypeDef],  # (2)
```

1. See [:material-code-braces: FixedResponseActionTypeDef](./type_defs.md#fixedresponseactiontypedef) 
2. See [:material-code-braces: ForwardActionTypeDef](./type_defs.md#forwardactiontypedef) [:material-code-braces: ForwardActionOutputTypeDef](./type_defs.md#forwardactionoutputtypedef) 
## CreateTargetGroupRequestRequestTypeDef

```python
# CreateTargetGroupRequestRequestTypeDef definition

class CreateTargetGroupRequestRequestTypeDef(TypedDict):
    name: str,
    type: TargetGroupTypeType,  # (1)
    clientToken: NotRequired[str],
    config: NotRequired[TargetGroupConfigTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
2. See [:material-code-braces: TargetGroupConfigTypeDef](./type_defs.md#targetgroupconfigtypedef) 
## CreateTargetGroupResponseTypeDef

```python
# CreateTargetGroupResponseTypeDef definition

class CreateTargetGroupResponseTypeDef(TypedDict):
    arn: str,
    config: TargetGroupConfigTypeDef,  # (1)
    id: str,
    name: str,
    status: TargetGroupStatusType,  # (2)
    type: TargetGroupTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TargetGroupConfigTypeDef](./type_defs.md#targetgroupconfigtypedef) 
2. See [:material-code-brackets: TargetGroupStatusType](./literals.md#targetgroupstatustype) 
3. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTargetGroupResponseTypeDef

```python
# GetTargetGroupResponseTypeDef definition

class GetTargetGroupResponseTypeDef(TypedDict):
    arn: str,
    config: TargetGroupConfigTypeDef,  # (1)
    createdAt: datetime,
    failureCode: str,
    failureMessage: str,
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    serviceArns: List[str],
    status: TargetGroupStatusType,  # (2)
    type: TargetGroupTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TargetGroupConfigTypeDef](./type_defs.md#targetgroupconfigtypedef) 
2. See [:material-code-brackets: TargetGroupStatusType](./literals.md#targetgroupstatustype) 
3. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTargetGroupResponseTypeDef

```python
# UpdateTargetGroupResponseTypeDef definition

class UpdateTargetGroupResponseTypeDef(TypedDict):
    arn: str,
    config: TargetGroupConfigTypeDef,  # (1)
    id: str,
    name: str,
    status: TargetGroupStatusType,  # (2)
    type: TargetGroupTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TargetGroupConfigTypeDef](./type_defs.md#targetgroupconfigtypedef) 
2. See [:material-code-brackets: TargetGroupStatusType](./literals.md#targetgroupstatustype) 
3. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleMatchOutputTypeDef

```python
# RuleMatchOutputTypeDef definition

class RuleMatchOutputTypeDef(TypedDict):
    httpMatch: NotRequired[HttpMatchOutputTypeDef],  # (1)
```

1. See [:material-code-braces: HttpMatchOutputTypeDef](./type_defs.md#httpmatchoutputtypedef) 
## CreateListenerRequestRequestTypeDef

```python
# CreateListenerRequestRequestTypeDef definition

class CreateListenerRequestRequestTypeDef(TypedDict):
    defaultAction: RuleActionTypeDef,  # (1)
    name: str,
    protocol: ListenerProtocolType,  # (2)
    serviceIdentifier: str,
    clientToken: NotRequired[str],
    port: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-brackets: ListenerProtocolType](./literals.md#listenerprotocoltype) 
## UpdateListenerRequestRequestTypeDef

```python
# UpdateListenerRequestRequestTypeDef definition

class UpdateListenerRequestRequestTypeDef(TypedDict):
    defaultAction: RuleActionTypeDef,  # (1)
    listenerIdentifier: str,
    serviceIdentifier: str,
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
## CreateRuleResponseTypeDef

```python
# CreateRuleResponseTypeDef definition

class CreateRuleResponseTypeDef(TypedDict):
    action: RuleActionOutputTypeDef,  # (1)
    arn: str,
    id: str,
    match: RuleMatchOutputTypeDef,  # (2)
    name: str,
    priority: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRuleResponseTypeDef

```python
# GetRuleResponseTypeDef definition

class GetRuleResponseTypeDef(TypedDict):
    action: RuleActionOutputTypeDef,  # (1)
    arn: str,
    createdAt: datetime,
    id: str,
    isDefault: bool,
    lastUpdatedAt: datetime,
    match: RuleMatchOutputTypeDef,  # (2)
    name: str,
    priority: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleUpdateSuccessTypeDef

```python
# RuleUpdateSuccessTypeDef definition

class RuleUpdateSuccessTypeDef(TypedDict):
    action: NotRequired[RuleActionOutputTypeDef],  # (1)
    arn: NotRequired[str],
    id: NotRequired[str],
    isDefault: NotRequired[bool],
    match: NotRequired[RuleMatchOutputTypeDef],  # (2)
    name: NotRequired[str],
    priority: NotRequired[int],
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef) 
## UpdateRuleResponseTypeDef

```python
# UpdateRuleResponseTypeDef definition

class UpdateRuleResponseTypeDef(TypedDict):
    action: RuleActionOutputTypeDef,  # (1)
    arn: str,
    id: str,
    isDefault: bool,
    match: RuleMatchOutputTypeDef,  # (2)
    name: str,
    priority: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleMatchTypeDef

```python
# RuleMatchTypeDef definition

class RuleMatchTypeDef(TypedDict):
    httpMatch: NotRequired[HttpMatchUnionTypeDef],  # (1)
```

1. See [:material-code-braces: HttpMatchTypeDef](./type_defs.md#httpmatchtypedef) [:material-code-braces: HttpMatchOutputTypeDef](./type_defs.md#httpmatchoutputtypedef) 
## BatchUpdateRuleResponseTypeDef

```python
# BatchUpdateRuleResponseTypeDef definition

class BatchUpdateRuleResponseTypeDef(TypedDict):
    successful: List[RuleUpdateSuccessTypeDef],  # (1)
    unsuccessful: List[RuleUpdateFailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuleUpdateSuccessTypeDef](./type_defs.md#ruleupdatesuccesstypedef) 
2. See [:material-code-braces: RuleUpdateFailureTypeDef](./type_defs.md#ruleupdatefailuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleRequestRequestTypeDef

```python
# CreateRuleRequestRequestTypeDef definition

class CreateRuleRequestRequestTypeDef(TypedDict):
    action: RuleActionTypeDef,  # (1)
    listenerIdentifier: str,
    match: RuleMatchTypeDef,  # (2)
    name: str,
    priority: int,
    serviceIdentifier: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-braces: RuleMatchTypeDef](./type_defs.md#rulematchtypedef) 
## UpdateRuleRequestRequestTypeDef

```python
# UpdateRuleRequestRequestTypeDef definition

class UpdateRuleRequestRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    ruleIdentifier: str,
    serviceIdentifier: str,
    action: NotRequired[RuleActionTypeDef],  # (1)
    match: NotRequired[RuleMatchTypeDef],  # (2)
    priority: NotRequired[int],
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-braces: RuleMatchTypeDef](./type_defs.md#rulematchtypedef) 
## RuleUpdateTypeDef

```python
# RuleUpdateTypeDef definition

class RuleUpdateTypeDef(TypedDict):
    ruleIdentifier: str,
    action: NotRequired[RuleActionUnionTypeDef],  # (1)
    match: NotRequired[RuleMatchUnionTypeDef],  # (2)
    priority: NotRequired[int],
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleMatchTypeDef](./type_defs.md#rulematchtypedef) [:material-code-braces: RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef) 
## BatchUpdateRuleRequestRequestTypeDef

```python
# BatchUpdateRuleRequestRequestTypeDef definition

class BatchUpdateRuleRequestRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    rules: Sequence[RuleUpdateTypeDef],  # (1)
    serviceIdentifier: str,
```

1. See [:material-code-braces: RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef) 
