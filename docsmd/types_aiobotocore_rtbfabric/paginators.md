# Paginators

> [Index](../README.md) > [RTBFabric](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RTBFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#rtbfabric)
    type annotations stubs module [types-aiobotocore-rtbfabric](https://pypi.org/project/types-aiobotocore-rtbfabric/).

## ListLinksPaginator

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_paginator("list_links")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/paginator/ListLinks.html#RTBFabric.Paginator.ListLinks)

```python
# ListLinksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rtbfabric.paginator import ListLinksPaginator

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    paginator: ListLinksPaginator = client.get_paginator("list_links")  # (2)
    async for item in paginator.paginate(...):
        item: ListLinksResponseTypeDef
        print(item)  # (3)
```

1. client: [RTBFabricClient](./client.md)
2. paginator: [ListLinksPaginator](./paginators.md#listlinkspaginator)
3. item: `AioPageIterator[ListLinksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLinksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    gatewayId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLinksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLinksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLinksRequestPaginateTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLinksRequestPaginateTypeDef](./type_defs.md#listlinksrequestpaginatetypedef)
## ListRequesterGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_paginator("list_requester_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/paginator/ListRequesterGateways.html#RTBFabric.Paginator.ListRequesterGateways)

```python
# ListRequesterGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rtbfabric.paginator import ListRequesterGatewaysPaginator

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    paginator: ListRequesterGatewaysPaginator = client.get_paginator("list_requester_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: ListRequesterGatewaysResponseTypeDef
        print(item)  # (3)
```

1. client: [RTBFabricClient](./client.md)
2. paginator: [ListRequesterGatewaysPaginator](./paginators.md#listrequestergatewayspaginator)
3. item: `AioPageIterator[ListRequesterGatewaysResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRequesterGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRequesterGatewaysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRequesterGatewaysResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRequesterGatewaysRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequesterGatewaysRequestPaginateTypeDef](./type_defs.md#listrequestergatewaysrequestpaginatetypedef)
## ListResponderGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("rtbfabric").get_paginator("list_responder_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric/paginator/ListResponderGateways.html#RTBFabric.Paginator.ListResponderGateways)

```python
# ListResponderGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rtbfabric.paginator import ListResponderGatewaysPaginator

session = get_session()
async with session.create_client("rtbfabric") as client:  # (1)
    paginator: ListResponderGatewaysPaginator = client.get_paginator("list_responder_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: ListResponderGatewaysResponseTypeDef
        print(item)  # (3)
```

1. client: [RTBFabricClient](./client.md)
2. paginator: [ListResponderGatewaysPaginator](./paginators.md#listrespondergatewayspaginator)
3. item: `AioPageIterator[ListResponderGatewaysResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListResponderGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListResponderGatewaysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListResponderGatewaysResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListResponderGatewaysRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResponderGatewaysRequestPaginateTypeDef](./type_defs.md#listrespondergatewaysrequestpaginatetypedef)
