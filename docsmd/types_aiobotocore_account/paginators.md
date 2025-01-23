# Paginators

> [Index](../README.md) > [Account](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#account)
    type annotations stubs module [types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

## ListRegionsPaginator

Type annotations and code completion for `#!python session.create_client("account").get_paginator("list_regions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account/paginator/ListRegions.html#Account.Paginator.ListRegions)

```python
# ListRegionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_account.paginator import ListRegionsPaginator

session = get_session()
async with session.create_client("account") as client:  # (1)
    paginator: ListRegionsPaginator = client.get_paginator("list_regions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegionsResponseTypeDef
        print(item)  # (3)
```

1. client: [AccountClient](./client.md)
2. paginator: [ListRegionsPaginator](./paginators.md#listregionspaginator)
3. item: [:material-code-braces: ListRegionsResponseTypeDef](./type_defs.md#listregionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRegionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str = ...,
    RegionOptStatusContains: Sequence[RegionOptStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListRegionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RegionOptStatusType](./literals.md#regionoptstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListRegionsResponseTypeDef](./type_defs.md#listregionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRegionsRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegionsRequestPaginateTypeDef](./type_defs.md#listregionsrequestpaginatetypedef) 
