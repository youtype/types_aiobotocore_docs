# MediaConnectClient

> [Index](../README.md) > [MediaConnect](./README.md) > MediaConnectClient

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## MediaConnectClient

Type annotations and code completion for `#!python session.create_client("mediaconnect")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client)

```python
# MediaConnectClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_mediaconnect.client import MediaConnectClient

session = get_session()
async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("mediaconnect").exceptions` structure.

```python
# MediaConnectClient.exceptions usage example

async with session.create_client("mediaconnect") as client:
    try:
        do_something(client)
    except (
            client.AddFlowOutputs420Exception,
        client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.CreateBridge420Exception,
        client.CreateFlow420Exception,
        client.CreateGateway420Exception,
        client.ForbiddenException,
        client.GrantFlowEntitlements420Exception,
        client.InternalServerErrorException,
        client.NotFoundException,
        client.ServiceUnavailableException,
        client.TooManyRequestsException,
    ) as e:
        print(e)
```

```python
# MediaConnectClient usage type checking example

from types_aiobotocore_mediaconnect.client import Exceptions

def handle_error(exc: Exceptions.AddFlowOutputs420Exception) -> None:
    ...
```


## Methods


### add\_bridge\_outputs

Adds outputs to an existing bridge.

Type annotations and code completion for `#!python session.create_client("mediaconnect").add_bridge_outputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_bridge_outputs)

```python
# add_bridge_outputs method definition

await def add_bridge_outputs(
    self,
    *,
    BridgeArn: str,
    Outputs: Sequence[AddBridgeOutputRequestTypeDef],  # (1)
) -> AddBridgeOutputsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AddBridgeOutputRequestTypeDef](./type_defs.md#addbridgeoutputrequesttypedef) 
2. See [:material-code-braces: AddBridgeOutputsResponseTypeDef](./type_defs.md#addbridgeoutputsresponsetypedef) 


```python
# add_bridge_outputs method usage example with argument unpacking

kwargs: AddBridgeOutputsRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
    "Outputs": ...,
}

parent.add_bridge_outputs(**kwargs)
```

1. See [:material-code-braces: AddBridgeOutputsRequestRequestTypeDef](./type_defs.md#addbridgeoutputsrequestrequesttypedef) 

### add\_bridge\_sources

Adds sources to an existing bridge.

Type annotations and code completion for `#!python session.create_client("mediaconnect").add_bridge_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_bridge_sources)

```python
# add_bridge_sources method definition

await def add_bridge_sources(
    self,
    *,
    BridgeArn: str,
    Sources: Sequence[AddBridgeSourceRequestTypeDef],  # (1)
) -> AddBridgeSourcesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AddBridgeSourceRequestTypeDef](./type_defs.md#addbridgesourcerequesttypedef) 
2. See [:material-code-braces: AddBridgeSourcesResponseTypeDef](./type_defs.md#addbridgesourcesresponsetypedef) 


```python
# add_bridge_sources method usage example with argument unpacking

kwargs: AddBridgeSourcesRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
    "Sources": ...,
}

parent.add_bridge_sources(**kwargs)
```

1. See [:material-code-braces: AddBridgeSourcesRequestRequestTypeDef](./type_defs.md#addbridgesourcesrequestrequesttypedef) 

### add\_flow\_media\_streams

Adds media streams to an existing flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").add_flow_media_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_flow_media_streams)

```python
# add_flow_media_streams method definition

await def add_flow_media_streams(
    self,
    *,
    FlowArn: str,
    MediaStreams: Sequence[AddMediaStreamRequestTypeDef],  # (1)
) -> AddFlowMediaStreamsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AddMediaStreamRequestTypeDef](./type_defs.md#addmediastreamrequesttypedef) 
2. See [:material-code-braces: AddFlowMediaStreamsResponseTypeDef](./type_defs.md#addflowmediastreamsresponsetypedef) 


```python
# add_flow_media_streams method usage example with argument unpacking

kwargs: AddFlowMediaStreamsRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "MediaStreams": ...,
}

parent.add_flow_media_streams(**kwargs)
```

1. See [:material-code-braces: AddFlowMediaStreamsRequestRequestTypeDef](./type_defs.md#addflowmediastreamsrequestrequesttypedef) 

### add\_flow\_outputs

Adds outputs to an existing flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").add_flow_outputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_flow_outputs)

```python
# add_flow_outputs method definition

await def add_flow_outputs(
    self,
    *,
    FlowArn: str,
    Outputs: Sequence[AddOutputRequestTypeDef],  # (1)
) -> AddFlowOutputsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AddOutputRequestTypeDef](./type_defs.md#addoutputrequesttypedef) 
2. See [:material-code-braces: AddFlowOutputsResponseTypeDef](./type_defs.md#addflowoutputsresponsetypedef) 


```python
# add_flow_outputs method usage example with argument unpacking

kwargs: AddFlowOutputsRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "Outputs": ...,
}

parent.add_flow_outputs(**kwargs)
```

1. See [:material-code-braces: AddFlowOutputsRequestRequestTypeDef](./type_defs.md#addflowoutputsrequestrequesttypedef) 

### add\_flow\_sources

Adds Sources to flow See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/AddFlowSources).

Type annotations and code completion for `#!python session.create_client("mediaconnect").add_flow_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_flow_sources)

```python
# add_flow_sources method definition

await def add_flow_sources(
    self,
    *,
    FlowArn: str,
    Sources: Sequence[SetSourceRequestTypeDef],  # (1)
) -> AddFlowSourcesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef) 
2. See [:material-code-braces: AddFlowSourcesResponseTypeDef](./type_defs.md#addflowsourcesresponsetypedef) 


```python
# add_flow_sources method usage example with argument unpacking

kwargs: AddFlowSourcesRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "Sources": ...,
}

parent.add_flow_sources(**kwargs)
```

1. See [:material-code-braces: AddFlowSourcesRequestRequestTypeDef](./type_defs.md#addflowsourcesrequestrequesttypedef) 

### add\_flow\_vpc\_interfaces

Adds VPC interfaces to flow See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/AddFlowVpcInterfaces).

Type annotations and code completion for `#!python session.create_client("mediaconnect").add_flow_vpc_interfaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_flow_vpc_interfaces)

```python
# add_flow_vpc_interfaces method definition

await def add_flow_vpc_interfaces(
    self,
    *,
    FlowArn: str,
    VpcInterfaces: Sequence[VpcInterfaceRequestTypeDef],  # (1)
) -> AddFlowVpcInterfacesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VpcInterfaceRequestTypeDef](./type_defs.md#vpcinterfacerequesttypedef) 
2. See [:material-code-braces: AddFlowVpcInterfacesResponseTypeDef](./type_defs.md#addflowvpcinterfacesresponsetypedef) 


```python
# add_flow_vpc_interfaces method usage example with argument unpacking

kwargs: AddFlowVpcInterfacesRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "VpcInterfaces": ...,
}

