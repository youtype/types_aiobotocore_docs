# Paginators

> [Index](../README.md) > [Interconnect](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Interconnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/interconnect.html#interconnect)
    type annotations stubs module [types-aiobotocore-interconnect](https://pypi.org/project/types-aiobotocore-interconnect/).

## ListAttachPointsPaginator

Type annotations and code completion for `#!python session.create_client("interconnect").get_paginator("list_attach_points")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/interconnect/paginator/ListAttachPoints.html#Interconnect.Paginator.ListAttachPoints)

```python
# ListAttachPointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_interconnect.paginator import ListAttachPointsPaginator

session = get_session()
async with session.create_client("interconnect") as client:  # (1)
    paginator: ListAttachPointsPaginator = client.get_paginator("list_attach_points")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachPointsResponseTypeDef
        print(item)  # (3)
```

1. client: [InterconnectClient](./client.md)
2. paginator: [ListAttachPointsPaginator](./paginators.md#listattachpointspaginator)
3. item: `AioPageIterator[ListAttachPointsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAttachPointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    environmentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAttachPointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAttachPointsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAttachPointsRequestPaginateTypeDef = {  # (1)
    "environmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachPointsRequestPaginateTypeDef](./type_defs.md#listattachpointsrequestpaginatetypedef)
## ListConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("interconnect").get_paginator("list_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/interconnect/paginator/ListConnections.html#Interconnect.Paginator.ListConnections)

```python
# ListConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_interconnect.paginator import ListConnectionsPaginator

session = get_session()
async with session.create_client("interconnect") as client:  # (1)
    paginator: ListConnectionsPaginator = client.get_paginator("list_connections")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [InterconnectClient](./client.md)
2. paginator: [ListConnectionsPaginator](./paginators.md#listconnectionspaginator)
3. item: `AioPageIterator[ListConnectionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    state: ConnectionStateType = ...,  # (1)
    environmentId: str = ...,
    provider: ProviderTypeDef = ...,  # (2)
    attachPoint: AttachPointTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListConnectionsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype)
2. See [:material-code-braces: ProviderTypeDef](./type_defs.md#providertypedef)
3. See [:material-code-braces: AttachPointTypeDef](./type_defs.md#attachpointtypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListConnectionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectionsRequestPaginateTypeDef = {  # (1)
    "state": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectionsRequestPaginateTypeDef](./type_defs.md#listconnectionsrequestpaginatetypedef)
## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("interconnect").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/interconnect/paginator/ListEnvironments.html#Interconnect.Paginator.ListEnvironments)

```python
# ListEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_interconnect.paginator import ListEnvironmentsPaginator

session = get_session()
async with session.create_client("interconnect") as client:  # (1)
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [InterconnectClient](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: `AioPageIterator[ListEnvironmentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    provider: ProviderTypeDef = ...,  # (1)
    location: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEnvironmentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ProviderTypeDef](./type_defs.md#providertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEnvironmentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentsRequestPaginateTypeDef = {  # (1)
    "provider": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestPaginateTypeDef](./type_defs.md#listenvironmentsrequestpaginatetypedef)
