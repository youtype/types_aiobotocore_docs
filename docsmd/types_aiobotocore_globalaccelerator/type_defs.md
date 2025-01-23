# Type definitions

> [Index](../README.md) > [GlobalAccelerator](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [GlobalAccelerator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#globalaccelerator)
    type annotations stubs module [types-aiobotocore-globalaccelerator](https://pypi.org/project/types-aiobotocore-globalaccelerator/).



## AcceleratorAttributesTypeDef

```python
# AcceleratorAttributesTypeDef definition

class AcceleratorAttributesTypeDef(TypedDict):
    FlowLogsEnabled: NotRequired[bool],
    FlowLogsS3Bucket: NotRequired[str],
    FlowLogsS3Prefix: NotRequired[str],
```

## AcceleratorEventTypeDef

```python
# AcceleratorEventTypeDef definition

class AcceleratorEventTypeDef(TypedDict):
    Message: NotRequired[str],
    Timestamp: NotRequired[datetime],
```

## IpSetTypeDef

```python
# IpSetTypeDef definition

class IpSetTypeDef(TypedDict):
    IpFamily: NotRequired[str],
    IpAddresses: NotRequired[List[str]],
    IpAddressFamily: NotRequired[IpAddressFamilyType],  # (1)
```

1. See [:material-code-brackets: IpAddressFamilyType](./literals.md#ipaddressfamilytype) 
## CustomRoutingEndpointConfigurationTypeDef

```python
# CustomRoutingEndpointConfigurationTypeDef definition

class CustomRoutingEndpointConfigurationTypeDef(TypedDict):
    EndpointId: NotRequired[str],
    AttachmentArn: NotRequired[str],
```

## CustomRoutingEndpointDescriptionTypeDef

```python
# CustomRoutingEndpointDescriptionTypeDef definition

class CustomRoutingEndpointDescriptionTypeDef(TypedDict):
    EndpointId: NotRequired[str],
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

## EndpointConfigurationTypeDef

```python
# EndpointConfigurationTypeDef definition

class EndpointConfigurationTypeDef(TypedDict):
    EndpointId: NotRequired[str],
    Weight: NotRequired[int],
    ClientIPPreservationEnabled: NotRequired[bool],
    AttachmentArn: NotRequired[str],
```

## EndpointDescriptionTypeDef

```python
# EndpointDescriptionTypeDef definition

class EndpointDescriptionTypeDef(TypedDict):
    EndpointId: NotRequired[str],
    Weight: NotRequired[int],
    HealthState: NotRequired[HealthStateType],  # (1)
    HealthReason: NotRequired[str],
    ClientIPPreservationEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: HealthStateType](./literals.md#healthstatetype) 
## AdvertiseByoipCidrRequestRequestTypeDef

```python
# AdvertiseByoipCidrRequestRequestTypeDef definition

class AdvertiseByoipCidrRequestRequestTypeDef(TypedDict):
    Cidr: str,
```

## AllowCustomRoutingTrafficRequestRequestTypeDef

```python
# AllowCustomRoutingTrafficRequestRequestTypeDef definition

class AllowCustomRoutingTrafficRequestRequestTypeDef(TypedDict):
    EndpointGroupArn: str,
    EndpointId: str,
    DestinationAddresses: NotRequired[Sequence[str]],
    DestinationPorts: NotRequired[Sequence[int]],
    AllowAllTrafficToEndpoint: NotRequired[bool],
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    EndpointId: NotRequired[str],
    Cidr: NotRequired[str],
    Region: NotRequired[str],
```

## ByoipCidrEventTypeDef

```python
# ByoipCidrEventTypeDef definition

class ByoipCidrEventTypeDef(TypedDict):
    Message: NotRequired[str],
    Timestamp: NotRequired[datetime],
```

## CidrAuthorizationContextTypeDef

```python
# CidrAuthorizationContextTypeDef definition

class CidrAuthorizationContextTypeDef(TypedDict):
    Message: str,
    Signature: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CustomRoutingDestinationConfigurationTypeDef

```python
# CustomRoutingDestinationConfigurationTypeDef definition

class CustomRoutingDestinationConfigurationTypeDef(TypedDict):
    FromPort: int,
    ToPort: int,
    Protocols: Sequence[CustomRoutingProtocolType],  # (1)
```

1. See [:material-code-brackets: CustomRoutingProtocolType](./literals.md#customroutingprotocoltype) 
## PortRangeTypeDef

```python
# PortRangeTypeDef definition

class PortRangeTypeDef(TypedDict):
    FromPort: NotRequired[int],
    ToPort: NotRequired[int],
```

## PortOverrideTypeDef

```python
# PortOverrideTypeDef definition

class PortOverrideTypeDef(TypedDict):
    ListenerPort: NotRequired[int],
    EndpointPort: NotRequired[int],
```

## CrossAccountResourceTypeDef

```python
# CrossAccountResourceTypeDef definition

class CrossAccountResourceTypeDef(TypedDict):
    EndpointId: NotRequired[str],
    Cidr: NotRequired[str],
    AttachmentArn: NotRequired[str],
```

## CustomRoutingAcceleratorAttributesTypeDef

```python
# CustomRoutingAcceleratorAttributesTypeDef definition

class CustomRoutingAcceleratorAttributesTypeDef(TypedDict):
    FlowLogsEnabled: NotRequired[bool],
    FlowLogsS3Bucket: NotRequired[str],
    FlowLogsS3Prefix: NotRequired[str],
```

## CustomRoutingDestinationDescriptionTypeDef

```python
# CustomRoutingDestinationDescriptionTypeDef definition

class CustomRoutingDestinationDescriptionTypeDef(TypedDict):
    FromPort: NotRequired[int],
    ToPort: NotRequired[int],
    Protocols: NotRequired[List[ProtocolType]],  # (1)
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## DeleteAcceleratorRequestRequestTypeDef

```python
# DeleteAcceleratorRequestRequestTypeDef definition

class DeleteAcceleratorRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
```

## DeleteCrossAccountAttachmentRequestRequestTypeDef

```python
# DeleteCrossAccountAttachmentRequestRequestTypeDef definition

class DeleteCrossAccountAttachmentRequestRequestTypeDef(TypedDict):
    AttachmentArn: str,
```

## DeleteCustomRoutingAcceleratorRequestRequestTypeDef

```python
# DeleteCustomRoutingAcceleratorRequestRequestTypeDef definition

class DeleteCustomRoutingAcceleratorRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
```

## DeleteCustomRoutingEndpointGroupRequestRequestTypeDef

```python
# DeleteCustomRoutingEndpointGroupRequestRequestTypeDef definition

class DeleteCustomRoutingEndpointGroupRequestRequestTypeDef(TypedDict):
    EndpointGroupArn: str,
```

## DeleteCustomRoutingListenerRequestRequestTypeDef

```python
# DeleteCustomRoutingListenerRequestRequestTypeDef definition

class DeleteCustomRoutingListenerRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
```

## DeleteEndpointGroupRequestRequestTypeDef

```python
# DeleteEndpointGroupRequestRequestTypeDef definition

class DeleteEndpointGroupRequestRequestTypeDef(TypedDict):
    EndpointGroupArn: str,
```

## DeleteListenerRequestRequestTypeDef

```python
# DeleteListenerRequestRequestTypeDef definition

class DeleteListenerRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
```

## DenyCustomRoutingTrafficRequestRequestTypeDef

```python
# DenyCustomRoutingTrafficRequestRequestTypeDef definition

class DenyCustomRoutingTrafficRequestRequestTypeDef(TypedDict):
    EndpointGroupArn: str,
    EndpointId: str,
    DestinationAddresses: NotRequired[Sequence[str]],
    DestinationPorts: NotRequired[Sequence[int]],
    DenyAllTrafficToEndpoint: NotRequired[bool],
```

## DeprovisionByoipCidrRequestRequestTypeDef

```python
# DeprovisionByoipCidrRequestRequestTypeDef definition

class DeprovisionByoipCidrRequestRequestTypeDef(TypedDict):
    Cidr: str,
```

## DescribeAcceleratorAttributesRequestRequestTypeDef

```python
# DescribeAcceleratorAttributesRequestRequestTypeDef definition

class DescribeAcceleratorAttributesRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
```

## DescribeAcceleratorRequestRequestTypeDef

```python
# DescribeAcceleratorRequestRequestTypeDef definition

class DescribeAcceleratorRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
```

## DescribeCrossAccountAttachmentRequestRequestTypeDef

```python
# DescribeCrossAccountAttachmentRequestRequestTypeDef definition

class DescribeCrossAccountAttachmentRequestRequestTypeDef(TypedDict):
    AttachmentArn: str,
```

## DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef

```python
# DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef definition

class DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
```

## DescribeCustomRoutingAcceleratorRequestRequestTypeDef

```python
# DescribeCustomRoutingAcceleratorRequestRequestTypeDef definition

class DescribeCustomRoutingAcceleratorRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
```

## DescribeCustomRoutingEndpointGroupRequestRequestTypeDef

```python
# DescribeCustomRoutingEndpointGroupRequestRequestTypeDef definition

class DescribeCustomRoutingEndpointGroupRequestRequestTypeDef(TypedDict):
    EndpointGroupArn: str,
```

## DescribeCustomRoutingListenerRequestRequestTypeDef

```python
# DescribeCustomRoutingListenerRequestRequestTypeDef definition

class DescribeCustomRoutingListenerRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
```

## DescribeEndpointGroupRequestRequestTypeDef

```python
# DescribeEndpointGroupRequestRequestTypeDef definition

class DescribeEndpointGroupRequestRequestTypeDef(TypedDict):
    EndpointGroupArn: str,
```

## DescribeListenerRequestRequestTypeDef

```python
# DescribeListenerRequestRequestTypeDef definition

class DescribeListenerRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
```

## SocketAddressTypeDef

```python
# SocketAddressTypeDef definition

class SocketAddressTypeDef(TypedDict):
    IpAddress: NotRequired[str],
    Port: NotRequired[int],
```

## EndpointIdentifierTypeDef

```python
# EndpointIdentifierTypeDef definition

class EndpointIdentifierTypeDef(TypedDict):
    EndpointId: str,
    ClientIPPreservationEnabled: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAcceleratorsRequestRequestTypeDef

```python
# ListAcceleratorsRequestRequestTypeDef definition

class ListAcceleratorsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListByoipCidrsRequestRequestTypeDef

```python
# ListByoipCidrsRequestRequestTypeDef definition

class ListByoipCidrsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCrossAccountAttachmentsRequestRequestTypeDef

```python
# ListCrossAccountAttachmentsRequestRequestTypeDef definition

class ListCrossAccountAttachmentsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCrossAccountResourcesRequestRequestTypeDef

```python
# ListCrossAccountResourcesRequestRequestTypeDef definition

class ListCrossAccountResourcesRequestRequestTypeDef(TypedDict):
    ResourceOwnerAwsAccountId: str,
    AcceleratorArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCustomRoutingAcceleratorsRequestRequestTypeDef

```python
# ListCustomRoutingAcceleratorsRequestRequestTypeDef definition

class ListCustomRoutingAcceleratorsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCustomRoutingEndpointGroupsRequestRequestTypeDef

```python
# ListCustomRoutingEndpointGroupsRequestRequestTypeDef definition

class ListCustomRoutingEndpointGroupsRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCustomRoutingListenersRequestRequestTypeDef

```python
# ListCustomRoutingListenersRequestRequestTypeDef definition

class ListCustomRoutingListenersRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef

```python
# ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef definition

class ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef(TypedDict):
    EndpointId: str,
    DestinationAddress: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCustomRoutingPortMappingsRequestRequestTypeDef

```python
# ListCustomRoutingPortMappingsRequestRequestTypeDef definition

class ListCustomRoutingPortMappingsRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
    EndpointGroupArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEndpointGroupsRequestRequestTypeDef

```python
# ListEndpointGroupsRequestRequestTypeDef definition

class ListEndpointGroupsRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListListenersRequestRequestTypeDef

```python
# ListListenersRequestRequestTypeDef definition

class ListListenersRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## RemoveCustomRoutingEndpointsRequestRequestTypeDef

```python
# RemoveCustomRoutingEndpointsRequestRequestTypeDef definition

class RemoveCustomRoutingEndpointsRequestRequestTypeDef(TypedDict):
    EndpointIds: Sequence[str],
    EndpointGroupArn: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateAcceleratorAttributesRequestRequestTypeDef

```python
# UpdateAcceleratorAttributesRequestRequestTypeDef definition

class UpdateAcceleratorAttributesRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
    FlowLogsEnabled: NotRequired[bool],
    FlowLogsS3Bucket: NotRequired[str],
    FlowLogsS3Prefix: NotRequired[str],
```

## UpdateAcceleratorRequestRequestTypeDef

```python
# UpdateAcceleratorRequestRequestTypeDef definition

class UpdateAcceleratorRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
    Name: NotRequired[str],
    IpAddressType: NotRequired[IpAddressTypeType],  # (1)
    IpAddresses: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef

```python
# UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef definition

class UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
    FlowLogsEnabled: NotRequired[bool],
    FlowLogsS3Bucket: NotRequired[str],
    FlowLogsS3Prefix: NotRequired[str],
```

## UpdateCustomRoutingAcceleratorRequestRequestTypeDef

```python
# UpdateCustomRoutingAcceleratorRequestRequestTypeDef definition

class UpdateCustomRoutingAcceleratorRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
    Name: NotRequired[str],
    IpAddressType: NotRequired[IpAddressTypeType],  # (1)
    IpAddresses: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## WithdrawByoipCidrRequestRequestTypeDef

```python
# WithdrawByoipCidrRequestRequestTypeDef definition

class WithdrawByoipCidrRequestRequestTypeDef(TypedDict):
    Cidr: str,
```

## AcceleratorTypeDef

```python
# AcceleratorTypeDef definition

class AcceleratorTypeDef(TypedDict):
    AcceleratorArn: NotRequired[str],
    Name: NotRequired[str],
    IpAddressType: NotRequired[IpAddressTypeType],  # (1)
    Enabled: NotRequired[bool],
    IpSets: NotRequired[List[IpSetTypeDef]],  # (2)
    DnsName: NotRequired[str],
    Status: NotRequired[AcceleratorStatusType],  # (3)
    CreatedTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    DualStackDnsName: NotRequired[str],
    Events: NotRequired[List[AcceleratorEventTypeDef]],  # (4)
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
2. See [:material-code-braces: IpSetTypeDef](./type_defs.md#ipsettypedef) 
3. See [:material-code-brackets: AcceleratorStatusType](./literals.md#acceleratorstatustype) 
4. See [:material-code-braces: AcceleratorEventTypeDef](./type_defs.md#acceleratoreventtypedef) 
## CustomRoutingAcceleratorTypeDef

```python
# CustomRoutingAcceleratorTypeDef definition

class CustomRoutingAcceleratorTypeDef(TypedDict):
    AcceleratorArn: NotRequired[str],
    Name: NotRequired[str],
    IpAddressType: NotRequired[IpAddressTypeType],  # (1)
    Enabled: NotRequired[bool],
    IpSets: NotRequired[List[IpSetTypeDef]],  # (2)
    DnsName: NotRequired[str],
    Status: NotRequired[CustomRoutingAcceleratorStatusType],  # (3)
    CreatedTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
2. See [:material-code-braces: IpSetTypeDef](./type_defs.md#ipsettypedef) 
3. See [:material-code-brackets: CustomRoutingAcceleratorStatusType](./literals.md#customroutingacceleratorstatustype) 
## AddCustomRoutingEndpointsRequestRequestTypeDef

```python
# AddCustomRoutingEndpointsRequestRequestTypeDef definition

class AddCustomRoutingEndpointsRequestRequestTypeDef(TypedDict):
    EndpointConfigurations: Sequence[CustomRoutingEndpointConfigurationTypeDef],  # (1)
    EndpointGroupArn: str,
```

1. See [:material-code-braces: CustomRoutingEndpointConfigurationTypeDef](./type_defs.md#customroutingendpointconfigurationtypedef) 
## AddCustomRoutingEndpointsResponseTypeDef

```python
# AddCustomRoutingEndpointsResponseTypeDef definition

class AddCustomRoutingEndpointsResponseTypeDef(TypedDict):
    EndpointDescriptions: List[CustomRoutingEndpointDescriptionTypeDef],  # (1)
    EndpointGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingEndpointDescriptionTypeDef](./type_defs.md#customroutingendpointdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAcceleratorAttributesResponseTypeDef

```python
# DescribeAcceleratorAttributesResponseTypeDef definition

class DescribeAcceleratorAttributesResponseTypeDef(TypedDict):
    AcceleratorAttributes: AcceleratorAttributesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AcceleratorAttributesTypeDef](./type_defs.md#acceleratorattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCrossAccountResourceAccountsResponseTypeDef

```python
# ListCrossAccountResourceAccountsResponseTypeDef definition

class ListCrossAccountResourceAccountsResponseTypeDef(TypedDict):
    ResourceOwnerAwsAccountIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAcceleratorAttributesResponseTypeDef

```python
# UpdateAcceleratorAttributesResponseTypeDef definition

class UpdateAcceleratorAttributesResponseTypeDef(TypedDict):
    AcceleratorAttributes: AcceleratorAttributesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AcceleratorAttributesTypeDef](./type_defs.md#acceleratorattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddEndpointsRequestRequestTypeDef

```python
# AddEndpointsRequestRequestTypeDef definition

class AddEndpointsRequestRequestTypeDef(TypedDict):
    EndpointConfigurations: Sequence[EndpointConfigurationTypeDef],  # (1)
    EndpointGroupArn: str,
```

1. See [:material-code-braces: EndpointConfigurationTypeDef](./type_defs.md#endpointconfigurationtypedef) 
## AddEndpointsResponseTypeDef

```python
# AddEndpointsResponseTypeDef definition

class AddEndpointsResponseTypeDef(TypedDict):
    EndpointDescriptions: List[EndpointDescriptionTypeDef],  # (1)
    EndpointGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointDescriptionTypeDef](./type_defs.md#endpointdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachmentTypeDef

```python
# AttachmentTypeDef definition

class AttachmentTypeDef(TypedDict):
    AttachmentArn: NotRequired[str],
    Name: NotRequired[str],
    Principals: NotRequired[List[str]],
    Resources: NotRequired[List[ResourceTypeDef]],  # (1)
    LastModifiedTime: NotRequired[datetime],
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## UpdateCrossAccountAttachmentRequestRequestTypeDef

```python
# UpdateCrossAccountAttachmentRequestRequestTypeDef definition

class UpdateCrossAccountAttachmentRequestRequestTypeDef(TypedDict):
    AttachmentArn: str,
    Name: NotRequired[str],
    AddPrincipals: NotRequired[Sequence[str]],
    RemovePrincipals: NotRequired[Sequence[str]],
    AddResources: NotRequired[Sequence[ResourceTypeDef]],  # (1)
    RemoveResources: NotRequired[Sequence[ResourceTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## ByoipCidrTypeDef

```python
# ByoipCidrTypeDef definition

class ByoipCidrTypeDef(TypedDict):
    Cidr: NotRequired[str],
    State: NotRequired[ByoipCidrStateType],  # (1)
    Events: NotRequired[List[ByoipCidrEventTypeDef]],  # (2)
```

1. See [:material-code-brackets: ByoipCidrStateType](./literals.md#byoipcidrstatetype) 
2. See [:material-code-braces: ByoipCidrEventTypeDef](./type_defs.md#byoipcidreventtypedef) 
## ProvisionByoipCidrRequestRequestTypeDef

```python
# ProvisionByoipCidrRequestRequestTypeDef definition

class ProvisionByoipCidrRequestRequestTypeDef(TypedDict):
    Cidr: str,
    CidrAuthorizationContext: CidrAuthorizationContextTypeDef,  # (1)
```

1. See [:material-code-braces: CidrAuthorizationContextTypeDef](./type_defs.md#cidrauthorizationcontexttypedef) 
## CreateAcceleratorRequestRequestTypeDef

```python
# CreateAcceleratorRequestRequestTypeDef definition

class CreateAcceleratorRequestRequestTypeDef(TypedDict):
    Name: str,
    IdempotencyToken: str,
    IpAddressType: NotRequired[IpAddressTypeType],  # (1)
    IpAddresses: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCrossAccountAttachmentRequestRequestTypeDef

```python
# CreateCrossAccountAttachmentRequestRequestTypeDef definition

class CreateCrossAccountAttachmentRequestRequestTypeDef(TypedDict):
    Name: str,
    IdempotencyToken: str,
    Principals: NotRequired[Sequence[str]],
    Resources: NotRequired[Sequence[ResourceTypeDef]],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCustomRoutingAcceleratorRequestRequestTypeDef

```python
# CreateCustomRoutingAcceleratorRequestRequestTypeDef definition

class CreateCustomRoutingAcceleratorRequestRequestTypeDef(TypedDict):
    Name: str,
    IdempotencyToken: str,
    IpAddressType: NotRequired[IpAddressTypeType],  # (1)
    IpAddresses: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCustomRoutingEndpointGroupRequestRequestTypeDef

```python
# CreateCustomRoutingEndpointGroupRequestRequestTypeDef definition

class CreateCustomRoutingEndpointGroupRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
    EndpointGroupRegion: str,
    DestinationConfigurations: Sequence[CustomRoutingDestinationConfigurationTypeDef],  # (1)
    IdempotencyToken: str,
```

1. See [:material-code-braces: CustomRoutingDestinationConfigurationTypeDef](./type_defs.md#customroutingdestinationconfigurationtypedef) 
## CreateCustomRoutingListenerRequestRequestTypeDef

```python
# CreateCustomRoutingListenerRequestRequestTypeDef definition

class CreateCustomRoutingListenerRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
    PortRanges: Sequence[PortRangeTypeDef],  # (1)
    IdempotencyToken: str,
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## CreateListenerRequestRequestTypeDef

```python
# CreateListenerRequestRequestTypeDef definition

class CreateListenerRequestRequestTypeDef(TypedDict):
    AcceleratorArn: str,
    PortRanges: Sequence[PortRangeTypeDef],  # (1)
    Protocol: ProtocolType,  # (2)
    IdempotencyToken: str,
    ClientAffinity: NotRequired[ClientAffinityType],  # (3)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
3. See [:material-code-brackets: ClientAffinityType](./literals.md#clientaffinitytype) 
## CustomRoutingListenerTypeDef

```python
# CustomRoutingListenerTypeDef definition

class CustomRoutingListenerTypeDef(TypedDict):
    ListenerArn: NotRequired[str],
    PortRanges: NotRequired[List[PortRangeTypeDef]],  # (1)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## ListenerTypeDef

```python
# ListenerTypeDef definition

class ListenerTypeDef(TypedDict):
    ListenerArn: NotRequired[str],
    PortRanges: NotRequired[List[PortRangeTypeDef]],  # (1)
    Protocol: NotRequired[ProtocolType],  # (2)
    ClientAffinity: NotRequired[ClientAffinityType],  # (3)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
3. See [:material-code-brackets: ClientAffinityType](./literals.md#clientaffinitytype) 
## UpdateCustomRoutingListenerRequestRequestTypeDef

```python
# UpdateCustomRoutingListenerRequestRequestTypeDef definition

class UpdateCustomRoutingListenerRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
    PortRanges: Sequence[PortRangeTypeDef],  # (1)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## UpdateListenerRequestRequestTypeDef

```python
# UpdateListenerRequestRequestTypeDef definition

class UpdateListenerRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
    PortRanges: NotRequired[Sequence[PortRangeTypeDef]],  # (1)
    Protocol: NotRequired[ProtocolType],  # (2)
    ClientAffinity: NotRequired[ClientAffinityType],  # (3)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
3. See [:material-code-brackets: ClientAffinityType](./literals.md#clientaffinitytype) 
## CreateEndpointGroupRequestRequestTypeDef

```python
# CreateEndpointGroupRequestRequestTypeDef definition

class CreateEndpointGroupRequestRequestTypeDef(TypedDict):
    ListenerArn: str,
    EndpointGroupRegion: str,
    IdempotencyToken: str,
    EndpointConfigurations: NotRequired[Sequence[EndpointConfigurationTypeDef]],  # (1)
    TrafficDialPercentage: NotRequired[float],
    HealthCheckPort: NotRequired[int],
    HealthCheckProtocol: NotRequired[HealthCheckProtocolType],  # (2)
    HealthCheckPath: NotRequired[str],
    HealthCheckIntervalSeconds: NotRequired[int],
    ThresholdCount: NotRequired[int],
    PortOverrides: NotRequired[Sequence[PortOverrideTypeDef]],  # (3)
```

1. See [:material-code-braces: EndpointConfigurationTypeDef](./type_defs.md#endpointconfigurationtypedef) 
2. See [:material-code-brackets: HealthCheckProtocolType](./literals.md#healthcheckprotocoltype) 
3. See [:material-code-braces: PortOverrideTypeDef](./type_defs.md#portoverridetypedef) 
## EndpointGroupTypeDef

```python
# EndpointGroupTypeDef definition

class EndpointGroupTypeDef(TypedDict):
    EndpointGroupArn: NotRequired[str],
    EndpointGroupRegion: NotRequired[str],
    EndpointDescriptions: NotRequired[List[EndpointDescriptionTypeDef]],  # (1)
    TrafficDialPercentage: NotRequired[float],
    HealthCheckPort: NotRequired[int],
    HealthCheckProtocol: NotRequired[HealthCheckProtocolType],  # (2)
    HealthCheckPath: NotRequired[str],
    HealthCheckIntervalSeconds: NotRequired[int],
    ThresholdCount: NotRequired[int],
    PortOverrides: NotRequired[List[PortOverrideTypeDef]],  # (3)
```

1. See [:material-code-braces: EndpointDescriptionTypeDef](./type_defs.md#endpointdescriptiontypedef) 
2. See [:material-code-brackets: HealthCheckProtocolType](./literals.md#healthcheckprotocoltype) 
3. See [:material-code-braces: PortOverrideTypeDef](./type_defs.md#portoverridetypedef) 
## UpdateEndpointGroupRequestRequestTypeDef

```python
# UpdateEndpointGroupRequestRequestTypeDef definition

class UpdateEndpointGroupRequestRequestTypeDef(TypedDict):
    EndpointGroupArn: str,
    EndpointConfigurations: NotRequired[Sequence[EndpointConfigurationTypeDef]],  # (1)
    TrafficDialPercentage: NotRequired[float],
    HealthCheckPort: NotRequired[int],
    HealthCheckProtocol: NotRequired[HealthCheckProtocolType],  # (2)
    HealthCheckPath: NotRequired[str],
    HealthCheckIntervalSeconds: NotRequired[int],
    ThresholdCount: NotRequired[int],
    PortOverrides: NotRequired[Sequence[PortOverrideTypeDef]],  # (3)
```

1. See [:material-code-braces: EndpointConfigurationTypeDef](./type_defs.md#endpointconfigurationtypedef) 
2. See [:material-code-brackets: HealthCheckProtocolType](./literals.md#healthcheckprotocoltype) 
3. See [:material-code-braces: PortOverrideTypeDef](./type_defs.md#portoverridetypedef) 
## ListCrossAccountResourcesResponseTypeDef

```python
# ListCrossAccountResourcesResponseTypeDef definition

class ListCrossAccountResourcesResponseTypeDef(TypedDict):
    CrossAccountResources: List[CrossAccountResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CrossAccountResourceTypeDef](./type_defs.md#crossaccountresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCustomRoutingAcceleratorAttributesResponseTypeDef

```python
# DescribeCustomRoutingAcceleratorAttributesResponseTypeDef definition

class DescribeCustomRoutingAcceleratorAttributesResponseTypeDef(TypedDict):
    AcceleratorAttributes: CustomRoutingAcceleratorAttributesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingAcceleratorAttributesTypeDef](./type_defs.md#customroutingacceleratorattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCustomRoutingAcceleratorAttributesResponseTypeDef

```python
# UpdateCustomRoutingAcceleratorAttributesResponseTypeDef definition

class UpdateCustomRoutingAcceleratorAttributesResponseTypeDef(TypedDict):
    AcceleratorAttributes: CustomRoutingAcceleratorAttributesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingAcceleratorAttributesTypeDef](./type_defs.md#customroutingacceleratorattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomRoutingEndpointGroupTypeDef

```python
# CustomRoutingEndpointGroupTypeDef definition

class CustomRoutingEndpointGroupTypeDef(TypedDict):
    EndpointGroupArn: NotRequired[str],
    EndpointGroupRegion: NotRequired[str],
    DestinationDescriptions: NotRequired[List[CustomRoutingDestinationDescriptionTypeDef]],  # (1)
    EndpointDescriptions: NotRequired[List[CustomRoutingEndpointDescriptionTypeDef]],  # (2)
```

1. See [:material-code-braces: CustomRoutingDestinationDescriptionTypeDef](./type_defs.md#customroutingdestinationdescriptiontypedef) 
2. See [:material-code-braces: CustomRoutingEndpointDescriptionTypeDef](./type_defs.md#customroutingendpointdescriptiontypedef) 
## DestinationPortMappingTypeDef

```python
# DestinationPortMappingTypeDef definition

class DestinationPortMappingTypeDef(TypedDict):
    AcceleratorArn: NotRequired[str],
    AcceleratorSocketAddresses: NotRequired[List[SocketAddressTypeDef]],  # (1)
    EndpointGroupArn: NotRequired[str],
    EndpointId: NotRequired[str],
    EndpointGroupRegion: NotRequired[str],
    DestinationSocketAddress: NotRequired[SocketAddressTypeDef],  # (2)
    IpAddressType: NotRequired[IpAddressTypeType],  # (3)
    DestinationTrafficState: NotRequired[CustomRoutingDestinationTrafficStateType],  # (4)
```

1. See [:material-code-braces: SocketAddressTypeDef](./type_defs.md#socketaddresstypedef) 
2. See [:material-code-braces: SocketAddressTypeDef](./type_defs.md#socketaddresstypedef) 
3. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
4. See [:material-code-brackets: CustomRoutingDestinationTrafficStateType](./literals.md#customroutingdestinationtrafficstatetype) 
## PortMappingTypeDef

```python
# PortMappingTypeDef definition

class PortMappingTypeDef(TypedDict):
    AcceleratorPort: NotRequired[int],
    EndpointGroupArn: NotRequired[str],
    EndpointId: NotRequired[str],
    DestinationSocketAddress: NotRequired[SocketAddressTypeDef],  # (1)
    Protocols: NotRequired[List[CustomRoutingProtocolType]],  # (2)
    DestinationTrafficState: NotRequired[CustomRoutingDestinationTrafficStateType],  # (3)
```

1. See [:material-code-braces: SocketAddressTypeDef](./type_defs.md#socketaddresstypedef) 
2. See [:material-code-brackets: CustomRoutingProtocolType](./literals.md#customroutingprotocoltype) 
3. See [:material-code-brackets: CustomRoutingDestinationTrafficStateType](./literals.md#customroutingdestinationtrafficstatetype) 
## RemoveEndpointsRequestRequestTypeDef

```python
# RemoveEndpointsRequestRequestTypeDef definition

class RemoveEndpointsRequestRequestTypeDef(TypedDict):
    EndpointIdentifiers: Sequence[EndpointIdentifierTypeDef],  # (1)
    EndpointGroupArn: str,
```

1. See [:material-code-braces: EndpointIdentifierTypeDef](./type_defs.md#endpointidentifiertypedef) 
## ListAcceleratorsRequestPaginateTypeDef

```python
# ListAcceleratorsRequestPaginateTypeDef definition

class ListAcceleratorsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListByoipCidrsRequestPaginateTypeDef

```python
# ListByoipCidrsRequestPaginateTypeDef definition

class ListByoipCidrsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCrossAccountAttachmentsRequestPaginateTypeDef

```python
# ListCrossAccountAttachmentsRequestPaginateTypeDef definition

class ListCrossAccountAttachmentsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCrossAccountResourcesRequestPaginateTypeDef

```python
# ListCrossAccountResourcesRequestPaginateTypeDef definition

class ListCrossAccountResourcesRequestPaginateTypeDef(TypedDict):
    ResourceOwnerAwsAccountId: str,
    AcceleratorArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomRoutingAcceleratorsRequestPaginateTypeDef

```python
# ListCustomRoutingAcceleratorsRequestPaginateTypeDef definition

class ListCustomRoutingAcceleratorsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomRoutingEndpointGroupsRequestPaginateTypeDef

```python
# ListCustomRoutingEndpointGroupsRequestPaginateTypeDef definition

class ListCustomRoutingEndpointGroupsRequestPaginateTypeDef(TypedDict):
    ListenerArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomRoutingListenersRequestPaginateTypeDef

```python
# ListCustomRoutingListenersRequestPaginateTypeDef definition

class ListCustomRoutingListenersRequestPaginateTypeDef(TypedDict):
    AcceleratorArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomRoutingPortMappingsByDestinationRequestPaginateTypeDef

```python
# ListCustomRoutingPortMappingsByDestinationRequestPaginateTypeDef definition

class ListCustomRoutingPortMappingsByDestinationRequestPaginateTypeDef(TypedDict):
    EndpointId: str,
    DestinationAddress: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomRoutingPortMappingsRequestPaginateTypeDef

```python
# ListCustomRoutingPortMappingsRequestPaginateTypeDef definition

class ListCustomRoutingPortMappingsRequestPaginateTypeDef(TypedDict):
    AcceleratorArn: str,
    EndpointGroupArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEndpointGroupsRequestPaginateTypeDef

```python
# ListEndpointGroupsRequestPaginateTypeDef definition

class ListEndpointGroupsRequestPaginateTypeDef(TypedDict):
    ListenerArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListListenersRequestPaginateTypeDef

```python
# ListListenersRequestPaginateTypeDef definition

class ListListenersRequestPaginateTypeDef(TypedDict):
    AcceleratorArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## CreateAcceleratorResponseTypeDef

```python
# CreateAcceleratorResponseTypeDef definition

class CreateAcceleratorResponseTypeDef(TypedDict):
    Accelerator: AcceleratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AcceleratorTypeDef](./type_defs.md#acceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAcceleratorResponseTypeDef

```python
# DescribeAcceleratorResponseTypeDef definition

class DescribeAcceleratorResponseTypeDef(TypedDict):
    Accelerator: AcceleratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AcceleratorTypeDef](./type_defs.md#acceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAcceleratorsResponseTypeDef

```python
# ListAcceleratorsResponseTypeDef definition

class ListAcceleratorsResponseTypeDef(TypedDict):
    Accelerators: List[AcceleratorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AcceleratorTypeDef](./type_defs.md#acceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAcceleratorResponseTypeDef

```python
# UpdateAcceleratorResponseTypeDef definition

class UpdateAcceleratorResponseTypeDef(TypedDict):
    Accelerator: AcceleratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AcceleratorTypeDef](./type_defs.md#acceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomRoutingAcceleratorResponseTypeDef

```python
# CreateCustomRoutingAcceleratorResponseTypeDef definition

class CreateCustomRoutingAcceleratorResponseTypeDef(TypedDict):
    Accelerator: CustomRoutingAcceleratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingAcceleratorTypeDef](./type_defs.md#customroutingacceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCustomRoutingAcceleratorResponseTypeDef

```python
# DescribeCustomRoutingAcceleratorResponseTypeDef definition

class DescribeCustomRoutingAcceleratorResponseTypeDef(TypedDict):
    Accelerator: CustomRoutingAcceleratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingAcceleratorTypeDef](./type_defs.md#customroutingacceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomRoutingAcceleratorsResponseTypeDef

```python
# ListCustomRoutingAcceleratorsResponseTypeDef definition

class ListCustomRoutingAcceleratorsResponseTypeDef(TypedDict):
    Accelerators: List[CustomRoutingAcceleratorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomRoutingAcceleratorTypeDef](./type_defs.md#customroutingacceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCustomRoutingAcceleratorResponseTypeDef

```python
# UpdateCustomRoutingAcceleratorResponseTypeDef definition

class UpdateCustomRoutingAcceleratorResponseTypeDef(TypedDict):
    Accelerator: CustomRoutingAcceleratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingAcceleratorTypeDef](./type_defs.md#customroutingacceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCrossAccountAttachmentResponseTypeDef

```python
# CreateCrossAccountAttachmentResponseTypeDef definition

class CreateCrossAccountAttachmentResponseTypeDef(TypedDict):
    CrossAccountAttachment: AttachmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCrossAccountAttachmentResponseTypeDef

```python
# DescribeCrossAccountAttachmentResponseTypeDef definition

class DescribeCrossAccountAttachmentResponseTypeDef(TypedDict):
    CrossAccountAttachment: AttachmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCrossAccountAttachmentsResponseTypeDef

```python
# ListCrossAccountAttachmentsResponseTypeDef definition

class ListCrossAccountAttachmentsResponseTypeDef(TypedDict):
    CrossAccountAttachments: List[AttachmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCrossAccountAttachmentResponseTypeDef

```python
# UpdateCrossAccountAttachmentResponseTypeDef definition

class UpdateCrossAccountAttachmentResponseTypeDef(TypedDict):
    CrossAccountAttachment: AttachmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdvertiseByoipCidrResponseTypeDef

```python
# AdvertiseByoipCidrResponseTypeDef definition

class AdvertiseByoipCidrResponseTypeDef(TypedDict):
    ByoipCidr: ByoipCidrTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByoipCidrTypeDef](./type_defs.md#byoipcidrtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeprovisionByoipCidrResponseTypeDef

```python
# DeprovisionByoipCidrResponseTypeDef definition

class DeprovisionByoipCidrResponseTypeDef(TypedDict):
    ByoipCidr: ByoipCidrTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByoipCidrTypeDef](./type_defs.md#byoipcidrtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListByoipCidrsResponseTypeDef

```python
# ListByoipCidrsResponseTypeDef definition

class ListByoipCidrsResponseTypeDef(TypedDict):
    ByoipCidrs: List[ByoipCidrTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ByoipCidrTypeDef](./type_defs.md#byoipcidrtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisionByoipCidrResponseTypeDef

```python
# ProvisionByoipCidrResponseTypeDef definition

class ProvisionByoipCidrResponseTypeDef(TypedDict):
    ByoipCidr: ByoipCidrTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByoipCidrTypeDef](./type_defs.md#byoipcidrtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WithdrawByoipCidrResponseTypeDef

```python
# WithdrawByoipCidrResponseTypeDef definition

class WithdrawByoipCidrResponseTypeDef(TypedDict):
    ByoipCidr: ByoipCidrTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByoipCidrTypeDef](./type_defs.md#byoipcidrtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomRoutingListenerResponseTypeDef

```python
# CreateCustomRoutingListenerResponseTypeDef definition

class CreateCustomRoutingListenerResponseTypeDef(TypedDict):
    Listener: CustomRoutingListenerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingListenerTypeDef](./type_defs.md#customroutinglistenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCustomRoutingListenerResponseTypeDef

```python
# DescribeCustomRoutingListenerResponseTypeDef definition

class DescribeCustomRoutingListenerResponseTypeDef(TypedDict):
    Listener: CustomRoutingListenerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingListenerTypeDef](./type_defs.md#customroutinglistenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomRoutingListenersResponseTypeDef

```python
# ListCustomRoutingListenersResponseTypeDef definition

class ListCustomRoutingListenersResponseTypeDef(TypedDict):
    Listeners: List[CustomRoutingListenerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomRoutingListenerTypeDef](./type_defs.md#customroutinglistenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCustomRoutingListenerResponseTypeDef

```python
# UpdateCustomRoutingListenerResponseTypeDef definition

class UpdateCustomRoutingListenerResponseTypeDef(TypedDict):
    Listener: CustomRoutingListenerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingListenerTypeDef](./type_defs.md#customroutinglistenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateListenerResponseTypeDef

```python
# CreateListenerResponseTypeDef definition

class CreateListenerResponseTypeDef(TypedDict):
    Listener: ListenerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeListenerResponseTypeDef

```python
# DescribeListenerResponseTypeDef definition

class DescribeListenerResponseTypeDef(TypedDict):
    Listener: ListenerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListListenersResponseTypeDef

```python
# ListListenersResponseTypeDef definition

class ListListenersResponseTypeDef(TypedDict):
    Listeners: List[ListenerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateListenerResponseTypeDef

```python
# UpdateListenerResponseTypeDef definition

class UpdateListenerResponseTypeDef(TypedDict):
    Listener: ListenerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEndpointGroupResponseTypeDef

```python
# CreateEndpointGroupResponseTypeDef definition

class CreateEndpointGroupResponseTypeDef(TypedDict):
    EndpointGroup: EndpointGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointGroupTypeDef](./type_defs.md#endpointgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointGroupResponseTypeDef

```python
# DescribeEndpointGroupResponseTypeDef definition

class DescribeEndpointGroupResponseTypeDef(TypedDict):
    EndpointGroup: EndpointGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointGroupTypeDef](./type_defs.md#endpointgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEndpointGroupsResponseTypeDef

```python
# ListEndpointGroupsResponseTypeDef definition

class ListEndpointGroupsResponseTypeDef(TypedDict):
    EndpointGroups: List[EndpointGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EndpointGroupTypeDef](./type_defs.md#endpointgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEndpointGroupResponseTypeDef

```python
# UpdateEndpointGroupResponseTypeDef definition

class UpdateEndpointGroupResponseTypeDef(TypedDict):
    EndpointGroup: EndpointGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointGroupTypeDef](./type_defs.md#endpointgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomRoutingEndpointGroupResponseTypeDef

```python
# CreateCustomRoutingEndpointGroupResponseTypeDef definition

class CreateCustomRoutingEndpointGroupResponseTypeDef(TypedDict):
    EndpointGroup: CustomRoutingEndpointGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingEndpointGroupTypeDef](./type_defs.md#customroutingendpointgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCustomRoutingEndpointGroupResponseTypeDef

```python
# DescribeCustomRoutingEndpointGroupResponseTypeDef definition

class DescribeCustomRoutingEndpointGroupResponseTypeDef(TypedDict):
    EndpointGroup: CustomRoutingEndpointGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomRoutingEndpointGroupTypeDef](./type_defs.md#customroutingendpointgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomRoutingEndpointGroupsResponseTypeDef

```python
# ListCustomRoutingEndpointGroupsResponseTypeDef definition

class ListCustomRoutingEndpointGroupsResponseTypeDef(TypedDict):
    EndpointGroups: List[CustomRoutingEndpointGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomRoutingEndpointGroupTypeDef](./type_defs.md#customroutingendpointgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomRoutingPortMappingsByDestinationResponseTypeDef

```python
# ListCustomRoutingPortMappingsByDestinationResponseTypeDef definition

class ListCustomRoutingPortMappingsByDestinationResponseTypeDef(TypedDict):
    DestinationPortMappings: List[DestinationPortMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DestinationPortMappingTypeDef](./type_defs.md#destinationportmappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomRoutingPortMappingsResponseTypeDef

```python
# ListCustomRoutingPortMappingsResponseTypeDef definition

class ListCustomRoutingPortMappingsResponseTypeDef(TypedDict):
    PortMappings: List[PortMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PortMappingTypeDef](./type_defs.md#portmappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
