# Type definitions

> [Index](../README.md) > [RTBFabric](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RTBFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#rtbfabric)
    type annotations stubs module [types-aiobotocore-rtbfabric](https://pypi.org/project/types-aiobotocore-rtbfabric/).

## FilterCriterionUnionTypeDef

```python
# FilterCriterionUnionTypeDef Union usage example

from types_aiobotocore_rtbfabric.type_defs import FilterCriterionUnionTypeDef


def get_value() -> FilterCriterionUnionTypeDef:
    return ...


# FilterCriterionUnionTypeDef definition

FilterCriterionUnionTypeDef = Union[
    FilterCriterionTypeDef,  # (1)
    FilterCriterionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FilterCriterionTypeDef](./type_defs.md#filtercriteriontypedef)
2. See [:material-code-braces: FilterCriterionOutputTypeDef](./type_defs.md#filtercriterionoutputtypedef)

## TrustStoreConfigurationUnionTypeDef

```python
# TrustStoreConfigurationUnionTypeDef Union usage example

from types_aiobotocore_rtbfabric.type_defs import TrustStoreConfigurationUnionTypeDef


def get_value() -> TrustStoreConfigurationUnionTypeDef:
    return ...


# TrustStoreConfigurationUnionTypeDef definition

TrustStoreConfigurationUnionTypeDef = Union[
    TrustStoreConfigurationTypeDef,  # (1)
    TrustStoreConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TrustStoreConfigurationTypeDef](./type_defs.md#truststoreconfigurationtypedef)
2. See [:material-code-braces: TrustStoreConfigurationOutputTypeDef](./type_defs.md#truststoreconfigurationoutputtypedef)

## ManagedEndpointConfigurationUnionTypeDef

```python
# ManagedEndpointConfigurationUnionTypeDef Union usage example

from types_aiobotocore_rtbfabric.type_defs import ManagedEndpointConfigurationUnionTypeDef


def get_value() -> ManagedEndpointConfigurationUnionTypeDef:
    return ...


# ManagedEndpointConfigurationUnionTypeDef definition

ManagedEndpointConfigurationUnionTypeDef = Union[
    ManagedEndpointConfigurationTypeDef,  # (1)
    ManagedEndpointConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ManagedEndpointConfigurationTypeDef](./type_defs.md#managedendpointconfigurationtypedef)
2. See [:material-code-braces: ManagedEndpointConfigurationOutputTypeDef](./type_defs.md#managedendpointconfigurationoutputtypedef)

## LinkAttributesUnionTypeDef

```python
# LinkAttributesUnionTypeDef Union usage example

from types_aiobotocore_rtbfabric.type_defs import LinkAttributesUnionTypeDef


def get_value() -> LinkAttributesUnionTypeDef:
    return ...


# LinkAttributesUnionTypeDef definition

LinkAttributesUnionTypeDef = Union[
    LinkAttributesTypeDef,  # (1)
    LinkAttributesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LinkAttributesTypeDef](./type_defs.md#linkattributestypedef)
2. See [:material-code-braces: LinkAttributesOutputTypeDef](./type_defs.md#linkattributesoutputtypedef)

## FilterUnionTypeDef

```python
# FilterUnionTypeDef Union usage example

from types_aiobotocore_rtbfabric.type_defs import FilterUnionTypeDef


def get_value() -> FilterUnionTypeDef:
    return ...


# FilterUnionTypeDef definition

FilterUnionTypeDef = Union[
    FilterTypeDef,  # (1)
    FilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef)
2. See [:material-code-braces: FilterOutputTypeDef](./type_defs.md#filteroutputtypedef)

## OpenRtbAttributeModuleParametersUnionTypeDef

```python
# OpenRtbAttributeModuleParametersUnionTypeDef Union usage example

from types_aiobotocore_rtbfabric.type_defs import OpenRtbAttributeModuleParametersUnionTypeDef


def get_value() -> OpenRtbAttributeModuleParametersUnionTypeDef:
    return ...


# OpenRtbAttributeModuleParametersUnionTypeDef definition

OpenRtbAttributeModuleParametersUnionTypeDef = Union[
    OpenRtbAttributeModuleParametersTypeDef,  # (1)
    OpenRtbAttributeModuleParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OpenRtbAttributeModuleParametersTypeDef](./type_defs.md#openrtbattributemoduleparameterstypedef)
2. See [:material-code-braces: OpenRtbAttributeModuleParametersOutputTypeDef](./type_defs.md#openrtbattributemoduleparametersoutputtypedef)

## ModuleParametersUnionTypeDef

```python
# ModuleParametersUnionTypeDef Union usage example

from types_aiobotocore_rtbfabric.type_defs import ModuleParametersUnionTypeDef


def get_value() -> ModuleParametersUnionTypeDef:
    return ...


# ModuleParametersUnionTypeDef definition

ModuleParametersUnionTypeDef = Union[
    ModuleParametersTypeDef,  # (1)
    ModuleParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ModuleParametersTypeDef](./type_defs.md#moduleparameterstypedef)
2. See [:material-code-braces: ModuleParametersOutputTypeDef](./type_defs.md#moduleparametersoutputtypedef)

## ModuleConfigurationUnionTypeDef

```python
# ModuleConfigurationUnionTypeDef Union usage example

from types_aiobotocore_rtbfabric.type_defs import ModuleConfigurationUnionTypeDef


def get_value() -> ModuleConfigurationUnionTypeDef:
    return ...


# ModuleConfigurationUnionTypeDef definition

ModuleConfigurationUnionTypeDef = Union[
    ModuleConfigurationTypeDef,  # (1)
    ModuleConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ModuleConfigurationTypeDef](./type_defs.md#moduleconfigurationtypedef)
2. See [:material-code-braces: ModuleConfigurationOutputTypeDef](./type_defs.md#moduleconfigurationoutputtypedef)



## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## HeaderTagActionTypeDef

```python
# HeaderTagActionTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import HeaderTagActionTypeDef


def get_value() -> HeaderTagActionTypeDef:
    return {
        "name": ...,
    }


# HeaderTagActionTypeDef definition

class HeaderTagActionTypeDef(TypedDict):
    name: str,
    value: str,
```


## NoBidActionTypeDef

```python
# NoBidActionTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import NoBidActionTypeDef


def get_value() -> NoBidActionTypeDef:
    return {
        "noBidReasonCode": ...,
    }


# NoBidActionTypeDef definition

class NoBidActionTypeDef(TypedDict):
    noBidReasonCode: NotRequired[int],
```


## AutoScalingGroupsConfigurationOutputTypeDef

```python
# AutoScalingGroupsConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import AutoScalingGroupsConfigurationOutputTypeDef


def get_value() -> AutoScalingGroupsConfigurationOutputTypeDef:
    return {
        "autoScalingGroupNames": ...,
    }


# AutoScalingGroupsConfigurationOutputTypeDef definition

class AutoScalingGroupsConfigurationOutputTypeDef(TypedDict):
    autoScalingGroupNames: list[str],
    roleArn: str,
```


## AutoScalingGroupsConfigurationTypeDef

```python
# AutoScalingGroupsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import AutoScalingGroupsConfigurationTypeDef


def get_value() -> AutoScalingGroupsConfigurationTypeDef:
    return {
        "autoScalingGroupNames": ...,
    }


# AutoScalingGroupsConfigurationTypeDef definition

class AutoScalingGroupsConfigurationTypeDef(TypedDict):
    autoScalingGroupNames: Sequence[str],
    roleArn: str,
```


## CreateRequesterGatewayRequestTypeDef

```python
# CreateRequesterGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateRequesterGatewayRequestTypeDef


def get_value() -> CreateRequesterGatewayRequestTypeDef:
    return {
        "vpcId": ...,
    }


# CreateRequesterGatewayRequestTypeDef definition

class CreateRequesterGatewayRequestTypeDef(TypedDict):
    vpcId: str,
    subnetIds: Sequence[str],
    securityGroupIds: Sequence[str],
    clientToken: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```


## DeleteInboundExternalLinkRequestTypeDef

```python
# DeleteInboundExternalLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteInboundExternalLinkRequestTypeDef


def get_value() -> DeleteInboundExternalLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# DeleteInboundExternalLinkRequestTypeDef definition

class DeleteInboundExternalLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
```


## DeleteLinkRequestTypeDef

```python
# DeleteLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteLinkRequestTypeDef


def get_value() -> DeleteLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# DeleteLinkRequestTypeDef definition

class DeleteLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
```


## DeleteOutboundExternalLinkRequestTypeDef

```python
# DeleteOutboundExternalLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteOutboundExternalLinkRequestTypeDef


def get_value() -> DeleteOutboundExternalLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# DeleteOutboundExternalLinkRequestTypeDef definition

class DeleteOutboundExternalLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
```


## DeleteRequesterGatewayRequestTypeDef

```python
# DeleteRequesterGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteRequesterGatewayRequestTypeDef


def get_value() -> DeleteRequesterGatewayRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# DeleteRequesterGatewayRequestTypeDef definition

class DeleteRequesterGatewayRequestTypeDef(TypedDict):
    gatewayId: str,
```


## DeleteResponderGatewayRequestTypeDef

```python
# DeleteResponderGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteResponderGatewayRequestTypeDef


def get_value() -> DeleteResponderGatewayRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# DeleteResponderGatewayRequestTypeDef definition

class DeleteResponderGatewayRequestTypeDef(TypedDict):
    gatewayId: str,
```


## EksEndpointsConfigurationTypeDef

```python
# EksEndpointsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import EksEndpointsConfigurationTypeDef


def get_value() -> EksEndpointsConfigurationTypeDef:
    return {
        "endpointsResourceName": ...,
    }


# EksEndpointsConfigurationTypeDef definition

class EksEndpointsConfigurationTypeDef(TypedDict):
    endpointsResourceName: str,
    endpointsResourceNamespace: str,
    clusterApiServerEndpointUri: str,
    clusterApiServerCaCertificateChain: str,
    clusterName: str,
    roleArn: str,
```


## FilterCriterionOutputTypeDef

```python
# FilterCriterionOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import FilterCriterionOutputTypeDef


def get_value() -> FilterCriterionOutputTypeDef:
    return {
        "path": ...,
    }


# FilterCriterionOutputTypeDef definition

class FilterCriterionOutputTypeDef(TypedDict):
    path: str,
    values: list[str],
```


## FilterCriterionTypeDef

```python
# FilterCriterionTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import FilterCriterionTypeDef


def get_value() -> FilterCriterionTypeDef:
    return {
        "path": ...,
    }


# FilterCriterionTypeDef definition

class FilterCriterionTypeDef(TypedDict):
    path: str,
    values: Sequence[str],
```


## GetInboundExternalLinkRequestTypeDef

```python
# GetInboundExternalLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetInboundExternalLinkRequestTypeDef


def get_value() -> GetInboundExternalLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# GetInboundExternalLinkRequestTypeDef definition

class GetInboundExternalLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
```


## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```


## GetLinkRequestTypeDef

```python
# GetLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetLinkRequestTypeDef


def get_value() -> GetLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# GetLinkRequestTypeDef definition

class GetLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
```


## GetOutboundExternalLinkRequestTypeDef

```python
# GetOutboundExternalLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetOutboundExternalLinkRequestTypeDef


def get_value() -> GetOutboundExternalLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# GetOutboundExternalLinkRequestTypeDef definition

class GetOutboundExternalLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
```


## GetRequesterGatewayRequestTypeDef

```python
# GetRequesterGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetRequesterGatewayRequestTypeDef


def get_value() -> GetRequesterGatewayRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# GetRequesterGatewayRequestTypeDef definition

class GetRequesterGatewayRequestTypeDef(TypedDict):
    gatewayId: str,
```


## GetResponderGatewayRequestTypeDef

```python
# GetResponderGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetResponderGatewayRequestTypeDef


def get_value() -> GetResponderGatewayRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# GetResponderGatewayRequestTypeDef definition

class GetResponderGatewayRequestTypeDef(TypedDict):
    gatewayId: str,
```


## TrustStoreConfigurationOutputTypeDef

```python
# TrustStoreConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import TrustStoreConfigurationOutputTypeDef


def get_value() -> TrustStoreConfigurationOutputTypeDef:
    return {
        "certificateAuthorityCertificates": ...,
    }


# TrustStoreConfigurationOutputTypeDef definition

class TrustStoreConfigurationOutputTypeDef(TypedDict):
    certificateAuthorityCertificates: list[str],
```


## LinkApplicationLogSamplingTypeDef

```python
# LinkApplicationLogSamplingTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import LinkApplicationLogSamplingTypeDef


def get_value() -> LinkApplicationLogSamplingTypeDef:
    return {
        "errorLog": ...,
    }


# LinkApplicationLogSamplingTypeDef definition

class LinkApplicationLogSamplingTypeDef(TypedDict):
    errorLog: float,
    filterLog: float,
```


## ResponderErrorMaskingForHttpCodeOutputTypeDef

```python
# ResponderErrorMaskingForHttpCodeOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ResponderErrorMaskingForHttpCodeOutputTypeDef


def get_value() -> ResponderErrorMaskingForHttpCodeOutputTypeDef:
    return {
        "httpCode": ...,
    }


# ResponderErrorMaskingForHttpCodeOutputTypeDef definition

class ResponderErrorMaskingForHttpCodeOutputTypeDef(TypedDict):
    httpCode: str,
    action: ResponderErrorMaskingActionType,  # (1)
    loggingTypes: list[ResponderErrorMaskingLoggingTypeType],  # (2)
    responseLoggingPercentage: NotRequired[float],
```

1. See [:material-code-brackets: ResponderErrorMaskingActionType](./literals.md#respondererrormaskingactiontype)
2. See `list[ResponderErrorMaskingLoggingTypeType]`

## ResponderErrorMaskingForHttpCodeTypeDef

```python
# ResponderErrorMaskingForHttpCodeTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ResponderErrorMaskingForHttpCodeTypeDef


def get_value() -> ResponderErrorMaskingForHttpCodeTypeDef:
    return {
        "httpCode": ...,
    }


# ResponderErrorMaskingForHttpCodeTypeDef definition

class ResponderErrorMaskingForHttpCodeTypeDef(TypedDict):
    httpCode: str,
    action: ResponderErrorMaskingActionType,  # (1)
    loggingTypes: Sequence[ResponderErrorMaskingLoggingTypeType],  # (2)
    responseLoggingPercentage: NotRequired[float],
```

1. See [:material-code-brackets: ResponderErrorMaskingActionType](./literals.md#respondererrormaskingactiontype)
2. See `Sequence[ResponderErrorMaskingLoggingTypeType]`

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import PaginatorConfigTypeDef


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


## ListLinksRequestTypeDef

```python
# ListLinksRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListLinksRequestTypeDef


def get_value() -> ListLinksRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# ListLinksRequestTypeDef definition

class ListLinksRequestTypeDef(TypedDict):
    gatewayId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```


## ListRequesterGatewaysRequestTypeDef

```python
# ListRequesterGatewaysRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListRequesterGatewaysRequestTypeDef


def get_value() -> ListRequesterGatewaysRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListRequesterGatewaysRequestTypeDef definition

class ListRequesterGatewaysRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListResponderGatewaysRequestTypeDef

```python
# ListResponderGatewaysRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListResponderGatewaysRequestTypeDef


def get_value() -> ListResponderGatewaysRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListResponderGatewaysRequestTypeDef definition

class ListResponderGatewaysRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```


## NoBidModuleParametersTypeDef

```python
# NoBidModuleParametersTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import NoBidModuleParametersTypeDef


def get_value() -> NoBidModuleParametersTypeDef:
    return {
        "reason": ...,
    }


# NoBidModuleParametersTypeDef definition

class NoBidModuleParametersTypeDef(TypedDict):
    reason: NotRequired[str],
    reasonCode: NotRequired[int],
    passThroughPercentage: NotRequired[float],
```


## RateLimiterModuleParametersTypeDef

```python
# RateLimiterModuleParametersTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import RateLimiterModuleParametersTypeDef


def get_value() -> RateLimiterModuleParametersTypeDef:
    return {
        "tps": ...,
    }


# RateLimiterModuleParametersTypeDef definition

class RateLimiterModuleParametersTypeDef(TypedDict):
    tps: NotRequired[float],
```


## RejectLinkRequestTypeDef

```python
# RejectLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import RejectLinkRequestTypeDef


def get_value() -> RejectLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# RejectLinkRequestTypeDef definition

class RejectLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
```


## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```


## TrustStoreConfigurationTypeDef

```python
# TrustStoreConfigurationTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import TrustStoreConfigurationTypeDef


def get_value() -> TrustStoreConfigurationTypeDef:
    return {
        "certificateAuthorityCertificates": ...,
    }


# TrustStoreConfigurationTypeDef definition

class TrustStoreConfigurationTypeDef(TypedDict):
    certificateAuthorityCertificates: Sequence[str],
```


## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```


## UpdateRequesterGatewayRequestTypeDef

```python
# UpdateRequesterGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import UpdateRequesterGatewayRequestTypeDef


def get_value() -> UpdateRequesterGatewayRequestTypeDef:
    return {
        "clientToken": ...,
    }


# UpdateRequesterGatewayRequestTypeDef definition

class UpdateRequesterGatewayRequestTypeDef(TypedDict):
    clientToken: str,
    gatewayId: str,
    description: NotRequired[str],
```


## CreateInboundExternalLinkResponseTypeDef

```python
# CreateInboundExternalLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateInboundExternalLinkResponseTypeDef


def get_value() -> CreateInboundExternalLinkResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# CreateInboundExternalLinkResponseTypeDef definition

class CreateInboundExternalLinkResponseTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    status: LinkStatusType,  # (1)
    domainName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateOutboundExternalLinkResponseTypeDef

```python
# CreateOutboundExternalLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateOutboundExternalLinkResponseTypeDef


def get_value() -> CreateOutboundExternalLinkResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# CreateOutboundExternalLinkResponseTypeDef definition

class CreateOutboundExternalLinkResponseTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    status: LinkStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateRequesterGatewayResponseTypeDef

```python
# CreateRequesterGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateRequesterGatewayResponseTypeDef


def get_value() -> CreateRequesterGatewayResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# CreateRequesterGatewayResponseTypeDef definition

class CreateRequesterGatewayResponseTypeDef(TypedDict):
    gatewayId: str,
    domainName: str,
    status: RequesterGatewayStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequesterGatewayStatusType](./literals.md#requestergatewaystatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateResponderGatewayResponseTypeDef

```python
# CreateResponderGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateResponderGatewayResponseTypeDef


def get_value() -> CreateResponderGatewayResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# CreateResponderGatewayResponseTypeDef definition

class CreateResponderGatewayResponseTypeDef(TypedDict):
    gatewayId: str,
    status: ResponderGatewayStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResponderGatewayStatusType](./literals.md#respondergatewaystatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteInboundExternalLinkResponseTypeDef

```python
# DeleteInboundExternalLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteInboundExternalLinkResponseTypeDef


def get_value() -> DeleteInboundExternalLinkResponseTypeDef:
    return {
        "linkId": ...,
    }


# DeleteInboundExternalLinkResponseTypeDef definition

class DeleteInboundExternalLinkResponseTypeDef(TypedDict):
    linkId: str,
    status: LinkStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteLinkResponseTypeDef

```python
# DeleteLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteLinkResponseTypeDef


def get_value() -> DeleteLinkResponseTypeDef:
    return {
        "linkId": ...,
    }


# DeleteLinkResponseTypeDef definition

class DeleteLinkResponseTypeDef(TypedDict):
    linkId: str,
    status: LinkStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteOutboundExternalLinkResponseTypeDef

```python
# DeleteOutboundExternalLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteOutboundExternalLinkResponseTypeDef


def get_value() -> DeleteOutboundExternalLinkResponseTypeDef:
    return {
        "linkId": ...,
    }


# DeleteOutboundExternalLinkResponseTypeDef definition

class DeleteOutboundExternalLinkResponseTypeDef(TypedDict):
    linkId: str,
    status: LinkStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteRequesterGatewayResponseTypeDef

```python
# DeleteRequesterGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteRequesterGatewayResponseTypeDef


def get_value() -> DeleteRequesterGatewayResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# DeleteRequesterGatewayResponseTypeDef definition

class DeleteRequesterGatewayResponseTypeDef(TypedDict):
    gatewayId: str,
    status: RequesterGatewayStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequesterGatewayStatusType](./literals.md#requestergatewaystatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteResponderGatewayResponseTypeDef

```python
# DeleteResponderGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import DeleteResponderGatewayResponseTypeDef


def get_value() -> DeleteResponderGatewayResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# DeleteResponderGatewayResponseTypeDef definition

class DeleteResponderGatewayResponseTypeDef(TypedDict):
    gatewayId: str,
    status: ResponderGatewayStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResponderGatewayStatusType](./literals.md#respondergatewaystatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetRequesterGatewayResponseTypeDef

```python
# GetRequesterGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetRequesterGatewayResponseTypeDef


def get_value() -> GetRequesterGatewayResponseTypeDef:
    return {
        "status": ...,
    }


# GetRequesterGatewayResponseTypeDef definition

class GetRequesterGatewayResponseTypeDef(TypedDict):
    status: RequesterGatewayStatusType,  # (1)
    domainName: str,
    description: str,
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    vpcId: str,
    subnetIds: list[str],
    securityGroupIds: list[str],
    gatewayId: str,
    tags: dict[str, str],
    activeLinksCount: int,
    totalLinksCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequesterGatewayStatusType](./literals.md#requestergatewaystatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListRequesterGatewaysResponseTypeDef

```python
# ListRequesterGatewaysResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListRequesterGatewaysResponseTypeDef


def get_value() -> ListRequesterGatewaysResponseTypeDef:
    return {
        "gatewayIds": ...,
    }


# ListRequesterGatewaysResponseTypeDef definition

class ListRequesterGatewaysResponseTypeDef(TypedDict):
    gatewayIds: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListResponderGatewaysResponseTypeDef

```python
# ListResponderGatewaysResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListResponderGatewaysResponseTypeDef


def get_value() -> ListResponderGatewaysResponseTypeDef:
    return {
        "gatewayIds": ...,
    }


# ListResponderGatewaysResponseTypeDef definition

class ListResponderGatewaysResponseTypeDef(TypedDict):
    gatewayIds: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateLinkModuleFlowResponseTypeDef

```python
# UpdateLinkModuleFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import UpdateLinkModuleFlowResponseTypeDef


def get_value() -> UpdateLinkModuleFlowResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# UpdateLinkModuleFlowResponseTypeDef definition

class UpdateLinkModuleFlowResponseTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    status: LinkStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateLinkResponseTypeDef

```python
# UpdateLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import UpdateLinkResponseTypeDef


def get_value() -> UpdateLinkResponseTypeDef:
    return {
        "linkId": ...,
    }


# UpdateLinkResponseTypeDef definition

class UpdateLinkResponseTypeDef(TypedDict):
    linkId: str,
    status: LinkStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateRequesterGatewayResponseTypeDef

```python
# UpdateRequesterGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import UpdateRequesterGatewayResponseTypeDef


def get_value() -> UpdateRequesterGatewayResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# UpdateRequesterGatewayResponseTypeDef definition

class UpdateRequesterGatewayResponseTypeDef(TypedDict):
    gatewayId: str,
    status: RequesterGatewayStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequesterGatewayStatusType](./literals.md#requestergatewaystatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateResponderGatewayResponseTypeDef

```python
# UpdateResponderGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import UpdateResponderGatewayResponseTypeDef


def get_value() -> UpdateResponderGatewayResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# UpdateResponderGatewayResponseTypeDef definition

class UpdateResponderGatewayResponseTypeDef(TypedDict):
    gatewayId: str,
    status: ResponderGatewayStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResponderGatewayStatusType](./literals.md#respondergatewaystatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ActionTypeDef

```python
# ActionTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ActionTypeDef


def get_value() -> ActionTypeDef:
    return {
        "noBid": ...,
    }


# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    noBid: NotRequired[NoBidActionTypeDef],  # (1)
    headerTag: NotRequired[HeaderTagActionTypeDef],  # (2)
```

1. See [:material-code-braces: NoBidActionTypeDef](./type_defs.md#nobidactiontypedef)
2. See [:material-code-braces: HeaderTagActionTypeDef](./type_defs.md#headertagactiontypedef)

## ManagedEndpointConfigurationOutputTypeDef

```python
# ManagedEndpointConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ManagedEndpointConfigurationOutputTypeDef


def get_value() -> ManagedEndpointConfigurationOutputTypeDef:
    return {
        "autoScalingGroups": ...,
    }


# ManagedEndpointConfigurationOutputTypeDef definition

class ManagedEndpointConfigurationOutputTypeDef(TypedDict):
    autoScalingGroups: NotRequired[AutoScalingGroupsConfigurationOutputTypeDef],  # (1)
    eksEndpoints: NotRequired[EksEndpointsConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: AutoScalingGroupsConfigurationOutputTypeDef](./type_defs.md#autoscalinggroupsconfigurationoutputtypedef)
2. See [:material-code-braces: EksEndpointsConfigurationTypeDef](./type_defs.md#eksendpointsconfigurationtypedef)

## ManagedEndpointConfigurationTypeDef

```python
# ManagedEndpointConfigurationTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ManagedEndpointConfigurationTypeDef


def get_value() -> ManagedEndpointConfigurationTypeDef:
    return {
        "autoScalingGroups": ...,
    }


# ManagedEndpointConfigurationTypeDef definition

class ManagedEndpointConfigurationTypeDef(TypedDict):
    autoScalingGroups: NotRequired[AutoScalingGroupsConfigurationTypeDef],  # (1)
    eksEndpoints: NotRequired[EksEndpointsConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: AutoScalingGroupsConfigurationTypeDef](./type_defs.md#autoscalinggroupsconfigurationtypedef)
2. See [:material-code-braces: EksEndpointsConfigurationTypeDef](./type_defs.md#eksendpointsconfigurationtypedef)

## FilterOutputTypeDef

```python
# FilterOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import FilterOutputTypeDef


def get_value() -> FilterOutputTypeDef:
    return {
        "criteria": ...,
    }


# FilterOutputTypeDef definition

class FilterOutputTypeDef(TypedDict):
    criteria: list[FilterCriterionOutputTypeDef],  # (1)
```

1. See `list[FilterCriterionOutputTypeDef]`

## GetInboundExternalLinkRequestWaitTypeDef

```python
# GetInboundExternalLinkRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetInboundExternalLinkRequestWaitTypeDef


def get_value() -> GetInboundExternalLinkRequestWaitTypeDef:
    return {
        "gatewayId": ...,
    }


# GetInboundExternalLinkRequestWaitTypeDef definition

class GetInboundExternalLinkRequestWaitTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## GetLinkRequestWaitExtraTypeDef

```python
# GetLinkRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetLinkRequestWaitExtraTypeDef


def get_value() -> GetLinkRequestWaitExtraTypeDef:
    return {
        "gatewayId": ...,
    }


# GetLinkRequestWaitExtraTypeDef definition

class GetLinkRequestWaitExtraTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## GetLinkRequestWaitTypeDef

```python
# GetLinkRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetLinkRequestWaitTypeDef


def get_value() -> GetLinkRequestWaitTypeDef:
    return {
        "gatewayId": ...,
    }


# GetLinkRequestWaitTypeDef definition

class GetLinkRequestWaitTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## GetOutboundExternalLinkRequestWaitTypeDef

```python
# GetOutboundExternalLinkRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetOutboundExternalLinkRequestWaitTypeDef


def get_value() -> GetOutboundExternalLinkRequestWaitTypeDef:
    return {
        "gatewayId": ...,
    }


# GetOutboundExternalLinkRequestWaitTypeDef definition

class GetOutboundExternalLinkRequestWaitTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## GetRequesterGatewayRequestWaitExtraTypeDef

```python
# GetRequesterGatewayRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetRequesterGatewayRequestWaitExtraTypeDef


def get_value() -> GetRequesterGatewayRequestWaitExtraTypeDef:
    return {
        "gatewayId": ...,
    }


# GetRequesterGatewayRequestWaitExtraTypeDef definition

class GetRequesterGatewayRequestWaitExtraTypeDef(TypedDict):
    gatewayId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## GetRequesterGatewayRequestWaitTypeDef

```python
# GetRequesterGatewayRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetRequesterGatewayRequestWaitTypeDef


def get_value() -> GetRequesterGatewayRequestWaitTypeDef:
    return {
        "gatewayId": ...,
    }


# GetRequesterGatewayRequestWaitTypeDef definition

class GetRequesterGatewayRequestWaitTypeDef(TypedDict):
    gatewayId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## GetResponderGatewayRequestWaitExtraTypeDef

```python
# GetResponderGatewayRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetResponderGatewayRequestWaitExtraTypeDef


def get_value() -> GetResponderGatewayRequestWaitExtraTypeDef:
    return {
        "gatewayId": ...,
    }


# GetResponderGatewayRequestWaitExtraTypeDef definition

class GetResponderGatewayRequestWaitExtraTypeDef(TypedDict):
    gatewayId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## GetResponderGatewayRequestWaitTypeDef

```python
# GetResponderGatewayRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetResponderGatewayRequestWaitTypeDef


def get_value() -> GetResponderGatewayRequestWaitTypeDef:
    return {
        "gatewayId": ...,
    }


# GetResponderGatewayRequestWaitTypeDef definition

class GetResponderGatewayRequestWaitTypeDef(TypedDict):
    gatewayId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## LinkApplicationLogConfigurationTypeDef

```python
# LinkApplicationLogConfigurationTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import LinkApplicationLogConfigurationTypeDef


def get_value() -> LinkApplicationLogConfigurationTypeDef:
    return {
        "sampling": ...,
    }


# LinkApplicationLogConfigurationTypeDef definition

class LinkApplicationLogConfigurationTypeDef(TypedDict):
    sampling: LinkApplicationLogSamplingTypeDef,  # (1)
```

1. See [:material-code-braces: LinkApplicationLogSamplingTypeDef](./type_defs.md#linkapplicationlogsamplingtypedef)

## LinkAttributesOutputTypeDef

```python
# LinkAttributesOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import LinkAttributesOutputTypeDef


def get_value() -> LinkAttributesOutputTypeDef:
    return {
        "responderErrorMasking": ...,
    }


# LinkAttributesOutputTypeDef definition

class LinkAttributesOutputTypeDef(TypedDict):
    responderErrorMasking: NotRequired[list[ResponderErrorMaskingForHttpCodeOutputTypeDef]],  # (1)
    customerProvidedId: NotRequired[str],
```

1. See `list[ResponderErrorMaskingForHttpCodeOutputTypeDef]`

## LinkAttributesTypeDef

```python
# LinkAttributesTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import LinkAttributesTypeDef


def get_value() -> LinkAttributesTypeDef:
    return {
        "responderErrorMasking": ...,
    }


# LinkAttributesTypeDef definition

class LinkAttributesTypeDef(TypedDict):
    responderErrorMasking: NotRequired[Sequence[ResponderErrorMaskingForHttpCodeTypeDef]],  # (1)
    customerProvidedId: NotRequired[str],
```

1. See `Sequence[ResponderErrorMaskingForHttpCodeTypeDef]`

## ListLinksRequestPaginateTypeDef

```python
# ListLinksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListLinksRequestPaginateTypeDef


def get_value() -> ListLinksRequestPaginateTypeDef:
    return {
        "gatewayId": ...,
    }


# ListLinksRequestPaginateTypeDef definition

class ListLinksRequestPaginateTypeDef(TypedDict):
    gatewayId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListRequesterGatewaysRequestPaginateTypeDef

```python
# ListRequesterGatewaysRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListRequesterGatewaysRequestPaginateTypeDef


def get_value() -> ListRequesterGatewaysRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListRequesterGatewaysRequestPaginateTypeDef definition

class ListRequesterGatewaysRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListResponderGatewaysRequestPaginateTypeDef

```python
# ListResponderGatewaysRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListResponderGatewaysRequestPaginateTypeDef


def get_value() -> ListResponderGatewaysRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListResponderGatewaysRequestPaginateTypeDef definition

class ListResponderGatewaysRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## GetResponderGatewayResponseTypeDef

```python
# GetResponderGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetResponderGatewayResponseTypeDef


def get_value() -> GetResponderGatewayResponseTypeDef:
    return {
        "vpcId": ...,
    }


# GetResponderGatewayResponseTypeDef definition

class GetResponderGatewayResponseTypeDef(TypedDict):
    vpcId: str,
    subnetIds: list[str],
    securityGroupIds: list[str],
    status: ResponderGatewayStatusType,  # (1)
    description: str,
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    domainName: str,
    port: int,
    protocol: ProtocolType,  # (2)
    trustStoreConfiguration: TrustStoreConfigurationOutputTypeDef,  # (3)
    managedEndpointConfiguration: ManagedEndpointConfigurationOutputTypeDef,  # (4)
    gatewayId: str,
    tags: dict[str, str],
    activeLinksCount: int,
    totalLinksCount: int,
    inboundLinksCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ResponderGatewayStatusType](./literals.md#respondergatewaystatustype)
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype)
3. See [:material-code-braces: TrustStoreConfigurationOutputTypeDef](./type_defs.md#truststoreconfigurationoutputtypedef)
4. See [:material-code-braces: ManagedEndpointConfigurationOutputTypeDef](./type_defs.md#managedendpointconfigurationoutputtypedef)
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## OpenRtbAttributeModuleParametersOutputTypeDef

```python
# OpenRtbAttributeModuleParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import OpenRtbAttributeModuleParametersOutputTypeDef


def get_value() -> OpenRtbAttributeModuleParametersOutputTypeDef:
    return {
        "filterType": ...,
    }


# OpenRtbAttributeModuleParametersOutputTypeDef definition

class OpenRtbAttributeModuleParametersOutputTypeDef(TypedDict):
    filterType: FilterTypeType,  # (1)
    filterConfiguration: list[FilterOutputTypeDef],  # (2)
    action: ActionTypeDef,  # (3)
    holdbackPercentage: float,
```

1. See [:material-code-brackets: FilterTypeType](./literals.md#filtertypetype)
2. See `list[FilterOutputTypeDef]`
3. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef)

## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "criteria": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    criteria: Sequence[FilterCriterionUnionTypeDef],  # (1)
```

1. See `Sequence[FilterCriterionUnionTypeDef]`

## LinkLogSettingsTypeDef

```python
# LinkLogSettingsTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import LinkLogSettingsTypeDef


def get_value() -> LinkLogSettingsTypeDef:
    return {
        "applicationLogs": ...,
    }


# LinkLogSettingsTypeDef definition

class LinkLogSettingsTypeDef(TypedDict):
    applicationLogs: LinkApplicationLogConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: LinkApplicationLogConfigurationTypeDef](./type_defs.md#linkapplicationlogconfigurationtypedef)

## CreateResponderGatewayRequestTypeDef

```python
# CreateResponderGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateResponderGatewayRequestTypeDef


def get_value() -> CreateResponderGatewayRequestTypeDef:
    return {
        "vpcId": ...,
    }


# CreateResponderGatewayRequestTypeDef definition

class CreateResponderGatewayRequestTypeDef(TypedDict):
    vpcId: str,
    subnetIds: Sequence[str],
    securityGroupIds: Sequence[str],
    port: int,
    protocol: ProtocolType,  # (1)
    clientToken: str,
    domainName: NotRequired[str],
    trustStoreConfiguration: NotRequired[TrustStoreConfigurationUnionTypeDef],  # (2)
    managedEndpointConfiguration: NotRequired[ManagedEndpointConfigurationUnionTypeDef],  # (3)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype)
2. See [:material-code-braces: TrustStoreConfigurationUnionTypeDef](#truststoreconfigurationuniontypedef)
3. See [:material-code-braces: ManagedEndpointConfigurationUnionTypeDef](#managedendpointconfigurationuniontypedef)

## UpdateResponderGatewayRequestTypeDef

```python
# UpdateResponderGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import UpdateResponderGatewayRequestTypeDef


def get_value() -> UpdateResponderGatewayRequestTypeDef:
    return {
        "port": ...,
    }


# UpdateResponderGatewayRequestTypeDef definition

class UpdateResponderGatewayRequestTypeDef(TypedDict):
    port: int,
    protocol: ProtocolType,  # (1)
    clientToken: str,
    gatewayId: str,
    domainName: NotRequired[str],
    trustStoreConfiguration: NotRequired[TrustStoreConfigurationUnionTypeDef],  # (2)
    managedEndpointConfiguration: NotRequired[ManagedEndpointConfigurationUnionTypeDef],  # (3)
    description: NotRequired[str],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype)
2. See [:material-code-braces: TrustStoreConfigurationUnionTypeDef](#truststoreconfigurationuniontypedef)
3. See [:material-code-braces: ManagedEndpointConfigurationUnionTypeDef](#managedendpointconfigurationuniontypedef)

## ModuleParametersOutputTypeDef

```python
# ModuleParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ModuleParametersOutputTypeDef


def get_value() -> ModuleParametersOutputTypeDef:
    return {
        "noBid": ...,
    }


# ModuleParametersOutputTypeDef definition

class ModuleParametersOutputTypeDef(TypedDict):
    noBid: NotRequired[NoBidModuleParametersTypeDef],  # (1)
    openRtbAttribute: NotRequired[OpenRtbAttributeModuleParametersOutputTypeDef],  # (2)
    rateLimiter: NotRequired[RateLimiterModuleParametersTypeDef],  # (3)
```

1. See [:material-code-braces: NoBidModuleParametersTypeDef](./type_defs.md#nobidmoduleparameterstypedef)
2. See [:material-code-braces: OpenRtbAttributeModuleParametersOutputTypeDef](./type_defs.md#openrtbattributemoduleparametersoutputtypedef)
3. See [:material-code-braces: RateLimiterModuleParametersTypeDef](./type_defs.md#ratelimitermoduleparameterstypedef)

## GetOutboundExternalLinkResponseTypeDef

```python
# GetOutboundExternalLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetOutboundExternalLinkResponseTypeDef


def get_value() -> GetOutboundExternalLinkResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# GetOutboundExternalLinkResponseTypeDef definition

class GetOutboundExternalLinkResponseTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    status: LinkStatusType,  # (1)
    publicEndpoint: str,
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    tags: dict[str, str],
    logSettings: LinkLogSettingsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateLinkRequestTypeDef

```python
# UpdateLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import UpdateLinkRequestTypeDef


def get_value() -> UpdateLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# UpdateLinkRequestTypeDef definition

class UpdateLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    logSettings: NotRequired[LinkLogSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)

## AcceptLinkRequestTypeDef

```python
# AcceptLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import AcceptLinkRequestTypeDef


def get_value() -> AcceptLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# AcceptLinkRequestTypeDef definition

class AcceptLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    logSettings: LinkLogSettingsTypeDef,  # (1)
    attributes: NotRequired[LinkAttributesUnionTypeDef],  # (2)
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
2. See [:material-code-braces: LinkAttributesUnionTypeDef](#linkattributesuniontypedef)

## CreateInboundExternalLinkRequestTypeDef

```python
# CreateInboundExternalLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateInboundExternalLinkRequestTypeDef


def get_value() -> CreateInboundExternalLinkRequestTypeDef:
    return {
        "clientToken": ...,
    }


# CreateInboundExternalLinkRequestTypeDef definition

class CreateInboundExternalLinkRequestTypeDef(TypedDict):
    clientToken: str,
    gatewayId: str,
    logSettings: LinkLogSettingsTypeDef,  # (1)
    attributes: NotRequired[LinkAttributesUnionTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
2. See [:material-code-braces: LinkAttributesUnionTypeDef](#linkattributesuniontypedef)

## CreateLinkRequestTypeDef

```python
# CreateLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateLinkRequestTypeDef


def get_value() -> CreateLinkRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# CreateLinkRequestTypeDef definition

class CreateLinkRequestTypeDef(TypedDict):
    gatewayId: str,
    peerGatewayId: str,
    logSettings: LinkLogSettingsTypeDef,  # (1)
    attributes: NotRequired[LinkAttributesUnionTypeDef],  # (2)
    httpResponderAllowed: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
2. See [:material-code-braces: LinkAttributesUnionTypeDef](#linkattributesuniontypedef)

## CreateOutboundExternalLinkRequestTypeDef

```python
# CreateOutboundExternalLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateOutboundExternalLinkRequestTypeDef


def get_value() -> CreateOutboundExternalLinkRequestTypeDef:
    return {
        "clientToken": ...,
    }


# CreateOutboundExternalLinkRequestTypeDef definition

class CreateOutboundExternalLinkRequestTypeDef(TypedDict):
    clientToken: str,
    gatewayId: str,
    publicEndpoint: str,
    logSettings: LinkLogSettingsTypeDef,  # (1)
    attributes: NotRequired[LinkAttributesUnionTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
2. See [:material-code-braces: LinkAttributesUnionTypeDef](#linkattributesuniontypedef)

## ModuleConfigurationOutputTypeDef

```python
# ModuleConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ModuleConfigurationOutputTypeDef


def get_value() -> ModuleConfigurationOutputTypeDef:
    return {
        "version": ...,
    }


# ModuleConfigurationOutputTypeDef definition

class ModuleConfigurationOutputTypeDef(TypedDict):
    name: str,
    version: NotRequired[str],
    dependsOn: NotRequired[list[str]],
    moduleParameters: NotRequired[ModuleParametersOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ModuleParametersOutputTypeDef](./type_defs.md#moduleparametersoutputtypedef)

## OpenRtbAttributeModuleParametersTypeDef

```python
# OpenRtbAttributeModuleParametersTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import OpenRtbAttributeModuleParametersTypeDef


def get_value() -> OpenRtbAttributeModuleParametersTypeDef:
    return {
        "filterType": ...,
    }


# OpenRtbAttributeModuleParametersTypeDef definition

class OpenRtbAttributeModuleParametersTypeDef(TypedDict):
    filterType: FilterTypeType,  # (1)
    filterConfiguration: Sequence[FilterUnionTypeDef],  # (2)
    action: ActionTypeDef,  # (3)
    holdbackPercentage: float,
```

1. See [:material-code-brackets: FilterTypeType](./literals.md#filtertypetype)
2. See `Sequence[FilterUnionTypeDef]`
3. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef)

## AcceptLinkResponseTypeDef

```python
# AcceptLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import AcceptLinkResponseTypeDef


def get_value() -> AcceptLinkResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# AcceptLinkResponseTypeDef definition

class AcceptLinkResponseTypeDef(TypedDict):
    gatewayId: str,
    peerGatewayId: str,
    status: LinkStatusType,  # (1)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    direction: LinkDirectionType,  # (2)
    flowModules: list[ModuleConfigurationOutputTypeDef],  # (3)
    pendingFlowModules: list[ModuleConfigurationOutputTypeDef],  # (3)
    attributes: LinkAttributesOutputTypeDef,  # (5)
    linkId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-brackets: LinkDirectionType](./literals.md#linkdirectiontype)
3. See `list[ModuleConfigurationOutputTypeDef]`
4. See `list[ModuleConfigurationOutputTypeDef]`
5. See [:material-code-braces: LinkAttributesOutputTypeDef](./type_defs.md#linkattributesoutputtypedef)
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateLinkResponseTypeDef

```python
# CreateLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import CreateLinkResponseTypeDef


def get_value() -> CreateLinkResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# CreateLinkResponseTypeDef definition

class CreateLinkResponseTypeDef(TypedDict):
    gatewayId: str,
    peerGatewayId: str,
    status: LinkStatusType,  # (1)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    direction: LinkDirectionType,  # (2)
    flowModules: list[ModuleConfigurationOutputTypeDef],  # (3)
    pendingFlowModules: list[ModuleConfigurationOutputTypeDef],  # (3)
    attributes: LinkAttributesOutputTypeDef,  # (5)
    linkId: str,
    customerProvidedId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-brackets: LinkDirectionType](./literals.md#linkdirectiontype)
3. See `list[ModuleConfigurationOutputTypeDef]`
4. See `list[ModuleConfigurationOutputTypeDef]`
5. See [:material-code-braces: LinkAttributesOutputTypeDef](./type_defs.md#linkattributesoutputtypedef)
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetInboundExternalLinkResponseTypeDef

```python
# GetInboundExternalLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetInboundExternalLinkResponseTypeDef


def get_value() -> GetInboundExternalLinkResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# GetInboundExternalLinkResponseTypeDef definition

class GetInboundExternalLinkResponseTypeDef(TypedDict):
    gatewayId: str,
    linkId: str,
    status: LinkStatusType,  # (1)
    domainName: str,
    flowModules: list[ModuleConfigurationOutputTypeDef],  # (2)
    pendingFlowModules: list[ModuleConfigurationOutputTypeDef],  # (2)
    attributes: LinkAttributesOutputTypeDef,  # (4)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    tags: dict[str, str],
    logSettings: LinkLogSettingsTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See `list[ModuleConfigurationOutputTypeDef]`
3. See `list[ModuleConfigurationOutputTypeDef]`
4. See [:material-code-braces: LinkAttributesOutputTypeDef](./type_defs.md#linkattributesoutputtypedef)
5. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetLinkResponseTypeDef

```python
# GetLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import GetLinkResponseTypeDef


def get_value() -> GetLinkResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# GetLinkResponseTypeDef definition

class GetLinkResponseTypeDef(TypedDict):
    gatewayId: str,
    peerGatewayId: str,
    status: LinkStatusType,  # (1)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    direction: LinkDirectionType,  # (2)
    flowModules: list[ModuleConfigurationOutputTypeDef],  # (3)
    pendingFlowModules: list[ModuleConfigurationOutputTypeDef],  # (3)
    attributes: LinkAttributesOutputTypeDef,  # (5)
    linkId: str,
    tags: dict[str, str],
    logSettings: LinkLogSettingsTypeDef,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-brackets: LinkDirectionType](./literals.md#linkdirectiontype)
3. See `list[ModuleConfigurationOutputTypeDef]`
4. See `list[ModuleConfigurationOutputTypeDef]`
5. See [:material-code-braces: LinkAttributesOutputTypeDef](./type_defs.md#linkattributesoutputtypedef)
6. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListLinksResponseStructureTypeDef

```python
# ListLinksResponseStructureTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListLinksResponseStructureTypeDef


def get_value() -> ListLinksResponseStructureTypeDef:
    return {
        "gatewayId": ...,
    }


# ListLinksResponseStructureTypeDef definition

class ListLinksResponseStructureTypeDef(TypedDict):
    gatewayId: str,
    peerGatewayId: str,
    status: LinkStatusType,  # (1)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    linkId: str,
    direction: NotRequired[LinkDirectionType],  # (2)
    flowModules: NotRequired[list[ModuleConfigurationOutputTypeDef]],  # (3)
    pendingFlowModules: NotRequired[list[ModuleConfigurationOutputTypeDef]],  # (3)
    attributes: NotRequired[LinkAttributesOutputTypeDef],  # (5)
    tags: NotRequired[dict[str, str]],
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-brackets: LinkDirectionType](./literals.md#linkdirectiontype)
3. See `list[ModuleConfigurationOutputTypeDef]`
4. See `list[ModuleConfigurationOutputTypeDef]`
5. See [:material-code-braces: LinkAttributesOutputTypeDef](./type_defs.md#linkattributesoutputtypedef)

## RejectLinkResponseTypeDef

```python
# RejectLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import RejectLinkResponseTypeDef


def get_value() -> RejectLinkResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# RejectLinkResponseTypeDef definition

class RejectLinkResponseTypeDef(TypedDict):
    gatewayId: str,
    peerGatewayId: str,
    status: LinkStatusType,  # (1)
    createdAt: datetime.datetime,
    updatedAt: datetime.datetime,
    direction: LinkDirectionType,  # (2)
    flowModules: list[ModuleConfigurationOutputTypeDef],  # (3)
    pendingFlowModules: list[ModuleConfigurationOutputTypeDef],  # (3)
    attributes: LinkAttributesOutputTypeDef,  # (5)
    linkId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: LinkStatusType](./literals.md#linkstatustype)
2. See [:material-code-brackets: LinkDirectionType](./literals.md#linkdirectiontype)
3. See `list[ModuleConfigurationOutputTypeDef]`
4. See `list[ModuleConfigurationOutputTypeDef]`
5. See [:material-code-braces: LinkAttributesOutputTypeDef](./type_defs.md#linkattributesoutputtypedef)
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListLinksResponseTypeDef

```python
# ListLinksResponseTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ListLinksResponseTypeDef


def get_value() -> ListLinksResponseTypeDef:
    return {
        "links": ...,
    }


# ListLinksResponseTypeDef definition

class ListLinksResponseTypeDef(TypedDict):
    links: list[ListLinksResponseStructureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ListLinksResponseStructureTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ModuleParametersTypeDef

```python
# ModuleParametersTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ModuleParametersTypeDef


def get_value() -> ModuleParametersTypeDef:
    return {
        "noBid": ...,
    }


# ModuleParametersTypeDef definition

class ModuleParametersTypeDef(TypedDict):
    noBid: NotRequired[NoBidModuleParametersTypeDef],  # (1)
    openRtbAttribute: NotRequired[OpenRtbAttributeModuleParametersUnionTypeDef],  # (2)
    rateLimiter: NotRequired[RateLimiterModuleParametersTypeDef],  # (3)
```

1. See [:material-code-braces: NoBidModuleParametersTypeDef](./type_defs.md#nobidmoduleparameterstypedef)
2. See [:material-code-braces: OpenRtbAttributeModuleParametersUnionTypeDef](#openrtbattributemoduleparametersuniontypedef)
3. See [:material-code-braces: RateLimiterModuleParametersTypeDef](./type_defs.md#ratelimitermoduleparameterstypedef)

## ModuleConfigurationTypeDef

```python
# ModuleConfigurationTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import ModuleConfigurationTypeDef


def get_value() -> ModuleConfigurationTypeDef:
    return {
        "version": ...,
    }


# ModuleConfigurationTypeDef definition

class ModuleConfigurationTypeDef(TypedDict):
    name: str,
    version: NotRequired[str],
    dependsOn: NotRequired[Sequence[str]],
    moduleParameters: NotRequired[ModuleParametersUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ModuleParametersUnionTypeDef](#moduleparametersuniontypedef)

## UpdateLinkModuleFlowRequestTypeDef

```python
# UpdateLinkModuleFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_rtbfabric.type_defs import UpdateLinkModuleFlowRequestTypeDef


def get_value() -> UpdateLinkModuleFlowRequestTypeDef:
    return {
        "clientToken": ...,
    }


# UpdateLinkModuleFlowRequestTypeDef definition

class UpdateLinkModuleFlowRequestTypeDef(TypedDict):
    clientToken: str,
    gatewayId: str,
    linkId: str,
    modules: Sequence[ModuleConfigurationUnionTypeDef],  # (1)
```

1. See `Sequence[ModuleConfigurationUnionTypeDef]`