parent.add_flow_vpc_interfaces(**kwargs)
```

1. See [:material-code-braces: AddFlowVpcInterfacesRequestRequestTypeDef](./type_defs.md#addflowvpcinterfacesrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("mediaconnect").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("mediaconnect").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_bridge

Creates a new bridge.

Type annotations and code completion for `#!python session.create_client("mediaconnect").create_bridge` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_bridge)

```python
# create_bridge method definition

await def create_bridge(
    self,
    *,
    Name: str,
    PlacementArn: str,
    Sources: Sequence[AddBridgeSourceRequestTypeDef],  # (1)
    EgressGatewayBridge: AddEgressGatewayBridgeRequestTypeDef = ...,  # (2)
    IngressGatewayBridge: AddIngressGatewayBridgeRequestTypeDef = ...,  # (3)
    Outputs: Sequence[AddBridgeOutputRequestTypeDef] = ...,  # (4)
    SourceFailoverConfig: FailoverConfigTypeDef = ...,  # (5)
) -> CreateBridgeResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: AddBridgeSourceRequestTypeDef](./type_defs.md#addbridgesourcerequesttypedef) 
2. See [:material-code-braces: AddEgressGatewayBridgeRequestTypeDef](./type_defs.md#addegressgatewaybridgerequesttypedef) 
3. See [:material-code-braces: AddIngressGatewayBridgeRequestTypeDef](./type_defs.md#addingressgatewaybridgerequesttypedef) 
4. See [:material-code-braces: AddBridgeOutputRequestTypeDef](./type_defs.md#addbridgeoutputrequesttypedef) 
5. See [:material-code-braces: FailoverConfigTypeDef](./type_defs.md#failoverconfigtypedef) 
6. See [:material-code-braces: CreateBridgeResponseTypeDef](./type_defs.md#createbridgeresponsetypedef) 


```python
# create_bridge method usage example with argument unpacking

kwargs: CreateBridgeRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "PlacementArn": ...,
    "Sources": ...,
}

parent.create_bridge(**kwargs)
```

1. See [:material-code-braces: CreateBridgeRequestRequestTypeDef](./type_defs.md#createbridgerequestrequesttypedef) 

### create\_flow

Creates a new flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").create_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_flow)

```python
# create_flow method definition

await def create_flow(
    self,
    *,
    Name: str,
    AvailabilityZone: str = ...,
    Entitlements: Sequence[GrantEntitlementRequestTypeDef] = ...,  # (1)
    MediaStreams: Sequence[AddMediaStreamRequestTypeDef] = ...,  # (2)
    Outputs: Sequence[AddOutputRequestTypeDef] = ...,  # (3)
    Source: SetSourceRequestTypeDef = ...,  # (4)
    SourceFailoverConfig: FailoverConfigTypeDef = ...,  # (5)
    Sources: Sequence[SetSourceRequestTypeDef] = ...,  # (6)
    VpcInterfaces: Sequence[VpcInterfaceRequestTypeDef] = ...,  # (7)
    Maintenance: AddMaintenanceTypeDef = ...,  # (8)
    SourceMonitoringConfig: MonitoringConfigTypeDef = ...,  # (9)
) -> CreateFlowResponseTypeDef:  # (10)
    ...
```

1. See [:material-code-braces: GrantEntitlementRequestTypeDef](./type_defs.md#grantentitlementrequesttypedef) 
2. See [:material-code-braces: AddMediaStreamRequestTypeDef](./type_defs.md#addmediastreamrequesttypedef) 
3. See [:material-code-braces: AddOutputRequestTypeDef](./type_defs.md#addoutputrequesttypedef) 
4. See [:material-code-braces: SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef) 
5. See [:material-code-braces: FailoverConfigTypeDef](./type_defs.md#failoverconfigtypedef) 
6. See [:material-code-braces: SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef) 
7. See [:material-code-braces: VpcInterfaceRequestTypeDef](./type_defs.md#vpcinterfacerequesttypedef) 
8. See [:material-code-braces: AddMaintenanceTypeDef](./type_defs.md#addmaintenancetypedef) 
9. See [:material-code-braces: MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef) 
10. See [:material-code-braces: CreateFlowResponseTypeDef](./type_defs.md#createflowresponsetypedef) 


```python
# create_flow method usage example with argument unpacking

kwargs: CreateFlowRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_flow(**kwargs)
```

1. See [:material-code-braces: CreateFlowRequestRequestTypeDef](./type_defs.md#createflowrequestrequesttypedef) 

### create\_gateway

Creates a new gateway.

Type annotations and code completion for `#!python session.create_client("mediaconnect").create_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_gateway)

```python
# create_gateway method definition

await def create_gateway(
    self,
    *,
    EgressCidrBlocks: Sequence[str],
    Name: str,
    Networks: Sequence[GatewayNetworkTypeDef],  # (1)
) -> CreateGatewayResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GatewayNetworkTypeDef](./type_defs.md#gatewaynetworktypedef) 
2. See [:material-code-braces: CreateGatewayResponseTypeDef](./type_defs.md#creategatewayresponsetypedef) 


```python
# create_gateway method usage example with argument unpacking

kwargs: CreateGatewayRequestRequestTypeDef = {  # (1)
    "EgressCidrBlocks": ...,
    "Name": ...,
    "Networks": ...,
}

