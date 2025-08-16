# Paginators

> [Index](../README.md) > [AIOps](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AIOps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops.html#aiops)
    type annotations stubs module [types-aiobotocore-aiops](https://pypi.org/project/types-aiobotocore-aiops/).

## ListInvestigationGroupsPaginator

Type annotations and code completion for `#!python session.create_client("aiops").get_paginator("list_investigation_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/paginator/ListInvestigationGroups.html#AIOps.Paginator.ListInvestigationGroups)

```python
# ListInvestigationGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_aiops.paginator import ListInvestigationGroupsPaginator

session = get_session()
async with session.create_client("aiops") as client:  # (1)
    paginator: ListInvestigationGroupsPaginator = client.get_paginator("list_investigation_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvestigationGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [AIOpsClient](./client.md)
2. paginator: [ListInvestigationGroupsPaginator](./paginators.md#listinvestigationgroupspaginator)
3. item: `AioPageIterator[ListInvestigationGroupsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInvestigationGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListInvestigationGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListInvestigationGroupsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInvestigationGroupsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvestigationGroupsInputPaginateTypeDef](./type_defs.md#listinvestigationgroupsinputpaginatetypedef)
