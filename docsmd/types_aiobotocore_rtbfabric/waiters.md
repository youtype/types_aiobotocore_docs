# Waiters

> [Index](../README.md) > [RTBFabric](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [RTBFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#rtbfabric)
    type annotations stubs module [types-aiobotocore-rtbfabric](https://pypi.org/project/types-aiobotocore-rtbfabric/).

## InboundExternalLinkActiveWaiter

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_waiter("inbound_external_link_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/waiter/InboundExternalLinkActive.html#RTBFabric.Waiter.InboundExternalLinkActive)

```python
# InboundExternalLinkActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rtbfabric.waiter import InboundExternalLinkActiveWaiter

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    waiter: InboundExternalLinkActiveWaiter = client.get_waiter("inbound_external_link_active")  # (2)
    await waiter.wait(...)
```

1. client: [RTBFabricClient](./client.md)
2. waiter: [InboundExternalLinkActiveWaiter](./waiters.md#inboundexternallinkactivewaiter)


### wait

Type annotations and code completion for `#!python InboundExternalLinkActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    gatewayId: str,
    linkId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetInboundExternalLinkRequestWaitTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetInboundExternalLinkRequestWaitTypeDef](./type_defs.md#getinboundexternallinkrequestwaittypedef)
## LinkAcceptedWaiter

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_waiter("link_accepted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/waiter/LinkAccepted.html#RTBFabric.Waiter.LinkAccepted)

```python
# LinkAcceptedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rtbfabric.waiter import LinkAcceptedWaiter

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    waiter: LinkAcceptedWaiter = client.get_waiter("link_accepted")  # (2)
    await waiter.wait(...)
```

1. client: [RTBFabricClient](./client.md)
2. waiter: [LinkAcceptedWaiter](./waiters.md#linkacceptedwaiter)


### wait

Type annotations and code completion for `#!python LinkAcceptedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    gatewayId: str,
    linkId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetLinkRequestWaitTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetLinkRequestWaitTypeDef](./type_defs.md#getlinkrequestwaittypedef)
## LinkActiveWaiter

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_waiter("link_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/waiter/LinkActive.html#RTBFabric.Waiter.LinkActive)

```python
# LinkActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rtbfabric.waiter import LinkActiveWaiter

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    waiter: LinkActiveWaiter = client.get_waiter("link_active")  # (2)
    await waiter.wait(...)
```

1. client: [RTBFabricClient](./client.md)
2. waiter: [LinkActiveWaiter](./waiters.md#linkactivewaiter)


### wait

Type annotations and code completion for `#!python LinkActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    gatewayId: str,
    linkId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetLinkRequestWaitExtraTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetLinkRequestWaitExtraTypeDef](./type_defs.md#getlinkrequestwaitextratypedef)
## OutboundExternalLinkActiveWaiter

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_waiter("outbound_external_link_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/waiter/OutboundExternalLinkActive.html#RTBFabric.Waiter.OutboundExternalLinkActive)

```python
# OutboundExternalLinkActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rtbfabric.waiter import OutboundExternalLinkActiveWaiter

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    waiter: OutboundExternalLinkActiveWaiter = client.get_waiter("outbound_external_link_active")  # (2)
    await waiter.wait(...)
```

1. client: [RTBFabricClient](./client.md)
2. waiter: [OutboundExternalLinkActiveWaiter](./waiters.md#outboundexternallinkactivewaiter)


### wait

Type annotations and code completion for `#!python OutboundExternalLinkActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    gatewayId: str,
    linkId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetOutboundExternalLinkRequestWaitTypeDef = {  # (1)
    "gatewayId": ...,
    "linkId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetOutboundExternalLinkRequestWaitTypeDef](./type_defs.md#getoutboundexternallinkrequestwaittypedef)
## RequesterGatewayActiveWaiter

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_waiter("requester_gateway_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/waiter/RequesterGatewayActive.html#RTBFabric.Waiter.RequesterGatewayActive)

```python
# RequesterGatewayActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rtbfabric.waiter import RequesterGatewayActiveWaiter

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    waiter: RequesterGatewayActiveWaiter = client.get_waiter("requester_gateway_active")  # (2)
    await waiter.wait(...)
```

1. client: [RTBFabricClient](./client.md)
2. waiter: [RequesterGatewayActiveWaiter](./waiters.md#requestergatewayactivewaiter)


### wait

Type annotations and code completion for `#!python RequesterGatewayActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    gatewayId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetRequesterGatewayRequestWaitTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetRequesterGatewayRequestWaitTypeDef](./type_defs.md#getrequestergatewayrequestwaittypedef)
## RequesterGatewayDeletedWaiter

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_waiter("requester_gateway_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/waiter/RequesterGatewayDeleted.html#RTBFabric.Waiter.RequesterGatewayDeleted)

```python
# RequesterGatewayDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rtbfabric.waiter import RequesterGatewayDeletedWaiter

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    waiter: RequesterGatewayDeletedWaiter = client.get_waiter("requester_gateway_deleted")  # (2)
    await waiter.wait(...)
```

1. client: [RTBFabricClient](./client.md)
2. waiter: [RequesterGatewayDeletedWaiter](./waiters.md#requestergatewaydeletedwaiter)


### wait

Type annotations and code completion for `#!python RequesterGatewayDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    gatewayId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetRequesterGatewayRequestWaitExtraTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetRequesterGatewayRequestWaitExtraTypeDef](./type_defs.md#getrequestergatewayrequestwaitextratypedef)
## ResponderGatewayActiveWaiter

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_waiter("responder_gateway_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/waiter/ResponderGatewayActive.html#RTBFabric.Waiter.ResponderGatewayActive)

```python
# ResponderGatewayActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rtbfabric.waiter import ResponderGatewayActiveWaiter

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    waiter: ResponderGatewayActiveWaiter = client.get_waiter("responder_gateway_active")  # (2)
    await waiter.wait(...)
```

1. client: [RTBFabricClient](./client.md)
2. waiter: [ResponderGatewayActiveWaiter](./waiters.md#respondergatewayactivewaiter)


### wait

Type annotations and code completion for `#!python ResponderGatewayActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    gatewayId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetResponderGatewayRequestWaitTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetResponderGatewayRequestWaitTypeDef](./type_defs.md#getrespondergatewayrequestwaittypedef)
## ResponderGatewayDeletedWaiter

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_waiter("responder_gateway_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/waiter/ResponderGatewayDeleted.html#RTBFabric.Waiter.ResponderGatewayDeleted)

```python
# ResponderGatewayDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rtbfabric.waiter import ResponderGatewayDeletedWaiter

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    waiter: ResponderGatewayDeletedWaiter = client.get_waiter("responder_gateway_deleted")  # (2)
    await waiter.wait(...)
```

1. client: [RTBFabricClient](./client.md)
2. waiter: [ResponderGatewayDeletedWaiter](./waiters.md#respondergatewaydeletedwaiter)


### wait

Type annotations and code completion for `#!python ResponderGatewayDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    gatewayId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetResponderGatewayRequestWaitExtraTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetResponderGatewayRequestWaitExtraTypeDef](./type_defs.md#getrespondergatewayrequestwaitextratypedef)
