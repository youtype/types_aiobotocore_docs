# RTBFabricClient

> [Index](../README.md) > [RTBFabric](./README.md) > RTBFabricClient

!!! note ""

    Auto-generated documentation for [RTBFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#rtbfabric)
    type annotations stubs module [types-aiobotocore-rtbfabric](https://pypi.org/project/types-aiobotocore-rtbfabric/).

## RTBFabricClient

Type annotations and code completion for `#!python session.create_client("rtbfabric")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#RTBFabric.Client)

```python
# RTBFabricClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_rtbfabric.client import RTBFabricClient

session = get_session()
async with session.create_client("rtbfabric") as client:
    client: RTBFabricClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("rtbfabric").exceptions` structure.

```python
# RTBFabricClient.exceptions usage example

async with session.create_client("rtbfabric") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# RTBFabricClient usage type checking example

from types_aiobotocore_rtbfabric.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("rtbfabric").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("rtbfabric").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/generate_presigned_url.html)

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


### accept\_link

Accepts a link request between gateways.

Type annotations and code completion for `#!python session.create_client("rtbfabric").accept_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/accept_link.html)

```python
# accept_link method definition

await def accept_link(
    self,
    *,
    gatewayId: str,
    linkId: str,
    logSettings: LinkLogSettingsTypeDef,  # (1)
    attributes: LinkAttributesUnionTypeDef = ...,  # (2)
) -> AcceptLinkResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
2. See [:material-code-braces: LinkAttributesUnionTypeDef](#linkattributesuniontypedef)
3. See [:material-code-braces: AcceptLinkResponseTypeDef](./type_defs.md#acceptlinkresponsetypedef)


```python
# accept_link method usage example with argument unpacking

kwargs: AcceptLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
    "logSettings": ...,
}

parent.accept_link(**kwargs)
```

1. See [:material-code-braces: AcceptLinkRequestTypeDef](./type_defs.md#acceptlinkrequesttypedef)

### create\_inbound\_external\_link

Creates an inbound external link.

Type annotations and code completion for `#!python session.create_client("rtbfabric").create_inbound_external_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/create_inbound_external_link.html)

```python
# create_inbound_external_link method definition

await def create_inbound_external_link(
    self,
    *,
    clientToken: str,
    gatewayId: str,
    logSettings: LinkLogSettingsTypeDef,  # (1)
    attributes: LinkAttributesUnionTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateInboundExternalLinkResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
2. See [:material-code-braces: LinkAttributesUnionTypeDef](#linkattributesuniontypedef)
3. See [:material-code-braces: CreateInboundExternalLinkResponseTypeDef](./type_defs.md#createinboundexternallinkresponsetypedef)


```python
# create_inbound_external_link method usage example with argument unpacking

kwargs: CreateInboundExternalLinkRequestTypeDef = {  # (1)
    "clientToken": ...,
    "gatewayId": ...,
    "logSettings": ...,
}

parent.create_inbound_external_link(**kwargs)
```

1. See [:material-code-braces: CreateInboundExternalLinkRequestTypeDef](./type_defs.md#createinboundexternallinkrequesttypedef)

### create\_link

Creates a new link between gateways.

Type annotations and code completion for `#!python session.create_client("rtbfabric").create_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/create_link.html)

```python
# create_link method definition

await def create_link(
    self,
    *,
    gatewayId: str,
    peerGatewayId: str,
    logSettings: LinkLogSettingsTypeDef,  # (1)
    attributes: LinkAttributesUnionTypeDef = ...,  # (2)
    httpResponderAllowed: bool = ...,
    tags: Mapping[str, str] = ...,
) -> CreateLinkResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
2. See [:material-code-braces: LinkAttributesUnionTypeDef](#linkattributesuniontypedef)
3. See [:material-code-braces: CreateLinkResponseTypeDef](./type_defs.md#createlinkresponsetypedef)


```python
# create_link method usage example with argument unpacking

kwargs: CreateLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "peerGatewayId": ...,
    "logSettings": ...,
}

parent.create_link(**kwargs)
```

1. See [:material-code-braces: CreateLinkRequestTypeDef](./type_defs.md#createlinkrequesttypedef)

### create\_outbound\_external\_link

Creates an outbound external link.

Type annotations and code completion for `#!python session.create_client("rtbfabric").create_outbound_external_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/create_outbound_external_link.html)

```python
# create_outbound_external_link method definition

await def create_outbound_external_link(
    self,
    *,
    clientToken: str,
    gatewayId: str,
    publicEndpoint: str,
    logSettings: LinkLogSettingsTypeDef,  # (1)
    attributes: LinkAttributesUnionTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateOutboundExternalLinkResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
2. See [:material-code-braces: LinkAttributesUnionTypeDef](#linkattributesuniontypedef)
3. See [:material-code-braces: CreateOutboundExternalLinkResponseTypeDef](./type_defs.md#createoutboundexternallinkresponsetypedef)


```python
# create_outbound_external_link method usage example with argument unpacking

kwargs: CreateOutboundExternalLinkRequestTypeDef = {  # (1)
    "clientToken": ...,
    "gatewayId": ...,
    "publicEndpoint": ...,
    "logSettings": ...,
}

parent.create_outbound_external_link(**kwargs)
```

1. See [:material-code-braces: CreateOutboundExternalLinkRequestTypeDef](./type_defs.md#createoutboundexternallinkrequesttypedef)

### create\_requester\_gateway

Creates a requester gateway.

Type annotations and code completion for `#!python session.create_client("rtbfabric").create_requester_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/create_requester_gateway.html)

```python
# create_requester_gateway method definition

await def create_requester_gateway(
    self,
    *,
    vpcId: str,
    subnetIds: Sequence[str],
    securityGroupIds: Sequence[str],
    clientToken: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateRequesterGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRequesterGatewayResponseTypeDef](./type_defs.md#createrequestergatewayresponsetypedef)


```python
# create_requester_gateway method usage example with argument unpacking

kwargs: CreateRequesterGatewayRequestTypeDef = {  # (1)
    "vpcId": ...,
    "subnetIds": ...,
    "securityGroupIds": ...,
    "clientToken": ...,
}

parent.create_requester_gateway(**kwargs)
```

1. See [:material-code-braces: CreateRequesterGatewayRequestTypeDef](./type_defs.md#createrequestergatewayrequesttypedef)

### create\_responder\_gateway

Creates a responder gateway.

Type annotations and code completion for `#!python session.create_client("rtbfabric").create_responder_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/create_responder_gateway.html)

```python
# create_responder_gateway method definition

await def create_responder_gateway(
    self,
    *,
    vpcId: str,
    subnetIds: Sequence[str],
    securityGroupIds: Sequence[str],
    port: int,
    protocol: ProtocolType,  # (1)
    clientToken: str,
    domainName: str = ...,
    trustStoreConfiguration: TrustStoreConfigurationUnionTypeDef = ...,  # (2)
    managedEndpointConfiguration: ManagedEndpointConfigurationUnionTypeDef = ...,  # (3)
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateResponderGatewayResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype)
2. See [:material-code-braces: TrustStoreConfigurationUnionTypeDef](#truststoreconfigurationuniontypedef)
3. See [:material-code-braces: ManagedEndpointConfigurationUnionTypeDef](#managedendpointconfigurationuniontypedef)
4. See [:material-code-braces: CreateResponderGatewayResponseTypeDef](./type_defs.md#createrespondergatewayresponsetypedef)


```python
# create_responder_gateway method usage example with argument unpacking

kwargs: CreateResponderGatewayRequestTypeDef = {  # (1)
    "vpcId": ...,
    "subnetIds": ...,
    "securityGroupIds": ...,
    "port": ...,
    "protocol": ...,
    "clientToken": ...,
}

parent.create_responder_gateway(**kwargs)
```

1. See [:material-code-braces: CreateResponderGatewayRequestTypeDef](./type_defs.md#createrespondergatewayrequesttypedef)

### delete\_inbound\_external\_link

Deletes an inbound external link.

Type annotations and code completion for `#!python session.create_client("rtbfabric").delete_inbound_external_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/delete_inbound_external_link.html)

```python
# delete_inbound_external_link method definition

await def delete_inbound_external_link(
    self,
    *,
    gatewayId: str,
    linkId: str,
) -> DeleteInboundExternalLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInboundExternalLinkResponseTypeDef](./type_defs.md#deleteinboundexternallinkresponsetypedef)


```python
# delete_inbound_external_link method usage example with argument unpacking

kwargs: DeleteInboundExternalLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.delete_inbound_external_link(**kwargs)
```

1. See [:material-code-braces: DeleteInboundExternalLinkRequestTypeDef](./type_defs.md#deleteinboundexternallinkrequesttypedef)

### delete\_link

Deletes a link between gateways.

Type annotations and code completion for `#!python session.create_client("rtbfabric").delete_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/delete_link.html)

```python
# delete_link method definition

await def delete_link(
    self,
    *,
    gatewayId: str,
    linkId: str,
) -> DeleteLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteLinkResponseTypeDef](./type_defs.md#deletelinkresponsetypedef)


```python
# delete_link method usage example with argument unpacking

kwargs: DeleteLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.delete_link(**kwargs)
```

1. See [:material-code-braces: DeleteLinkRequestTypeDef](./type_defs.md#deletelinkrequesttypedef)

### delete\_outbound\_external\_link

Deletes an outbound external link.

Type annotations and code completion for `#!python session.create_client("rtbfabric").delete_outbound_external_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/delete_outbound_external_link.html)

```python
# delete_outbound_external_link method definition

await def delete_outbound_external_link(
    self,
    *,
    gatewayId: str,
    linkId: str,
) -> DeleteOutboundExternalLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteOutboundExternalLinkResponseTypeDef](./type_defs.md#deleteoutboundexternallinkresponsetypedef)


```python
# delete_outbound_external_link method usage example with argument unpacking

kwargs: DeleteOutboundExternalLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.delete_outbound_external_link(**kwargs)
```

1. See [:material-code-braces: DeleteOutboundExternalLinkRequestTypeDef](./type_defs.md#deleteoutboundexternallinkrequesttypedef)

### delete\_requester\_gateway

Deletes a requester gateway.

Type annotations and code completion for `#!python session.create_client("rtbfabric").delete_requester_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/delete_requester_gateway.html)

```python
# delete_requester_gateway method definition

await def delete_requester_gateway(
    self,
    *,
    gatewayId: str,
) -> DeleteRequesterGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteRequesterGatewayResponseTypeDef](./type_defs.md#deleterequestergatewayresponsetypedef)


```python
# delete_requester_gateway method usage example with argument unpacking

kwargs: DeleteRequesterGatewayRequestTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.delete_requester_gateway(**kwargs)
```

1. See [:material-code-braces: DeleteRequesterGatewayRequestTypeDef](./type_defs.md#deleterequestergatewayrequesttypedef)

### delete\_responder\_gateway

Deletes a responder gateway.

Type annotations and code completion for `#!python session.create_client("rtbfabric").delete_responder_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/delete_responder_gateway.html)

```python
# delete_responder_gateway method definition

await def delete_responder_gateway(
    self,
    *,
    gatewayId: str,
) -> DeleteResponderGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteResponderGatewayResponseTypeDef](./type_defs.md#deleterespondergatewayresponsetypedef)


```python
# delete_responder_gateway method usage example with argument unpacking

kwargs: DeleteResponderGatewayRequestTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.delete_responder_gateway(**kwargs)
```

1. See [:material-code-braces: DeleteResponderGatewayRequestTypeDef](./type_defs.md#deleterespondergatewayrequesttypedef)

### get\_inbound\_external\_link

Retrieves information about an inbound external link.

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_inbound_external_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/get_inbound_external_link.html)

```python
# get_inbound_external_link method definition

await def get_inbound_external_link(
    self,
    *,
    gatewayId: str,
    linkId: str,
) -> GetInboundExternalLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInboundExternalLinkResponseTypeDef](./type_defs.md#getinboundexternallinkresponsetypedef)


```python
# get_inbound_external_link method usage example with argument unpacking

kwargs: GetInboundExternalLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.get_inbound_external_link(**kwargs)
```

1. See [:material-code-braces: GetInboundExternalLinkRequestTypeDef](./type_defs.md#getinboundexternallinkrequesttypedef)

### get\_link

Retrieves information about a link between gateways.

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/get_link.html)

```python
# get_link method definition

await def get_link(
    self,
    *,
    gatewayId: str,
    linkId: str,
) -> GetLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLinkResponseTypeDef](./type_defs.md#getlinkresponsetypedef)


```python
# get_link method usage example with argument unpacking

kwargs: GetLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.get_link(**kwargs)
```

1. See [:material-code-braces: GetLinkRequestTypeDef](./type_defs.md#getlinkrequesttypedef)

### get\_outbound\_external\_link

Retrieves information about an outbound external link.

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_outbound_external_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/get_outbound_external_link.html)

```python
# get_outbound_external_link method definition

await def get_outbound_external_link(
    self,
    *,
    gatewayId: str,
    linkId: str,
) -> GetOutboundExternalLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOutboundExternalLinkResponseTypeDef](./type_defs.md#getoutboundexternallinkresponsetypedef)


```python
# get_outbound_external_link method usage example with argument unpacking

kwargs: GetOutboundExternalLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.get_outbound_external_link(**kwargs)
```

1. See [:material-code-braces: GetOutboundExternalLinkRequestTypeDef](./type_defs.md#getoutboundexternallinkrequesttypedef)

### get\_requester\_gateway

Retrieves information about a requester gateway.

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_requester_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/get_requester_gateway.html)

```python
# get_requester_gateway method definition

await def get_requester_gateway(
    self,
    *,
    gatewayId: str,
) -> GetRequesterGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRequesterGatewayResponseTypeDef](./type_defs.md#getrequestergatewayresponsetypedef)


```python
# get_requester_gateway method usage example with argument unpacking

kwargs: GetRequesterGatewayRequestTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.get_requester_gateway(**kwargs)
```

1. See [:material-code-braces: GetRequesterGatewayRequestTypeDef](./type_defs.md#getrequestergatewayrequesttypedef)

### get\_responder\_gateway

Retrieves information about a responder gateway.

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_responder_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/get_responder_gateway.html)

```python
# get_responder_gateway method definition

await def get_responder_gateway(
    self,
    *,
    gatewayId: str,
) -> GetResponderGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResponderGatewayResponseTypeDef](./type_defs.md#getrespondergatewayresponsetypedef)


```python
# get_responder_gateway method usage example with argument unpacking

kwargs: GetResponderGatewayRequestTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.get_responder_gateway(**kwargs)
```

1. See [:material-code-braces: GetResponderGatewayRequestTypeDef](./type_defs.md#getrespondergatewayrequesttypedef)

### list\_links

Lists links associated with gateways.

Type annotations and code completion for `#!python session.create_client("rtbfabric").list_links` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/list_links.html)

```python
# list_links method definition

await def list_links(
    self,
    *,
    gatewayId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListLinksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLinksResponseTypeDef](./type_defs.md#listlinksresponsetypedef)


```python
# list_links method usage example with argument unpacking

kwargs: ListLinksRequestTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.list_links(**kwargs)
```

1. See [:material-code-braces: ListLinksRequestTypeDef](./type_defs.md#listlinksrequesttypedef)

### list\_requester\_gateways

Lists requester gateways.

Type annotations and code completion for `#!python session.create_client("rtbfabric").list_requester_gateways` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/list_requester_gateways.html)

```python
# list_requester_gateways method definition

await def list_requester_gateways(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListRequesterGatewaysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRequesterGatewaysResponseTypeDef](./type_defs.md#listrequestergatewaysresponsetypedef)


```python
# list_requester_gateways method usage example with argument unpacking

kwargs: ListRequesterGatewaysRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_requester_gateways(**kwargs)
```

1. See [:material-code-braces: ListRequesterGatewaysRequestTypeDef](./type_defs.md#listrequestergatewaysrequesttypedef)

### list\_responder\_gateways

Lists reponder gateways.

Type annotations and code completion for `#!python session.create_client("rtbfabric").list_responder_gateways` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/list_responder_gateways.html)

```python
# list_responder_gateways method definition

await def list_responder_gateways(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListResponderGatewaysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResponderGatewaysResponseTypeDef](./type_defs.md#listrespondergatewaysresponsetypedef)


```python
# list_responder_gateways method usage example with argument unpacking

kwargs: ListResponderGatewaysRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_responder_gateways(**kwargs)
```

1. See [:material-code-braces: ListResponderGatewaysRequestTypeDef](./type_defs.md#listrespondergatewaysrequesttypedef)

### list\_tags\_for\_resource

Lists tags for a resource.

Type annotations and code completion for `#!python session.create_client("rtbfabric").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### reject\_link

Rejects a link request between gateways.

Type annotations and code completion for `#!python session.create_client("rtbfabric").reject_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/reject_link.html)

```python
# reject_link method definition

await def reject_link(
    self,
    *,
    gatewayId: str,
    linkId: str,
) -> RejectLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RejectLinkResponseTypeDef](./type_defs.md#rejectlinkresponsetypedef)


```python
# reject_link method usage example with argument unpacking

kwargs: RejectLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.reject_link(**kwargs)
```

1. See [:material-code-braces: RejectLinkRequestTypeDef](./type_defs.md#rejectlinkrequesttypedef)

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified resource.

Type annotations and code completion for `#!python session.create_client("rtbfabric").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```

```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Removes a tag or tags from a resource.

Type annotations and code completion for `#!python session.create_client("rtbfabric").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_link

Updates the configuration of a link between gateways.

Type annotations and code completion for `#!python session.create_client("rtbfabric").update_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/update_link.html)

```python
# update_link method definition

await def update_link(
    self,
    *,
    gatewayId: str,
    linkId: str,
    logSettings: LinkLogSettingsTypeDef = ...,  # (1)
) -> UpdateLinkResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
2. See [:material-code-braces: UpdateLinkResponseTypeDef](./type_defs.md#updatelinkresponsetypedef)


```python
# update_link method usage example with argument unpacking

kwargs: UpdateLinkRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.update_link(**kwargs)
```

1. See [:material-code-braces: UpdateLinkRequestTypeDef](./type_defs.md#updatelinkrequesttypedef)

### update\_link\_module\_flow

Updates a link module flow.

Type annotations and code completion for `#!python session.create_client("rtbfabric").update_link_module_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/update_link_module_flow.html)

```python
# update_link_module_flow method definition

await def update_link_module_flow(
    self,
    *,
    clientToken: str,
    gatewayId: str,
    linkId: str,
    modules: Sequence[ModuleConfigurationUnionTypeDef],  # (1)
) -> UpdateLinkModuleFlowResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[ModuleConfigurationUnionTypeDef]`
2. See [:material-code-braces: UpdateLinkModuleFlowResponseTypeDef](./type_defs.md#updatelinkmoduleflowresponsetypedef)


```python
# update_link_module_flow method usage example with argument unpacking

kwargs: UpdateLinkModuleFlowRequestTypeDef = {  # (1)
    "clientToken": ...,
    "gatewayId": ...,
    "linkId": ...,
    "modules": ...,
}

parent.update_link_module_flow(**kwargs)
```

1. See [:material-code-braces: UpdateLinkModuleFlowRequestTypeDef](./type_defs.md#updatelinkmoduleflowrequesttypedef)

### update\_requester\_gateway

Updates a requester gateway.

Type annotations and code completion for `#!python session.create_client("rtbfabric").update_requester_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/update_requester_gateway.html)

```python
# update_requester_gateway method definition

await def update_requester_gateway(
    self,
    *,
    clientToken: str,
    gatewayId: str,
    description: str = ...,
) -> UpdateRequesterGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateRequesterGatewayResponseTypeDef](./type_defs.md#updaterequestergatewayresponsetypedef)


```python
# update_requester_gateway method usage example with argument unpacking

kwargs: UpdateRequesterGatewayRequestTypeDef = {  # (1)
    "clientToken": ...,
    "gatewayId": ...,
}

parent.update_requester_gateway(**kwargs)
```

1. See [:material-code-braces: UpdateRequesterGatewayRequestTypeDef](./type_defs.md#updaterequestergatewayrequesttypedef)

### update\_responder\_gateway

Updates a responder gateway.

Type annotations and code completion for `#!python session.create_client("rtbfabric").update_responder_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/client/update_responder_gateway.html)

```python
# update_responder_gateway method definition

await def update_responder_gateway(
    self,
    *,
    port: int,
    protocol: ProtocolType,  # (1)
    clientToken: str,
    gatewayId: str,
    domainName: str = ...,
    trustStoreConfiguration: TrustStoreConfigurationUnionTypeDef = ...,  # (2)
    managedEndpointConfiguration: ManagedEndpointConfigurationUnionTypeDef = ...,  # (3)
    description: str = ...,
) -> UpdateResponderGatewayResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype)
2. See [:material-code-braces: TrustStoreConfigurationUnionTypeDef](#truststoreconfigurationuniontypedef)
3. See [:material-code-braces: ManagedEndpointConfigurationUnionTypeDef](#managedendpointconfigurationuniontypedef)
4. See [:material-code-braces: UpdateResponderGatewayResponseTypeDef](./type_defs.md#updaterespondergatewayresponsetypedef)


```python
# update_responder_gateway method usage example with argument unpacking

kwargs: UpdateResponderGatewayRequestTypeDef = {  # (1)
    "port": ...,
    "protocol": ...,
    "clientToken": ...,
    "gatewayId": ...,
}

parent.update_responder_gateway(**kwargs)
```

1. See [:material-code-braces: UpdateResponderGatewayRequestTypeDef](./type_defs.md#updaterespondergatewayrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("rtbfabric").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#RTBFabric.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("rtbfabric").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#RTBFabric.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_paginator` method with overloads.

- `client.get_paginator("list_links")` -> [ListLinksPaginator](./paginators.md#listlinkspaginator)
- `client.get_paginator("list_requester_gateways")` -> [ListRequesterGatewaysPaginator](./paginators.md#listrequestergatewayspaginator)
- `client.get_paginator("list_responder_gateways")` -> [ListResponderGatewaysPaginator](./paginators.md#listrespondergatewayspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_waiter` method with overloads.

- `client.get_waiter("inbound_external_link_active")` -> [InboundExternalLinkActiveWaiter](./waiters.md#inboundexternallinkactivewaiter)
- `client.get_waiter("link_accepted")` -> [LinkAcceptedWaiter](./waiters.md#linkacceptedwaiter)
- `client.get_waiter("link_active")` -> [LinkActiveWaiter](./waiters.md#linkactivewaiter)
- `client.get_waiter("outbound_external_link_active")` -> [OutboundExternalLinkActiveWaiter](./waiters.md#outboundexternallinkactivewaiter)
- `client.get_waiter("requester_gateway_active")` -> [RequesterGatewayActiveWaiter](./waiters.md#requestergatewayactivewaiter)
- `client.get_waiter("requester_gateway_deleted")` -> [RequesterGatewayDeletedWaiter](./waiters.md#requestergatewaydeletedwaiter)
- `client.get_waiter("responder_gateway_active")` -> [ResponderGatewayActiveWaiter](./waiters.md#respondergatewayactivewaiter)
- `client.get_waiter("responder_gateway_deleted")` -> [ResponderGatewayDeletedWaiter](./waiters.md#respondergatewaydeletedwaiter)