parent.create_gateway(**kwargs)
```

1. See [:material-code-braces: CreateGatewayRequestRequestTypeDef](./type_defs.md#creategatewayrequestrequesttypedef) 

### delete\_bridge

Deletes a bridge.

Type annotations and code completion for `#!python session.create_client("mediaconnect").delete_bridge` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.delete_bridge)

```python
# delete_bridge method definition

await def delete_bridge(
    self,
    *,
    BridgeArn: str,
) -> DeleteBridgeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBridgeResponseTypeDef](./type_defs.md#deletebridgeresponsetypedef) 


```python
# delete_bridge method usage example with argument unpacking

kwargs: DeleteBridgeRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
}

parent.delete_bridge(**kwargs)
```

1. See [:material-code-braces: DeleteBridgeRequestRequestTypeDef](./type_defs.md#deletebridgerequestrequesttypedef) 

### delete\_flow

Deletes a flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").delete_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.delete_flow)

```python
# delete_flow method definition

await def delete_flow(
    self,
    *,
    FlowArn: str,
) -> DeleteFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFlowResponseTypeDef](./type_defs.md#deleteflowresponsetypedef) 


```python
# delete_flow method usage example with argument unpacking

kwargs: DeleteFlowRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
}

parent.delete_flow(**kwargs)
```

1. See [:material-code-braces: DeleteFlowRequestRequestTypeDef](./type_defs.md#deleteflowrequestrequesttypedef) 

### delete\_gateway

Deletes a gateway.

Type annotations and code completion for `#!python session.create_client("mediaconnect").delete_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.delete_gateway)

```python
# delete_gateway method definition

await def delete_gateway(
    self,
    *,
    GatewayArn: str,
) -> DeleteGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGatewayResponseTypeDef](./type_defs.md#deletegatewayresponsetypedef) 


```python
# delete_gateway method usage example with argument unpacking

kwargs: DeleteGatewayRequestRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.delete_gateway(**kwargs)
```

1. See [:material-code-braces: DeleteGatewayRequestRequestTypeDef](./type_defs.md#deletegatewayrequestrequesttypedef) 

### deregister\_gateway\_instance

Deregisters an instance.

Type annotations and code completion for `#!python session.create_client("mediaconnect").deregister_gateway_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.deregister_gateway_instance)

```python
# deregister_gateway_instance method definition

await def deregister_gateway_instance(
    self,
    *,
    GatewayInstanceArn: str,
    Force: bool = ...,
) -> DeregisterGatewayInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeregisterGatewayInstanceResponseTypeDef](./type_defs.md#deregistergatewayinstanceresponsetypedef) 


```python
# deregister_gateway_instance method usage example with argument unpacking

kwargs: DeregisterGatewayInstanceRequestRequestTypeDef = {  # (1)
    "GatewayInstanceArn": ...,
}

parent.deregister_gateway_instance(**kwargs)
```

1. See [:material-code-braces: DeregisterGatewayInstanceRequestRequestTypeDef](./type_defs.md#deregistergatewayinstancerequestrequesttypedef) 

### describe\_bridge

Displays the details of a bridge.

Type annotations and code completion for `#!python session.create_client("mediaconnect").describe_bridge` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_bridge)

```python
# describe_bridge method definition

await def describe_bridge(
    self,
    *,
    BridgeArn: str,
) -> DescribeBridgeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBridgeResponseTypeDef](./type_defs.md#describebridgeresponsetypedef) 


```python
# describe_bridge method usage example with argument unpacking

kwargs: DescribeBridgeRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
}

parent.describe_bridge(**kwargs)
```

1. See [:material-code-braces: DescribeBridgeRequestRequestTypeDef](./type_defs.md#describebridgerequestrequesttypedef) 

### describe\_flow

Displays the details of a flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").describe_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_flow)

```python
# describe_flow method definition

await def describe_flow(
    self,
    *,
    FlowArn: str,
) -> DescribeFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFlowResponseTypeDef](./type_defs.md#describeflowresponsetypedef) 


```python
# describe_flow method usage example with argument unpacking

kwargs: DescribeFlowRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
}

parent.describe_flow(**kwargs)
```

1. See [:material-code-braces: DescribeFlowRequestRequestTypeDef](./type_defs.md#describeflowrequestrequesttypedef) 

### describe\_flow\_source\_metadata

Displays details of the flow's source stream.

Type annotations and code completion for `#!python session.create_client("mediaconnect").describe_flow_source_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_flow_source_metadata)

```python
# describe_flow_source_metadata method definition

await def describe_flow_source_metadata(
    self,
    *,
    FlowArn: str,
) -> DescribeFlowSourceMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFlowSourceMetadataResponseTypeDef](./type_defs.md#describeflowsourcemetadataresponsetypedef) 


```python
# describe_flow_source_metadata method usage example with argument unpacking

kwargs: DescribeFlowSourceMetadataRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
}

parent.describe_flow_source_metadata(**kwargs)
```

1. See [:material-code-braces: DescribeFlowSourceMetadataRequestRequestTypeDef](./type_defs.md#describeflowsourcemetadatarequestrequesttypedef) 

### describe\_flow\_source\_thumbnail

Displays the thumbnail details of a flow's source stream.

Type annotations and code completion for `#!python session.create_client("mediaconnect").describe_flow_source_thumbnail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_flow_source_thumbnail)

```python
# describe_flow_source_thumbnail method definition

await def describe_flow_source_thumbnail(
    self,
    *,
    FlowArn: str,
) -> DescribeFlowSourceThumbnailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFlowSourceThumbnailResponseTypeDef](./type_defs.md#describeflowsourcethumbnailresponsetypedef) 


```python
# describe_flow_source_thumbnail method usage example with argument unpacking

kwargs: DescribeFlowSourceThumbnailRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
}

parent.describe_flow_source_thumbnail(**kwargs)
```

1. See [:material-code-braces: DescribeFlowSourceThumbnailRequestRequestTypeDef](./type_defs.md#describeflowsourcethumbnailrequestrequesttypedef) 

### describe\_gateway

Displays the details of a gateway.

Type annotations and code completion for `#!python session.create_client("mediaconnect").describe_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_gateway)

```python
# describe_gateway method definition

await def describe_gateway(
    self,
    *,
    GatewayArn: str,
) -> DescribeGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGatewayResponseTypeDef](./type_defs.md#describegatewayresponsetypedef) 


```python
# describe_gateway method usage example with argument unpacking

kwargs: DescribeGatewayRequestRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.describe_gateway(**kwargs)
```

1. See [:material-code-braces: DescribeGatewayRequestRequestTypeDef](./type_defs.md#describegatewayrequestrequesttypedef) 

### describe\_gateway\_instance

Displays the details of an instance.

Type annotations and code completion for `#!python session.create_client("mediaconnect").describe_gateway_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_gateway_instance)

```python
# describe_gateway_instance method definition

await def describe_gateway_instance(
    self,
    *,
    GatewayInstanceArn: str,
) -> DescribeGatewayInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGatewayInstanceResponseTypeDef](./type_defs.md#describegatewayinstanceresponsetypedef) 


```python
# describe_gateway_instance method usage example with argument unpacking

kwargs: DescribeGatewayInstanceRequestRequestTypeDef = {  # (1)
    "GatewayInstanceArn": ...,
}

parent.describe_gateway_instance(**kwargs)
```

1. See [:material-code-braces: DescribeGatewayInstanceRequestRequestTypeDef](./type_defs.md#describegatewayinstancerequestrequesttypedef) 

### describe\_offering

Displays the details of an offering.

Type annotations and code completion for `#!python session.create_client("mediaconnect").describe_offering` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_offering)

```python
# describe_offering method definition

await def describe_offering(
    self,
    *,
    OfferingArn: str,
) -> DescribeOfferingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOfferingResponseTypeDef](./type_defs.md#describeofferingresponsetypedef) 


```python
# describe_offering method usage example with argument unpacking

kwargs: DescribeOfferingRequestRequestTypeDef = {  # (1)
    "OfferingArn": ...,
}

parent.describe_offering(**kwargs)
```

1. See [:material-code-braces: DescribeOfferingRequestRequestTypeDef](./type_defs.md#describeofferingrequestrequesttypedef) 

### describe\_reservation

Displays the details of a reservation.

Type annotations and code completion for `#!python session.create_client("mediaconnect").describe_reservation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_reservation)

```python
# describe_reservation method definition

await def describe_reservation(
    self,
    *,
    ReservationArn: str,
) -> DescribeReservationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReservationResponseTypeDef](./type_defs.md#describereservationresponsetypedef) 


```python
# describe_reservation method usage example with argument unpacking

kwargs: DescribeReservationRequestRequestTypeDef = {  # (1)
    "ReservationArn": ...,
}

parent.describe_reservation(**kwargs)
```

1. See [:material-code-braces: DescribeReservationRequestRequestTypeDef](./type_defs.md#describereservationrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("mediaconnect").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### grant\_flow\_entitlements

Grants entitlements to an existing flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").grant_flow_entitlements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.grant_flow_entitlements)

```python
# grant_flow_entitlements method definition

await def grant_flow_entitlements(
    self,
    *,
    Entitlements: Sequence[GrantEntitlementRequestTypeDef],  # (1)
    FlowArn: str,
) -> GrantFlowEntitlementsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GrantEntitlementRequestTypeDef](./type_defs.md#grantentitlementrequesttypedef) 
2. See [:material-code-braces: GrantFlowEntitlementsResponseTypeDef](./type_defs.md#grantflowentitlementsresponsetypedef) 


```python
# grant_flow_entitlements method usage example with argument unpacking

kwargs: GrantFlowEntitlementsRequestRequestTypeDef = {  # (1)
    "Entitlements": ...,
    "FlowArn": ...,
}

parent.grant_flow_entitlements(**kwargs)
```

1. See [:material-code-braces: GrantFlowEntitlementsRequestRequestTypeDef](./type_defs.md#grantflowentitlementsrequestrequesttypedef) 

### list\_bridges

Displays a list of bridges that are associated with this account and an
optionally specified
Arn.

Type annotations and code completion for `#!python session.create_client("mediaconnect").list_bridges` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_bridges)

```python
# list_bridges method definition

await def list_bridges(
    self,
    *,
    FilterArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListBridgesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBridgesResponseTypeDef](./type_defs.md#listbridgesresponsetypedef) 


```python
# list_bridges method usage example with argument unpacking

kwargs: ListBridgesRequestRequestTypeDef = {  # (1)
    "FilterArn": ...,
}

parent.list_bridges(**kwargs)
```

1. See [:material-code-braces: ListBridgesRequestRequestTypeDef](./type_defs.md#listbridgesrequestrequesttypedef) 

### list\_entitlements

Displays a list of all entitlements that have been granted to this account.

Type annotations and code completion for `#!python session.create_client("mediaconnect").list_entitlements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_entitlements)

```python
# list_entitlements method definition

await def list_entitlements(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListEntitlementsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef) 


```python
# list_entitlements method usage example with argument unpacking

kwargs: ListEntitlementsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_entitlements(**kwargs)
```

1. See [:material-code-braces: ListEntitlementsRequestRequestTypeDef](./type_defs.md#listentitlementsrequestrequesttypedef) 

### list\_flows

Displays a list of flows that are associated with this account.

Type annotations and code completion for `#!python session.create_client("mediaconnect").list_flows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_flows)

```python
# list_flows method definition

await def list_flows(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListFlowsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef) 


```python
# list_flows method usage example with argument unpacking

kwargs: ListFlowsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_flows(**kwargs)
```

1. See [:material-code-braces: ListFlowsRequestRequestTypeDef](./type_defs.md#listflowsrequestrequesttypedef) 

### list\_gateway\_instances

Displays a list of instances associated with the AWS account.

Type annotations and code completion for `#!python session.create_client("mediaconnect").list_gateway_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_gateway_instances)

```python
# list_gateway_instances method definition

await def list_gateway_instances(
    self,
    *,
    FilterArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListGatewayInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGatewayInstancesResponseTypeDef](./type_defs.md#listgatewayinstancesresponsetypedef) 


```python
# list_gateway_instances method usage example with argument unpacking

kwargs: ListGatewayInstancesRequestRequestTypeDef = {  # (1)
    "FilterArn": ...,
}

parent.list_gateway_instances(**kwargs)
```

1. See [:material-code-braces: ListGatewayInstancesRequestRequestTypeDef](./type_defs.md#listgatewayinstancesrequestrequesttypedef) 

### list\_gateways

Displays a list of gateways that are associated with this account.

Type annotations and code completion for `#!python session.create_client("mediaconnect").list_gateways` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_gateways)

```python
# list_gateways method definition

await def list_gateways(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListGatewaysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef) 


```python
# list_gateways method usage example with argument unpacking

kwargs: ListGatewaysRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_gateways(**kwargs)
```

1. See [:material-code-braces: ListGatewaysRequestRequestTypeDef](./type_defs.md#listgatewaysrequestrequesttypedef) 

### list\_offerings

Displays a list of all offerings that are available to this account in the
current AWS
Region.

Type annotations and code completion for `#!python session.create_client("mediaconnect").list_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_offerings)

```python
# list_offerings method definition

await def list_offerings(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListOfferingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef) 


```python
# list_offerings method usage example with argument unpacking

kwargs: ListOfferingsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_offerings(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestRequestTypeDef](./type_defs.md#listofferingsrequestrequesttypedef) 

### list\_reservations

Displays a list of all reservations that have been purchased by this account in
the current AWS
Region.

Type annotations and code completion for `#!python session.create_client("mediaconnect").list_reservations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_reservations)

```python
# list_reservations method definition

await def list_reservations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListReservationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef) 


```python
# list_reservations method usage example with argument unpacking

kwargs: ListReservationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_reservations(**kwargs)
```

1. See [:material-code-braces: ListReservationsRequestRequestTypeDef](./type_defs.md#listreservationsrequestrequesttypedef) 

### list\_tags\_for\_resource

List all tags on an AWS Elemental MediaConnect resource See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/ListTagsForResource).

Type annotations and code completion for `#!python session.create_client("mediaconnect").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### purchase\_offering

Submits a request to purchase an offering.

Type annotations and code completion for `#!python session.create_client("mediaconnect").purchase_offering` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.purchase_offering)

```python
# purchase_offering method definition

await def purchase_offering(
    self,
    *,
    OfferingArn: str,
    ReservationName: str,
    Start: str,
) -> PurchaseOfferingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PurchaseOfferingResponseTypeDef](./type_defs.md#purchaseofferingresponsetypedef) 


```python
# purchase_offering method usage example with argument unpacking

kwargs: PurchaseOfferingRequestRequestTypeDef = {  # (1)
    "OfferingArn": ...,
    "ReservationName": ...,
    "Start": ...,
}

parent.purchase_offering(**kwargs)
```

1. See [:material-code-braces: PurchaseOfferingRequestRequestTypeDef](./type_defs.md#purchaseofferingrequestrequesttypedef) 

### remove\_bridge\_output

Removes an output from a bridge.

Type annotations and code completion for `#!python session.create_client("mediaconnect").remove_bridge_output` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_bridge_output)

```python
# remove_bridge_output method definition

await def remove_bridge_output(
    self,
    *,
    BridgeArn: str,
    OutputName: str,
) -> RemoveBridgeOutputResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveBridgeOutputResponseTypeDef](./type_defs.md#removebridgeoutputresponsetypedef) 


```python
# remove_bridge_output method usage example with argument unpacking

kwargs: RemoveBridgeOutputRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
    "OutputName": ...,
}

parent.remove_bridge_output(**kwargs)
```

1. See [:material-code-braces: RemoveBridgeOutputRequestRequestTypeDef](./type_defs.md#removebridgeoutputrequestrequesttypedef) 

### remove\_bridge\_source

Removes a source from a bridge.

Type annotations and code completion for `#!python session.create_client("mediaconnect").remove_bridge_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_bridge_source)

```python
# remove_bridge_source method definition

await def remove_bridge_source(
    self,
    *,
    BridgeArn: str,
    SourceName: str,
) -> RemoveBridgeSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveBridgeSourceResponseTypeDef](./type_defs.md#removebridgesourceresponsetypedef) 


```python
# remove_bridge_source method usage example with argument unpacking

kwargs: RemoveBridgeSourceRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
    "SourceName": ...,
}

parent.remove_bridge_source(**kwargs)
```

1. See [:material-code-braces: RemoveBridgeSourceRequestRequestTypeDef](./type_defs.md#removebridgesourcerequestrequesttypedef) 

### remove\_flow\_media\_stream

Removes a media stream from a flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").remove_flow_media_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_flow_media_stream)

```python
# remove_flow_media_stream method definition

await def remove_flow_media_stream(
    self,
    *,
    FlowArn: str,
    MediaStreamName: str,
) -> RemoveFlowMediaStreamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveFlowMediaStreamResponseTypeDef](./type_defs.md#removeflowmediastreamresponsetypedef) 


```python
# remove_flow_media_stream method usage example with argument unpacking

kwargs: RemoveFlowMediaStreamRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "MediaStreamName": ...,
}

parent.remove_flow_media_stream(**kwargs)
```

1. See [:material-code-braces: RemoveFlowMediaStreamRequestRequestTypeDef](./type_defs.md#removeflowmediastreamrequestrequesttypedef) 

### remove\_flow\_output

Removes an output from an existing flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").remove_flow_output` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_flow_output)

```python
# remove_flow_output method definition

await def remove_flow_output(
    self,
    *,
    FlowArn: str,
    OutputArn: str,
) -> RemoveFlowOutputResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveFlowOutputResponseTypeDef](./type_defs.md#removeflowoutputresponsetypedef) 


```python
# remove_flow_output method usage example with argument unpacking

kwargs: RemoveFlowOutputRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "OutputArn": ...,
}

parent.remove_flow_output(**kwargs)
```

1. See [:material-code-braces: RemoveFlowOutputRequestRequestTypeDef](./type_defs.md#removeflowoutputrequestrequesttypedef) 

### remove\_flow\_source

Removes a source from an existing flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").remove_flow_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_flow_source)

```python
# remove_flow_source method definition

await def remove_flow_source(
    self,
    *,
    FlowArn: str,
    SourceArn: str,
) -> RemoveFlowSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveFlowSourceResponseTypeDef](./type_defs.md#removeflowsourceresponsetypedef) 


```python
# remove_flow_source method usage example with argument unpacking

kwargs: RemoveFlowSourceRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "SourceArn": ...,
}

parent.remove_flow_source(**kwargs)
```

1. See [:material-code-braces: RemoveFlowSourceRequestRequestTypeDef](./type_defs.md#removeflowsourcerequestrequesttypedef) 

### remove\_flow\_vpc\_interface

Removes a VPC Interface from an existing flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").remove_flow_vpc_interface` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_flow_vpc_interface)

```python
# remove_flow_vpc_interface method definition

await def remove_flow_vpc_interface(
    self,
    *,
    FlowArn: str,
    VpcInterfaceName: str,
) -> RemoveFlowVpcInterfaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveFlowVpcInterfaceResponseTypeDef](./type_defs.md#removeflowvpcinterfaceresponsetypedef) 


```python
# remove_flow_vpc_interface method usage example with argument unpacking

kwargs: RemoveFlowVpcInterfaceRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "VpcInterfaceName": ...,
}

parent.remove_flow_vpc_interface(**kwargs)
```

1. See [:material-code-braces: RemoveFlowVpcInterfaceRequestRequestTypeDef](./type_defs.md#removeflowvpcinterfacerequestrequesttypedef) 

### revoke\_flow\_entitlement

Revokes an entitlement from a flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").revoke_flow_entitlement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.revoke_flow_entitlement)

```python
# revoke_flow_entitlement method definition

await def revoke_flow_entitlement(
    self,
    *,
    EntitlementArn: str,
    FlowArn: str,
) -> RevokeFlowEntitlementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RevokeFlowEntitlementResponseTypeDef](./type_defs.md#revokeflowentitlementresponsetypedef) 


```python
# revoke_flow_entitlement method usage example with argument unpacking

kwargs: RevokeFlowEntitlementRequestRequestTypeDef = {  # (1)
    "EntitlementArn": ...,
    "FlowArn": ...,
}

parent.revoke_flow_entitlement(**kwargs)
```

1. See [:material-code-braces: RevokeFlowEntitlementRequestRequestTypeDef](./type_defs.md#revokeflowentitlementrequestrequesttypedef) 

### start\_flow

Starts a flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").start_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.start_flow)

```python
# start_flow method definition

await def start_flow(
    self,
    *,
    FlowArn: str,
) -> StartFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartFlowResponseTypeDef](./type_defs.md#startflowresponsetypedef) 


```python
# start_flow method usage example with argument unpacking

kwargs: StartFlowRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
}

parent.start_flow(**kwargs)
```

1. See [:material-code-braces: StartFlowRequestRequestTypeDef](./type_defs.md#startflowrequestrequesttypedef) 

### stop\_flow

Stops a flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").stop_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.stop_flow)

```python
# stop_flow method definition

await def stop_flow(
    self,
    *,
    FlowArn: str,
) -> StopFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopFlowResponseTypeDef](./type_defs.md#stopflowresponsetypedef) 


```python
# stop_flow method usage example with argument unpacking

kwargs: StopFlowRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
}

parent.stop_flow(**kwargs)
```

1. See [:material-code-braces: StopFlowRequestRequestTypeDef](./type_defs.md#stopflowrequestrequesttypedef) 

### tag\_resource

Associates the specified tags to a resource with the specified resourceArn.

Type annotations and code completion for `#!python session.create_client("mediaconnect").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes specified tags from a resource.

Type annotations and code completion for `#!python session.create_client("mediaconnect").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_bridge

Updates the bridge See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateBridge).

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_bridge` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge)

```python
# update_bridge method definition

await def update_bridge(
    self,
    *,
    BridgeArn: str,
    EgressGatewayBridge: UpdateEgressGatewayBridgeRequestTypeDef = ...,  # (1)
    IngressGatewayBridge: UpdateIngressGatewayBridgeRequestTypeDef = ...,  # (2)
    SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...,  # (3)
) -> UpdateBridgeResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: UpdateEgressGatewayBridgeRequestTypeDef](./type_defs.md#updateegressgatewaybridgerequesttypedef) 
2. See [:material-code-braces: UpdateIngressGatewayBridgeRequestTypeDef](./type_defs.md#updateingressgatewaybridgerequesttypedef) 
3. See [:material-code-braces: UpdateFailoverConfigTypeDef](./type_defs.md#updatefailoverconfigtypedef) 
4. See [:material-code-braces: UpdateBridgeResponseTypeDef](./type_defs.md#updatebridgeresponsetypedef) 


```python
# update_bridge method usage example with argument unpacking

kwargs: UpdateBridgeRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
}

parent.update_bridge(**kwargs)
```

1. See [:material-code-braces: UpdateBridgeRequestRequestTypeDef](./type_defs.md#updatebridgerequestrequesttypedef) 

### update\_bridge\_output

Updates an existing bridge output.

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_bridge_output` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_output)

```python
# update_bridge_output method definition

await def update_bridge_output(
    self,
    *,
    BridgeArn: str,
    OutputName: str,
    NetworkOutput: UpdateBridgeNetworkOutputRequestTypeDef = ...,  # (1)
) -> UpdateBridgeOutputResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateBridgeNetworkOutputRequestTypeDef](./type_defs.md#updatebridgenetworkoutputrequesttypedef) 
2. See [:material-code-braces: UpdateBridgeOutputResponseTypeDef](./type_defs.md#updatebridgeoutputresponsetypedef) 


```python
# update_bridge_output method usage example with argument unpacking

kwargs: UpdateBridgeOutputRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
    "OutputName": ...,
}

parent.update_bridge_output(**kwargs)
```

1. See [:material-code-braces: UpdateBridgeOutputRequestRequestTypeDef](./type_defs.md#updatebridgeoutputrequestrequesttypedef) 

### update\_bridge\_source

Updates an existing bridge source.

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_bridge_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_source)

```python
# update_bridge_source method definition

await def update_bridge_source(
    self,
    *,
    BridgeArn: str,
    SourceName: str,
    FlowSource: UpdateBridgeFlowSourceRequestTypeDef = ...,  # (1)
    NetworkSource: UpdateBridgeNetworkSourceRequestTypeDef = ...,  # (2)
) -> UpdateBridgeSourceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UpdateBridgeFlowSourceRequestTypeDef](./type_defs.md#updatebridgeflowsourcerequesttypedef) 
2. See [:material-code-braces: UpdateBridgeNetworkSourceRequestTypeDef](./type_defs.md#updatebridgenetworksourcerequesttypedef) 
3. See [:material-code-braces: UpdateBridgeSourceResponseTypeDef](./type_defs.md#updatebridgesourceresponsetypedef) 


```python
# update_bridge_source method usage example with argument unpacking

kwargs: UpdateBridgeSourceRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
    "SourceName": ...,
}

parent.update_bridge_source(**kwargs)
```

1. See [:material-code-braces: UpdateBridgeSourceRequestRequestTypeDef](./type_defs.md#updatebridgesourcerequestrequesttypedef) 

### update\_bridge\_state

Updates the bridge state See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateBridgeState).

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_bridge_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_state)

```python
# update_bridge_state method definition

await def update_bridge_state(
    self,
    *,
    BridgeArn: str,
    DesiredState: DesiredStateType,  # (1)
) -> UpdateBridgeStateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DesiredStateType](./literals.md#desiredstatetype) 
2. See [:material-code-braces: UpdateBridgeStateResponseTypeDef](./type_defs.md#updatebridgestateresponsetypedef) 


```python
# update_bridge_state method usage example with argument unpacking

kwargs: UpdateBridgeStateRequestRequestTypeDef = {  # (1)
    "BridgeArn": ...,
    "DesiredState": ...,
}

parent.update_bridge_state(**kwargs)
```

1. See [:material-code-braces: UpdateBridgeStateRequestRequestTypeDef](./type_defs.md#updatebridgestaterequestrequesttypedef) 

### update\_flow

Updates flow See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateFlow).

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow)

```python
# update_flow method definition

await def update_flow(
    self,
    *,
    FlowArn: str,
    SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...,  # (1)
    Maintenance: UpdateMaintenanceTypeDef = ...,  # (2)
    SourceMonitoringConfig: MonitoringConfigTypeDef = ...,  # (3)
) -> UpdateFlowResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: UpdateFailoverConfigTypeDef](./type_defs.md#updatefailoverconfigtypedef) 
2. See [:material-code-braces: UpdateMaintenanceTypeDef](./type_defs.md#updatemaintenancetypedef) 
3. See [:material-code-braces: MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef) 
4. See [:material-code-braces: UpdateFlowResponseTypeDef](./type_defs.md#updateflowresponsetypedef) 


```python
# update_flow method usage example with argument unpacking

kwargs: UpdateFlowRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
}

parent.update_flow(**kwargs)
```

1. See [:material-code-braces: UpdateFlowRequestRequestTypeDef](./type_defs.md#updateflowrequestrequesttypedef) 

### update\_flow\_entitlement

You can change an entitlement's description, subscribers, and encryption.

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_flow_entitlement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_entitlement)

```python
# update_flow_entitlement method definition

await def update_flow_entitlement(
    self,
    *,
    EntitlementArn: str,
    FlowArn: str,
    Description: str = ...,
    Encryption: UpdateEncryptionTypeDef = ...,  # (1)
    EntitlementStatus: EntitlementStatusType = ...,  # (2)
    Subscribers: Sequence[str] = ...,
) -> UpdateFlowEntitlementResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UpdateEncryptionTypeDef](./type_defs.md#updateencryptiontypedef) 
2. See [:material-code-brackets: EntitlementStatusType](./literals.md#entitlementstatustype) 
3. See [:material-code-braces: UpdateFlowEntitlementResponseTypeDef](./type_defs.md#updateflowentitlementresponsetypedef) 


```python
# update_flow_entitlement method usage example with argument unpacking

kwargs: UpdateFlowEntitlementRequestRequestTypeDef = {  # (1)
    "EntitlementArn": ...,
    "FlowArn": ...,
}

parent.update_flow_entitlement(**kwargs)
```

1. See [:material-code-braces: UpdateFlowEntitlementRequestRequestTypeDef](./type_defs.md#updateflowentitlementrequestrequesttypedef) 

### update\_flow\_media\_stream

Updates an existing media stream.

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_flow_media_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_media_stream)

```python
# update_flow_media_stream method definition

await def update_flow_media_stream(
    self,
    *,
    FlowArn: str,
    MediaStreamName: str,
    Attributes: MediaStreamAttributesRequestTypeDef = ...,  # (1)
    ClockRate: int = ...,
    Description: str = ...,
    MediaStreamType: MediaStreamTypeType = ...,  # (2)
    VideoFormat: str = ...,
) -> UpdateFlowMediaStreamResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MediaStreamAttributesRequestTypeDef](./type_defs.md#mediastreamattributesrequesttypedef) 
2. See [:material-code-brackets: MediaStreamTypeType](./literals.md#mediastreamtypetype) 
3. See [:material-code-braces: UpdateFlowMediaStreamResponseTypeDef](./type_defs.md#updateflowmediastreamresponsetypedef) 


```python
# update_flow_media_stream method usage example with argument unpacking

kwargs: UpdateFlowMediaStreamRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "MediaStreamName": ...,
}

parent.update_flow_media_stream(**kwargs)
```

1. See [:material-code-braces: UpdateFlowMediaStreamRequestRequestTypeDef](./type_defs.md#updateflowmediastreamrequestrequesttypedef) 

### update\_flow\_output

Updates an existing flow output.

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_flow_output` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_output)

```python
# update_flow_output method definition

await def update_flow_output(
    self,
    *,
    FlowArn: str,
    OutputArn: str,
    CidrAllowList: Sequence[str] = ...,
    Description: str = ...,
    Destination: str = ...,
    Encryption: UpdateEncryptionTypeDef = ...,  # (1)
    MaxLatency: int = ...,
    MediaStreamOutputConfigurations: Sequence[MediaStreamOutputConfigurationRequestTypeDef] = ...,  # (2)
    MinLatency: int = ...,
    Port: int = ...,
    Protocol: ProtocolType = ...,  # (3)
    RemoteId: str = ...,
    SenderControlPort: int = ...,
    SenderIpAddress: str = ...,
    SmoothingLatency: int = ...,
    StreamId: str = ...,
    VpcInterfaceAttachment: VpcInterfaceAttachmentTypeDef = ...,  # (4)
    OutputStatus: OutputStatusType = ...,  # (5)
) -> UpdateFlowOutputResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: UpdateEncryptionTypeDef](./type_defs.md#updateencryptiontypedef) 
2. See [:material-code-braces: MediaStreamOutputConfigurationRequestTypeDef](./type_defs.md#mediastreamoutputconfigurationrequesttypedef) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
4. See [:material-code-braces: VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef) 
5. See [:material-code-brackets: OutputStatusType](./literals.md#outputstatustype) 
6. See [:material-code-braces: UpdateFlowOutputResponseTypeDef](./type_defs.md#updateflowoutputresponsetypedef) 


```python
# update_flow_output method usage example with argument unpacking

kwargs: UpdateFlowOutputRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "OutputArn": ...,
}

parent.update_flow_output(**kwargs)
```

1. See [:material-code-braces: UpdateFlowOutputRequestRequestTypeDef](./type_defs.md#updateflowoutputrequestrequesttypedef) 

### update\_flow\_source

Updates the source of a flow.

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_flow_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_source)

```python
# update_flow_source method definition

await def update_flow_source(
    self,
    *,
    FlowArn: str,
    SourceArn: str,
    Decryption: UpdateEncryptionTypeDef = ...,  # (1)
    Description: str = ...,
    EntitlementArn: str = ...,
    IngestPort: int = ...,
    MaxBitrate: int = ...,
    MaxLatency: int = ...,
    MaxSyncBuffer: int = ...,
    MediaStreamSourceConfigurations: Sequence[MediaStreamSourceConfigurationRequestTypeDef] = ...,  # (2)
    MinLatency: int = ...,
    Protocol: ProtocolType = ...,  # (3)
    SenderControlPort: int = ...,
    SenderIpAddress: str = ...,
    SourceListenerAddress: str = ...,
    SourceListenerPort: int = ...,
    StreamId: str = ...,
    VpcInterfaceName: str = ...,
    WhitelistCidr: str = ...,
    GatewayBridgeSource: UpdateGatewayBridgeSourceRequestTypeDef = ...,  # (4)
) -> UpdateFlowSourceResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: UpdateEncryptionTypeDef](./type_defs.md#updateencryptiontypedef) 
2. See [:material-code-braces: MediaStreamSourceConfigurationRequestTypeDef](./type_defs.md#mediastreamsourceconfigurationrequesttypedef) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
4. See [:material-code-braces: UpdateGatewayBridgeSourceRequestTypeDef](./type_defs.md#updategatewaybridgesourcerequesttypedef) 
5. See [:material-code-braces: UpdateFlowSourceResponseTypeDef](./type_defs.md#updateflowsourceresponsetypedef) 


```python
# update_flow_source method usage example with argument unpacking

kwargs: UpdateFlowSourceRequestRequestTypeDef = {  # (1)
    "FlowArn": ...,
    "SourceArn": ...,
}

parent.update_flow_source(**kwargs)
```

1. See [:material-code-braces: UpdateFlowSourceRequestRequestTypeDef](./type_defs.md#updateflowsourcerequestrequesttypedef) 

### update\_gateway\_instance

Updates the configuration of an existing Gateway Instance.

Type annotations and code completion for `#!python session.create_client("mediaconnect").update_gateway_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_gateway_instance)

```python
# update_gateway_instance method definition

await def update_gateway_instance(
    self,
    *,
    GatewayInstanceArn: str,
    BridgePlacement: BridgePlacementType = ...,  # (1)
) -> UpdateGatewayInstanceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: BridgePlacementType](./literals.md#bridgeplacementtype) 
2. See [:material-code-braces: UpdateGatewayInstanceResponseTypeDef](./type_defs.md#updategatewayinstanceresponsetypedef) 


```python
# update_gateway_instance method usage example with argument unpacking

kwargs: UpdateGatewayInstanceRequestRequestTypeDef = {  # (1)
    "GatewayInstanceArn": ...,
}

parent.update_gateway_instance(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayInstanceRequestRequestTypeDef](./type_defs.md#updategatewayinstancerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("mediaconnect").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "MediaConnectClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("mediaconnect").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator` method with overloads.

- `client.get_paginator("list_bridges")` -> [ListBridgesPaginator](./paginators.md#listbridgespaginator)
- `client.get_paginator("list_entitlements")` -> [ListEntitlementsPaginator](./paginators.md#listentitlementspaginator)
- `client.get_paginator("list_flows")` -> [ListFlowsPaginator](./paginators.md#listflowspaginator)
- `client.get_paginator("list_gateway_instances")` -> [ListGatewayInstancesPaginator](./paginators.md#listgatewayinstancespaginator)
- `client.get_paginator("list_gateways")` -> [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
- `client.get_paginator("list_offerings")` -> [ListOfferingsPaginator](./paginators.md#listofferingspaginator)
- `client.get_paginator("list_reservations")` -> [ListReservationsPaginator](./paginators.md#listreservationspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_waiter` method with overloads.

- `client.get_waiter("flow_active")` -> [FlowActiveWaiter](./waiters.md#flowactivewaiter)
- `client.get_waiter("flow_deleted")` -> [FlowDeletedWaiter](./waiters.md#flowdeletedwaiter)
- `client.get_waiter("flow_standby")` -> [FlowStandbyWaiter](./waiters.md#flowstandbywaiter)

