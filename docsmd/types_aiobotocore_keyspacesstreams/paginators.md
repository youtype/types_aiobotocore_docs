# Paginators

> [Index](../README.md) > [KeyspacesStreams](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [KeyspacesStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspacesstreams.html#keyspacesstreams)
    type annotations stubs module [types-aiobotocore-keyspacesstreams](https://pypi.org/project/types-aiobotocore-keyspacesstreams/).

## GetStreamPaginator

Type annotations and code completion for `#!python session.create_client("keyspacesstreams").get_paginator("get_stream")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspacesstreams/paginator/GetStream.html#KeyspacesStreams.Paginator.GetStream)

```python
# GetStreamPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_keyspacesstreams.paginator import GetStreamPaginator

session = get_session()
async with session.create_client("keyspacesstreams") as client:  # (1)
    paginator: GetStreamPaginator = client.get_paginator("get_stream")  # (2)
    async for item in paginator.paginate(...):
        item: GetStreamOutputTypeDef
        print(item)  # (3)
```

1. client: [KeyspacesStreamsClient](./client.md)
2. paginator: [GetStreamPaginator](./paginators.md#getstreampaginator)
3. item: `AioPageIterator[GetStreamOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetStreamPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    streamArn: str,
    shardFilter: ShardFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetStreamOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ShardFilterTypeDef](./type_defs.md#shardfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetStreamOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetStreamInputPaginateTypeDef = {  # (1)
    "streamArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetStreamInputPaginateTypeDef](./type_defs.md#getstreaminputpaginatetypedef)
## ListStreamsPaginator

Type annotations and code completion for `#!python session.create_client("keyspacesstreams").get_paginator("list_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspacesstreams/paginator/ListStreams.html#KeyspacesStreams.Paginator.ListStreams)

```python
# ListStreamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_keyspacesstreams.paginator import ListStreamsPaginator

session = get_session()
async with session.create_client("keyspacesstreams") as client:  # (1)
    paginator: ListStreamsPaginator = client.get_paginator("list_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamsOutputTypeDef
        print(item)  # (3)
```

1. client: [KeyspacesStreamsClient](./client.md)
2. paginator: [ListStreamsPaginator](./paginators.md#liststreamspaginator)
3. item: `AioPageIterator[ListStreamsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStreamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    keyspaceName: str = ...,
    tableName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListStreamsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListStreamsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamsInputPaginateTypeDef = {  # (1)
    "keyspaceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamsInputPaginateTypeDef](./type_defs.md#liststreamsinputpaginatetypedef)
