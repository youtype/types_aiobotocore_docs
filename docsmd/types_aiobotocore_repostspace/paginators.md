# Paginators

> [Index](../README.md) > [RePostPrivate](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RePostPrivate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#repostprivate)
    type annotations stubs module [types-aiobotocore-repostspace](https://pypi.org/project/types-aiobotocore-repostspace/).

## ListSpacesPaginator

Type annotations and code completion for `#!python session.create_client("repostspace").get_paginator("list_spaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/paginator/ListSpaces.html#RePostPrivate.Paginator.ListSpaces)

```python
# ListSpacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_repostspace.paginator import ListSpacesPaginator

session = get_session()
async with session.create_client("repostspace") as client:  # (1)
    paginator: ListSpacesPaginator = client.get_paginator("list_spaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListSpacesOutputTypeDef
        print(item)  # (3)
```

1. client: [RePostPrivateClient](./client.md)
2. paginator: [ListSpacesPaginator](./paginators.md#listspacespaginator)
3. item: [:material-code-braces: ListSpacesOutputTypeDef](./type_defs.md#listspacesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSpacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSpacesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSpacesOutputTypeDef](./type_defs.md#listspacesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSpacesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSpacesInputPaginateTypeDef](./type_defs.md#listspacesinputpaginatetypedef) 
