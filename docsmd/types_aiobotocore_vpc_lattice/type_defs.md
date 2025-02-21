# Type definitions

> [Index](../README.md) > [VPCLattice](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [VPCLattice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#vpclattice)
    type annotations stubs module [types-aiobotocore-vpc-lattice](https://pypi.org/project/types-aiobotocore-vpc-lattice/).

## ForwardActionUnionTypeDef

```python
# ForwardActionUnionTypeDef Union usage example

from types_aiobotocore_vpc_lattice.type_defs import ForwardActionUnionTypeDef


def get_value() -> ForwardActionUnionTypeDef:
    return ...


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
# HttpMatchUnionTypeDef Union usage example

from types_aiobotocore_vpc_lattice.type_defs import HttpMatchUnionTypeDef


def get_value() -> HttpMatchUnionTypeDef:
    return ...


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
# RuleActionUnionTypeDef Union usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleActionUnionTypeDef


def get_value() -> RuleActionUnionTypeDef:
    return ...


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
# RuleMatchUnionTypeDef Union usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleMatchUnionTypeDef


def get_value() -> RuleMatchUnionTypeDef:
    return ...


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
# AccessLogSubscriptionSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import AccessLogSubscriptionSummaryTypeDef


def get_value() -> AccessLogSubscriptionSummaryTypeDef:
    return {
        "arn": ...,
    }


# AccessLogSubscriptionSummaryTypeDef definition

class AccessLogSubscriptionSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    destinationArn: str,
    id: str,
    lastUpdatedAt: datetime,
    resourceArn: str,
    resourceId: str,
    serviceNetworkLogType: NotRequired[ServiceNetworkLogTypeType],  # (1)
```

1. See [:material-code-brackets: ServiceNetworkLogTypeType](./literals.md#servicenetworklogtypetype) 
## ArnResourceTypeDef

```python
# ArnResourceTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ArnResourceTypeDef


def get_value() -> ArnResourceTypeDef:
    return {
        "arn": ...,
    }


# ArnResourceTypeDef definition

class ArnResourceTypeDef(TypedDict):
    arn: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


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
# RuleUpdateFailureTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleUpdateFailureTypeDef


def get_value() -> RuleUpdateFailureTypeDef:
    return {
        "failureCode": ...,
    }


# RuleUpdateFailureTypeDef definition

class RuleUpdateFailureTypeDef(TypedDict):
    failureCode: NotRequired[str],
    failureMessage: NotRequired[str],
    ruleIdentifier: NotRequired[str],
```

## CreateAccessLogSubscriptionRequestTypeDef

```python
# CreateAccessLogSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateAccessLogSubscriptionRequestTypeDef


def get_value() -> CreateAccessLogSubscriptionRequestTypeDef:
    return {
        "destinationArn": ...,
    }


# CreateAccessLogSubscriptionRequestTypeDef definition

class CreateAccessLogSubscriptionRequestTypeDef(TypedDict):
    destinationArn: str,
    resourceIdentifier: str,
    clientToken: NotRequired[str],
    serviceNetworkLogType: NotRequired[ServiceNetworkLogTypeType],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ServiceNetworkLogTypeType](./literals.md#servicenetworklogtypetype) 
## CreateResourceGatewayRequestTypeDef

```python
# CreateResourceGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateResourceGatewayRequestTypeDef


def get_value() -> CreateResourceGatewayRequestTypeDef:
    return {
        "name": ...,
    }


# CreateResourceGatewayRequestTypeDef definition

class CreateResourceGatewayRequestTypeDef(TypedDict):
    name: str,
    subnetIds: Sequence[str],
    vpcIdentifier: str,
    clientToken: NotRequired[str],
    ipAddressType: NotRequired[ResourceGatewayIpAddressTypeType],  # (1)
    securityGroupIds: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ResourceGatewayIpAddressTypeType](./literals.md#resourcegatewayipaddresstypetype) 
## SharingConfigTypeDef

```python
# SharingConfigTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import SharingConfigTypeDef


def get_value() -> SharingConfigTypeDef:
    return {
        "enabled": ...,
    }


# SharingConfigTypeDef definition

class SharingConfigTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## CreateServiceNetworkResourceAssociationRequestTypeDef

```python
# CreateServiceNetworkResourceAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceNetworkResourceAssociationRequestTypeDef


def get_value() -> CreateServiceNetworkResourceAssociationRequestTypeDef:
    return {
        "resourceConfigurationIdentifier": ...,
    }


# CreateServiceNetworkResourceAssociationRequestTypeDef definition

class CreateServiceNetworkResourceAssociationRequestTypeDef(TypedDict):
    resourceConfigurationIdentifier: str,
    serviceNetworkIdentifier: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateServiceNetworkServiceAssociationRequestTypeDef

```python
# CreateServiceNetworkServiceAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceNetworkServiceAssociationRequestTypeDef


def get_value() -> CreateServiceNetworkServiceAssociationRequestTypeDef:
    return {
        "serviceIdentifier": ...,
    }


# CreateServiceNetworkServiceAssociationRequestTypeDef definition

class CreateServiceNetworkServiceAssociationRequestTypeDef(TypedDict):
    serviceIdentifier: str,
    serviceNetworkIdentifier: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## DnsEntryTypeDef

```python
# DnsEntryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DnsEntryTypeDef


def get_value() -> DnsEntryTypeDef:
    return {
        "domainName": ...,
    }


# DnsEntryTypeDef definition

class DnsEntryTypeDef(TypedDict):
    domainName: NotRequired[str],
    hostedZoneId: NotRequired[str],
```

## CreateServiceNetworkVpcAssociationRequestTypeDef

```python
# CreateServiceNetworkVpcAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceNetworkVpcAssociationRequestTypeDef


def get_value() -> CreateServiceNetworkVpcAssociationRequestTypeDef:
    return {
        "serviceNetworkIdentifier": ...,
    }


# CreateServiceNetworkVpcAssociationRequestTypeDef definition

class CreateServiceNetworkVpcAssociationRequestTypeDef(TypedDict):
    serviceNetworkIdentifier: str,
    vpcIdentifier: str,
    clientToken: NotRequired[str],
    securityGroupIds: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
```

## CreateServiceRequestTypeDef

```python
# CreateServiceRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceRequestTypeDef


def get_value() -> CreateServiceRequestTypeDef:
    return {
        "name": ...,
    }


# CreateServiceRequestTypeDef definition

class CreateServiceRequestTypeDef(TypedDict):
    name: str,
    authType: NotRequired[AuthTypeType],  # (1)
    certificateArn: NotRequired[str],
    clientToken: NotRequired[str],
    customDomainName: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
## DeleteAccessLogSubscriptionRequestTypeDef

```python
# DeleteAccessLogSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteAccessLogSubscriptionRequestTypeDef


def get_value() -> DeleteAccessLogSubscriptionRequestTypeDef:
    return {
        "accessLogSubscriptionIdentifier": ...,
    }


# DeleteAccessLogSubscriptionRequestTypeDef definition

class DeleteAccessLogSubscriptionRequestTypeDef(TypedDict):
    accessLogSubscriptionIdentifier: str,
```

## DeleteAuthPolicyRequestTypeDef

```python
# DeleteAuthPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteAuthPolicyRequestTypeDef


def get_value() -> DeleteAuthPolicyRequestTypeDef:
    return {
        "resourceIdentifier": ...,
    }


# DeleteAuthPolicyRequestTypeDef definition

class DeleteAuthPolicyRequestTypeDef(TypedDict):
    resourceIdentifier: str,
```

## DeleteListenerRequestTypeDef

```python
# DeleteListenerRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteListenerRequestTypeDef


def get_value() -> DeleteListenerRequestTypeDef:
    return {
        "listenerIdentifier": ...,
    }


# DeleteListenerRequestTypeDef definition

class DeleteListenerRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    serviceIdentifier: str,
```

## DeleteResourceConfigurationRequestTypeDef

```python
# DeleteResourceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteResourceConfigurationRequestTypeDef


def get_value() -> DeleteResourceConfigurationRequestTypeDef:
    return {
        "resourceConfigurationIdentifier": ...,
    }


# DeleteResourceConfigurationRequestTypeDef definition

class DeleteResourceConfigurationRequestTypeDef(TypedDict):
    resourceConfigurationIdentifier: str,
```

## DeleteResourceEndpointAssociationRequestTypeDef

```python
# DeleteResourceEndpointAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteResourceEndpointAssociationRequestTypeDef


def get_value() -> DeleteResourceEndpointAssociationRequestTypeDef:
    return {
        "resourceEndpointAssociationIdentifier": ...,
    }


# DeleteResourceEndpointAssociationRequestTypeDef definition

class DeleteResourceEndpointAssociationRequestTypeDef(TypedDict):
    resourceEndpointAssociationIdentifier: str,
```

## DeleteResourceGatewayRequestTypeDef

```python
# DeleteResourceGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteResourceGatewayRequestTypeDef


def get_value() -> DeleteResourceGatewayRequestTypeDef:
    return {
        "resourceGatewayIdentifier": ...,
    }


# DeleteResourceGatewayRequestTypeDef definition

class DeleteResourceGatewayRequestTypeDef(TypedDict):
    resourceGatewayIdentifier: str,
```

## DeleteResourcePolicyRequestTypeDef

```python
# DeleteResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteResourcePolicyRequestTypeDef


def get_value() -> DeleteResourcePolicyRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# DeleteResourcePolicyRequestTypeDef definition

class DeleteResourcePolicyRequestTypeDef(TypedDict):
    resourceArn: str,
```

## DeleteRuleRequestTypeDef

```python
# DeleteRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteRuleRequestTypeDef


def get_value() -> DeleteRuleRequestTypeDef:
    return {
        "listenerIdentifier": ...,
    }


# DeleteRuleRequestTypeDef definition

class DeleteRuleRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    ruleIdentifier: str,
    serviceIdentifier: str,
```

## DeleteServiceNetworkRequestTypeDef

```python
# DeleteServiceNetworkRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteServiceNetworkRequestTypeDef


def get_value() -> DeleteServiceNetworkRequestTypeDef:
    return {
        "serviceNetworkIdentifier": ...,
    }


# DeleteServiceNetworkRequestTypeDef definition

class DeleteServiceNetworkRequestTypeDef(TypedDict):
    serviceNetworkIdentifier: str,
```

## DeleteServiceNetworkResourceAssociationRequestTypeDef

```python
# DeleteServiceNetworkResourceAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteServiceNetworkResourceAssociationRequestTypeDef


def get_value() -> DeleteServiceNetworkResourceAssociationRequestTypeDef:
    return {
        "serviceNetworkResourceAssociationIdentifier": ...,
    }


# DeleteServiceNetworkResourceAssociationRequestTypeDef definition

class DeleteServiceNetworkResourceAssociationRequestTypeDef(TypedDict):
    serviceNetworkResourceAssociationIdentifier: str,
```

## DeleteServiceNetworkServiceAssociationRequestTypeDef

```python
# DeleteServiceNetworkServiceAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteServiceNetworkServiceAssociationRequestTypeDef


def get_value() -> DeleteServiceNetworkServiceAssociationRequestTypeDef:
    return {
        "serviceNetworkServiceAssociationIdentifier": ...,
    }


# DeleteServiceNetworkServiceAssociationRequestTypeDef definition

class DeleteServiceNetworkServiceAssociationRequestTypeDef(TypedDict):
    serviceNetworkServiceAssociationIdentifier: str,
```

## DeleteServiceNetworkVpcAssociationRequestTypeDef

```python
# DeleteServiceNetworkVpcAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteServiceNetworkVpcAssociationRequestTypeDef


def get_value() -> DeleteServiceNetworkVpcAssociationRequestTypeDef:
    return {
        "serviceNetworkVpcAssociationIdentifier": ...,
    }


# DeleteServiceNetworkVpcAssociationRequestTypeDef definition

class DeleteServiceNetworkVpcAssociationRequestTypeDef(TypedDict):
    serviceNetworkVpcAssociationIdentifier: str,
```

## DeleteServiceRequestTypeDef

```python
# DeleteServiceRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteServiceRequestTypeDef


def get_value() -> DeleteServiceRequestTypeDef:
    return {
        "serviceIdentifier": ...,
    }


# DeleteServiceRequestTypeDef definition

class DeleteServiceRequestTypeDef(TypedDict):
    serviceIdentifier: str,
```

## DeleteTargetGroupRequestTypeDef

```python
# DeleteTargetGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteTargetGroupRequestTypeDef


def get_value() -> DeleteTargetGroupRequestTypeDef:
    return {
        "targetGroupIdentifier": ...,
    }


# DeleteTargetGroupRequestTypeDef definition

class DeleteTargetGroupRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
```

## TargetTypeDef

```python
# TargetTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import TargetTypeDef


def get_value() -> TargetTypeDef:
    return {
        "id": ...,
    }


# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    id: str,
    port: NotRequired[int],
```

## TargetFailureTypeDef

```python
# TargetFailureTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import TargetFailureTypeDef


def get_value() -> TargetFailureTypeDef:
    return {
        "failureCode": ...,
    }


# TargetFailureTypeDef definition

class TargetFailureTypeDef(TypedDict):
    failureCode: NotRequired[str],
    failureMessage: NotRequired[str],
    id: NotRequired[str],
    port: NotRequired[int],
```

## DnsResourceTypeDef

```python
# DnsResourceTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DnsResourceTypeDef


def get_value() -> DnsResourceTypeDef:
    return {
        "domainName": ...,
    }


# DnsResourceTypeDef definition

class DnsResourceTypeDef(TypedDict):
    domainName: NotRequired[str],
    ipAddressType: NotRequired[ResourceConfigurationIpAddressTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceConfigurationIpAddressTypeType](./literals.md#resourceconfigurationipaddresstypetype) 
## FixedResponseActionTypeDef

```python
# FixedResponseActionTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import FixedResponseActionTypeDef


def get_value() -> FixedResponseActionTypeDef:
    return {
        "statusCode": ...,
    }


# FixedResponseActionTypeDef definition

class FixedResponseActionTypeDef(TypedDict):
    statusCode: int,
```

## WeightedTargetGroupTypeDef

```python
# WeightedTargetGroupTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import WeightedTargetGroupTypeDef


def get_value() -> WeightedTargetGroupTypeDef:
    return {
        "targetGroupIdentifier": ...,
    }


# WeightedTargetGroupTypeDef definition

class WeightedTargetGroupTypeDef(TypedDict):
    targetGroupIdentifier: str,
    weight: NotRequired[int],
```

## GetAccessLogSubscriptionRequestTypeDef

```python
# GetAccessLogSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetAccessLogSubscriptionRequestTypeDef


def get_value() -> GetAccessLogSubscriptionRequestTypeDef:
    return {
        "accessLogSubscriptionIdentifier": ...,
    }


# GetAccessLogSubscriptionRequestTypeDef definition

class GetAccessLogSubscriptionRequestTypeDef(TypedDict):
    accessLogSubscriptionIdentifier: str,
```

## GetAuthPolicyRequestTypeDef

```python
# GetAuthPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetAuthPolicyRequestTypeDef


def get_value() -> GetAuthPolicyRequestTypeDef:
    return {
        "resourceIdentifier": ...,
    }


# GetAuthPolicyRequestTypeDef definition

class GetAuthPolicyRequestTypeDef(TypedDict):
    resourceIdentifier: str,
```

## GetListenerRequestTypeDef

```python
# GetListenerRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetListenerRequestTypeDef


def get_value() -> GetListenerRequestTypeDef:
    return {
        "listenerIdentifier": ...,
    }


# GetListenerRequestTypeDef definition

class GetListenerRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    serviceIdentifier: str,
```

## GetResourceConfigurationRequestTypeDef

```python
# GetResourceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetResourceConfigurationRequestTypeDef


def get_value() -> GetResourceConfigurationRequestTypeDef:
    return {
        "resourceConfigurationIdentifier": ...,
    }


# GetResourceConfigurationRequestTypeDef definition

class GetResourceConfigurationRequestTypeDef(TypedDict):
    resourceConfigurationIdentifier: str,
```

## GetResourceGatewayRequestTypeDef

```python
# GetResourceGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetResourceGatewayRequestTypeDef


def get_value() -> GetResourceGatewayRequestTypeDef:
    return {
        "resourceGatewayIdentifier": ...,
    }


# GetResourceGatewayRequestTypeDef definition

class GetResourceGatewayRequestTypeDef(TypedDict):
    resourceGatewayIdentifier: str,
```

## GetResourcePolicyRequestTypeDef

```python
# GetResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetResourcePolicyRequestTypeDef


def get_value() -> GetResourcePolicyRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# GetResourcePolicyRequestTypeDef definition

class GetResourcePolicyRequestTypeDef(TypedDict):
    resourceArn: str,
```

## GetRuleRequestTypeDef

```python
# GetRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetRuleRequestTypeDef


def get_value() -> GetRuleRequestTypeDef:
    return {
        "listenerIdentifier": ...,
    }


# GetRuleRequestTypeDef definition

class GetRuleRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    ruleIdentifier: str,
    serviceIdentifier: str,
```

## GetServiceNetworkRequestTypeDef

```python
# GetServiceNetworkRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceNetworkRequestTypeDef


def get_value() -> GetServiceNetworkRequestTypeDef:
    return {
        "serviceNetworkIdentifier": ...,
    }


# GetServiceNetworkRequestTypeDef definition

class GetServiceNetworkRequestTypeDef(TypedDict):
    serviceNetworkIdentifier: str,
```

## GetServiceNetworkResourceAssociationRequestTypeDef

```python
# GetServiceNetworkResourceAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceNetworkResourceAssociationRequestTypeDef


def get_value() -> GetServiceNetworkResourceAssociationRequestTypeDef:
    return {
        "serviceNetworkResourceAssociationIdentifier": ...,
    }


# GetServiceNetworkResourceAssociationRequestTypeDef definition

class GetServiceNetworkResourceAssociationRequestTypeDef(TypedDict):
    serviceNetworkResourceAssociationIdentifier: str,
```

## GetServiceNetworkServiceAssociationRequestTypeDef

```python
# GetServiceNetworkServiceAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceNetworkServiceAssociationRequestTypeDef


def get_value() -> GetServiceNetworkServiceAssociationRequestTypeDef:
    return {
        "serviceNetworkServiceAssociationIdentifier": ...,
    }


# GetServiceNetworkServiceAssociationRequestTypeDef definition

class GetServiceNetworkServiceAssociationRequestTypeDef(TypedDict):
    serviceNetworkServiceAssociationIdentifier: str,
```

## GetServiceNetworkVpcAssociationRequestTypeDef

```python
# GetServiceNetworkVpcAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceNetworkVpcAssociationRequestTypeDef


def get_value() -> GetServiceNetworkVpcAssociationRequestTypeDef:
    return {
        "serviceNetworkVpcAssociationIdentifier": ...,
    }


# GetServiceNetworkVpcAssociationRequestTypeDef definition

class GetServiceNetworkVpcAssociationRequestTypeDef(TypedDict):
    serviceNetworkVpcAssociationIdentifier: str,
```

## GetServiceRequestTypeDef

```python
# GetServiceRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceRequestTypeDef


def get_value() -> GetServiceRequestTypeDef:
    return {
        "serviceIdentifier": ...,
    }


# GetServiceRequestTypeDef definition

class GetServiceRequestTypeDef(TypedDict):
    serviceIdentifier: str,
```

## GetTargetGroupRequestTypeDef

```python
# GetTargetGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetTargetGroupRequestTypeDef


def get_value() -> GetTargetGroupRequestTypeDef:
    return {
        "targetGroupIdentifier": ...,
    }


# GetTargetGroupRequestTypeDef definition

class GetTargetGroupRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
```

## HeaderMatchTypeTypeDef

```python
# HeaderMatchTypeTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import HeaderMatchTypeTypeDef


def get_value() -> HeaderMatchTypeTypeDef:
    return {
        "contains": ...,
    }


# HeaderMatchTypeTypeDef definition

class HeaderMatchTypeTypeDef(TypedDict):
    contains: NotRequired[str],
    exact: NotRequired[str],
    prefix: NotRequired[str],
```

## MatcherTypeDef

```python
# MatcherTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import MatcherTypeDef


def get_value() -> MatcherTypeDef:
    return {
        "httpCode": ...,
    }


# MatcherTypeDef definition

class MatcherTypeDef(TypedDict):
    httpCode: NotRequired[str],
```

## IpResourceTypeDef

```python
# IpResourceTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import IpResourceTypeDef


def get_value() -> IpResourceTypeDef:
    return {
        "ipAddress": ...,
    }


# IpResourceTypeDef definition

class IpResourceTypeDef(TypedDict):
    ipAddress: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccessLogSubscriptionsRequestTypeDef

```python
# ListAccessLogSubscriptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListAccessLogSubscriptionsRequestTypeDef


def get_value() -> ListAccessLogSubscriptionsRequestTypeDef:
    return {
        "resourceIdentifier": ...,
    }


# ListAccessLogSubscriptionsRequestTypeDef definition

class ListAccessLogSubscriptionsRequestTypeDef(TypedDict):
    resourceIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListListenersRequestTypeDef

```python
# ListListenersRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListListenersRequestTypeDef


def get_value() -> ListListenersRequestTypeDef:
    return {
        "serviceIdentifier": ...,
    }


# ListListenersRequestTypeDef definition

class ListListenersRequestTypeDef(TypedDict):
    serviceIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListenerSummaryTypeDef

```python
# ListenerSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListenerSummaryTypeDef


def get_value() -> ListenerSummaryTypeDef:
    return {
        "arn": ...,
    }


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
## ListResourceConfigurationsRequestTypeDef

```python
# ListResourceConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListResourceConfigurationsRequestTypeDef


def get_value() -> ListResourceConfigurationsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListResourceConfigurationsRequestTypeDef definition

class ListResourceConfigurationsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resourceConfigurationGroupIdentifier: NotRequired[str],
    resourceGatewayIdentifier: NotRequired[str],
```

## ResourceConfigurationSummaryTypeDef

```python
# ResourceConfigurationSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ResourceConfigurationSummaryTypeDef


def get_value() -> ResourceConfigurationSummaryTypeDef:
    return {
        "amazonManaged": ...,
    }


# ResourceConfigurationSummaryTypeDef definition

class ResourceConfigurationSummaryTypeDef(TypedDict):
    amazonManaged: NotRequired[bool],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    id: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    resourceConfigurationGroupId: NotRequired[str],
    resourceGatewayId: NotRequired[str],
    status: NotRequired[ResourceConfigurationStatusType],  # (1)
    type: NotRequired[ResourceConfigurationTypeType],  # (2)
```

1. See [:material-code-brackets: ResourceConfigurationStatusType](./literals.md#resourceconfigurationstatustype) 
2. See [:material-code-brackets: ResourceConfigurationTypeType](./literals.md#resourceconfigurationtypetype) 
## ListResourceEndpointAssociationsRequestTypeDef

```python
# ListResourceEndpointAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListResourceEndpointAssociationsRequestTypeDef


def get_value() -> ListResourceEndpointAssociationsRequestTypeDef:
    return {
        "resourceConfigurationIdentifier": ...,
    }


# ListResourceEndpointAssociationsRequestTypeDef definition

class ListResourceEndpointAssociationsRequestTypeDef(TypedDict):
    resourceConfigurationIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resourceEndpointAssociationIdentifier: NotRequired[str],
    vpcEndpointId: NotRequired[str],
    vpcEndpointOwner: NotRequired[str],
```

## ResourceEndpointAssociationSummaryTypeDef

```python
# ResourceEndpointAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ResourceEndpointAssociationSummaryTypeDef


def get_value() -> ResourceEndpointAssociationSummaryTypeDef:
    return {
        "arn": ...,
    }


# ResourceEndpointAssociationSummaryTypeDef definition

class ResourceEndpointAssociationSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    id: NotRequired[str],
    resourceConfigurationArn: NotRequired[str],
    resourceConfigurationId: NotRequired[str],
    resourceConfigurationName: NotRequired[str],
    vpcEndpointId: NotRequired[str],
    vpcEndpointOwner: NotRequired[str],
```

## ListResourceGatewaysRequestTypeDef

```python
# ListResourceGatewaysRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListResourceGatewaysRequestTypeDef


def get_value() -> ListResourceGatewaysRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListResourceGatewaysRequestTypeDef definition

class ListResourceGatewaysRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ResourceGatewaySummaryTypeDef

```python
# ResourceGatewaySummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ResourceGatewaySummaryTypeDef


def get_value() -> ResourceGatewaySummaryTypeDef:
    return {
        "arn": ...,
    }


# ResourceGatewaySummaryTypeDef definition

class ResourceGatewaySummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    id: NotRequired[str],
    ipAddressType: NotRequired[ResourceGatewayIpAddressTypeType],  # (1)
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    securityGroupIds: NotRequired[List[str]],
    status: NotRequired[ResourceGatewayStatusType],  # (2)
    subnetIds: NotRequired[List[str]],
    vpcIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: ResourceGatewayIpAddressTypeType](./literals.md#resourcegatewayipaddresstypetype) 
2. See [:material-code-brackets: ResourceGatewayStatusType](./literals.md#resourcegatewaystatustype) 
## ListRulesRequestTypeDef

```python
# ListRulesRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListRulesRequestTypeDef


def get_value() -> ListRulesRequestTypeDef:
    return {
        "listenerIdentifier": ...,
    }


# ListRulesRequestTypeDef definition

class ListRulesRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    serviceIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## RuleSummaryTypeDef

```python
# RuleSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleSummaryTypeDef


def get_value() -> RuleSummaryTypeDef:
    return {
        "arn": ...,
    }


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

## ListServiceNetworkResourceAssociationsRequestTypeDef

```python
# ListServiceNetworkResourceAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkResourceAssociationsRequestTypeDef


def get_value() -> ListServiceNetworkResourceAssociationsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListServiceNetworkResourceAssociationsRequestTypeDef definition

class ListServiceNetworkResourceAssociationsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resourceConfigurationIdentifier: NotRequired[str],
    serviceNetworkIdentifier: NotRequired[str],
```

## ListServiceNetworkServiceAssociationsRequestTypeDef

```python
# ListServiceNetworkServiceAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkServiceAssociationsRequestTypeDef


def get_value() -> ListServiceNetworkServiceAssociationsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListServiceNetworkServiceAssociationsRequestTypeDef definition

class ListServiceNetworkServiceAssociationsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    serviceIdentifier: NotRequired[str],
    serviceNetworkIdentifier: NotRequired[str],
```

## ListServiceNetworkVpcAssociationsRequestTypeDef

```python
# ListServiceNetworkVpcAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkVpcAssociationsRequestTypeDef


def get_value() -> ListServiceNetworkVpcAssociationsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListServiceNetworkVpcAssociationsRequestTypeDef definition

class ListServiceNetworkVpcAssociationsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    serviceNetworkIdentifier: NotRequired[str],
    vpcIdentifier: NotRequired[str],
```

## ServiceNetworkVpcAssociationSummaryTypeDef

```python
# ServiceNetworkVpcAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ServiceNetworkVpcAssociationSummaryTypeDef


def get_value() -> ServiceNetworkVpcAssociationSummaryTypeDef:
    return {
        "arn": ...,
    }


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
## ListServiceNetworkVpcEndpointAssociationsRequestTypeDef

```python
# ListServiceNetworkVpcEndpointAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkVpcEndpointAssociationsRequestTypeDef


def get_value() -> ListServiceNetworkVpcEndpointAssociationsRequestTypeDef:
    return {
        "serviceNetworkIdentifier": ...,
    }


# ListServiceNetworkVpcEndpointAssociationsRequestTypeDef definition

class ListServiceNetworkVpcEndpointAssociationsRequestTypeDef(TypedDict):
    serviceNetworkIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceNetworkEndpointAssociationTypeDef

```python
# ServiceNetworkEndpointAssociationTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ServiceNetworkEndpointAssociationTypeDef


def get_value() -> ServiceNetworkEndpointAssociationTypeDef:
    return {
        "createdAt": ...,
    }


# ServiceNetworkEndpointAssociationTypeDef definition

class ServiceNetworkEndpointAssociationTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    id: NotRequired[str],
    serviceNetworkArn: NotRequired[str],
    state: NotRequired[str],
    vpcEndpointId: NotRequired[str],
    vpcEndpointOwnerId: NotRequired[str],
    vpcId: NotRequired[str],
```

## ListServiceNetworksRequestTypeDef

```python
# ListServiceNetworksRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworksRequestTypeDef


def get_value() -> ListServiceNetworksRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListServiceNetworksRequestTypeDef definition

class ListServiceNetworksRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceNetworkSummaryTypeDef

```python
# ServiceNetworkSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ServiceNetworkSummaryTypeDef


def get_value() -> ServiceNetworkSummaryTypeDef:
    return {
        "arn": ...,
    }


# ServiceNetworkSummaryTypeDef definition

class ServiceNetworkSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    id: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    numberOfAssociatedResourceConfigurations: NotRequired[int],
    numberOfAssociatedServices: NotRequired[int],
    numberOfAssociatedVPCs: NotRequired[int],
```

## ListServicesRequestTypeDef

```python
# ListServicesRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServicesRequestTypeDef


def get_value() -> ListServicesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListServicesRequestTypeDef definition

class ListServicesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTargetGroupsRequestTypeDef

```python
# ListTargetGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListTargetGroupsRequestTypeDef


def get_value() -> ListTargetGroupsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListTargetGroupsRequestTypeDef definition

class ListTargetGroupsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    targetGroupType: NotRequired[TargetGroupTypeType],  # (1)
    vpcIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
## TargetGroupSummaryTypeDef

```python
# TargetGroupSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import TargetGroupSummaryTypeDef


def get_value() -> TargetGroupSummaryTypeDef:
    return {
        "arn": ...,
    }


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
# TargetSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import TargetSummaryTypeDef


def get_value() -> TargetSummaryTypeDef:
    return {
        "id": ...,
    }


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
# PathMatchTypeTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import PathMatchTypeTypeDef


def get_value() -> PathMatchTypeTypeDef:
    return {
        "exact": ...,
    }


# PathMatchTypeTypeDef definition

class PathMatchTypeTypeDef(TypedDict):
    exact: NotRequired[str],
    prefix: NotRequired[str],
```

## PutAuthPolicyRequestTypeDef

```python
# PutAuthPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import PutAuthPolicyRequestTypeDef


def get_value() -> PutAuthPolicyRequestTypeDef:
    return {
        "policy": ...,
    }


# PutAuthPolicyRequestTypeDef definition

class PutAuthPolicyRequestTypeDef(TypedDict):
    policy: str,
    resourceIdentifier: str,
```

## PutResourcePolicyRequestTypeDef

```python
# PutResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import PutResourcePolicyRequestTypeDef


def get_value() -> PutResourcePolicyRequestTypeDef:
    return {
        "policy": ...,
    }


# PutResourcePolicyRequestTypeDef definition

class PutResourcePolicyRequestTypeDef(TypedDict):
    policy: str,
    resourceArn: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAccessLogSubscriptionRequestTypeDef

```python
# UpdateAccessLogSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateAccessLogSubscriptionRequestTypeDef


def get_value() -> UpdateAccessLogSubscriptionRequestTypeDef:
    return {
        "accessLogSubscriptionIdentifier": ...,
    }


# UpdateAccessLogSubscriptionRequestTypeDef definition

class UpdateAccessLogSubscriptionRequestTypeDef(TypedDict):
    accessLogSubscriptionIdentifier: str,
    destinationArn: str,
```

## UpdateResourceGatewayRequestTypeDef

```python
# UpdateResourceGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateResourceGatewayRequestTypeDef


def get_value() -> UpdateResourceGatewayRequestTypeDef:
    return {
        "resourceGatewayIdentifier": ...,
    }


# UpdateResourceGatewayRequestTypeDef definition

class UpdateResourceGatewayRequestTypeDef(TypedDict):
    resourceGatewayIdentifier: str,
    securityGroupIds: NotRequired[Sequence[str]],
```

## UpdateServiceNetworkRequestTypeDef

```python
# UpdateServiceNetworkRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateServiceNetworkRequestTypeDef


def get_value() -> UpdateServiceNetworkRequestTypeDef:
    return {
        "authType": ...,
    }


# UpdateServiceNetworkRequestTypeDef definition

class UpdateServiceNetworkRequestTypeDef(TypedDict):
    authType: AuthTypeType,  # (1)
    serviceNetworkIdentifier: str,
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
## UpdateServiceNetworkVpcAssociationRequestTypeDef

```python
# UpdateServiceNetworkVpcAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateServiceNetworkVpcAssociationRequestTypeDef


def get_value() -> UpdateServiceNetworkVpcAssociationRequestTypeDef:
    return {
        "securityGroupIds": ...,
    }


# UpdateServiceNetworkVpcAssociationRequestTypeDef definition

class UpdateServiceNetworkVpcAssociationRequestTypeDef(TypedDict):
    securityGroupIds: Sequence[str],
    serviceNetworkVpcAssociationIdentifier: str,
```

## UpdateServiceRequestTypeDef

```python
# UpdateServiceRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateServiceRequestTypeDef


def get_value() -> UpdateServiceRequestTypeDef:
    return {
        "serviceIdentifier": ...,
    }


# UpdateServiceRequestTypeDef definition

class UpdateServiceRequestTypeDef(TypedDict):
    serviceIdentifier: str,
    authType: NotRequired[AuthTypeType],  # (1)
    certificateArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
## CreateAccessLogSubscriptionResponseTypeDef

```python
# CreateAccessLogSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateAccessLogSubscriptionResponseTypeDef


def get_value() -> CreateAccessLogSubscriptionResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateAccessLogSubscriptionResponseTypeDef definition

class CreateAccessLogSubscriptionResponseTypeDef(TypedDict):
    arn: str,
    destinationArn: str,
    id: str,
    resourceArn: str,
    resourceId: str,
    serviceNetworkLogType: ServiceNetworkLogTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceNetworkLogTypeType](./literals.md#servicenetworklogtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceGatewayResponseTypeDef

```python
# CreateResourceGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateResourceGatewayResponseTypeDef


def get_value() -> CreateResourceGatewayResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateResourceGatewayResponseTypeDef definition

class CreateResourceGatewayResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    ipAddressType: ResourceGatewayIpAddressTypeType,  # (1)
    name: str,
    securityGroupIds: List[str],
    status: ResourceGatewayStatusType,  # (2)
    subnetIds: List[str],
    vpcIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ResourceGatewayIpAddressTypeType](./literals.md#resourcegatewayipaddresstypetype) 
2. See [:material-code-brackets: ResourceGatewayStatusType](./literals.md#resourcegatewaystatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceNetworkResourceAssociationResponseTypeDef

```python
# CreateServiceNetworkResourceAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceNetworkResourceAssociationResponseTypeDef


def get_value() -> CreateServiceNetworkResourceAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateServiceNetworkResourceAssociationResponseTypeDef definition

class CreateServiceNetworkResourceAssociationResponseTypeDef(TypedDict):
    arn: str,
    createdBy: str,
    id: str,
    status: ServiceNetworkResourceAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceNetworkResourceAssociationStatusType](./literals.md#servicenetworkresourceassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceNetworkVpcAssociationResponseTypeDef

```python
# CreateServiceNetworkVpcAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceNetworkVpcAssociationResponseTypeDef


def get_value() -> CreateServiceNetworkVpcAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


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
## DeleteResourceEndpointAssociationResponseTypeDef

```python
# DeleteResourceEndpointAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteResourceEndpointAssociationResponseTypeDef


def get_value() -> DeleteResourceEndpointAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


# DeleteResourceEndpointAssociationResponseTypeDef definition

class DeleteResourceEndpointAssociationResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    resourceConfigurationArn: str,
    resourceConfigurationId: str,
    vpcEndpointId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResourceGatewayResponseTypeDef

```python
# DeleteResourceGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteResourceGatewayResponseTypeDef


def get_value() -> DeleteResourceGatewayResponseTypeDef:
    return {
        "arn": ...,
    }


# DeleteResourceGatewayResponseTypeDef definition

class DeleteResourceGatewayResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    status: ResourceGatewayStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceGatewayStatusType](./literals.md#resourcegatewaystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceNetworkResourceAssociationResponseTypeDef

```python
# DeleteServiceNetworkResourceAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteServiceNetworkResourceAssociationResponseTypeDef


def get_value() -> DeleteServiceNetworkResourceAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


# DeleteServiceNetworkResourceAssociationResponseTypeDef definition

class DeleteServiceNetworkResourceAssociationResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    status: ServiceNetworkResourceAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceNetworkResourceAssociationStatusType](./literals.md#servicenetworkresourceassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceNetworkServiceAssociationResponseTypeDef

```python
# DeleteServiceNetworkServiceAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteServiceNetworkServiceAssociationResponseTypeDef


def get_value() -> DeleteServiceNetworkServiceAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


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
# DeleteServiceNetworkVpcAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteServiceNetworkVpcAssociationResponseTypeDef


def get_value() -> DeleteServiceNetworkVpcAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


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
# DeleteServiceResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteServiceResponseTypeDef


def get_value() -> DeleteServiceResponseTypeDef:
    return {
        "arn": ...,
    }


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
# DeleteTargetGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeleteTargetGroupResponseTypeDef


def get_value() -> DeleteTargetGroupResponseTypeDef:
    return {
        "arn": ...,
    }


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
# GetAccessLogSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetAccessLogSubscriptionResponseTypeDef


def get_value() -> GetAccessLogSubscriptionResponseTypeDef:
    return {
        "arn": ...,
    }


# GetAccessLogSubscriptionResponseTypeDef definition

class GetAccessLogSubscriptionResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    destinationArn: str,
    id: str,
    lastUpdatedAt: datetime,
    resourceArn: str,
    resourceId: str,
    serviceNetworkLogType: ServiceNetworkLogTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceNetworkLogTypeType](./literals.md#servicenetworklogtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAuthPolicyResponseTypeDef

```python
# GetAuthPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetAuthPolicyResponseTypeDef


def get_value() -> GetAuthPolicyResponseTypeDef:
    return {
        "createdAt": ...,
    }


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
## GetResourceGatewayResponseTypeDef

```python
# GetResourceGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetResourceGatewayResponseTypeDef


def get_value() -> GetResourceGatewayResponseTypeDef:
    return {
        "arn": ...,
    }


# GetResourceGatewayResponseTypeDef definition

class GetResourceGatewayResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    id: str,
    ipAddressType: ResourceGatewayIpAddressTypeType,  # (1)
    lastUpdatedAt: datetime,
    name: str,
    securityGroupIds: List[str],
    status: ResourceGatewayStatusType,  # (2)
    subnetIds: List[str],
    vpcId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ResourceGatewayIpAddressTypeType](./literals.md#resourcegatewayipaddresstypetype) 
2. See [:material-code-brackets: ResourceGatewayStatusType](./literals.md#resourcegatewaystatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetResourcePolicyResponseTypeDef


def get_value() -> GetResourcePolicyResponseTypeDef:
    return {
        "policy": ...,
    }


# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceNetworkVpcAssociationResponseTypeDef

```python
# GetServiceNetworkVpcAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceNetworkVpcAssociationResponseTypeDef


def get_value() -> GetServiceNetworkVpcAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


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
# ListAccessLogSubscriptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListAccessLogSubscriptionsResponseTypeDef


def get_value() -> ListAccessLogSubscriptionsResponseTypeDef:
    return {
        "items": ...,
    }


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
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAuthPolicyResponseTypeDef

```python
# PutAuthPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import PutAuthPolicyResponseTypeDef


def get_value() -> PutAuthPolicyResponseTypeDef:
    return {
        "policy": ...,
    }


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
# UpdateAccessLogSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateAccessLogSubscriptionResponseTypeDef


def get_value() -> UpdateAccessLogSubscriptionResponseTypeDef:
    return {
        "arn": ...,
    }


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
## UpdateResourceGatewayResponseTypeDef

```python
# UpdateResourceGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateResourceGatewayResponseTypeDef


def get_value() -> UpdateResourceGatewayResponseTypeDef:
    return {
        "arn": ...,
    }


# UpdateResourceGatewayResponseTypeDef definition

class UpdateResourceGatewayResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    ipAddressType: IpAddressTypeType,  # (1)
    name: str,
    securityGroupIds: List[str],
    status: ResourceGatewayStatusType,  # (2)
    subnetIds: List[str],
    vpcId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
2. See [:material-code-brackets: ResourceGatewayStatusType](./literals.md#resourcegatewaystatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceNetworkResponseTypeDef

```python
# UpdateServiceNetworkResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateServiceNetworkResponseTypeDef


def get_value() -> UpdateServiceNetworkResponseTypeDef:
    return {
        "arn": ...,
    }


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
# UpdateServiceNetworkVpcAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateServiceNetworkVpcAssociationResponseTypeDef


def get_value() -> UpdateServiceNetworkVpcAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


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
# UpdateServiceResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateServiceResponseTypeDef


def get_value() -> UpdateServiceResponseTypeDef:
    return {
        "arn": ...,
    }


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
## CreateServiceNetworkRequestTypeDef

```python
# CreateServiceNetworkRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceNetworkRequestTypeDef


def get_value() -> CreateServiceNetworkRequestTypeDef:
    return {
        "name": ...,
    }


# CreateServiceNetworkRequestTypeDef definition

class CreateServiceNetworkRequestTypeDef(TypedDict):
    name: str,
    authType: NotRequired[AuthTypeType],  # (1)
    clientToken: NotRequired[str],
    sharingConfig: NotRequired[SharingConfigTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: SharingConfigTypeDef](./type_defs.md#sharingconfigtypedef) 
## CreateServiceNetworkResponseTypeDef

```python
# CreateServiceNetworkResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceNetworkResponseTypeDef


def get_value() -> CreateServiceNetworkResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateServiceNetworkResponseTypeDef definition

class CreateServiceNetworkResponseTypeDef(TypedDict):
    arn: str,
    authType: AuthTypeType,  # (1)
    id: str,
    name: str,
    sharingConfig: SharingConfigTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: SharingConfigTypeDef](./type_defs.md#sharingconfigtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceNetworkResponseTypeDef

```python
# GetServiceNetworkResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceNetworkResponseTypeDef


def get_value() -> GetServiceNetworkResponseTypeDef:
    return {
        "arn": ...,
    }


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
    sharingConfig: SharingConfigTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: SharingConfigTypeDef](./type_defs.md#sharingconfigtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceNetworkServiceAssociationResponseTypeDef

```python
# CreateServiceNetworkServiceAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceNetworkServiceAssociationResponseTypeDef


def get_value() -> CreateServiceNetworkServiceAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


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
# CreateServiceResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateServiceResponseTypeDef


def get_value() -> CreateServiceResponseTypeDef:
    return {
        "arn": ...,
    }


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
## GetServiceNetworkResourceAssociationResponseTypeDef

```python
# GetServiceNetworkResourceAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceNetworkResourceAssociationResponseTypeDef


def get_value() -> GetServiceNetworkResourceAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


# GetServiceNetworkResourceAssociationResponseTypeDef definition

class GetServiceNetworkResourceAssociationResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    createdBy: str,
    dnsEntry: DnsEntryTypeDef,  # (1)
    failureCode: str,
    failureReason: str,
    id: str,
    isManagedAssociation: bool,
    lastUpdatedAt: datetime,
    privateDnsEntry: DnsEntryTypeDef,  # (1)
    resourceConfigurationArn: str,
    resourceConfigurationId: str,
    resourceConfigurationName: str,
    serviceNetworkArn: str,
    serviceNetworkId: str,
    serviceNetworkName: str,
    status: ServiceNetworkResourceAssociationStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
2. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
3. See [:material-code-brackets: ServiceNetworkResourceAssociationStatusType](./literals.md#servicenetworkresourceassociationstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceNetworkServiceAssociationResponseTypeDef

```python
# GetServiceNetworkServiceAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceNetworkServiceAssociationResponseTypeDef


def get_value() -> GetServiceNetworkServiceAssociationResponseTypeDef:
    return {
        "arn": ...,
    }


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
# GetServiceResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetServiceResponseTypeDef


def get_value() -> GetServiceResponseTypeDef:
    return {
        "arn": ...,
    }


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
## ServiceNetworkResourceAssociationSummaryTypeDef

```python
# ServiceNetworkResourceAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ServiceNetworkResourceAssociationSummaryTypeDef


def get_value() -> ServiceNetworkResourceAssociationSummaryTypeDef:
    return {
        "arn": ...,
    }


# ServiceNetworkResourceAssociationSummaryTypeDef definition

class ServiceNetworkResourceAssociationSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    dnsEntry: NotRequired[DnsEntryTypeDef],  # (1)
    failureCode: NotRequired[str],
    id: NotRequired[str],
    isManagedAssociation: NotRequired[bool],
    privateDnsEntry: NotRequired[DnsEntryTypeDef],  # (1)
    resourceConfigurationArn: NotRequired[str],
    resourceConfigurationId: NotRequired[str],
    resourceConfigurationName: NotRequired[str],
    serviceNetworkArn: NotRequired[str],
    serviceNetworkId: NotRequired[str],
    serviceNetworkName: NotRequired[str],
    status: NotRequired[ServiceNetworkResourceAssociationStatusType],  # (3)
```

1. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
2. See [:material-code-braces: DnsEntryTypeDef](./type_defs.md#dnsentrytypedef) 
3. See [:material-code-brackets: ServiceNetworkResourceAssociationStatusType](./literals.md#servicenetworkresourceassociationstatustype) 
## ServiceNetworkServiceAssociationSummaryTypeDef

```python
# ServiceNetworkServiceAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ServiceNetworkServiceAssociationSummaryTypeDef


def get_value() -> ServiceNetworkServiceAssociationSummaryTypeDef:
    return {
        "arn": ...,
    }


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
# ServiceSummaryTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ServiceSummaryTypeDef


def get_value() -> ServiceSummaryTypeDef:
    return {
        "arn": ...,
    }


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
## DeregisterTargetsRequestTypeDef

```python
# DeregisterTargetsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeregisterTargetsRequestTypeDef


def get_value() -> DeregisterTargetsRequestTypeDef:
    return {
        "targetGroupIdentifier": ...,
    }


# DeregisterTargetsRequestTypeDef definition

class DeregisterTargetsRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
    targets: Sequence[TargetTypeDef],  # (1)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## ListTargetsRequestTypeDef

```python
# ListTargetsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListTargetsRequestTypeDef


def get_value() -> ListTargetsRequestTypeDef:
    return {
        "targetGroupIdentifier": ...,
    }


# ListTargetsRequestTypeDef definition

class ListTargetsRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    targets: NotRequired[Sequence[TargetTypeDef]],  # (1)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## RegisterTargetsRequestTypeDef

```python
# RegisterTargetsRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RegisterTargetsRequestTypeDef


def get_value() -> RegisterTargetsRequestTypeDef:
    return {
        "targetGroupIdentifier": ...,
    }


# RegisterTargetsRequestTypeDef definition

class RegisterTargetsRequestTypeDef(TypedDict):
    targetGroupIdentifier: str,
    targets: Sequence[TargetTypeDef],  # (1)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## DeregisterTargetsResponseTypeDef

```python
# DeregisterTargetsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import DeregisterTargetsResponseTypeDef


def get_value() -> DeregisterTargetsResponseTypeDef:
    return {
        "successful": ...,
    }


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
# RegisterTargetsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RegisterTargetsResponseTypeDef


def get_value() -> RegisterTargetsResponseTypeDef:
    return {
        "successful": ...,
    }


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
# ForwardActionOutputTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ForwardActionOutputTypeDef


def get_value() -> ForwardActionOutputTypeDef:
    return {
        "targetGroups": ...,
    }


# ForwardActionOutputTypeDef definition

class ForwardActionOutputTypeDef(TypedDict):
    targetGroups: List[WeightedTargetGroupTypeDef],  # (1)
```

1. See [:material-code-braces: WeightedTargetGroupTypeDef](./type_defs.md#weightedtargetgrouptypedef) 
## ForwardActionTypeDef

```python
# ForwardActionTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ForwardActionTypeDef


def get_value() -> ForwardActionTypeDef:
    return {
        "targetGroups": ...,
    }


# ForwardActionTypeDef definition

class ForwardActionTypeDef(TypedDict):
    targetGroups: Sequence[WeightedTargetGroupTypeDef],  # (1)
```

1. See [:material-code-braces: WeightedTargetGroupTypeDef](./type_defs.md#weightedtargetgrouptypedef) 
## HeaderMatchTypeDef

```python
# HeaderMatchTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import HeaderMatchTypeDef


def get_value() -> HeaderMatchTypeDef:
    return {
        "caseSensitive": ...,
    }


# HeaderMatchTypeDef definition

class HeaderMatchTypeDef(TypedDict):
    match: HeaderMatchTypeTypeDef,  # (1)
    name: str,
    caseSensitive: NotRequired[bool],
```

1. See [:material-code-braces: HeaderMatchTypeTypeDef](./type_defs.md#headermatchtypetypedef) 
## HealthCheckConfigTypeDef

```python
# HealthCheckConfigTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import HealthCheckConfigTypeDef


def get_value() -> HealthCheckConfigTypeDef:
    return {
        "enabled": ...,
    }


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
## ResourceConfigurationDefinitionTypeDef

```python
# ResourceConfigurationDefinitionTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ResourceConfigurationDefinitionTypeDef


def get_value() -> ResourceConfigurationDefinitionTypeDef:
    return {
        "arnResource": ...,
    }


# ResourceConfigurationDefinitionTypeDef definition

class ResourceConfigurationDefinitionTypeDef(TypedDict):
    arnResource: NotRequired[ArnResourceTypeDef],  # (1)
    dnsResource: NotRequired[DnsResourceTypeDef],  # (2)
    ipResource: NotRequired[IpResourceTypeDef],  # (3)
```

1. See [:material-code-braces: ArnResourceTypeDef](./type_defs.md#arnresourcetypedef) 
2. See [:material-code-braces: DnsResourceTypeDef](./type_defs.md#dnsresourcetypedef) 
3. See [:material-code-braces: IpResourceTypeDef](./type_defs.md#ipresourcetypedef) 
## ListAccessLogSubscriptionsRequestPaginateTypeDef

```python
# ListAccessLogSubscriptionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListAccessLogSubscriptionsRequestPaginateTypeDef


def get_value() -> ListAccessLogSubscriptionsRequestPaginateTypeDef:
    return {
        "resourceIdentifier": ...,
    }


# ListAccessLogSubscriptionsRequestPaginateTypeDef definition

class ListAccessLogSubscriptionsRequestPaginateTypeDef(TypedDict):
    resourceIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListListenersRequestPaginateTypeDef

```python
# ListListenersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListListenersRequestPaginateTypeDef


def get_value() -> ListListenersRequestPaginateTypeDef:
    return {
        "serviceIdentifier": ...,
    }


# ListListenersRequestPaginateTypeDef definition

class ListListenersRequestPaginateTypeDef(TypedDict):
    serviceIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceConfigurationsRequestPaginateTypeDef

```python
# ListResourceConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListResourceConfigurationsRequestPaginateTypeDef


def get_value() -> ListResourceConfigurationsRequestPaginateTypeDef:
    return {
        "resourceConfigurationGroupIdentifier": ...,
    }


# ListResourceConfigurationsRequestPaginateTypeDef definition

class ListResourceConfigurationsRequestPaginateTypeDef(TypedDict):
    resourceConfigurationGroupIdentifier: NotRequired[str],
    resourceGatewayIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceEndpointAssociationsRequestPaginateTypeDef

```python
# ListResourceEndpointAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListResourceEndpointAssociationsRequestPaginateTypeDef


def get_value() -> ListResourceEndpointAssociationsRequestPaginateTypeDef:
    return {
        "resourceConfigurationIdentifier": ...,
    }


# ListResourceEndpointAssociationsRequestPaginateTypeDef definition

class ListResourceEndpointAssociationsRequestPaginateTypeDef(TypedDict):
    resourceConfigurationIdentifier: str,
    resourceEndpointAssociationIdentifier: NotRequired[str],
    vpcEndpointId: NotRequired[str],
    vpcEndpointOwner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceGatewaysRequestPaginateTypeDef

```python
# ListResourceGatewaysRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListResourceGatewaysRequestPaginateTypeDef


def get_value() -> ListResourceGatewaysRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListResourceGatewaysRequestPaginateTypeDef definition

class ListResourceGatewaysRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesRequestPaginateTypeDef

```python
# ListRulesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListRulesRequestPaginateTypeDef


def get_value() -> ListRulesRequestPaginateTypeDef:
    return {
        "listenerIdentifier": ...,
    }


# ListRulesRequestPaginateTypeDef definition

class ListRulesRequestPaginateTypeDef(TypedDict):
    listenerIdentifier: str,
    serviceIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceNetworkResourceAssociationsRequestPaginateTypeDef

```python
# ListServiceNetworkResourceAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkResourceAssociationsRequestPaginateTypeDef


def get_value() -> ListServiceNetworkResourceAssociationsRequestPaginateTypeDef:
    return {
        "resourceConfigurationIdentifier": ...,
    }


# ListServiceNetworkResourceAssociationsRequestPaginateTypeDef definition

class ListServiceNetworkResourceAssociationsRequestPaginateTypeDef(TypedDict):
    resourceConfigurationIdentifier: NotRequired[str],
    serviceNetworkIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceNetworkServiceAssociationsRequestPaginateTypeDef

```python
# ListServiceNetworkServiceAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkServiceAssociationsRequestPaginateTypeDef


def get_value() -> ListServiceNetworkServiceAssociationsRequestPaginateTypeDef:
    return {
        "serviceIdentifier": ...,
    }


# ListServiceNetworkServiceAssociationsRequestPaginateTypeDef definition

class ListServiceNetworkServiceAssociationsRequestPaginateTypeDef(TypedDict):
    serviceIdentifier: NotRequired[str],
    serviceNetworkIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceNetworkVpcAssociationsRequestPaginateTypeDef

```python
# ListServiceNetworkVpcAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkVpcAssociationsRequestPaginateTypeDef


def get_value() -> ListServiceNetworkVpcAssociationsRequestPaginateTypeDef:
    return {
        "serviceNetworkIdentifier": ...,
    }


# ListServiceNetworkVpcAssociationsRequestPaginateTypeDef definition

class ListServiceNetworkVpcAssociationsRequestPaginateTypeDef(TypedDict):
    serviceNetworkIdentifier: NotRequired[str],
    vpcIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceNetworkVpcEndpointAssociationsRequestPaginateTypeDef

```python
# ListServiceNetworkVpcEndpointAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkVpcEndpointAssociationsRequestPaginateTypeDef


def get_value() -> ListServiceNetworkVpcEndpointAssociationsRequestPaginateTypeDef:
    return {
        "serviceNetworkIdentifier": ...,
    }


# ListServiceNetworkVpcEndpointAssociationsRequestPaginateTypeDef definition

class ListServiceNetworkVpcEndpointAssociationsRequestPaginateTypeDef(TypedDict):
    serviceNetworkIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceNetworksRequestPaginateTypeDef

```python
# ListServiceNetworksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworksRequestPaginateTypeDef


def get_value() -> ListServiceNetworksRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListServiceNetworksRequestPaginateTypeDef definition

class ListServiceNetworksRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesRequestPaginateTypeDef

```python
# ListServicesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServicesRequestPaginateTypeDef


def get_value() -> ListServicesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListServicesRequestPaginateTypeDef definition

class ListServicesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTargetGroupsRequestPaginateTypeDef

```python
# ListTargetGroupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListTargetGroupsRequestPaginateTypeDef


def get_value() -> ListTargetGroupsRequestPaginateTypeDef:
    return {
        "targetGroupType": ...,
    }


# ListTargetGroupsRequestPaginateTypeDef definition

class ListTargetGroupsRequestPaginateTypeDef(TypedDict):
    targetGroupType: NotRequired[TargetGroupTypeType],  # (1)
    vpcIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTargetsRequestPaginateTypeDef

```python
# ListTargetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListTargetsRequestPaginateTypeDef


def get_value() -> ListTargetsRequestPaginateTypeDef:
    return {
        "targetGroupIdentifier": ...,
    }


# ListTargetsRequestPaginateTypeDef definition

class ListTargetsRequestPaginateTypeDef(TypedDict):
    targetGroupIdentifier: str,
    targets: NotRequired[Sequence[TargetTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListListenersResponseTypeDef

```python
# ListListenersResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListListenersResponseTypeDef


def get_value() -> ListListenersResponseTypeDef:
    return {
        "items": ...,
    }


# ListListenersResponseTypeDef definition

class ListListenersResponseTypeDef(TypedDict):
    items: List[ListenerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListenerSummaryTypeDef](./type_defs.md#listenersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceConfigurationsResponseTypeDef

```python
# ListResourceConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListResourceConfigurationsResponseTypeDef


def get_value() -> ListResourceConfigurationsResponseTypeDef:
    return {
        "items": ...,
    }


# ListResourceConfigurationsResponseTypeDef definition

class ListResourceConfigurationsResponseTypeDef(TypedDict):
    items: List[ResourceConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceConfigurationSummaryTypeDef](./type_defs.md#resourceconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceEndpointAssociationsResponseTypeDef

```python
# ListResourceEndpointAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListResourceEndpointAssociationsResponseTypeDef


def get_value() -> ListResourceEndpointAssociationsResponseTypeDef:
    return {
        "items": ...,
    }


# ListResourceEndpointAssociationsResponseTypeDef definition

class ListResourceEndpointAssociationsResponseTypeDef(TypedDict):
    items: List[ResourceEndpointAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceEndpointAssociationSummaryTypeDef](./type_defs.md#resourceendpointassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceGatewaysResponseTypeDef

```python
# ListResourceGatewaysResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListResourceGatewaysResponseTypeDef


def get_value() -> ListResourceGatewaysResponseTypeDef:
    return {
        "items": ...,
    }


# ListResourceGatewaysResponseTypeDef definition

class ListResourceGatewaysResponseTypeDef(TypedDict):
    items: List[ResourceGatewaySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceGatewaySummaryTypeDef](./type_defs.md#resourcegatewaysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRulesResponseTypeDef

```python
# ListRulesResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListRulesResponseTypeDef


def get_value() -> ListRulesResponseTypeDef:
    return {
        "items": ...,
    }


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
# ListServiceNetworkVpcAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkVpcAssociationsResponseTypeDef


def get_value() -> ListServiceNetworkVpcAssociationsResponseTypeDef:
    return {
        "items": ...,
    }


# ListServiceNetworkVpcAssociationsResponseTypeDef definition

class ListServiceNetworkVpcAssociationsResponseTypeDef(TypedDict):
    items: List[ServiceNetworkVpcAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceNetworkVpcAssociationSummaryTypeDef](./type_defs.md#servicenetworkvpcassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceNetworkVpcEndpointAssociationsResponseTypeDef

```python
# ListServiceNetworkVpcEndpointAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkVpcEndpointAssociationsResponseTypeDef


def get_value() -> ListServiceNetworkVpcEndpointAssociationsResponseTypeDef:
    return {
        "items": ...,
    }


# ListServiceNetworkVpcEndpointAssociationsResponseTypeDef definition

class ListServiceNetworkVpcEndpointAssociationsResponseTypeDef(TypedDict):
    items: List[ServiceNetworkEndpointAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceNetworkEndpointAssociationTypeDef](./type_defs.md#servicenetworkendpointassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceNetworksResponseTypeDef

```python
# ListServiceNetworksResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworksResponseTypeDef


def get_value() -> ListServiceNetworksResponseTypeDef:
    return {
        "items": ...,
    }


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
# ListTargetGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListTargetGroupsResponseTypeDef


def get_value() -> ListTargetGroupsResponseTypeDef:
    return {
        "items": ...,
    }


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
# ListTargetsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListTargetsResponseTypeDef


def get_value() -> ListTargetsResponseTypeDef:
    return {
        "items": ...,
    }


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
# PathMatchTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import PathMatchTypeDef


def get_value() -> PathMatchTypeDef:
    return {
        "caseSensitive": ...,
    }


# PathMatchTypeDef definition

class PathMatchTypeDef(TypedDict):
    match: PathMatchTypeTypeDef,  # (1)
    caseSensitive: NotRequired[bool],
```

1. See [:material-code-braces: PathMatchTypeTypeDef](./type_defs.md#pathmatchtypetypedef) 
## ListServiceNetworkResourceAssociationsResponseTypeDef

```python
# ListServiceNetworkResourceAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkResourceAssociationsResponseTypeDef


def get_value() -> ListServiceNetworkResourceAssociationsResponseTypeDef:
    return {
        "items": ...,
    }


# ListServiceNetworkResourceAssociationsResponseTypeDef definition

class ListServiceNetworkResourceAssociationsResponseTypeDef(TypedDict):
    items: List[ServiceNetworkResourceAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceNetworkResourceAssociationSummaryTypeDef](./type_defs.md#servicenetworkresourceassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceNetworkServiceAssociationsResponseTypeDef

```python
# ListServiceNetworkServiceAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServiceNetworkServiceAssociationsResponseTypeDef


def get_value() -> ListServiceNetworkServiceAssociationsResponseTypeDef:
    return {
        "items": ...,
    }


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
# ListServicesResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import ListServicesResponseTypeDef


def get_value() -> ListServicesResponseTypeDef:
    return {
        "items": ...,
    }


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
# RuleActionOutputTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleActionOutputTypeDef


def get_value() -> RuleActionOutputTypeDef:
    return {
        "fixedResponse": ...,
    }


# RuleActionOutputTypeDef definition

class RuleActionOutputTypeDef(TypedDict):
    fixedResponse: NotRequired[FixedResponseActionTypeDef],  # (1)
    forward: NotRequired[ForwardActionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: FixedResponseActionTypeDef](./type_defs.md#fixedresponseactiontypedef) 
2. See [:material-code-braces: ForwardActionOutputTypeDef](./type_defs.md#forwardactionoutputtypedef) 
## TargetGroupConfigTypeDef

```python
# TargetGroupConfigTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import TargetGroupConfigTypeDef


def get_value() -> TargetGroupConfigTypeDef:
    return {
        "healthCheck": ...,
    }


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
## UpdateTargetGroupRequestTypeDef

```python
# UpdateTargetGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateTargetGroupRequestTypeDef


def get_value() -> UpdateTargetGroupRequestTypeDef:
    return {
        "healthCheck": ...,
    }


# UpdateTargetGroupRequestTypeDef definition

class UpdateTargetGroupRequestTypeDef(TypedDict):
    healthCheck: HealthCheckConfigTypeDef,  # (1)
    targetGroupIdentifier: str,
```

1. See [:material-code-braces: HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef) 
## CreateResourceConfigurationRequestTypeDef

```python
# CreateResourceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateResourceConfigurationRequestTypeDef


def get_value() -> CreateResourceConfigurationRequestTypeDef:
    return {
        "name": ...,
    }


# CreateResourceConfigurationRequestTypeDef definition

class CreateResourceConfigurationRequestTypeDef(TypedDict):
    name: str,
    type: ResourceConfigurationTypeType,  # (1)
    allowAssociationToShareableServiceNetwork: NotRequired[bool],
    clientToken: NotRequired[str],
    portRanges: NotRequired[Sequence[str]],
    protocol: NotRequired[ProtocolTypeType],  # (2)
    resourceConfigurationDefinition: NotRequired[ResourceConfigurationDefinitionTypeDef],  # (3)
    resourceConfigurationGroupIdentifier: NotRequired[str],
    resourceGatewayIdentifier: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ResourceConfigurationTypeType](./literals.md#resourceconfigurationtypetype) 
2. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
3. See [:material-code-braces: ResourceConfigurationDefinitionTypeDef](./type_defs.md#resourceconfigurationdefinitiontypedef) 
## CreateResourceConfigurationResponseTypeDef

```python
# CreateResourceConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateResourceConfigurationResponseTypeDef


def get_value() -> CreateResourceConfigurationResponseTypeDef:
    return {
        "allowAssociationToShareableServiceNetwork": ...,
    }


# CreateResourceConfigurationResponseTypeDef definition

class CreateResourceConfigurationResponseTypeDef(TypedDict):
    allowAssociationToShareableServiceNetwork: bool,
    arn: str,
    createdAt: datetime,
    failureReason: str,
    id: str,
    name: str,
    portRanges: List[str],
    protocol: ProtocolTypeType,  # (1)
    resourceConfigurationDefinition: ResourceConfigurationDefinitionTypeDef,  # (2)
    resourceConfigurationGroupId: str,
    resourceGatewayId: str,
    status: ResourceConfigurationStatusType,  # (3)
    type: ResourceConfigurationTypeType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
2. See [:material-code-braces: ResourceConfigurationDefinitionTypeDef](./type_defs.md#resourceconfigurationdefinitiontypedef) 
3. See [:material-code-brackets: ResourceConfigurationStatusType](./literals.md#resourceconfigurationstatustype) 
4. See [:material-code-brackets: ResourceConfigurationTypeType](./literals.md#resourceconfigurationtypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceConfigurationResponseTypeDef

```python
# GetResourceConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetResourceConfigurationResponseTypeDef


def get_value() -> GetResourceConfigurationResponseTypeDef:
    return {
        "allowAssociationToShareableServiceNetwork": ...,
    }


# GetResourceConfigurationResponseTypeDef definition

class GetResourceConfigurationResponseTypeDef(TypedDict):
    allowAssociationToShareableServiceNetwork: bool,
    amazonManaged: bool,
    arn: str,
    createdAt: datetime,
    customDomainName: str,
    failureReason: str,
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    portRanges: List[str],
    protocol: ProtocolTypeType,  # (1)
    resourceConfigurationDefinition: ResourceConfigurationDefinitionTypeDef,  # (2)
    resourceConfigurationGroupId: str,
    resourceGatewayId: str,
    status: ResourceConfigurationStatusType,  # (3)
    type: ResourceConfigurationTypeType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
2. See [:material-code-braces: ResourceConfigurationDefinitionTypeDef](./type_defs.md#resourceconfigurationdefinitiontypedef) 
3. See [:material-code-brackets: ResourceConfigurationStatusType](./literals.md#resourceconfigurationstatustype) 
4. See [:material-code-brackets: ResourceConfigurationTypeType](./literals.md#resourceconfigurationtypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResourceConfigurationRequestTypeDef

```python
# UpdateResourceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateResourceConfigurationRequestTypeDef


def get_value() -> UpdateResourceConfigurationRequestTypeDef:
    return {
        "resourceConfigurationIdentifier": ...,
    }


# UpdateResourceConfigurationRequestTypeDef definition

class UpdateResourceConfigurationRequestTypeDef(TypedDict):
    resourceConfigurationIdentifier: str,
    allowAssociationToShareableServiceNetwork: NotRequired[bool],
    portRanges: NotRequired[Sequence[str]],
    resourceConfigurationDefinition: NotRequired[ResourceConfigurationDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceConfigurationDefinitionTypeDef](./type_defs.md#resourceconfigurationdefinitiontypedef) 
## UpdateResourceConfigurationResponseTypeDef

```python
# UpdateResourceConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateResourceConfigurationResponseTypeDef


def get_value() -> UpdateResourceConfigurationResponseTypeDef:
    return {
        "allowAssociationToShareableServiceNetwork": ...,
    }


# UpdateResourceConfigurationResponseTypeDef definition

class UpdateResourceConfigurationResponseTypeDef(TypedDict):
    allowAssociationToShareableServiceNetwork: bool,
    arn: str,
    id: str,
    name: str,
    portRanges: List[str],
    protocol: ProtocolTypeType,  # (1)
    resourceConfigurationDefinition: ResourceConfigurationDefinitionTypeDef,  # (2)
    resourceConfigurationGroupId: str,
    resourceGatewayId: str,
    status: ResourceConfigurationStatusType,  # (3)
    type: ResourceConfigurationTypeType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
2. See [:material-code-braces: ResourceConfigurationDefinitionTypeDef](./type_defs.md#resourceconfigurationdefinitiontypedef) 
3. See [:material-code-brackets: ResourceConfigurationStatusType](./literals.md#resourceconfigurationstatustype) 
4. See [:material-code-brackets: ResourceConfigurationTypeType](./literals.md#resourceconfigurationtypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HttpMatchOutputTypeDef

```python
# HttpMatchOutputTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import HttpMatchOutputTypeDef


def get_value() -> HttpMatchOutputTypeDef:
    return {
        "headerMatches": ...,
    }


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
# HttpMatchTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import HttpMatchTypeDef


def get_value() -> HttpMatchTypeDef:
    return {
        "headerMatches": ...,
    }


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
# CreateListenerResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateListenerResponseTypeDef


def get_value() -> CreateListenerResponseTypeDef:
    return {
        "arn": ...,
    }


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
# GetListenerResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetListenerResponseTypeDef


def get_value() -> GetListenerResponseTypeDef:
    return {
        "arn": ...,
    }


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
# UpdateListenerResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateListenerResponseTypeDef


def get_value() -> UpdateListenerResponseTypeDef:
    return {
        "arn": ...,
    }


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
# RuleActionTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleActionTypeDef


def get_value() -> RuleActionTypeDef:
    return {
        "fixedResponse": ...,
    }


# RuleActionTypeDef definition

class RuleActionTypeDef(TypedDict):
    fixedResponse: NotRequired[FixedResponseActionTypeDef],  # (1)
    forward: NotRequired[ForwardActionUnionTypeDef],  # (2)
```

1. See [:material-code-braces: FixedResponseActionTypeDef](./type_defs.md#fixedresponseactiontypedef) 
2. See [:material-code-braces: ForwardActionTypeDef](./type_defs.md#forwardactiontypedef) [:material-code-braces: ForwardActionOutputTypeDef](./type_defs.md#forwardactionoutputtypedef) 
## CreateTargetGroupRequestTypeDef

```python
# CreateTargetGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateTargetGroupRequestTypeDef


def get_value() -> CreateTargetGroupRequestTypeDef:
    return {
        "name": ...,
    }


# CreateTargetGroupRequestTypeDef definition

class CreateTargetGroupRequestTypeDef(TypedDict):
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
# CreateTargetGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateTargetGroupResponseTypeDef


def get_value() -> CreateTargetGroupResponseTypeDef:
    return {
        "arn": ...,
    }


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
# GetTargetGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetTargetGroupResponseTypeDef


def get_value() -> GetTargetGroupResponseTypeDef:
    return {
        "arn": ...,
    }


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
# UpdateTargetGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateTargetGroupResponseTypeDef


def get_value() -> UpdateTargetGroupResponseTypeDef:
    return {
        "arn": ...,
    }


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
# RuleMatchOutputTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleMatchOutputTypeDef


def get_value() -> RuleMatchOutputTypeDef:
    return {
        "httpMatch": ...,
    }


# RuleMatchOutputTypeDef definition

class RuleMatchOutputTypeDef(TypedDict):
    httpMatch: NotRequired[HttpMatchOutputTypeDef],  # (1)
```

1. See [:material-code-braces: HttpMatchOutputTypeDef](./type_defs.md#httpmatchoutputtypedef) 
## CreateRuleResponseTypeDef

```python
# CreateRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateRuleResponseTypeDef


def get_value() -> CreateRuleResponseTypeDef:
    return {
        "action": ...,
    }


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
# GetRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import GetRuleResponseTypeDef


def get_value() -> GetRuleResponseTypeDef:
    return {
        "action": ...,
    }


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
# RuleUpdateSuccessTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleUpdateSuccessTypeDef


def get_value() -> RuleUpdateSuccessTypeDef:
    return {
        "action": ...,
    }


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
# UpdateRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateRuleResponseTypeDef


def get_value() -> UpdateRuleResponseTypeDef:
    return {
        "action": ...,
    }


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
# RuleMatchTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleMatchTypeDef


def get_value() -> RuleMatchTypeDef:
    return {
        "httpMatch": ...,
    }


# RuleMatchTypeDef definition

class RuleMatchTypeDef(TypedDict):
    httpMatch: NotRequired[HttpMatchUnionTypeDef],  # (1)
```

1. See [:material-code-braces: HttpMatchTypeDef](./type_defs.md#httpmatchtypedef) [:material-code-braces: HttpMatchOutputTypeDef](./type_defs.md#httpmatchoutputtypedef) 
## CreateListenerRequestTypeDef

```python
# CreateListenerRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateListenerRequestTypeDef


def get_value() -> CreateListenerRequestTypeDef:
    return {
        "defaultAction": ...,
    }


# CreateListenerRequestTypeDef definition

class CreateListenerRequestTypeDef(TypedDict):
    defaultAction: RuleActionUnionTypeDef,  # (1)
    name: str,
    protocol: ListenerProtocolType,  # (2)
    serviceIdentifier: str,
    clientToken: NotRequired[str],
    port: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-brackets: ListenerProtocolType](./literals.md#listenerprotocoltype) 
## UpdateListenerRequestTypeDef

```python
# UpdateListenerRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateListenerRequestTypeDef


def get_value() -> UpdateListenerRequestTypeDef:
    return {
        "defaultAction": ...,
    }


# UpdateListenerRequestTypeDef definition

class UpdateListenerRequestTypeDef(TypedDict):
    defaultAction: RuleActionUnionTypeDef,  # (1)
    listenerIdentifier: str,
    serviceIdentifier: str,
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
## BatchUpdateRuleResponseTypeDef

```python
# BatchUpdateRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import BatchUpdateRuleResponseTypeDef


def get_value() -> BatchUpdateRuleResponseTypeDef:
    return {
        "successful": ...,
    }


# BatchUpdateRuleResponseTypeDef definition

class BatchUpdateRuleResponseTypeDef(TypedDict):
    successful: List[RuleUpdateSuccessTypeDef],  # (1)
    unsuccessful: List[RuleUpdateFailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuleUpdateSuccessTypeDef](./type_defs.md#ruleupdatesuccesstypedef) 
2. See [:material-code-braces: RuleUpdateFailureTypeDef](./type_defs.md#ruleupdatefailuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleRequestTypeDef

```python
# CreateRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import CreateRuleRequestTypeDef


def get_value() -> CreateRuleRequestTypeDef:
    return {
        "action": ...,
    }


# CreateRuleRequestTypeDef definition

class CreateRuleRequestTypeDef(TypedDict):
    action: RuleActionUnionTypeDef,  # (1)
    listenerIdentifier: str,
    match: RuleMatchUnionTypeDef,  # (2)
    name: str,
    priority: int,
    serviceIdentifier: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleMatchTypeDef](./type_defs.md#rulematchtypedef) [:material-code-braces: RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef) 
## RuleUpdateTypeDef

```python
# RuleUpdateTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import RuleUpdateTypeDef


def get_value() -> RuleUpdateTypeDef:
    return {
        "action": ...,
    }


# RuleUpdateTypeDef definition

class RuleUpdateTypeDef(TypedDict):
    ruleIdentifier: str,
    action: NotRequired[RuleActionUnionTypeDef],  # (1)
    match: NotRequired[RuleMatchUnionTypeDef],  # (2)
    priority: NotRequired[int],
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleMatchTypeDef](./type_defs.md#rulematchtypedef) [:material-code-braces: RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef) 
## UpdateRuleRequestTypeDef

```python
# UpdateRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import UpdateRuleRequestTypeDef


def get_value() -> UpdateRuleRequestTypeDef:
    return {
        "listenerIdentifier": ...,
    }


# UpdateRuleRequestTypeDef definition

class UpdateRuleRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    ruleIdentifier: str,
    serviceIdentifier: str,
    action: NotRequired[RuleActionUnionTypeDef],  # (1)
    match: NotRequired[RuleMatchUnionTypeDef],  # (2)
    priority: NotRequired[int],
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
2. See [:material-code-braces: RuleMatchTypeDef](./type_defs.md#rulematchtypedef) [:material-code-braces: RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef) 
## BatchUpdateRuleRequestTypeDef

```python
# BatchUpdateRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_vpc_lattice.type_defs import BatchUpdateRuleRequestTypeDef


def get_value() -> BatchUpdateRuleRequestTypeDef:
    return {
        "listenerIdentifier": ...,
    }


# BatchUpdateRuleRequestTypeDef definition

class BatchUpdateRuleRequestTypeDef(TypedDict):
    listenerIdentifier: str,
    rules: Sequence[RuleUpdateTypeDef],  # (1)
    serviceIdentifier: str,
```

1. See [:material-code-braces: RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef) 
