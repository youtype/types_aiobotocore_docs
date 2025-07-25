# Paginators

> [Index](../README.md) > [EVS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs.html#evs)
    type annotations stubs module [types-aiobotocore-evs](https://pypi.org/project/types-aiobotocore-evs/).

## ListEnvironmentHostsPaginator

Type annotations and code completion for `#!python session.create_client("evs").get_paginator("list_environment_hosts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/paginator/ListEnvironmentHosts.html#EVS.Paginator.ListEnvironmentHosts)

```python
# ListEnvironmentHostsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_evs.paginator import ListEnvironmentHostsPaginator

session = get_session()
async with session.create_client("evs") as client:  # (1)
    paginator: ListEnvironmentHostsPaginator = client.get_paginator("list_environment_hosts")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentHostsResponseTypeDef
        print(item)  # (3)
```

1. client: [EVSClient](./client.md)
2. paginator: [ListEnvironmentHostsPaginator](./paginators.md#listenvironmenthostspaginator)
3. item: `AioPageIterator[ListEnvironmentHostsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEnvironmentHostsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    environmentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEnvironmentHostsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEnvironmentHostsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentHostsRequestPaginateTypeDef = {  # (1)
    "environmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentHostsRequestPaginateTypeDef](./type_defs.md#listenvironmenthostsrequestpaginatetypedef)
## ListEnvironmentVlansPaginator

Type annotations and code completion for `#!python session.create_client("evs").get_paginator("list_environment_vlans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/paginator/ListEnvironmentVlans.html#EVS.Paginator.ListEnvironmentVlans)

```python
# ListEnvironmentVlansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_evs.paginator import ListEnvironmentVlansPaginator

session = get_session()
async with session.create_client("evs") as client:  # (1)
    paginator: ListEnvironmentVlansPaginator = client.get_paginator("list_environment_vlans")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentVlansResponseTypeDef
        print(item)  # (3)
```

1. client: [EVSClient](./client.md)
2. paginator: [ListEnvironmentVlansPaginator](./paginators.md#listenvironmentvlanspaginator)
3. item: `AioPageIterator[ListEnvironmentVlansResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEnvironmentVlansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    environmentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEnvironmentVlansResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEnvironmentVlansResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentVlansRequestPaginateTypeDef = {  # (1)
    "environmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentVlansRequestPaginateTypeDef](./type_defs.md#listenvironmentvlansrequestpaginatetypedef)
## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("evs").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/paginator/ListEnvironments.html#EVS.Paginator.ListEnvironments)

```python
# ListEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_evs.paginator import ListEnvironmentsPaginator

session = get_session()
async with session.create_client("evs") as client:  # (1)
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [EVSClient](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: `AioPageIterator[ListEnvironmentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    state: Sequence[EnvironmentStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEnvironmentsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[EnvironmentStateType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEnvironmentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentsRequestPaginateTypeDef = {  # (1)
    "state": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestPaginateTypeDef](./type_defs.md#listenvironmentsrequestpaginatetypedef)
