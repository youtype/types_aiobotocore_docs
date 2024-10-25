# Type definitions

> [Index](../README.md) > [Private5G](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Private5G](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
    type annotations stubs module [types-aiobotocore-privatenetworks](https://pypi.org/project/types-aiobotocore-privatenetworks/).

## NetworkResourceDefinitionUnionTypeDef

```python
# NetworkResourceDefinitionUnionTypeDef definition

NetworkResourceDefinitionUnionTypeDef = Union[
    NetworkResourceDefinitionTypeDef,  # (1)
    NetworkResourceDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NetworkResourceDefinitionTypeDef](./type_defs.md#networkresourcedefinitiontypedef) 
2. See [:material-code-braces: NetworkResourceDefinitionOutputTypeDef](./type_defs.md#networkresourcedefinitionoutputtypedef) 



## AcknowledgeOrderReceiptRequestRequestTypeDef

```python
# AcknowledgeOrderReceiptRequestRequestTypeDef definition

class AcknowledgeOrderReceiptRequestRequestTypeDef(TypedDict):
    orderArn: str,
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

## ActivateDeviceIdentifierRequestRequestTypeDef

```python
# ActivateDeviceIdentifierRequestRequestTypeDef definition

class ActivateDeviceIdentifierRequestRequestTypeDef(TypedDict):
    deviceIdentifierArn: str,
    clientToken: NotRequired[str],
```

## DeviceIdentifierTypeDef

```python
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
# CommitmentConfigurationTypeDef definition

class CommitmentConfigurationTypeDef(TypedDict):
    automaticRenewal: bool,
    commitmentLength: CommitmentLengthType,  # (1)
```

1. See [:material-code-brackets: CommitmentLengthType](./literals.md#commitmentlengthtype) 
## PositionTypeDef

```python
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
## CreateNetworkRequestRequestTypeDef

```python
# CreateNetworkRequestRequestTypeDef definition

class CreateNetworkRequestRequestTypeDef(TypedDict):
    networkName: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## NetworkTypeDef

```python
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
## DeactivateDeviceIdentifierRequestRequestTypeDef

```python
# DeactivateDeviceIdentifierRequestRequestTypeDef definition

class DeactivateDeviceIdentifierRequestRequestTypeDef(TypedDict):
    deviceIdentifierArn: str,
    clientToken: NotRequired[str],
```

## DeleteNetworkRequestRequestTypeDef

```python
# DeleteNetworkRequestRequestTypeDef definition

class DeleteNetworkRequestRequestTypeDef(TypedDict):
    networkArn: str,
    clientToken: NotRequired[str],
```

## DeleteNetworkSiteRequestRequestTypeDef

```python
# DeleteNetworkSiteRequestRequestTypeDef definition

class DeleteNetworkSiteRequestRequestTypeDef(TypedDict):
    networkSiteArn: str,
    clientToken: NotRequired[str],
```

## GetDeviceIdentifierRequestRequestTypeDef

```python
# GetDeviceIdentifierRequestRequestTypeDef definition

class GetDeviceIdentifierRequestRequestTypeDef(TypedDict):
    deviceIdentifierArn: str,
```

## GetNetworkRequestRequestTypeDef

```python
# GetNetworkRequestRequestTypeDef definition

class GetNetworkRequestRequestTypeDef(TypedDict):
    networkArn: str,
```

## GetNetworkResourceRequestRequestTypeDef

```python
# GetNetworkResourceRequestRequestTypeDef definition

class GetNetworkResourceRequestRequestTypeDef(TypedDict):
    networkResourceArn: str,
```

## GetNetworkSiteRequestRequestTypeDef

```python
# GetNetworkSiteRequestRequestTypeDef definition

class GetNetworkSiteRequestRequestTypeDef(TypedDict):
    networkSiteArn: str,
```

## GetOrderRequestRequestTypeDef

```python
# GetOrderRequestRequestTypeDef definition

class GetOrderRequestRequestTypeDef(TypedDict):
    orderArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDeviceIdentifiersRequestRequestTypeDef

```python
# ListDeviceIdentifiersRequestRequestTypeDef definition

class ListDeviceIdentifiersRequestRequestTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[DeviceIdentifierFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: DeviceIdentifierFilterKeysType](./literals.md#deviceidentifierfilterkeystype) 
## ListNetworkResourcesRequestRequestTypeDef

```python
# ListNetworkResourcesRequestRequestTypeDef definition

class ListNetworkResourcesRequestRequestTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[NetworkResourceFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: NetworkResourceFilterKeysType](./literals.md#networkresourcefilterkeystype) 
## ListNetworkSitesRequestRequestTypeDef

```python
# ListNetworkSitesRequestRequestTypeDef definition

class ListNetworkSitesRequestRequestTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[NetworkSiteFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: NetworkSiteFilterKeysType](./literals.md#networksitefilterkeystype) 
## ListNetworksRequestRequestTypeDef

```python
# ListNetworksRequestRequestTypeDef definition

class ListNetworksRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Mapping[NetworkFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: NetworkFilterKeysType](./literals.md#networkfilterkeystype) 
## ListOrdersRequestRequestTypeDef

```python
# ListOrdersRequestRequestTypeDef definition

class ListOrdersRequestRequestTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[OrderFilterKeysType, Sequence[str]]],  # (1)
    maxResults: NotRequired[int],
    startToken: NotRequired[str],
```

1. See [:material-code-brackets: OrderFilterKeysType](./literals.md#orderfilterkeystype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## NameValuePairTypeDef

```python
# NameValuePairTypeDef definition

class NameValuePairTypeDef(TypedDict):
    name: str,
    value: NotRequired[str],
```

## TrackingInformationTypeDef

```python
# TrackingInformationTypeDef definition

class TrackingInformationTypeDef(TypedDict):
    trackingNumber: NotRequired[str],
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

## UpdateNetworkSiteRequestRequestTypeDef

```python
# UpdateNetworkSiteRequestRequestTypeDef definition

class UpdateNetworkSiteRequestRequestTypeDef(TypedDict):
    networkSiteArn: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PingResponseTypeDef

```python
# PingResponseTypeDef definition

class PingResponseTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActivateDeviceIdentifierResponseTypeDef

```python
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
# DeactivateDeviceIdentifierResponseTypeDef definition

class DeactivateDeviceIdentifierResponseTypeDef(TypedDict):
    deviceIdentifier: DeviceIdentifierTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceIdentifierTypeDef](./type_defs.md#deviceidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeviceIdentifierResponseTypeDef

```python
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
# ReturnInformationTypeDef definition

class ReturnInformationTypeDef(TypedDict):
    replacementOrderArn: NotRequired[str],
    returnReason: NotRequired[str],
    shippingAddress: NotRequired[AddressTypeDef],  # (1)
    shippingLabel: NotRequired[str],
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
## ActivateNetworkSiteRequestRequestTypeDef

```python
# ActivateNetworkSiteRequestRequestTypeDef definition

class ActivateNetworkSiteRequestRequestTypeDef(TypedDict):
    networkSiteArn: str,
    shippingAddress: AddressTypeDef,  # (1)
    clientToken: NotRequired[str],
    commitmentConfiguration: NotRequired[CommitmentConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef) 
## CommitmentInformationTypeDef

```python
# CommitmentInformationTypeDef definition

class CommitmentInformationTypeDef(TypedDict):
    commitmentConfiguration: CommitmentConfigurationTypeDef,  # (1)
    expiresOn: NotRequired[datetime],
    startAt: NotRequired[datetime],
```

1. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef) 
## OrderedResourceDefinitionTypeDef

```python
# OrderedResourceDefinitionTypeDef definition

class OrderedResourceDefinitionTypeDef(TypedDict):
    count: int,
    type: NetworkResourceDefinitionTypeType,  # (2)
    commitmentConfiguration: NotRequired[CommitmentConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef) 
2. See [:material-code-brackets: NetworkResourceDefinitionTypeType](./literals.md#networkresourcedefinitiontypetype) 
## StartNetworkResourceUpdateRequestRequestTypeDef

```python
# StartNetworkResourceUpdateRequestRequestTypeDef definition

class StartNetworkResourceUpdateRequestRequestTypeDef(TypedDict):
    networkResourceArn: str,
    updateType: UpdateTypeType,  # (1)
    commitmentConfiguration: NotRequired[CommitmentConfigurationTypeDef],  # (2)
    returnReason: NotRequired[str],
    shippingAddress: NotRequired[AddressTypeDef],  # (3)
```

1. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype) 
2. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef) 
3. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
## ConfigureAccessPointRequestRequestTypeDef

```python
# ConfigureAccessPointRequestRequestTypeDef definition

class ConfigureAccessPointRequestRequestTypeDef(TypedDict):
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
# DeleteNetworkResponseTypeDef definition

class DeleteNetworkResponseTypeDef(TypedDict):
    network: NetworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkTypeDef](./type_defs.md#networktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkResponseTypeDef

```python
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
# ListNetworksResponseTypeDef definition

class ListNetworksResponseTypeDef(TypedDict):
    networks: List[NetworkTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NetworkTypeDef](./type_defs.md#networktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef

```python
# ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef definition

class ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[DeviceIdentifierFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DeviceIdentifierFilterKeysType](./literals.md#deviceidentifierfilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef

```python
# ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef definition

class ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[NetworkResourceFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NetworkResourceFilterKeysType](./literals.md#networkresourcefilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNetworkSitesRequestListNetworkSitesPaginateTypeDef

```python
# ListNetworkSitesRequestListNetworkSitesPaginateTypeDef definition

class ListNetworkSitesRequestListNetworkSitesPaginateTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[NetworkSiteFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NetworkSiteFilterKeysType](./literals.md#networksitefilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNetworksRequestListNetworksPaginateTypeDef

```python
# ListNetworksRequestListNetworksPaginateTypeDef definition

class ListNetworksRequestListNetworksPaginateTypeDef(TypedDict):
    filters: NotRequired[Mapping[NetworkFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NetworkFilterKeysType](./literals.md#networkfilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrdersRequestListOrdersPaginateTypeDef

```python
# ListOrdersRequestListOrdersPaginateTypeDef definition

class ListOrdersRequestListOrdersPaginateTypeDef(TypedDict):
    networkArn: str,
    filters: NotRequired[Mapping[OrderFilterKeysType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OrderFilterKeysType](./literals.md#orderfilterkeystype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## NetworkResourceDefinitionOutputTypeDef

```python
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
# SitePlanOutputTypeDef definition

class SitePlanOutputTypeDef(TypedDict):
    options: NotRequired[List[NameValuePairTypeDef]],  # (1)
    resourceDefinitions: NotRequired[List[NetworkResourceDefinitionOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: NameValuePairTypeDef](./type_defs.md#namevaluepairtypedef) 
2. See [:material-code-braces: NetworkResourceDefinitionOutputTypeDef](./type_defs.md#networkresourcedefinitionoutputtypedef) 
## ConfigureAccessPointResponseTypeDef

```python
# ConfigureAccessPointResponseTypeDef definition

class ConfigureAccessPointResponseTypeDef(TypedDict):
    accessPoint: NetworkResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkResourceTypeDef](./type_defs.md#networkresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkResourceResponseTypeDef

```python
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
# StartNetworkResourceUpdateResponseTypeDef definition

class StartNetworkResourceUpdateResponseTypeDef(TypedDict):
    networkResource: NetworkResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkResourceTypeDef](./type_defs.md#networkresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcknowledgeOrderReceiptResponseTypeDef

```python
# AcknowledgeOrderReceiptResponseTypeDef definition

class AcknowledgeOrderReceiptResponseTypeDef(TypedDict):
    order: OrderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrderTypeDef](./type_defs.md#ordertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOrderResponseTypeDef

```python
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
## SitePlanTypeDef

```python
# SitePlanTypeDef definition

class SitePlanTypeDef(TypedDict):
    options: NotRequired[Sequence[NameValuePairTypeDef]],  # (1)
    resourceDefinitions: NotRequired[Sequence[NetworkResourceDefinitionUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: NameValuePairTypeDef](./type_defs.md#namevaluepairtypedef) 
2. See [:material-code-braces: NetworkResourceDefinitionTypeDef](./type_defs.md#networkresourcedefinitiontypedef) [:material-code-braces: NetworkResourceDefinitionOutputTypeDef](./type_defs.md#networkresourcedefinitionoutputtypedef) 
## ActivateNetworkSiteResponseTypeDef

```python
# ActivateNetworkSiteResponseTypeDef definition

class ActivateNetworkSiteResponseTypeDef(TypedDict):
    networkSite: NetworkSiteTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSiteTypeDef](./type_defs.md#networksitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNetworkSiteResponseTypeDef

```python
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
# DeleteNetworkSiteResponseTypeDef definition

class DeleteNetworkSiteResponseTypeDef(TypedDict):
    networkSite: NetworkSiteTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSiteTypeDef](./type_defs.md#networksitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkSiteResponseTypeDef

```python
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
# UpdateNetworkSiteResponseTypeDef definition

class UpdateNetworkSiteResponseTypeDef(TypedDict):
    networkSite: NetworkSiteTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSiteTypeDef](./type_defs.md#networksitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNetworkSiteRequestRequestTypeDef

```python
# CreateNetworkSiteRequestRequestTypeDef definition

class CreateNetworkSiteRequestRequestTypeDef(TypedDict):
    networkArn: str,
    networkSiteName: str,
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    clientToken: NotRequired[str],
    description: NotRequired[str],
    pendingPlan: NotRequired[SitePlanTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SitePlanTypeDef](./type_defs.md#siteplantypedef) 
## UpdateNetworkSitePlanRequestRequestTypeDef

```python
# UpdateNetworkSitePlanRequestRequestTypeDef definition

class UpdateNetworkSitePlanRequestRequestTypeDef(TypedDict):
    networkSiteArn: str,
    pendingPlan: SitePlanTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: SitePlanTypeDef](./type_defs.md#siteplantypedef) 
