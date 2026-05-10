# Paginators

> [Index](../README.md) > [Shield](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Shield](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#shield)
    type annotations stubs module [types-aiobotocore-shield](https://pypi.org/project/types-aiobotocore-shield/).

## ListAttacksPaginator

Type annotations and code completion for `#!python session.create_client("shield").get_paginator("list_attacks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/paginator/ListAttacks.html#Shield.Paginator.ListAttacks)

```python
# ListAttacksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_shield.paginator import ListAttacksPaginator

session = get_session()
async with session.create_client("shield") as client:  # (1)
    paginator: ListAttacksPaginator = client.get_paginator("list_attacks")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttacksResponseTypeDef
        print(item)  # (3)
```

1. client: [ShieldClient](./client.md)
2. paginator: [ListAttacksPaginator](./paginators.md#listattackspaginator)
3. item: `AioPageIterator[ListAttacksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAttacksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArns: Sequence[str] = ...,
    StartTime: TimeRangeUnionTypeDef = ...,  # (1)
    EndTime: TimeRangeUnionTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListAttacksResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: TimeRangeUnionTypeDef](#timerangeuniontypedef)
2. See [:material-code-braces: TimeRangeUnionTypeDef](#timerangeuniontypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListAttacksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAttacksRequestPaginateTypeDef = {  # (1)
    "ResourceArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttacksRequestPaginateTypeDef](./type_defs.md#listattacksrequestpaginatetypedef)
## ListProtectionsPaginator

Type annotations and code completion for `#!python session.create_client("shield").get_paginator("list_protections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield/paginator/ListProtections.html#Shield.Paginator.ListProtections)

```python
# ListProtectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_shield.paginator import ListProtectionsPaginator

session = get_session()
async with session.create_client("shield") as client:  # (1)
    paginator: ListProtectionsPaginator = client.get_paginator("list_protections")  # (2)
    async for item in paginator.paginate(...):
        item: ListProtectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ShieldClient](./client.md)
2. paginator: [ListProtectionsPaginator](./paginators.md#listprotectionspaginator)
3. item: `AioPageIterator[ListProtectionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProtectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InclusionFilters: InclusionProtectionFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListProtectionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: InclusionProtectionFiltersTypeDef](./type_defs.md#inclusionprotectionfilterstypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListProtectionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProtectionsRequestPaginateTypeDef = {  # (1)
    "InclusionFilters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectionsRequestPaginateTypeDef](./type_defs.md#listprotectionsrequestpaginatetypedef)
