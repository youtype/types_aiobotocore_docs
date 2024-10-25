# Type definitions

> [Index](../README.md) > [DirectConnect](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DirectConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
    type annotations stubs module [types-aiobotocore-directconnect](https://pypi.org/project/types-aiobotocore-directconnect/).



## RouteFilterPrefixTypeDef

```python
# RouteFilterPrefixTypeDef definition

class RouteFilterPrefixTypeDef(TypedDict):
    cidr: NotRequired[str],
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

## AllocateConnectionOnInterconnectRequestRequestTypeDef

```python
# AllocateConnectionOnInterconnectRequestRequestTypeDef definition

class AllocateConnectionOnInterconnectRequestRequestTypeDef(TypedDict):
    bandwidth: str,
    connectionName: str,
    ownerAccount: str,
    interconnectId: str,
    vlan: int,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## AssociateConnectionWithLagRequestRequestTypeDef

```python
# AssociateConnectionWithLagRequestRequestTypeDef definition

class AssociateConnectionWithLagRequestRequestTypeDef(TypedDict):
    connectionId: str,
    lagId: str,
```

## AssociateHostedConnectionRequestRequestTypeDef

```python
# AssociateHostedConnectionRequestRequestTypeDef definition

class AssociateHostedConnectionRequestRequestTypeDef(TypedDict):
    connectionId: str,
    parentConnectionId: str,
```

## AssociateMacSecKeyRequestRequestTypeDef

```python
# AssociateMacSecKeyRequestRequestTypeDef definition

class AssociateMacSecKeyRequestRequestTypeDef(TypedDict):
    connectionId: str,
    secretARN: NotRequired[str],
    ckn: NotRequired[str],
    cak: NotRequired[str],
```

## MacSecKeyTypeDef

```python
# MacSecKeyTypeDef definition

class MacSecKeyTypeDef(TypedDict):
    secretARN: NotRequired[str],
    ckn: NotRequired[str],
    state: NotRequired[str],
    startOn: NotRequired[str],
```

## AssociateVirtualInterfaceRequestRequestTypeDef

```python
# AssociateVirtualInterfaceRequestRequestTypeDef definition

class AssociateVirtualInterfaceRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: str,
    connectionId: str,
```

## AssociatedGatewayTypeDef

```python
# AssociatedGatewayTypeDef definition

class AssociatedGatewayTypeDef(TypedDict):
    id: NotRequired[str],
    type: NotRequired[GatewayTypeType],  # (1)
    ownerAccount: NotRequired[str],
    region: NotRequired[str],
```

1. See [:material-code-brackets: GatewayTypeType](./literals.md#gatewaytypetype) 
## BGPPeerTypeDef

```python
# BGPPeerTypeDef definition

class BGPPeerTypeDef(TypedDict):
    bgpPeerId: NotRequired[str],
    asn: NotRequired[int],
    authKey: NotRequired[str],
    addressFamily: NotRequired[AddressFamilyType],  # (1)
    amazonAddress: NotRequired[str],
    customerAddress: NotRequired[str],
    bgpPeerState: NotRequired[BGPPeerStateType],  # (2)
    bgpStatus: NotRequired[BGPStatusType],  # (3)
    awsDeviceV2: NotRequired[str],
    awsLogicalDeviceId: NotRequired[str],
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
2. See [:material-code-brackets: BGPPeerStateType](./literals.md#bgppeerstatetype) 
3. See [:material-code-brackets: BGPStatusType](./literals.md#bgpstatustype) 
## ConfirmConnectionRequestRequestTypeDef

```python
# ConfirmConnectionRequestRequestTypeDef definition

class ConfirmConnectionRequestRequestTypeDef(TypedDict):
    connectionId: str,
```

## ConfirmCustomerAgreementRequestRequestTypeDef

```python
# ConfirmCustomerAgreementRequestRequestTypeDef definition

class ConfirmCustomerAgreementRequestRequestTypeDef(TypedDict):
    agreementName: NotRequired[str],
```

## ConfirmPrivateVirtualInterfaceRequestRequestTypeDef

```python
# ConfirmPrivateVirtualInterfaceRequestRequestTypeDef definition

class ConfirmPrivateVirtualInterfaceRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: str,
    virtualGatewayId: NotRequired[str],
    directConnectGatewayId: NotRequired[str],
```

## ConfirmPublicVirtualInterfaceRequestRequestTypeDef

```python
# ConfirmPublicVirtualInterfaceRequestRequestTypeDef definition

class ConfirmPublicVirtualInterfaceRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: str,
```

## ConfirmTransitVirtualInterfaceRequestRequestTypeDef

```python
# ConfirmTransitVirtualInterfaceRequestRequestTypeDef definition

class ConfirmTransitVirtualInterfaceRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: str,
    directConnectGatewayId: str,
```

## NewBGPPeerTypeDef

```python
# NewBGPPeerTypeDef definition

class NewBGPPeerTypeDef(TypedDict):
    asn: NotRequired[int],
    authKey: NotRequired[str],
    addressFamily: NotRequired[AddressFamilyType],  # (1)
    amazonAddress: NotRequired[str],
    customerAddress: NotRequired[str],
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
## CreateDirectConnectGatewayRequestRequestTypeDef

```python
# CreateDirectConnectGatewayRequestRequestTypeDef definition

class CreateDirectConnectGatewayRequestRequestTypeDef(TypedDict):
    directConnectGatewayName: str,
    amazonSideAsn: NotRequired[int],
```

## DirectConnectGatewayTypeDef

```python
# DirectConnectGatewayTypeDef definition

class DirectConnectGatewayTypeDef(TypedDict):
    directConnectGatewayId: NotRequired[str],
    directConnectGatewayName: NotRequired[str],
    amazonSideAsn: NotRequired[int],
    ownerAccount: NotRequired[str],
    directConnectGatewayState: NotRequired[DirectConnectGatewayStateType],  # (1)
    stateChangeError: NotRequired[str],
```

1. See [:material-code-brackets: DirectConnectGatewayStateType](./literals.md#directconnectgatewaystatetype) 
## CustomerAgreementTypeDef

```python
# CustomerAgreementTypeDef definition

class CustomerAgreementTypeDef(TypedDict):
    agreementName: NotRequired[str],
    status: NotRequired[str],
```

## DeleteBGPPeerRequestRequestTypeDef

```python
# DeleteBGPPeerRequestRequestTypeDef definition

class DeleteBGPPeerRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: NotRequired[str],
    asn: NotRequired[int],
    customerAddress: NotRequired[str],
    bgpPeerId: NotRequired[str],
```

## DeleteConnectionRequestRequestTypeDef

```python
# DeleteConnectionRequestRequestTypeDef definition

class DeleteConnectionRequestRequestTypeDef(TypedDict):
    connectionId: str,
```

## DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef

```python
# DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef definition

class DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef(TypedDict):
    proposalId: str,
```

## DeleteDirectConnectGatewayAssociationRequestRequestTypeDef

```python
# DeleteDirectConnectGatewayAssociationRequestRequestTypeDef definition

class DeleteDirectConnectGatewayAssociationRequestRequestTypeDef(TypedDict):
    associationId: NotRequired[str],
    directConnectGatewayId: NotRequired[str],
    virtualGatewayId: NotRequired[str],
```

## DeleteDirectConnectGatewayRequestRequestTypeDef

```python
# DeleteDirectConnectGatewayRequestRequestTypeDef definition

class DeleteDirectConnectGatewayRequestRequestTypeDef(TypedDict):
    directConnectGatewayId: str,
```

## DeleteInterconnectRequestRequestTypeDef

```python
# DeleteInterconnectRequestRequestTypeDef definition

class DeleteInterconnectRequestRequestTypeDef(TypedDict):
    interconnectId: str,
```

## DeleteLagRequestRequestTypeDef

```python
# DeleteLagRequestRequestTypeDef definition

class DeleteLagRequestRequestTypeDef(TypedDict):
    lagId: str,
```

## DeleteVirtualInterfaceRequestRequestTypeDef

```python
# DeleteVirtualInterfaceRequestRequestTypeDef definition

class DeleteVirtualInterfaceRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: str,
```

## DescribeConnectionLoaRequestRequestTypeDef

```python
# DescribeConnectionLoaRequestRequestTypeDef definition

class DescribeConnectionLoaRequestRequestTypeDef(TypedDict):
    connectionId: str,
    providerName: NotRequired[str],
    loaContentType: NotRequired[LoaContentTypeType],  # (1)
```

1. See [:material-code-brackets: LoaContentTypeType](./literals.md#loacontenttypetype) 
## LoaTypeDef

```python
# LoaTypeDef definition

class LoaTypeDef(TypedDict):
    loaContent: NotRequired[bytes],
    loaContentType: NotRequired[LoaContentTypeType],  # (1)
```

1. See [:material-code-brackets: LoaContentTypeType](./literals.md#loacontenttypetype) 
## DescribeConnectionsOnInterconnectRequestRequestTypeDef

```python
# DescribeConnectionsOnInterconnectRequestRequestTypeDef definition

class DescribeConnectionsOnInterconnectRequestRequestTypeDef(TypedDict):
    interconnectId: str,
```

## DescribeConnectionsRequestRequestTypeDef

```python
# DescribeConnectionsRequestRequestTypeDef definition

class DescribeConnectionsRequestRequestTypeDef(TypedDict):
    connectionId: NotRequired[str],
```

## DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef

```python
# DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef definition

class DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef(TypedDict):
    directConnectGatewayId: NotRequired[str],
    proposalId: NotRequired[str],
    associatedGatewayId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef

```python
# DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef definition

class DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef(TypedDict):
    associationId: NotRequired[str],
    associatedGatewayId: NotRequired[str],
    directConnectGatewayId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    virtualGatewayId: NotRequired[str],
```

## DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef

```python
# DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef definition

class DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef(TypedDict):
    directConnectGatewayId: NotRequired[str],
    virtualInterfaceId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DirectConnectGatewayAttachmentTypeDef

```python
# DirectConnectGatewayAttachmentTypeDef definition

class DirectConnectGatewayAttachmentTypeDef(TypedDict):
    directConnectGatewayId: NotRequired[str],
    virtualInterfaceId: NotRequired[str],
    virtualInterfaceRegion: NotRequired[str],
    virtualInterfaceOwnerAccount: NotRequired[str],
    attachmentState: NotRequired[DirectConnectGatewayAttachmentStateType],  # (1)
    attachmentType: NotRequired[DirectConnectGatewayAttachmentTypeType],  # (2)
    stateChangeError: NotRequired[str],
```

1. See [:material-code-brackets: DirectConnectGatewayAttachmentStateType](./literals.md#directconnectgatewayattachmentstatetype) 
2. See [:material-code-brackets: DirectConnectGatewayAttachmentTypeType](./literals.md#directconnectgatewayattachmenttypetype) 
## DescribeDirectConnectGatewaysRequestRequestTypeDef

```python
# DescribeDirectConnectGatewaysRequestRequestTypeDef definition

class DescribeDirectConnectGatewaysRequestRequestTypeDef(TypedDict):
    directConnectGatewayId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DescribeHostedConnectionsRequestRequestTypeDef

```python
# DescribeHostedConnectionsRequestRequestTypeDef definition

class DescribeHostedConnectionsRequestRequestTypeDef(TypedDict):
    connectionId: str,
```

## DescribeInterconnectLoaRequestRequestTypeDef

```python
# DescribeInterconnectLoaRequestRequestTypeDef definition

class DescribeInterconnectLoaRequestRequestTypeDef(TypedDict):
    interconnectId: str,
    providerName: NotRequired[str],
    loaContentType: NotRequired[LoaContentTypeType],  # (1)
```

1. See [:material-code-brackets: LoaContentTypeType](./literals.md#loacontenttypetype) 
## DescribeInterconnectsRequestRequestTypeDef

```python
# DescribeInterconnectsRequestRequestTypeDef definition

class DescribeInterconnectsRequestRequestTypeDef(TypedDict):
    interconnectId: NotRequired[str],
```

## DescribeLagsRequestRequestTypeDef

```python
# DescribeLagsRequestRequestTypeDef definition

class DescribeLagsRequestRequestTypeDef(TypedDict):
    lagId: NotRequired[str],
```

## DescribeLoaRequestRequestTypeDef

```python
# DescribeLoaRequestRequestTypeDef definition

class DescribeLoaRequestRequestTypeDef(TypedDict):
    connectionId: str,
    providerName: NotRequired[str],
    loaContentType: NotRequired[LoaContentTypeType],  # (1)
```

1. See [:material-code-brackets: LoaContentTypeType](./literals.md#loacontenttypetype) 
## DescribeRouterConfigurationRequestRequestTypeDef

```python
# DescribeRouterConfigurationRequestRequestTypeDef definition

class DescribeRouterConfigurationRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: str,
    routerTypeIdentifier: NotRequired[str],
```

## RouterTypeTypeDef

```python
# RouterTypeTypeDef definition

class RouterTypeTypeDef(TypedDict):
    vendor: NotRequired[str],
    platform: NotRequired[str],
    software: NotRequired[str],
    xsltTemplateName: NotRequired[str],
    xsltTemplateNameForMacSec: NotRequired[str],
    routerTypeIdentifier: NotRequired[str],
```

## DescribeTagsRequestRequestTypeDef

```python
# DescribeTagsRequestRequestTypeDef definition

class DescribeTagsRequestRequestTypeDef(TypedDict):
    resourceArns: Sequence[str],
```

## DescribeVirtualInterfacesRequestRequestTypeDef

```python
# DescribeVirtualInterfacesRequestRequestTypeDef definition

class DescribeVirtualInterfacesRequestRequestTypeDef(TypedDict):
    connectionId: NotRequired[str],
    virtualInterfaceId: NotRequired[str],
```

## DisassociateConnectionFromLagRequestRequestTypeDef

```python
# DisassociateConnectionFromLagRequestRequestTypeDef definition

class DisassociateConnectionFromLagRequestRequestTypeDef(TypedDict):
    connectionId: str,
    lagId: str,
```

## DisassociateMacSecKeyRequestRequestTypeDef

```python
# DisassociateMacSecKeyRequestRequestTypeDef definition

class DisassociateMacSecKeyRequestRequestTypeDef(TypedDict):
    connectionId: str,
    secretARN: str,
```

## ListVirtualInterfaceTestHistoryRequestRequestTypeDef

```python
# ListVirtualInterfaceTestHistoryRequestRequestTypeDef definition

class ListVirtualInterfaceTestHistoryRequestRequestTypeDef(TypedDict):
    testId: NotRequired[str],
    virtualInterfaceId: NotRequired[str],
    bgpPeers: NotRequired[Sequence[str]],
    status: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## VirtualInterfaceTestHistoryTypeDef

```python
# VirtualInterfaceTestHistoryTypeDef definition

class VirtualInterfaceTestHistoryTypeDef(TypedDict):
    testId: NotRequired[str],
    virtualInterfaceId: NotRequired[str],
    bgpPeers: NotRequired[List[str]],
    status: NotRequired[str],
    ownerAccount: NotRequired[str],
    testDurationInMinutes: NotRequired[int],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

## LocationTypeDef

```python
# LocationTypeDef definition

class LocationTypeDef(TypedDict):
    locationCode: NotRequired[str],
    locationName: NotRequired[str],
    region: NotRequired[str],
    availablePortSpeeds: NotRequired[List[str]],
    availableProviders: NotRequired[List[str]],
    availableMacSecPortSpeeds: NotRequired[List[str]],
```

## StartBgpFailoverTestRequestRequestTypeDef

```python
# StartBgpFailoverTestRequestRequestTypeDef definition

class StartBgpFailoverTestRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: str,
    bgpPeers: NotRequired[Sequence[str]],
    testDurationInMinutes: NotRequired[int],
```

## StopBgpFailoverTestRequestRequestTypeDef

```python
# StopBgpFailoverTestRequestRequestTypeDef definition

class StopBgpFailoverTestRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateConnectionRequestRequestTypeDef

```python
# UpdateConnectionRequestRequestTypeDef definition

class UpdateConnectionRequestRequestTypeDef(TypedDict):
    connectionId: str,
    connectionName: NotRequired[str],
    encryptionMode: NotRequired[str],
```

## UpdateDirectConnectGatewayRequestRequestTypeDef

```python
# UpdateDirectConnectGatewayRequestRequestTypeDef definition

class UpdateDirectConnectGatewayRequestRequestTypeDef(TypedDict):
    directConnectGatewayId: str,
    newDirectConnectGatewayName: str,
```

## UpdateLagRequestRequestTypeDef

```python
# UpdateLagRequestRequestTypeDef definition

class UpdateLagRequestRequestTypeDef(TypedDict):
    lagId: str,
    lagName: NotRequired[str],
    minimumLinks: NotRequired[int],
    encryptionMode: NotRequired[str],
```

## UpdateVirtualInterfaceAttributesRequestRequestTypeDef

```python
# UpdateVirtualInterfaceAttributesRequestRequestTypeDef definition

class UpdateVirtualInterfaceAttributesRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: str,
    mtu: NotRequired[int],
    enableSiteLink: NotRequired[bool],
    virtualInterfaceName: NotRequired[str],
```

## VirtualGatewayTypeDef

```python
# VirtualGatewayTypeDef definition

class VirtualGatewayTypeDef(TypedDict):
    virtualGatewayId: NotRequired[str],
    virtualGatewayState: NotRequired[str],
```

## AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef

```python
# AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef definition

class AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef(TypedDict):
    directConnectGatewayId: str,
    proposalId: str,
    associatedGatewayOwnerAccount: str,
    overrideAllowedPrefixesToDirectConnectGateway: NotRequired[Sequence[RouteFilterPrefixTypeDef]],  # (1)
```

1. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
## CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef

```python
# CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef definition

class CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef(TypedDict):
    directConnectGatewayId: str,
    directConnectGatewayOwnerAccount: str,
    gatewayId: str,
    addAllowedPrefixesToDirectConnectGateway: NotRequired[Sequence[RouteFilterPrefixTypeDef]],  # (1)
    removeAllowedPrefixesToDirectConnectGateway: NotRequired[Sequence[RouteFilterPrefixTypeDef]],  # (1)
```

1. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
2. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
## CreateDirectConnectGatewayAssociationRequestRequestTypeDef

```python
# CreateDirectConnectGatewayAssociationRequestRequestTypeDef definition

class CreateDirectConnectGatewayAssociationRequestRequestTypeDef(TypedDict):
    directConnectGatewayId: str,
    gatewayId: NotRequired[str],
    addAllowedPrefixesToDirectConnectGateway: NotRequired[Sequence[RouteFilterPrefixTypeDef]],  # (1)
    virtualGatewayId: NotRequired[str],
```

1. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
## UpdateDirectConnectGatewayAssociationRequestRequestTypeDef

```python
# UpdateDirectConnectGatewayAssociationRequestRequestTypeDef definition

class UpdateDirectConnectGatewayAssociationRequestRequestTypeDef(TypedDict):
    associationId: NotRequired[str],
    addAllowedPrefixesToDirectConnectGateway: NotRequired[Sequence[RouteFilterPrefixTypeDef]],  # (1)
    removeAllowedPrefixesToDirectConnectGateway: NotRequired[Sequence[RouteFilterPrefixTypeDef]],  # (1)
```

1. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
2. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
## ConfirmConnectionResponseTypeDef

```python
# ConfirmConnectionResponseTypeDef definition

class ConfirmConnectionResponseTypeDef(TypedDict):
    connectionState: ConnectionStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfirmCustomerAgreementResponseTypeDef

```python
# ConfirmCustomerAgreementResponseTypeDef definition

class ConfirmCustomerAgreementResponseTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfirmPrivateVirtualInterfaceResponseTypeDef

```python
# ConfirmPrivateVirtualInterfaceResponseTypeDef definition

class ConfirmPrivateVirtualInterfaceResponseTypeDef(TypedDict):
    virtualInterfaceState: VirtualInterfaceStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VirtualInterfaceStateType](./literals.md#virtualinterfacestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfirmPublicVirtualInterfaceResponseTypeDef

```python
# ConfirmPublicVirtualInterfaceResponseTypeDef definition

class ConfirmPublicVirtualInterfaceResponseTypeDef(TypedDict):
    virtualInterfaceState: VirtualInterfaceStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VirtualInterfaceStateType](./literals.md#virtualinterfacestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfirmTransitVirtualInterfaceResponseTypeDef

```python
# ConfirmTransitVirtualInterfaceResponseTypeDef definition

class ConfirmTransitVirtualInterfaceResponseTypeDef(TypedDict):
    virtualInterfaceState: VirtualInterfaceStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VirtualInterfaceStateType](./literals.md#virtualinterfacestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInterconnectResponseTypeDef

```python
# DeleteInterconnectResponseTypeDef definition

class DeleteInterconnectResponseTypeDef(TypedDict):
    interconnectState: InterconnectStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: InterconnectStateType](./literals.md#interconnectstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVirtualInterfaceResponseTypeDef

```python
# DeleteVirtualInterfaceResponseTypeDef definition

class DeleteVirtualInterfaceResponseTypeDef(TypedDict):
    virtualInterfaceState: VirtualInterfaceStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VirtualInterfaceStateType](./literals.md#virtualinterfacestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoaResponseTypeDef

```python
# LoaResponseTypeDef definition

class LoaResponseTypeDef(TypedDict):
    loaContent: bytes,
    loaContentType: LoaContentTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LoaContentTypeType](./literals.md#loacontenttypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AllocateHostedConnectionRequestRequestTypeDef

```python
# AllocateHostedConnectionRequestRequestTypeDef definition

class AllocateHostedConnectionRequestRequestTypeDef(TypedDict):
    connectionId: str,
    ownerAccount: str,
    bandwidth: str,
    connectionName: str,
    vlan: int,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateConnectionRequestRequestTypeDef

```python
# CreateConnectionRequestRequestTypeDef definition

class CreateConnectionRequestRequestTypeDef(TypedDict):
    location: str,
    bandwidth: str,
    connectionName: str,
    lagId: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    providerName: NotRequired[str],
    requestMACSec: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateInterconnectRequestRequestTypeDef

```python
# CreateInterconnectRequestRequestTypeDef definition

class CreateInterconnectRequestRequestTypeDef(TypedDict):
    interconnectName: str,
    bandwidth: str,
    location: str,
    lagId: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    providerName: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateLagRequestRequestTypeDef

```python
# CreateLagRequestRequestTypeDef definition

class CreateLagRequestRequestTypeDef(TypedDict):
    numberOfConnections: int,
    location: str,
    connectionsBandwidth: str,
    lagName: str,
    connectionId: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    childConnectionTags: NotRequired[Sequence[TagTypeDef]],  # (1)
    providerName: NotRequired[str],
    requestMACSec: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## InterconnectResponseTypeDef

```python
# InterconnectResponseTypeDef definition

class InterconnectResponseTypeDef(TypedDict):
    interconnectId: str,
    interconnectName: str,
    interconnectState: InterconnectStateType,  # (1)
    region: str,
    location: str,
    bandwidth: str,
    loaIssueTime: datetime,
    lagId: str,
    awsDevice: str,
    jumboFrameCapable: bool,
    awsDeviceV2: str,
    awsLogicalDeviceId: str,
    hasLogicalRedundancy: HasLogicalRedundancyType,  # (2)
    tags: List[TagTypeDef],  # (3)
    providerName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: InterconnectStateType](./literals.md#interconnectstatetype) 
2. See [:material-code-brackets: HasLogicalRedundancyType](./literals.md#haslogicalredundancytype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InterconnectTypeDef

```python
# InterconnectTypeDef definition

class InterconnectTypeDef(TypedDict):
    interconnectId: NotRequired[str],
    interconnectName: NotRequired[str],
    interconnectState: NotRequired[InterconnectStateType],  # (1)
    region: NotRequired[str],
    location: NotRequired[str],
    bandwidth: NotRequired[str],
    loaIssueTime: NotRequired[datetime],
    lagId: NotRequired[str],
    awsDevice: NotRequired[str],
    jumboFrameCapable: NotRequired[bool],
    awsDeviceV2: NotRequired[str],
    awsLogicalDeviceId: NotRequired[str],
    hasLogicalRedundancy: NotRequired[HasLogicalRedundancyType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    providerName: NotRequired[str],
```

1. See [:material-code-brackets: InterconnectStateType](./literals.md#interconnectstatetype) 
2. See [:material-code-brackets: HasLogicalRedundancyType](./literals.md#haslogicalredundancytype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## NewPrivateVirtualInterfaceAllocationTypeDef

```python
# NewPrivateVirtualInterfaceAllocationTypeDef definition

class NewPrivateVirtualInterfaceAllocationTypeDef(TypedDict):
    virtualInterfaceName: str,
    vlan: int,
    asn: int,
    mtu: NotRequired[int],
    authKey: NotRequired[str],
    amazonAddress: NotRequired[str],
    addressFamily: NotRequired[AddressFamilyType],  # (1)
    customerAddress: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## NewPrivateVirtualInterfaceTypeDef

```python
# NewPrivateVirtualInterfaceTypeDef definition

class NewPrivateVirtualInterfaceTypeDef(TypedDict):
    virtualInterfaceName: str,
    vlan: int,
    asn: int,
    mtu: NotRequired[int],
    authKey: NotRequired[str],
    amazonAddress: NotRequired[str],
    customerAddress: NotRequired[str],
    addressFamily: NotRequired[AddressFamilyType],  # (1)
    virtualGatewayId: NotRequired[str],
    directConnectGatewayId: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    enableSiteLink: NotRequired[bool],
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## NewPublicVirtualInterfaceAllocationTypeDef

```python
# NewPublicVirtualInterfaceAllocationTypeDef definition

class NewPublicVirtualInterfaceAllocationTypeDef(TypedDict):
    virtualInterfaceName: str,
    vlan: int,
    asn: int,
    authKey: NotRequired[str],
    amazonAddress: NotRequired[str],
    customerAddress: NotRequired[str],
    addressFamily: NotRequired[AddressFamilyType],  # (1)
    routeFilterPrefixes: NotRequired[Sequence[RouteFilterPrefixTypeDef]],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
2. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## NewPublicVirtualInterfaceTypeDef

```python
# NewPublicVirtualInterfaceTypeDef definition

class NewPublicVirtualInterfaceTypeDef(TypedDict):
    virtualInterfaceName: str,
    vlan: int,
    asn: int,
    authKey: NotRequired[str],
    amazonAddress: NotRequired[str],
    customerAddress: NotRequired[str],
    addressFamily: NotRequired[AddressFamilyType],  # (1)
    routeFilterPrefixes: NotRequired[Sequence[RouteFilterPrefixTypeDef]],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
2. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## NewTransitVirtualInterfaceAllocationTypeDef

```python
# NewTransitVirtualInterfaceAllocationTypeDef definition

class NewTransitVirtualInterfaceAllocationTypeDef(TypedDict):
    virtualInterfaceName: NotRequired[str],
    vlan: NotRequired[int],
    asn: NotRequired[int],
    mtu: NotRequired[int],
    authKey: NotRequired[str],
    amazonAddress: NotRequired[str],
    customerAddress: NotRequired[str],
    addressFamily: NotRequired[AddressFamilyType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## NewTransitVirtualInterfaceTypeDef

```python
# NewTransitVirtualInterfaceTypeDef definition

class NewTransitVirtualInterfaceTypeDef(TypedDict):
    virtualInterfaceName: NotRequired[str],
    vlan: NotRequired[int],
    asn: NotRequired[int],
    mtu: NotRequired[int],
    authKey: NotRequired[str],
    amazonAddress: NotRequired[str],
    customerAddress: NotRequired[str],
    addressFamily: NotRequired[AddressFamilyType],  # (1)
    directConnectGatewayId: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    enableSiteLink: NotRequired[bool],
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ResourceTagTypeDef

```python
# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AssociateMacSecKeyResponseTypeDef

```python
# AssociateMacSecKeyResponseTypeDef definition

class AssociateMacSecKeyResponseTypeDef(TypedDict):
    connectionId: str,
    macSecKeys: List[MacSecKeyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MacSecKeyTypeDef](./type_defs.md#macseckeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionResponseTypeDef

```python
# ConnectionResponseTypeDef definition

class ConnectionResponseTypeDef(TypedDict):
    ownerAccount: str,
    connectionId: str,
    connectionName: str,
    connectionState: ConnectionStateType,  # (1)
    region: str,
    location: str,
    bandwidth: str,
    vlan: int,
    partnerName: str,
    loaIssueTime: datetime,
    lagId: str,
    awsDevice: str,
    jumboFrameCapable: bool,
    awsDeviceV2: str,
    awsLogicalDeviceId: str,
    hasLogicalRedundancy: HasLogicalRedundancyType,  # (2)
    tags: List[TagTypeDef],  # (3)
    providerName: str,
    macSecCapable: bool,
    portEncryptionStatus: str,
    encryptionMode: str,
    macSecKeys: List[MacSecKeyTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-brackets: HasLogicalRedundancyType](./literals.md#haslogicalredundancytype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: MacSecKeyTypeDef](./type_defs.md#macseckeytypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionTypeDef

```python
# ConnectionTypeDef definition

class ConnectionTypeDef(TypedDict):
    ownerAccount: NotRequired[str],
    connectionId: NotRequired[str],
    connectionName: NotRequired[str],
    connectionState: NotRequired[ConnectionStateType],  # (1)
    region: NotRequired[str],
    location: NotRequired[str],
    bandwidth: NotRequired[str],
    vlan: NotRequired[int],
    partnerName: NotRequired[str],
    loaIssueTime: NotRequired[datetime],
    lagId: NotRequired[str],
    awsDevice: NotRequired[str],
    jumboFrameCapable: NotRequired[bool],
    awsDeviceV2: NotRequired[str],
    awsLogicalDeviceId: NotRequired[str],
    hasLogicalRedundancy: NotRequired[HasLogicalRedundancyType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    providerName: NotRequired[str],
    macSecCapable: NotRequired[bool],
    portEncryptionStatus: NotRequired[str],
    encryptionMode: NotRequired[str],
    macSecKeys: NotRequired[List[MacSecKeyTypeDef]],  # (4)
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-brackets: HasLogicalRedundancyType](./literals.md#haslogicalredundancytype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: MacSecKeyTypeDef](./type_defs.md#macseckeytypedef) 
## DisassociateMacSecKeyResponseTypeDef

```python
# DisassociateMacSecKeyResponseTypeDef definition

class DisassociateMacSecKeyResponseTypeDef(TypedDict):
    connectionId: str,
    macSecKeys: List[MacSecKeyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MacSecKeyTypeDef](./type_defs.md#macseckeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DirectConnectGatewayAssociationProposalTypeDef

```python
# DirectConnectGatewayAssociationProposalTypeDef definition

class DirectConnectGatewayAssociationProposalTypeDef(TypedDict):
    proposalId: NotRequired[str],
    directConnectGatewayId: NotRequired[str],
    directConnectGatewayOwnerAccount: NotRequired[str],
    proposalState: NotRequired[DirectConnectGatewayAssociationProposalStateType],  # (1)
    associatedGateway: NotRequired[AssociatedGatewayTypeDef],  # (2)
    existingAllowedPrefixesToDirectConnectGateway: NotRequired[List[RouteFilterPrefixTypeDef]],  # (3)
    requestedAllowedPrefixesToDirectConnectGateway: NotRequired[List[RouteFilterPrefixTypeDef]],  # (3)
```

1. See [:material-code-brackets: DirectConnectGatewayAssociationProposalStateType](./literals.md#directconnectgatewayassociationproposalstatetype) 
2. See [:material-code-braces: AssociatedGatewayTypeDef](./type_defs.md#associatedgatewaytypedef) 
3. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
4. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
## DirectConnectGatewayAssociationTypeDef

```python
# DirectConnectGatewayAssociationTypeDef definition

class DirectConnectGatewayAssociationTypeDef(TypedDict):
    directConnectGatewayId: NotRequired[str],
    directConnectGatewayOwnerAccount: NotRequired[str],
    associationState: NotRequired[DirectConnectGatewayAssociationStateType],  # (1)
    stateChangeError: NotRequired[str],
    associatedGateway: NotRequired[AssociatedGatewayTypeDef],  # (2)
    associationId: NotRequired[str],
    allowedPrefixesToDirectConnectGateway: NotRequired[List[RouteFilterPrefixTypeDef]],  # (3)
    virtualGatewayId: NotRequired[str],
    virtualGatewayRegion: NotRequired[str],
    virtualGatewayOwnerAccount: NotRequired[str],
```

1. See [:material-code-brackets: DirectConnectGatewayAssociationStateType](./literals.md#directconnectgatewayassociationstatetype) 
2. See [:material-code-braces: AssociatedGatewayTypeDef](./type_defs.md#associatedgatewaytypedef) 
3. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
## VirtualInterfaceResponseTypeDef

```python
# VirtualInterfaceResponseTypeDef definition

class VirtualInterfaceResponseTypeDef(TypedDict):
    ownerAccount: str,
    virtualInterfaceId: str,
    location: str,
    connectionId: str,
    virtualInterfaceType: str,
    virtualInterfaceName: str,
    vlan: int,
    asn: int,
    amazonSideAsn: int,
    authKey: str,
    amazonAddress: str,
    customerAddress: str,
    addressFamily: AddressFamilyType,  # (1)
    virtualInterfaceState: VirtualInterfaceStateType,  # (2)
    customerRouterConfig: str,
    mtu: int,
    jumboFrameCapable: bool,
    virtualGatewayId: str,
    directConnectGatewayId: str,
    routeFilterPrefixes: List[RouteFilterPrefixTypeDef],  # (3)
    bgpPeers: List[BGPPeerTypeDef],  # (4)
    region: str,
    awsDeviceV2: str,
    awsLogicalDeviceId: str,
    tags: List[TagTypeDef],  # (5)
    siteLinkEnabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
2. See [:material-code-brackets: VirtualInterfaceStateType](./literals.md#virtualinterfacestatetype) 
3. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
4. See [:material-code-braces: BGPPeerTypeDef](./type_defs.md#bgppeertypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VirtualInterfaceTypeDef

```python
# VirtualInterfaceTypeDef definition

class VirtualInterfaceTypeDef(TypedDict):
    ownerAccount: NotRequired[str],
    virtualInterfaceId: NotRequired[str],
    location: NotRequired[str],
    connectionId: NotRequired[str],
    virtualInterfaceType: NotRequired[str],
    virtualInterfaceName: NotRequired[str],
    vlan: NotRequired[int],
    asn: NotRequired[int],
    amazonSideAsn: NotRequired[int],
    authKey: NotRequired[str],
    amazonAddress: NotRequired[str],
    customerAddress: NotRequired[str],
    addressFamily: NotRequired[AddressFamilyType],  # (1)
    virtualInterfaceState: NotRequired[VirtualInterfaceStateType],  # (2)
    customerRouterConfig: NotRequired[str],
    mtu: NotRequired[int],
    jumboFrameCapable: NotRequired[bool],
    virtualGatewayId: NotRequired[str],
    directConnectGatewayId: NotRequired[str],
    routeFilterPrefixes: NotRequired[List[RouteFilterPrefixTypeDef]],  # (3)
    bgpPeers: NotRequired[List[BGPPeerTypeDef]],  # (4)
    region: NotRequired[str],
    awsDeviceV2: NotRequired[str],
    awsLogicalDeviceId: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (5)
    siteLinkEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
2. See [:material-code-brackets: VirtualInterfaceStateType](./literals.md#virtualinterfacestatetype) 
3. See [:material-code-braces: RouteFilterPrefixTypeDef](./type_defs.md#routefilterprefixtypedef) 
4. See [:material-code-braces: BGPPeerTypeDef](./type_defs.md#bgppeertypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateBGPPeerRequestRequestTypeDef

```python
# CreateBGPPeerRequestRequestTypeDef definition

class CreateBGPPeerRequestRequestTypeDef(TypedDict):
    virtualInterfaceId: NotRequired[str],
    newBGPPeer: NotRequired[NewBGPPeerTypeDef],  # (1)
```

1. See [:material-code-braces: NewBGPPeerTypeDef](./type_defs.md#newbgppeertypedef) 
## CreateDirectConnectGatewayResultTypeDef

```python
# CreateDirectConnectGatewayResultTypeDef definition

class CreateDirectConnectGatewayResultTypeDef(TypedDict):
    directConnectGateway: DirectConnectGatewayTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectConnectGatewayTypeDef](./type_defs.md#directconnectgatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDirectConnectGatewayResultTypeDef

```python
# DeleteDirectConnectGatewayResultTypeDef definition

class DeleteDirectConnectGatewayResultTypeDef(TypedDict):
    directConnectGateway: DirectConnectGatewayTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectConnectGatewayTypeDef](./type_defs.md#directconnectgatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDirectConnectGatewaysResultTypeDef

```python
# DescribeDirectConnectGatewaysResultTypeDef definition

class DescribeDirectConnectGatewaysResultTypeDef(TypedDict):
    directConnectGateways: List[DirectConnectGatewayTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DirectConnectGatewayTypeDef](./type_defs.md#directconnectgatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDirectConnectGatewayResponseTypeDef

```python
# UpdateDirectConnectGatewayResponseTypeDef definition

class UpdateDirectConnectGatewayResponseTypeDef(TypedDict):
    directConnectGateway: DirectConnectGatewayTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectConnectGatewayTypeDef](./type_defs.md#directconnectgatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCustomerMetadataResponseTypeDef

```python
# DescribeCustomerMetadataResponseTypeDef definition

class DescribeCustomerMetadataResponseTypeDef(TypedDict):
    agreements: List[CustomerAgreementTypeDef],  # (1)
    nniPartnerType: NniPartnerTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CustomerAgreementTypeDef](./type_defs.md#customeragreementtypedef) 
2. See [:material-code-brackets: NniPartnerTypeType](./literals.md#nnipartnertypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConnectionLoaResponseTypeDef

```python
# DescribeConnectionLoaResponseTypeDef definition

class DescribeConnectionLoaResponseTypeDef(TypedDict):
    loa: LoaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoaTypeDef](./type_defs.md#loatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInterconnectLoaResponseTypeDef

```python
# DescribeInterconnectLoaResponseTypeDef definition

class DescribeInterconnectLoaResponseTypeDef(TypedDict):
    loa: LoaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoaTypeDef](./type_defs.md#loatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef

```python
# DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef definition

class DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef(TypedDict):
    associationId: NotRequired[str],
    associatedGatewayId: NotRequired[str],
    directConnectGatewayId: NotRequired[str],
    virtualGatewayId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef

```python
# DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef definition

class DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef(TypedDict):
    directConnectGatewayId: NotRequired[str],
    virtualInterfaceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef

```python
# DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef definition

class DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef(TypedDict):
    directConnectGatewayId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDirectConnectGatewayAttachmentsResultTypeDef

```python
# DescribeDirectConnectGatewayAttachmentsResultTypeDef definition

class DescribeDirectConnectGatewayAttachmentsResultTypeDef(TypedDict):
    directConnectGatewayAttachments: List[DirectConnectGatewayAttachmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DirectConnectGatewayAttachmentTypeDef](./type_defs.md#directconnectgatewayattachmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRouterConfigurationResponseTypeDef

```python
# DescribeRouterConfigurationResponseTypeDef definition

class DescribeRouterConfigurationResponseTypeDef(TypedDict):
    customerRouterConfig: str,
    router: RouterTypeTypeDef,  # (1)
    virtualInterfaceId: str,
    virtualInterfaceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RouterTypeTypeDef](./type_defs.md#routertypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVirtualInterfaceTestHistoryResponseTypeDef

```python
# ListVirtualInterfaceTestHistoryResponseTypeDef definition

class ListVirtualInterfaceTestHistoryResponseTypeDef(TypedDict):
    virtualInterfaceTestHistory: List[VirtualInterfaceTestHistoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VirtualInterfaceTestHistoryTypeDef](./type_defs.md#virtualinterfacetesthistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBgpFailoverTestResponseTypeDef

```python
# StartBgpFailoverTestResponseTypeDef definition

class StartBgpFailoverTestResponseTypeDef(TypedDict):
    virtualInterfaceTest: VirtualInterfaceTestHistoryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualInterfaceTestHistoryTypeDef](./type_defs.md#virtualinterfacetesthistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopBgpFailoverTestResponseTypeDef

```python
# StopBgpFailoverTestResponseTypeDef definition

class StopBgpFailoverTestResponseTypeDef(TypedDict):
    virtualInterfaceTest: VirtualInterfaceTestHistoryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualInterfaceTestHistoryTypeDef](./type_defs.md#virtualinterfacetesthistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LocationsTypeDef

```python
# LocationsTypeDef definition

class LocationsTypeDef(TypedDict):
    locations: List[LocationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VirtualGatewaysTypeDef

```python
# VirtualGatewaysTypeDef definition

class VirtualGatewaysTypeDef(TypedDict):
    virtualGateways: List[VirtualGatewayTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualGatewayTypeDef](./type_defs.md#virtualgatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InterconnectsTypeDef

```python
# InterconnectsTypeDef definition

class InterconnectsTypeDef(TypedDict):
    interconnects: List[InterconnectTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InterconnectTypeDef](./type_defs.md#interconnecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AllocatePrivateVirtualInterfaceRequestRequestTypeDef

```python
# AllocatePrivateVirtualInterfaceRequestRequestTypeDef definition

class AllocatePrivateVirtualInterfaceRequestRequestTypeDef(TypedDict):
    connectionId: str,
    ownerAccount: str,
    newPrivateVirtualInterfaceAllocation: NewPrivateVirtualInterfaceAllocationTypeDef,  # (1)
```

1. See [:material-code-braces: NewPrivateVirtualInterfaceAllocationTypeDef](./type_defs.md#newprivatevirtualinterfaceallocationtypedef) 
## CreatePrivateVirtualInterfaceRequestRequestTypeDef

```python
# CreatePrivateVirtualInterfaceRequestRequestTypeDef definition

class CreatePrivateVirtualInterfaceRequestRequestTypeDef(TypedDict):
    connectionId: str,
    newPrivateVirtualInterface: NewPrivateVirtualInterfaceTypeDef,  # (1)
```

1. See [:material-code-braces: NewPrivateVirtualInterfaceTypeDef](./type_defs.md#newprivatevirtualinterfacetypedef) 
## AllocatePublicVirtualInterfaceRequestRequestTypeDef

```python
# AllocatePublicVirtualInterfaceRequestRequestTypeDef definition

class AllocatePublicVirtualInterfaceRequestRequestTypeDef(TypedDict):
    connectionId: str,
    ownerAccount: str,
    newPublicVirtualInterfaceAllocation: NewPublicVirtualInterfaceAllocationTypeDef,  # (1)
```

1. See [:material-code-braces: NewPublicVirtualInterfaceAllocationTypeDef](./type_defs.md#newpublicvirtualinterfaceallocationtypedef) 
## CreatePublicVirtualInterfaceRequestRequestTypeDef

```python
# CreatePublicVirtualInterfaceRequestRequestTypeDef definition

class CreatePublicVirtualInterfaceRequestRequestTypeDef(TypedDict):
    connectionId: str,
    newPublicVirtualInterface: NewPublicVirtualInterfaceTypeDef,  # (1)
```

1. See [:material-code-braces: NewPublicVirtualInterfaceTypeDef](./type_defs.md#newpublicvirtualinterfacetypedef) 
## AllocateTransitVirtualInterfaceRequestRequestTypeDef

```python
# AllocateTransitVirtualInterfaceRequestRequestTypeDef definition

class AllocateTransitVirtualInterfaceRequestRequestTypeDef(TypedDict):
    connectionId: str,
    ownerAccount: str,
    newTransitVirtualInterfaceAllocation: NewTransitVirtualInterfaceAllocationTypeDef,  # (1)
```

1. See [:material-code-braces: NewTransitVirtualInterfaceAllocationTypeDef](./type_defs.md#newtransitvirtualinterfaceallocationtypedef) 
## CreateTransitVirtualInterfaceRequestRequestTypeDef

```python
# CreateTransitVirtualInterfaceRequestRequestTypeDef definition

class CreateTransitVirtualInterfaceRequestRequestTypeDef(TypedDict):
    connectionId: str,
    newTransitVirtualInterface: NewTransitVirtualInterfaceTypeDef,  # (1)
```

1. See [:material-code-braces: NewTransitVirtualInterfaceTypeDef](./type_defs.md#newtransitvirtualinterfacetypedef) 
## DescribeTagsResponseTypeDef

```python
# DescribeTagsResponseTypeDef definition

class DescribeTagsResponseTypeDef(TypedDict):
    resourceTags: List[ResourceTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionsTypeDef

```python
# ConnectionsTypeDef definition

class ConnectionsTypeDef(TypedDict):
    connections: List[ConnectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LagResponseTypeDef

```python
# LagResponseTypeDef definition

class LagResponseTypeDef(TypedDict):
    connectionsBandwidth: str,
    numberOfConnections: int,
    lagId: str,
    ownerAccount: str,
    lagName: str,
    lagState: LagStateType,  # (1)
    location: str,
    region: str,
    minimumLinks: int,
    awsDevice: str,
    awsDeviceV2: str,
    awsLogicalDeviceId: str,
    connections: List[ConnectionTypeDef],  # (2)
    allowsHostedConnections: bool,
    jumboFrameCapable: bool,
    hasLogicalRedundancy: HasLogicalRedundancyType,  # (3)
    tags: List[TagTypeDef],  # (4)
    providerName: str,
    macSecCapable: bool,
    encryptionMode: str,
    macSecKeys: List[MacSecKeyTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: LagStateType](./literals.md#lagstatetype) 
2. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
3. See [:material-code-brackets: HasLogicalRedundancyType](./literals.md#haslogicalredundancytype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: MacSecKeyTypeDef](./type_defs.md#macseckeytypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LagTypeDef

```python
# LagTypeDef definition

class LagTypeDef(TypedDict):
    connectionsBandwidth: NotRequired[str],
    numberOfConnections: NotRequired[int],
    lagId: NotRequired[str],
    ownerAccount: NotRequired[str],
    lagName: NotRequired[str],
    lagState: NotRequired[LagStateType],  # (1)
    location: NotRequired[str],
    region: NotRequired[str],
    minimumLinks: NotRequired[int],
    awsDevice: NotRequired[str],
    awsDeviceV2: NotRequired[str],
    awsLogicalDeviceId: NotRequired[str],
    connections: NotRequired[List[ConnectionTypeDef]],  # (2)
    allowsHostedConnections: NotRequired[bool],
    jumboFrameCapable: NotRequired[bool],
    hasLogicalRedundancy: NotRequired[HasLogicalRedundancyType],  # (3)
    tags: NotRequired[List[TagTypeDef]],  # (4)
    providerName: NotRequired[str],
    macSecCapable: NotRequired[bool],
    encryptionMode: NotRequired[str],
    macSecKeys: NotRequired[List[MacSecKeyTypeDef]],  # (5)
```

1. See [:material-code-brackets: LagStateType](./literals.md#lagstatetype) 
2. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
3. See [:material-code-brackets: HasLogicalRedundancyType](./literals.md#haslogicalredundancytype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: MacSecKeyTypeDef](./type_defs.md#macseckeytypedef) 
## CreateDirectConnectGatewayAssociationProposalResultTypeDef

```python
# CreateDirectConnectGatewayAssociationProposalResultTypeDef definition

class CreateDirectConnectGatewayAssociationProposalResultTypeDef(TypedDict):
    directConnectGatewayAssociationProposal: DirectConnectGatewayAssociationProposalTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectConnectGatewayAssociationProposalTypeDef](./type_defs.md#directconnectgatewayassociationproposaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDirectConnectGatewayAssociationProposalResultTypeDef

```python
# DeleteDirectConnectGatewayAssociationProposalResultTypeDef definition

class DeleteDirectConnectGatewayAssociationProposalResultTypeDef(TypedDict):
    directConnectGatewayAssociationProposal: DirectConnectGatewayAssociationProposalTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectConnectGatewayAssociationProposalTypeDef](./type_defs.md#directconnectgatewayassociationproposaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDirectConnectGatewayAssociationProposalsResultTypeDef

```python
# DescribeDirectConnectGatewayAssociationProposalsResultTypeDef definition

class DescribeDirectConnectGatewayAssociationProposalsResultTypeDef(TypedDict):
    directConnectGatewayAssociationProposals: List[DirectConnectGatewayAssociationProposalTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DirectConnectGatewayAssociationProposalTypeDef](./type_defs.md#directconnectgatewayassociationproposaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcceptDirectConnectGatewayAssociationProposalResultTypeDef

```python
# AcceptDirectConnectGatewayAssociationProposalResultTypeDef definition

class AcceptDirectConnectGatewayAssociationProposalResultTypeDef(TypedDict):
    directConnectGatewayAssociation: DirectConnectGatewayAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectConnectGatewayAssociationTypeDef](./type_defs.md#directconnectgatewayassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDirectConnectGatewayAssociationResultTypeDef

```python
# CreateDirectConnectGatewayAssociationResultTypeDef definition

class CreateDirectConnectGatewayAssociationResultTypeDef(TypedDict):
    directConnectGatewayAssociation: DirectConnectGatewayAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectConnectGatewayAssociationTypeDef](./type_defs.md#directconnectgatewayassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDirectConnectGatewayAssociationResultTypeDef

```python
# DeleteDirectConnectGatewayAssociationResultTypeDef definition

class DeleteDirectConnectGatewayAssociationResultTypeDef(TypedDict):
    directConnectGatewayAssociation: DirectConnectGatewayAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectConnectGatewayAssociationTypeDef](./type_defs.md#directconnectgatewayassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDirectConnectGatewayAssociationsResultTypeDef

```python
# DescribeDirectConnectGatewayAssociationsResultTypeDef definition

class DescribeDirectConnectGatewayAssociationsResultTypeDef(TypedDict):
    directConnectGatewayAssociations: List[DirectConnectGatewayAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DirectConnectGatewayAssociationTypeDef](./type_defs.md#directconnectgatewayassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDirectConnectGatewayAssociationResultTypeDef

```python
# UpdateDirectConnectGatewayAssociationResultTypeDef definition

class UpdateDirectConnectGatewayAssociationResultTypeDef(TypedDict):
    directConnectGatewayAssociation: DirectConnectGatewayAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectConnectGatewayAssociationTypeDef](./type_defs.md#directconnectgatewayassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AllocateTransitVirtualInterfaceResultTypeDef

```python
# AllocateTransitVirtualInterfaceResultTypeDef definition

class AllocateTransitVirtualInterfaceResultTypeDef(TypedDict):
    virtualInterface: VirtualInterfaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualInterfaceTypeDef](./type_defs.md#virtualinterfacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBGPPeerResponseTypeDef

```python
# CreateBGPPeerResponseTypeDef definition

class CreateBGPPeerResponseTypeDef(TypedDict):
    virtualInterface: VirtualInterfaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualInterfaceTypeDef](./type_defs.md#virtualinterfacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTransitVirtualInterfaceResultTypeDef

```python
# CreateTransitVirtualInterfaceResultTypeDef definition

class CreateTransitVirtualInterfaceResultTypeDef(TypedDict):
    virtualInterface: VirtualInterfaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualInterfaceTypeDef](./type_defs.md#virtualinterfacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBGPPeerResponseTypeDef

```python
# DeleteBGPPeerResponseTypeDef definition

class DeleteBGPPeerResponseTypeDef(TypedDict):
    virtualInterface: VirtualInterfaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualInterfaceTypeDef](./type_defs.md#virtualinterfacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VirtualInterfacesTypeDef

```python
# VirtualInterfacesTypeDef definition

class VirtualInterfacesTypeDef(TypedDict):
    virtualInterfaces: List[VirtualInterfaceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualInterfaceTypeDef](./type_defs.md#virtualinterfacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LagsTypeDef

```python
# LagsTypeDef definition

class LagsTypeDef(TypedDict):
    lags: List[LagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LagTypeDef](./type_defs.md#lagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
