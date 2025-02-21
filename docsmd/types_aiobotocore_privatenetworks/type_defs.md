# Type definitions

> [Index](../README.md) > [Private5G](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Private5G](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#private5g)
    type annotations stubs module [types-aiobotocore-privatenetworks](https://pypi.org/project/types-aiobotocore-privatenetworks/).

## SitePlanUnionTypeDef

```python
# SitePlanUnionTypeDef Union usage example

from types_aiobotocore_privatenetworks.type_defs import SitePlanUnionTypeDef


def get_value() -> SitePlanUnionTypeDef:
    return ...


# SitePlanUnionTypeDef definition

SitePlanUnionTypeDef = Union[
    SitePlanTypeDef,  # (1)
    SitePlanOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SitePlanTypeDef](./type_defs.md#siteplantypedef) 
2. See [:material-code-braces: SitePlanOutputTypeDef](./type_defs.md#siteplanoutputtypedef) 



## AcknowledgeOrderReceiptRequestTypeDef

```python
# AcknowledgeOrderReceiptRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestTypeDef


def get_value() -> AcknowledgeOrderReceiptRequestTypeDef:
    return {
        "orderArn": ...,
    }


# AcknowledgeOrderReceiptRequestTypeDef definition

class AcknowledgeOrderReceiptRequestTypeDef(TypedDict):
    orderArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ResponseMetadataTypeDef


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

## ActivateDeviceIdentifierRequestTypeDef

```python
# ActivateDeviceIdentifierRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ActivateDeviceIdentifierRequestTypeDef


def get_value() -> ActivateDeviceIdentifierRequestTypeDef:
    return {
        "deviceIdentifierArn": ...,
    }


# ActivateDeviceIdentifierRequestTypeDef definition

class ActivateDeviceIdentifierRequestTypeDef(TypedDict):
    deviceIdentifierArn: str,
    clientToken: NotRequired[str],
```

## DeviceIdentifierTypeDef

```python
# DeviceIdentifierTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import DeviceIdentifierTypeDef


def get_value() -> DeviceIdentifierTypeDef:
    return {
        "createdAt": ...,
    }


# DeviceIdentifierTypeDef definition

class DeviceIdentifierTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    deviceIdentifierArn: NotRequired[str],
    iccid: NotRequired[str],
    imsi: NotRequired[str],
    networkArn: NotRequired[str],
    orderArn: NotRequired[str],
    status: NotRequired[DeviceIdentifierStatusType],  # (1)
    trafficGroupArn: NotRequired[str],
    vendor: NotRequired[str],
```

1. See [:material-code-brackets: DeviceIdentifierStatusType](./literals.md#deviceidentifierstatustype) 
## AddressTypeDef

```python
# AddressTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import AddressTypeDef


def get_value() -> AddressTypeDef:
    return {
        "city": ...,
    }


# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    city: str,
    country: str,
    name: str,
    postalCode: str,
    stateOrProvince: str,
    street1: str,
    company: NotRequired[str],
    emailAddress: NotRequired[str],
    phoneNumber: NotRequired[str],
    street2: NotRequired[str],
    street3: NotRequired[str],
```

## CommitmentConfigurationTypeDef

```python
# CommitmentConfigurationTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import CommitmentConfigurationTypeDef


def get_value() -> CommitmentConfigurationTypeDef:
    return {
        "automaticRenewal": ...,
    }


# CommitmentConfigurationTypeDef definition

class CommitmentConfigurationTypeDef(TypedDict):
    automaticRenewal: bool,
    commitmentLength: CommitmentLengthType,  # (1)
```

1. See [:material-code-brackets: CommitmentLengthType](./literals.md#commitmentlengthtype) 
## PositionTypeDef

```python
# PositionTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import PositionTypeDef


def get_value() -> PositionTypeDef:
    return {
        "elevation": ...,
    }


# PositionTypeDef definition

class PositionTypeDef(TypedDict):
    elevation: NotRequired[float],
    elevationReference: NotRequired[ElevationReferenceType],  # (1)
    elevationUnit: NotRequired[ElevationUnitType],  # (2)
    latitude: NotRequired[float],
    longitude: NotRequired[float],
```

1. See [:material-code-brackets: ElevationReferenceType](./literals.md#elevationreferencetype) 
2. See [:material-code-brackets: ElevationUnitType](./literals.md#elevationunittype) 
## CreateNetworkRequestTypeDef

```python
# CreateNetworkRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import CreateNetworkRequestTypeDef


def get_value() -> CreateNetworkRequestTypeDef:
    return {
        "networkName": ...,
    }


# CreateNetworkRequestTypeDef definition

class CreateNetworkRequestTypeDef(TypedDict):
    networkName: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## NetworkTypeDef

```python
# NetworkTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import NetworkTypeDef


def get_value() -> NetworkTypeDef:
    return {
        "createdAt": ...,
    }


# NetworkTypeDef definition

class NetworkTypeDef(TypedDict):
    networkArn: str,
    networkName: str,
    status: NetworkStatusType,  # (1)
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: NetworkStatusType](./literals.md#networkstatustype) 
## DeactivateDeviceIdentifierRequestTypeDef

```python
# DeactivateDeviceIdentifierRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import DeactivateDeviceIdentifierRequestTypeDef


def get_value() -> DeactivateDeviceIdentifierRequestTypeDef:
    return {
        "deviceIdentifierArn": ...,
    }


# DeactivateDeviceIdentifierRequestTypeDef definition

class DeactivateDeviceIdentifierRequestTypeDef(TypedDict):
    deviceIdentifierArn: str,
    clientToken: NotRequired[str],
```

## DeleteNetworkRequestTypeDef

```python
# DeleteNetworkRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import DeleteNetworkRequestTypeDef


def get_value() -> DeleteNetworkRequestTypeDef:
    return {
        "networkArn": ...,
    }


# DeleteNetworkRequestTypeDef definition

class DeleteNetworkRequestTypeDef(TypedDict):
    networkArn: str,
    clientToken: NotRequired[str],
```

## DeleteNetworkSiteRequestTypeDef

```python
# DeleteNetworkSiteRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import DeleteNetworkSiteRequestTypeDef


def get_value() -> DeleteNetworkSiteRequestTypeDef:
    return {
        "networkSiteArn": ...,
    }


# DeleteNetworkSiteRequestTypeDef definition

class DeleteNetworkSiteRequestTypeDef(TypedDict):
    networkSiteArn: str,
    clientToken: NotRequired[str],
```

## GetDeviceIdentifierRequestTypeDef

```python
# GetDeviceIdentifierRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetDeviceIdentifierRequestTypeDef


def get_value() -> GetDeviceIdentifierRequestTypeDef:
    return {
        "deviceIdentifierArn": ...,
    }


# GetDeviceIdentifierRequestTypeDef definition

class GetDeviceIdentifierRequestTypeDef(TypedDict):
    deviceIdentifierArn: str,
```

## GetNetworkRequestTypeDef

```python
# GetNetworkRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetNetworkRequestTypeDef


def get_value() -> GetNetworkRequestTypeDef:
    return {
        "networkArn": ...,
    }


# GetNetworkRequestTypeDef definition

class GetNetworkRequestTypeDef(TypedDict):
    networkArn: str,
```

## GetNetworkResourceRequestTypeDef

```python
# GetNetworkResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetNetworkResourceRequestTypeDef


def get_value() -> GetNetworkResourceRequestTypeDef:
    return {
        "networkResourceArn": ...,
    }


# GetNetworkResourceRequestTypeDef definition

class GetNetworkResourceRequestTypeDef(TypedDict):
    networkResourceArn: str,
```

## GetNetworkSiteRequestTypeDef

```python
# GetNetworkSiteRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetNetworkSiteRequestTypeDef


def get_value() -> GetNetworkSiteRequestTypeDef:
    return {
        "networkSiteArn": ...,
    }


# GetNetworkSiteRequestTypeDef definition

class GetNetworkSiteRequestTypeDef(TypedDict):
    networkSiteArn: str,
```

## GetOrderRequestTypeDef

```python
# GetOrderRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetOrderRequestTypeDef


def get_value() -> GetOrderRequestTypeDef:
    return {
        "orderArn": ...,
    }


# GetOrderRequestTypeDef definition

class GetOrderRequestTypeDef(TypedDict):
    orderArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import PaginatorConfigTypeDef


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

## ListDeviceIdentifiersRequestTypeDef

```python
# ListDeviceIdentifiersRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListDeviceIdentifiersRequestTypeDef


def get_value() -> ListDeviceIdentifiersRequestTypeDef:
    return {
        "networkArn": ...,
    }


# ListDeviceIdentifiersRequestTypeDef definition

class ListDeviceIdentifiersRequestTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[DeviceIdentifierFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: DeviceIdentifierFilterKeysType](./literals.md#deviceidentifierfilterkeystype) 
## ListNetworkResourcesRequestTypeDef

```python
# ListNetworkResourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListNetworkResourcesRequestTypeDef


def get_value() -> ListNetworkResourcesRequestTypeDef:
    return {
        "networkArn": ...,
    }


# ListNetworkResourcesRequestTypeDef definition

class ListNetworkResourcesRequestTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[NetworkResourceFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: NetworkResourceFilterKeysType](./literals.md#networkresourcefilterkeystype) 
## ListNetworkSitesRequestTypeDef

```python
# ListNetworkSitesRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListNetworkSitesRequestTypeDef


def get_value() -> ListNetworkSitesRequestTypeDef:
    return {
        "networkArn": ...,
    }


# ListNetworkSitesRequestTypeDef definition

class ListNetworkSitesRequestTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[NetworkSiteFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: NetworkSiteFilterKeysType](./literals.md#networksitefilterkeystype) 
## ListNetworksRequestTypeDef

```python
# ListNetworksRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListNetworksRequestTypeDef


def get_value() -> ListNetworksRequestTypeDef:
    return {
        "filters": ...,
    }


# ListNetworksRequestTypeDef definition

class ListNetworksRequestTypeDef(TypedDict):
    filters: NotRequired[Mapping[NetworkFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: NetworkFilterKeysType](./literals.md#networkfilterkeystype) 
## ListOrdersRequestTypeDef

```python
# ListOrdersRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListOrdersRequestTypeDef


def get_value() -> ListOrdersRequestTypeDef:
    return {
        "networkArn": ...,
    }


# ListOrdersRequestTypeDef definition

class ListOrdersRequestTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[OrderFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: OrderFilterKeysType](./literals.md#orderfilterkeystype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## NameValuePairTypeDef

```python
# NameValuePairTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import NameValuePairTypeDef


def get_value() -> NameValuePairTypeDef:
    return {
        "name": ...,
    }


# NameValuePairTypeDef definition

class NameValuePairTypeDef(TypedDict):
    name: str,
    value: NotRequired[str],
```

## TrackingInformationTypeDef

```python
# TrackingInformationTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import TrackingInformationTypeDef


def get_value() -> TrackingInformationTypeDef:
    return {
        "trackingNumber": ...,
    }


# TrackingInformationTypeDef definition

class TrackingInformationTypeDef(TypedDict):
    trackingNumber: NotRequired[str],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import TagResourceRequestTypeDef


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

from types_aiobotocore_privatenetworks.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateNetworkSiteRequestTypeDef

```python
# UpdateNetworkSiteRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import UpdateNetworkSiteRequestTypeDef


def get_value() -> UpdateNetworkSiteRequestTypeDef:
    return {
        "networkSiteArn": ...,
    }


# UpdateNetworkSiteRequestTypeDef definition

class UpdateNetworkSiteRequestTypeDef(TypedDict):
    networkSiteArn: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListTagsForResourceResponseTypeDef


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
## PingResponseTypeDef

```python
# PingResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import PingResponseTypeDef


def get_value() -> PingResponseTypeDef:
    return {
        "status": ...,
    }


# PingResponseTypeDef definition

class PingResponseTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActivateDeviceIdentifierResponseTypeDef

```python
# ActivateDeviceIdentifierResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ActivateDeviceIdentifierResponseTypeDef


def get_value() -> ActivateDeviceIdentifierResponseTypeDef:
    return {
        "deviceIdentifier": ...,
    }


# ActivateDeviceIdentifierResponseTypeDef definition

class ActivateDeviceIdentifierResponseTypeDef(TypedDict):
    deviceIdentifier: DeviceIdentifierTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceIdentifierTypeDef](./type_defs.md#deviceidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeactivateDeviceIdentifierResponseTypeDef

```python
# DeactivateDeviceIdentifierResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import DeactivateDeviceIdentifierResponseTypeDef


def get_value() -> DeactivateDeviceIdentifierResponseTypeDef:
    return {
        "deviceIdentifier": ...,
    }


# DeactivateDeviceIdentifierResponseTypeDef definition

class DeactivateDeviceIdentifierResponseTypeDef(TypedDict):
    deviceIdentifier: DeviceIdentifierTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceIdentifierTypeDef](./type_defs.md#deviceidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeviceIdentifierResponseTypeDef

```python
# GetDeviceIdentifierResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetDeviceIdentifierResponseTypeDef


def get_value() -> GetDeviceIdentifierResponseTypeDef:
    return {
        "deviceIdentifier": ...,
    }


# GetDeviceIdentifierResponseTypeDef definition

class GetDeviceIdentifierResponseTypeDef(TypedDict):
    deviceIdentifier: DeviceIdentifierTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceIdentifierTypeDef](./type_defs.md#deviceidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeviceIdentifiersResponseTypeDef

```python
# ListDeviceIdentifiersResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListDeviceIdentifiersResponseTypeDef


def get_value() -> ListDeviceIdentifiersResponseTypeDef:
    return {
        "deviceIdentifiers": ...,
    }


# ListDeviceIdentifiersResponseTypeDef definition

class ListDeviceIdentifiersResponseTypeDef(TypedDict):
    deviceIdentifiers: List[DeviceIdentifierTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceIdentifierTypeDef](./type_defs.md#deviceidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReturnInformationTypeDef

```python
# ReturnInformationTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ReturnInformationTypeDef


def get_value() -> ReturnInformationTypeDef:
    return {
        "replacementOrderArn": ...,
    }


# ReturnInformationTypeDef definition

class ReturnInformationTypeDef(TypedDict):
    replacementOrderArn: NotRequired[str],
    returnReason: NotRequired[str],
    shippingAddress: NotRequired[AddressTypeDef],  # (1)
    shippingLabel: NotRequired[str],
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
## ActivateNetworkSiteRequestTypeDef

```python
# ActivateNetworkSiteRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ActivateNetworkSiteRequestTypeDef


def get_value() -> ActivateNetworkSiteRequestTypeDef:
    return {
        "networkSiteArn": ...,
    }


# ActivateNetworkSiteRequestTypeDef definition

class ActivateNetworkSiteRequestTypeDef(TypedDict):
    networkSiteArn: str,
    shippingAddress: AddressTypeDef,  # (1)
    clientToken: NotRequired[str],
    commitmentConfiguration: NotRequired[CommitmentConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef) 
## CommitmentInformationTypeDef

```python
# CommitmentInformationTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import CommitmentInformationTypeDef


def get_value() -> CommitmentInformationTypeDef:
    return {
        "commitmentConfiguration": ...,
    }


# CommitmentInformationTypeDef definition

class CommitmentInformationTypeDef(TypedDict):
    commitmentConfiguration: CommitmentConfigurationTypeDef,  # (1)
    expiresOn: NotRequired[datetime],
    startAt: NotRequired[datetime],
```

1. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef) 
## OrderedResourceDefinitionTypeDef

```python
# OrderedResourceDefinitionTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import OrderedResourceDefinitionTypeDef


def get_value() -> OrderedResourceDefinitionTypeDef:
    return {
        "commitmentConfiguration": ...,
    }


# OrderedResourceDefinitionTypeDef definition

class OrderedResourceDefinitionTypeDef(TypedDict):
    count: int,
    type: NetworkResourceDefinitionTypeType,  # (2)
    commitmentConfiguration: NotRequired[CommitmentConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef) 
2. See [:material-code-brackets: NetworkResourceDefinitionTypeType](./literals.md#networkresourcedefinitiontypetype) 
## StartNetworkResourceUpdateRequestTypeDef

```python
# StartNetworkResourceUpdateRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import StartNetworkResourceUpdateRequestTypeDef


def get_value() -> StartNetworkResourceUpdateRequestTypeDef:
    return {
        "networkResourceArn": ...,
    }


# StartNetworkResourceUpdateRequestTypeDef definition

class StartNetworkResourceUpdateRequestTypeDef(TypedDict):
    networkResourceArn: str,
    updateType: UpdateTypeType,  # (1)
    commitmentConfiguration: NotRequired[CommitmentConfigurationTypeDef],  # (2)
    returnReason: NotRequired[str],
    shippingAddress: NotRequired[AddressTypeDef],  # (3)
```

1. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype) 
2. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef) 
3. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
## ConfigureAccessPointRequestTypeDef

```python
# ConfigureAccessPointRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ConfigureAccessPointRequestTypeDef


def get_value() -> ConfigureAccessPointRequestTypeDef:
    return {
        "accessPointArn": ...,
    }


# ConfigureAccessPointRequestTypeDef definition

class ConfigureAccessPointRequestTypeDef(TypedDict):
    accessPointArn: str,
    cpiSecretKey: NotRequired[str],
    cpiUserId: NotRequired[str],
    cpiUserPassword: NotRequired[str],
    cpiUsername: NotRequired[str],
    position: NotRequired[PositionTypeDef],  # (1)
```

1. See [:material-code-braces: PositionTypeDef](./type_defs.md#positiontypedef) 
## CreateNetworkResponseTypeDef

```python
# CreateNetworkResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import CreateNetworkResponseTypeDef


def get_value() -> CreateNetworkResponseTypeDef:
    return {
        "network": ...,
    }


# CreateNetworkResponseTypeDef definition

class CreateNetworkResponseTypeDef(TypedDict):
    network: NetworkTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkTypeDef](./type_defs.md#networktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteNetworkResponseTypeDef

```python
# DeleteNetworkResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import DeleteNetworkResponseTypeDef


def get_value() -> DeleteNetworkResponseTypeDef:
    return {
        "network": ...,
    }


# DeleteNetworkResponseTypeDef definition

class DeleteNetworkResponseTypeDef(TypedDict):
    network: NetworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkTypeDef](./type_defs.md#networktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkResponseTypeDef

```python
# GetNetworkResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetNetworkResponseTypeDef


def get_value() -> GetNetworkResponseTypeDef:
    return {
        "network": ...,
    }


# GetNetworkResponseTypeDef definition

class GetNetworkResponseTypeDef(TypedDict):
    network: NetworkTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkTypeDef](./type_defs.md#networktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNetworksResponseTypeDef

```python
# ListNetworksResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListNetworksResponseTypeDef


def get_value() -> ListNetworksResponseTypeDef:
    return {
        "networks": ...,
    }


# ListNetworksResponseTypeDef definition

class ListNetworksResponseTypeDef(TypedDict):
    networks: List[NetworkTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NetworkTypeDef](./type_defs.md#networktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeviceIdentifiersRequestPaginateTypeDef

```python
# ListDeviceIdentifiersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListDeviceIdentifiersRequestPaginateTypeDef


def get_value() -> ListDeviceIdentifiersRequestPaginateTypeDef:
    return {
        "networkArn": ...,
    }


# ListDeviceIdentifiersRequestPaginateTypeDef definition

class ListDeviceIdentifiersRequestPaginateTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[DeviceIdentifierFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DeviceIdentifierFilterKeysType](./literals.md#deviceidentifierfilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNetworkResourcesRequestPaginateTypeDef

```python
# ListNetworkResourcesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListNetworkResourcesRequestPaginateTypeDef


def get_value() -> ListNetworkResourcesRequestPaginateTypeDef:
    return {
        "networkArn": ...,
    }


# ListNetworkResourcesRequestPaginateTypeDef definition

class ListNetworkResourcesRequestPaginateTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[NetworkResourceFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NetworkResourceFilterKeysType](./literals.md#networkresourcefilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNetworkSitesRequestPaginateTypeDef

```python
# ListNetworkSitesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListNetworkSitesRequestPaginateTypeDef


def get_value() -> ListNetworkSitesRequestPaginateTypeDef:
    return {
        "networkArn": ...,
    }


# ListNetworkSitesRequestPaginateTypeDef definition

class ListNetworkSitesRequestPaginateTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[NetworkSiteFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NetworkSiteFilterKeysType](./literals.md#networksitefilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNetworksRequestPaginateTypeDef

```python
# ListNetworksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListNetworksRequestPaginateTypeDef


def get_value() -> ListNetworksRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# ListNetworksRequestPaginateTypeDef definition

class ListNetworksRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[Mapping[NetworkFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NetworkFilterKeysType](./literals.md#networkfilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrdersRequestPaginateTypeDef

```python
# ListOrdersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListOrdersRequestPaginateTypeDef


def get_value() -> ListOrdersRequestPaginateTypeDef:
    return {
        "networkArn": ...,
    }


# ListOrdersRequestPaginateTypeDef definition

class ListOrdersRequestPaginateTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[OrderFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OrderFilterKeysType](./literals.md#orderfilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## NetworkResourceDefinitionOutputTypeDef

```python
# NetworkResourceDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import NetworkResourceDefinitionOutputTypeDef


def get_value() -> NetworkResourceDefinitionOutputTypeDef:
    return {
        "count": ...,
    }


# NetworkResourceDefinitionOutputTypeDef definition

class NetworkResourceDefinitionOutputTypeDef(TypedDict):
    count: int,
    type: NetworkResourceDefinitionTypeType,  # (2)
    options: NotRequired[List[NameValuePairTypeDef]],  # (1)
```

1. See [:material-code-braces: NameValuePairTypeDef](./type_defs.md#namevaluepairtypedef) 
2. See [:material-code-brackets: NetworkResourceDefinitionTypeType](./literals.md#networkresourcedefinitiontypetype) 
## NetworkResourceDefinitionTypeDef

```python
# NetworkResourceDefinitionTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import NetworkResourceDefinitionTypeDef


def get_value() -> NetworkResourceDefinitionTypeDef:
    return {
        "count": ...,
    }


# NetworkResourceDefinitionTypeDef definition

class NetworkResourceDefinitionTypeDef(TypedDict):
    count: int,
    type: NetworkResourceDefinitionTypeType,  # (2)
    options: NotRequired[Sequence[NameValuePairTypeDef]],  # (1)
```

1. See [:material-code-braces: NameValuePairTypeDef](./type_defs.md#namevaluepairtypedef) 
2. See [:material-code-brackets: NetworkResourceDefinitionTypeType](./literals.md#networkresourcedefinitiontypetype) 
## NetworkResourceTypeDef

```python
# NetworkResourceTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import NetworkResourceTypeDef


def get_value() -> NetworkResourceTypeDef:
    return {
        "attributes": ...,
    }


# NetworkResourceTypeDef definition

class NetworkResourceTypeDef(TypedDict):
    attributes: NotRequired[List[NameValuePairTypeDef]],  # (1)
    commitmentInformation: NotRequired[CommitmentInformationTypeDef],  # (2)
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    health: NotRequired[HealthStatusType],  # (3)
    model: NotRequired[str],
    networkArn: NotRequired[str],
    networkResourceArn: NotRequired[str],
    networkSiteArn: NotRequired[str],
    orderArn: NotRequired[str],
    position: NotRequired[PositionTypeDef],  # (4)
    returnInformation: NotRequired[ReturnInformationTypeDef],  # (5)
    serialNumber: NotRequired[str],
    status: NotRequired[NetworkResourceStatusType],  # (6)
    statusReason: NotRequired[str],
    type: NotRequired[NetworkResourceTypeType],  # (7)
    vendor: NotRequired[str],
```

1. See [:material-code-braces: NameValuePairTypeDef](./type_defs.md#namevaluepairtypedef) 
2. See [:material-code-braces: CommitmentInformationTypeDef](./type_defs.md#commitmentinformationtypedef) 
3. See [:material-code-brackets: HealthStatusType](./literals.md#healthstatustype) 
4. See [:material-code-braces: PositionTypeDef](./type_defs.md#positiontypedef) 
5. See [:material-code-braces: ReturnInformationTypeDef](./type_defs.md#returninformationtypedef) 
6. See [:material-code-brackets: NetworkResourceStatusType](./literals.md#networkresourcestatustype) 
7. See [:material-code-brackets: NetworkResourceTypeType](./literals.md#networkresourcetypetype) 
## OrderTypeDef

```python
# OrderTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import OrderTypeDef


def get_value() -> OrderTypeDef:
    return {
        "acknowledgmentStatus": ...,
    }


# OrderTypeDef definition

class OrderTypeDef(TypedDict):
    acknowledgmentStatus: NotRequired[AcknowledgmentStatusType],  # (1)
    createdAt: NotRequired[datetime],
    networkArn: NotRequired[str],
    networkSiteArn: NotRequired[str],
    orderArn: NotRequired[str],
    orderedResources: NotRequired[List[OrderedResourceDefinitionTypeDef]],  # (2)
    shippingAddress: NotRequired[AddressTypeDef],  # (3)
    trackingInformation: NotRequired[List[TrackingInformationTypeDef]],  # (4)
```

1. See [:material-code-brackets: AcknowledgmentStatusType](./literals.md#acknowledgmentstatustype) 
2. See [:material-code-braces: OrderedResourceDefinitionTypeDef](./type_defs.md#orderedresourcedefinitiontypedef) 
3. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
4. See [:material-code-braces: TrackingInformationTypeDef](./type_defs.md#trackinginformationtypedef) 
## SitePlanOutputTypeDef

```python
# SitePlanOutputTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import SitePlanOutputTypeDef


def get_value() -> SitePlanOutputTypeDef:
    return {
        "options": ...,
    }


# SitePlanOutputTypeDef definition

class SitePlanOutputTypeDef(TypedDict):
    options: NotRequired[List[NameValuePairTypeDef]],  # (1)
    resourceDefinitions: NotRequired[List[NetworkResourceDefinitionOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: NameValuePairTypeDef](./type_defs.md#namevaluepairtypedef) 
2. See [:material-code-braces: NetworkResourceDefinitionOutputTypeDef](./type_defs.md#networkresourcedefinitionoutputtypedef) 
## SitePlanTypeDef

```python
# SitePlanTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import SitePlanTypeDef


def get_value() -> SitePlanTypeDef:
    return {
        "options": ...,
    }


# SitePlanTypeDef definition

class SitePlanTypeDef(TypedDict):
    options: NotRequired[Sequence[NameValuePairTypeDef]],  # (1)
    resourceDefinitions: NotRequired[Sequence[NetworkResourceDefinitionTypeDef]],  # (2)
```

1. See [:material-code-braces: NameValuePairTypeDef](./type_defs.md#namevaluepairtypedef) 
2. See [:material-code-braces: NetworkResourceDefinitionTypeDef](./type_defs.md#networkresourcedefinitiontypedef) 
## ConfigureAccessPointResponseTypeDef

```python
# ConfigureAccessPointResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ConfigureAccessPointResponseTypeDef


def get_value() -> ConfigureAccessPointResponseTypeDef:
    return {
        "accessPoint": ...,
    }


# ConfigureAccessPointResponseTypeDef definition

class ConfigureAccessPointResponseTypeDef(TypedDict):
    accessPoint: NetworkResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkResourceTypeDef](./type_defs.md#networkresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkResourceResponseTypeDef

```python
# GetNetworkResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetNetworkResourceResponseTypeDef


def get_value() -> GetNetworkResourceResponseTypeDef:
    return {
        "networkResource": ...,
    }


# GetNetworkResourceResponseTypeDef definition

class GetNetworkResourceResponseTypeDef(TypedDict):
    networkResource: NetworkResourceTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkResourceTypeDef](./type_defs.md#networkresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNetworkResourcesResponseTypeDef

```python
# ListNetworkResourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListNetworkResourcesResponseTypeDef


def get_value() -> ListNetworkResourcesResponseTypeDef:
    return {
        "networkResources": ...,
    }


# ListNetworkResourcesResponseTypeDef definition

class ListNetworkResourcesResponseTypeDef(TypedDict):
    networkResources: List[NetworkResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NetworkResourceTypeDef](./type_defs.md#networkresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartNetworkResourceUpdateResponseTypeDef

```python
# StartNetworkResourceUpdateResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import StartNetworkResourceUpdateResponseTypeDef


def get_value() -> StartNetworkResourceUpdateResponseTypeDef:
    return {
        "networkResource": ...,
    }


# StartNetworkResourceUpdateResponseTypeDef definition

class StartNetworkResourceUpdateResponseTypeDef(TypedDict):
    networkResource: NetworkResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkResourceTypeDef](./type_defs.md#networkresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcknowledgeOrderReceiptResponseTypeDef

```python
# AcknowledgeOrderReceiptResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptResponseTypeDef


def get_value() -> AcknowledgeOrderReceiptResponseTypeDef:
    return {
        "order": ...,
    }


# AcknowledgeOrderReceiptResponseTypeDef definition

class AcknowledgeOrderReceiptResponseTypeDef(TypedDict):
    order: OrderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrderTypeDef](./type_defs.md#ordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOrderResponseTypeDef

```python
# GetOrderResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetOrderResponseTypeDef


def get_value() -> GetOrderResponseTypeDef:
    return {
        "order": ...,
    }


# GetOrderResponseTypeDef definition

class GetOrderResponseTypeDef(TypedDict):
    order: OrderTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrderTypeDef](./type_defs.md#ordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrdersResponseTypeDef

```python
# ListOrdersResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListOrdersResponseTypeDef


def get_value() -> ListOrdersResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListOrdersResponseTypeDef definition

class ListOrdersResponseTypeDef(TypedDict):
    orders: List[OrderTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OrderTypeDef](./type_defs.md#ordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkSiteTypeDef

```python
# NetworkSiteTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import NetworkSiteTypeDef


def get_value() -> NetworkSiteTypeDef:
    return {
        "availabilityZone": ...,
    }


# NetworkSiteTypeDef definition

class NetworkSiteTypeDef(TypedDict):
    networkArn: str,
    networkSiteArn: str,
    networkSiteName: str,
    status: NetworkSiteStatusType,  # (3)
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    createdAt: NotRequired[datetime],
    currentPlan: NotRequired[SitePlanOutputTypeDef],  # (1)
    description: NotRequired[str],
    pendingPlan: NotRequired[SitePlanOutputTypeDef],  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-braces: SitePlanOutputTypeDef](./type_defs.md#siteplanoutputtypedef) 
2. See [:material-code-braces: SitePlanOutputTypeDef](./type_defs.md#siteplanoutputtypedef) 
3. See [:material-code-brackets: NetworkSiteStatusType](./literals.md#networksitestatustype) 
## ActivateNetworkSiteResponseTypeDef

```python
# ActivateNetworkSiteResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ActivateNetworkSiteResponseTypeDef


def get_value() -> ActivateNetworkSiteResponseTypeDef:
    return {
        "networkSite": ...,
    }


# ActivateNetworkSiteResponseTypeDef definition

class ActivateNetworkSiteResponseTypeDef(TypedDict):
    networkSite: NetworkSiteTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSiteTypeDef](./type_defs.md#networksitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNetworkSiteResponseTypeDef

```python
# CreateNetworkSiteResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import CreateNetworkSiteResponseTypeDef


def get_value() -> CreateNetworkSiteResponseTypeDef:
    return {
        "networkSite": ...,
    }


# CreateNetworkSiteResponseTypeDef definition

class CreateNetworkSiteResponseTypeDef(TypedDict):
    networkSite: NetworkSiteTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSiteTypeDef](./type_defs.md#networksitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteNetworkSiteResponseTypeDef

```python
# DeleteNetworkSiteResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import DeleteNetworkSiteResponseTypeDef


def get_value() -> DeleteNetworkSiteResponseTypeDef:
    return {
        "networkSite": ...,
    }


# DeleteNetworkSiteResponseTypeDef definition

class DeleteNetworkSiteResponseTypeDef(TypedDict):
    networkSite: NetworkSiteTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSiteTypeDef](./type_defs.md#networksitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkSiteResponseTypeDef

```python
# GetNetworkSiteResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import GetNetworkSiteResponseTypeDef


def get_value() -> GetNetworkSiteResponseTypeDef:
    return {
        "networkSite": ...,
    }


# GetNetworkSiteResponseTypeDef definition

class GetNetworkSiteResponseTypeDef(TypedDict):
    networkSite: NetworkSiteTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSiteTypeDef](./type_defs.md#networksitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNetworkSitesResponseTypeDef

```python
# ListNetworkSitesResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import ListNetworkSitesResponseTypeDef


def get_value() -> ListNetworkSitesResponseTypeDef:
    return {
        "networkSites": ...,
    }


# ListNetworkSitesResponseTypeDef definition

class ListNetworkSitesResponseTypeDef(TypedDict):
    networkSites: List[NetworkSiteTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NetworkSiteTypeDef](./type_defs.md#networksitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNetworkSiteResponseTypeDef

```python
# UpdateNetworkSiteResponseTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import UpdateNetworkSiteResponseTypeDef


def get_value() -> UpdateNetworkSiteResponseTypeDef:
    return {
        "networkSite": ...,
    }


# UpdateNetworkSiteResponseTypeDef definition

class UpdateNetworkSiteResponseTypeDef(TypedDict):
    networkSite: NetworkSiteTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSiteTypeDef](./type_defs.md#networksitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNetworkSiteRequestTypeDef

```python
# CreateNetworkSiteRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import CreateNetworkSiteRequestTypeDef


def get_value() -> CreateNetworkSiteRequestTypeDef:
    return {
        "networkArn": ...,
    }


# CreateNetworkSiteRequestTypeDef definition

class CreateNetworkSiteRequestTypeDef(TypedDict):
    networkArn: str,
    networkSiteName: str,
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    clientToken: NotRequired[str],
    description: NotRequired[str],
    pendingPlan: NotRequired[SitePlanUnionTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SitePlanTypeDef](./type_defs.md#siteplantypedef) [:material-code-braces: SitePlanOutputTypeDef](./type_defs.md#siteplanoutputtypedef) 
## UpdateNetworkSitePlanRequestTypeDef

```python
# UpdateNetworkSitePlanRequestTypeDef TypedDict usage example

from types_aiobotocore_privatenetworks.type_defs import UpdateNetworkSitePlanRequestTypeDef


def get_value() -> UpdateNetworkSitePlanRequestTypeDef:
    return {
        "networkSiteArn": ...,
    }


# UpdateNetworkSitePlanRequestTypeDef definition

class UpdateNetworkSitePlanRequestTypeDef(TypedDict):
    networkSiteArn: str,
    pendingPlan: SitePlanUnionTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: SitePlanTypeDef](./type_defs.md#siteplantypedef) [:material-code-braces: SitePlanOutputTypeDef](./type_defs.md#siteplanoutputtypedef) 
