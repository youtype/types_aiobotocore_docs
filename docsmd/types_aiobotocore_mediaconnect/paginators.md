# Paginators

> [Index](../README.md) > [MediaConnect](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#mediaconnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## ListBridgesPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_bridges")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListBridges.html#MediaConnect.Paginator.ListBridges)

```python
# ListBridgesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListBridgesPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListBridgesPaginator = client.get_paginator("list_bridges")  # (2)
    async for item in paginator.paginate(...):
        item: ListBridgesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListBridgesPaginator](./paginators.md#listbridgespaginator)
3. item: `AioPageIterator[ListBridgesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBridgesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FilterArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBridgesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBridgesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBridgesRequestPaginateTypeDef = {  # (1)
    "FilterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBridgesRequestPaginateTypeDef](./type_defs.md#listbridgesrequestpaginatetypedef)
## ListEntitlementsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_entitlements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListEntitlements.html#MediaConnect.Paginator.ListEntitlements)

```python
# ListEntitlementsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListEntitlementsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListEntitlementsPaginator = client.get_paginator("list_entitlements")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntitlementsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListEntitlementsPaginator](./paginators.md#listentitlementspaginator)
3. item: `AioPageIterator[ListEntitlementsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEntitlementsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEntitlementsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEntitlementsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEntitlementsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitlementsRequestPaginateTypeDef](./type_defs.md#listentitlementsrequestpaginatetypedef)
## ListFlowsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListFlows.html#MediaConnect.Paginator.ListFlows)

```python
# ListFlowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListFlowsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListFlowsPaginator = client.get_paginator("list_flows")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListFlowsPaginator](./paginators.md#listflowspaginator)
3. item: `AioPageIterator[ListFlowsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFlowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFlowsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowsRequestPaginateTypeDef](./type_defs.md#listflowsrequestpaginatetypedef)
## ListGatewayInstancesPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_gateway_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListGatewayInstances.html#MediaConnect.Paginator.ListGatewayInstances)

```python
# ListGatewayInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListGatewayInstancesPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListGatewayInstancesPaginator = client.get_paginator("list_gateway_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListGatewayInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListGatewayInstancesPaginator](./paginators.md#listgatewayinstancespaginator)
3. item: `AioPageIterator[ListGatewayInstancesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGatewayInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FilterArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGatewayInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGatewayInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGatewayInstancesRequestPaginateTypeDef = {  # (1)
    "FilterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGatewayInstancesRequestPaginateTypeDef](./type_defs.md#listgatewayinstancesrequestpaginatetypedef)
## ListGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListGateways.html#MediaConnect.Paginator.ListGateways)

```python
# ListGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListGatewaysPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListGatewaysPaginator = client.get_paginator("list_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: ListGatewaysResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
3. item: `AioPageIterator[ListGatewaysResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGatewaysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGatewaysResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGatewaysRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGatewaysRequestPaginateTypeDef](./type_defs.md#listgatewaysrequestpaginatetypedef)
## ListOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListOfferings.html#MediaConnect.Paginator.ListOfferings)

```python
# ListOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListOfferingsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: ListOfferingsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListOfferingsPaginator](./paginators.md#listofferingspaginator)
3. item: `AioPageIterator[ListOfferingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOfferingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOfferingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOfferingsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestPaginateTypeDef](./type_defs.md#listofferingsrequestpaginatetypedef)
## ListReservationsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_reservations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListReservations.html#MediaConnect.Paginator.ListReservations)

```python
# ListReservationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListReservationsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListReservationsPaginator = client.get_paginator("list_reservations")  # (2)
    async for item in paginator.paginate(...):
        item: ListReservationsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListReservationsPaginator](./paginators.md#listreservationspaginator)
3. item: `AioPageIterator[ListReservationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListReservationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListReservationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListReservationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListReservationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReservationsRequestPaginateTypeDef](./type_defs.md#listreservationsrequestpaginatetypedef)
## ListRouterInputsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_router_inputs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListRouterInputs.html#MediaConnect.Paginator.ListRouterInputs)

```python
# ListRouterInputsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListRouterInputsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListRouterInputsPaginator = client.get_paginator("list_router_inputs")  # (2)
    async for item in paginator.paginate(...):
        item: ListRouterInputsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListRouterInputsPaginator](./paginators.md#listrouterinputspaginator)
3. item: `AioPageIterator[ListRouterInputsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRouterInputsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[RouterInputFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRouterInputsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[RouterInputFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRouterInputsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRouterInputsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRouterInputsRequestPaginateTypeDef](./type_defs.md#listrouterinputsrequestpaginatetypedef)
## ListRouterNetworkInterfacesPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_router_network_interfaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListRouterNetworkInterfaces.html#MediaConnect.Paginator.ListRouterNetworkInterfaces)

```python
# ListRouterNetworkInterfacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListRouterNetworkInterfacesPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListRouterNetworkInterfacesPaginator = client.get_paginator("list_router_network_interfaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListRouterNetworkInterfacesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListRouterNetworkInterfacesPaginator](./paginators.md#listrouternetworkinterfacespaginator)
3. item: `AioPageIterator[ListRouterNetworkInterfacesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRouterNetworkInterfacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[RouterNetworkInterfaceFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRouterNetworkInterfacesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[RouterNetworkInterfaceFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRouterNetworkInterfacesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRouterNetworkInterfacesRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRouterNetworkInterfacesRequestPaginateTypeDef](./type_defs.md#listrouternetworkinterfacesrequestpaginatetypedef)
## ListRouterOutputsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_router_outputs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListRouterOutputs.html#MediaConnect.Paginator.ListRouterOutputs)

```python
# ListRouterOutputsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListRouterOutputsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListRouterOutputsPaginator = client.get_paginator("list_router_outputs")  # (2)
    async for item in paginator.paginate(...):
        item: ListRouterOutputsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListRouterOutputsPaginator](./paginators.md#listrouteroutputspaginator)
3. item: `AioPageIterator[ListRouterOutputsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRouterOutputsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[RouterOutputFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRouterOutputsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[RouterOutputFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRouterOutputsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRouterOutputsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRouterOutputsRequestPaginateTypeDef](./type_defs.md#listrouteroutputsrequestpaginatetypedef)
