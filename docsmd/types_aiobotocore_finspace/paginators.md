# Paginators

> [Index](../README.md) > [Finspace](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## ListKxEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("finspace").get_paginator("list_kx_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace/paginator/ListKxEnvironments.html#Finspace.Paginator.ListKxEnvironments)

```python
# ListKxEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_finspace.paginator import ListKxEnvironmentsPaginator

session = get_session()
async with session.create_client("finspace") as client:  # (1)
    paginator: ListKxEnvironmentsPaginator = client.get_paginator("list_kx_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListKxEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinspaceClient](./client.md)
2. paginator: [ListKxEnvironmentsPaginator](./paginators.md#listkxenvironmentspaginator)
3. item: [:material-code-braces: ListKxEnvironmentsResponseTypeDef](./type_defs.md#listkxenvironmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListKxEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListKxEnvironmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKxEnvironmentsResponseTypeDef](./type_defs.md#listkxenvironmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKxEnvironmentsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKxEnvironmentsRequestPaginateTypeDef](./type_defs.md#listkxenvironmentsrequestpaginatetypedef) 
