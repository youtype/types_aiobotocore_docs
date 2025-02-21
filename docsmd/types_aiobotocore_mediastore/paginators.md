# Paginators

> [Index](../README.md) > [MediaStore](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#mediastore)
    type annotations stubs module [types-aiobotocore-mediastore](https://pypi.org/project/types-aiobotocore-mediastore/).

## ListContainersPaginator

Type annotations and code completion for `#!python session.create_client("mediastore").get_paginator("list_containers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/paginator/ListContainers.html#MediaStore.Paginator.ListContainers)

```python
# ListContainersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediastore.paginator import ListContainersPaginator

session = get_session()
async with session.create_client("mediastore") as client:  # (1)
    paginator: ListContainersPaginator = client.get_paginator("list_containers")  # (2)
    async for item in paginator.paginate(...):
        item: ListContainersOutputTypeDef
        print(item)  # (3)
```

1. client: [MediaStoreClient](./client.md)
2. paginator: [ListContainersPaginator](./paginators.md#listcontainerspaginator)
3. item: [:material-code-braces: ListContainersOutputTypeDef](./type_defs.md#listcontainersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListContainersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListContainersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListContainersOutputTypeDef](./type_defs.md#listcontainersoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListContainersInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContainersInputPaginateTypeDef](./type_defs.md#listcontainersinputpaginatetypedef) 
