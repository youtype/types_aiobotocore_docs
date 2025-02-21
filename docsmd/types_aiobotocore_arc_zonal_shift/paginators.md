# Paginators

> [Index](../README.md) > [ARCZonalShift](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#arczonalshift)
    type annotations stubs module [types-aiobotocore-arc-zonal-shift](https://pypi.org/project/types-aiobotocore-arc-zonal-shift/).

## ListAutoshiftsPaginator

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").get_paginator("list_autoshifts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/paginator/ListAutoshifts.html#ARCZonalShift.Paginator.ListAutoshifts)

```python
# ListAutoshiftsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_arc_zonal_shift.paginator import ListAutoshiftsPaginator

session = get_session()
async with session.create_client("arc-zonal-shift") as client:  # (1)
    paginator: ListAutoshiftsPaginator = client.get_paginator("list_autoshifts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutoshiftsResponseTypeDef
        print(item)  # (3)
```

1. client: [ARCZonalShiftClient](./client.md)
2. paginator: [ListAutoshiftsPaginator](./paginators.md#listautoshiftspaginator)
3. item: [:material-code-braces: ListAutoshiftsResponseTypeDef](./type_defs.md#listautoshiftsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAutoshiftsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    status: AutoshiftExecutionStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAutoshiftsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AutoshiftExecutionStatusType](./literals.md#autoshiftexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAutoshiftsResponseTypeDef](./type_defs.md#listautoshiftsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAutoshiftsRequestPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAutoshiftsRequestPaginateTypeDef](./type_defs.md#listautoshiftsrequestpaginatetypedef) 
## ListManagedResourcesPaginator

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").get_paginator("list_managed_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/paginator/ListManagedResources.html#ARCZonalShift.Paginator.ListManagedResources)

```python
# ListManagedResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_arc_zonal_shift.paginator import ListManagedResourcesPaginator

session = get_session()
async with session.create_client("arc-zonal-shift") as client:  # (1)
    paginator: ListManagedResourcesPaginator = client.get_paginator("list_managed_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [ARCZonalShiftClient](./client.md)
2. paginator: [ListManagedResourcesPaginator](./paginators.md#listmanagedresourcespaginator)
3. item: [:material-code-braces: ListManagedResourcesResponseTypeDef](./type_defs.md#listmanagedresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListManagedResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListManagedResourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListManagedResourcesResponseTypeDef](./type_defs.md#listmanagedresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedResourcesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedResourcesRequestPaginateTypeDef](./type_defs.md#listmanagedresourcesrequestpaginatetypedef) 
## ListZonalShiftsPaginator

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").get_paginator("list_zonal_shifts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/paginator/ListZonalShifts.html#ARCZonalShift.Paginator.ListZonalShifts)

```python
# ListZonalShiftsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_arc_zonal_shift.paginator import ListZonalShiftsPaginator

session = get_session()
async with session.create_client("arc-zonal-shift") as client:  # (1)
    paginator: ListZonalShiftsPaginator = client.get_paginator("list_zonal_shifts")  # (2)
    async for item in paginator.paginate(...):
        item: ListZonalShiftsResponseTypeDef
        print(item)  # (3)
```

1. client: [ARCZonalShiftClient](./client.md)
2. paginator: [ListZonalShiftsPaginator](./paginators.md#listzonalshiftspaginator)
3. item: [:material-code-braces: ListZonalShiftsResponseTypeDef](./type_defs.md#listzonalshiftsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListZonalShiftsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceIdentifier: str = ...,
    status: ZonalShiftStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListZonalShiftsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListZonalShiftsResponseTypeDef](./type_defs.md#listzonalshiftsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListZonalShiftsRequestPaginateTypeDef = {  # (1)
    "resourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListZonalShiftsRequestPaginateTypeDef](./type_defs.md#listzonalshiftsrequestpaginatetypedef) 
