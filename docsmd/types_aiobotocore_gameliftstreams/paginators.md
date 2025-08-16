# Paginators

> [Index](../README.md) > [GameLiftStreams](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GameLiftStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams.html#gameliftstreams)
    type annotations stubs module [types-aiobotocore-gameliftstreams](https://pypi.org/project/types-aiobotocore-gameliftstreams/).

## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("gameliftstreams").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/paginator/ListApplications.html#GameLiftStreams.Paginator.ListApplications)

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gameliftstreams.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("gameliftstreams") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftStreamsClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: `AioPageIterator[ListApplicationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListApplicationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListApplicationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsInputPaginateTypeDef](./type_defs.md#listapplicationsinputpaginatetypedef)
## ListStreamGroupsPaginator

Type annotations and code completion for `#!python session.create_client("gameliftstreams").get_paginator("list_stream_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/paginator/ListStreamGroups.html#GameLiftStreams.Paginator.ListStreamGroups)

```python
# ListStreamGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gameliftstreams.paginator import ListStreamGroupsPaginator

session = get_session()
async with session.create_client("gameliftstreams") as client:  # (1)
    paginator: ListStreamGroupsPaginator = client.get_paginator("list_stream_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftStreamsClient](./client.md)
2. paginator: [ListStreamGroupsPaginator](./paginators.md#liststreamgroupspaginator)
3. item: `AioPageIterator[ListStreamGroupsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStreamGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListStreamGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListStreamGroupsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamGroupsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamGroupsInputPaginateTypeDef](./type_defs.md#liststreamgroupsinputpaginatetypedef)
## ListStreamSessionsByAccountPaginator

Type annotations and code completion for `#!python session.create_client("gameliftstreams").get_paginator("list_stream_sessions_by_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/paginator/ListStreamSessionsByAccount.html#GameLiftStreams.Paginator.ListStreamSessionsByAccount)

```python
# ListStreamSessionsByAccountPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gameliftstreams.paginator import ListStreamSessionsByAccountPaginator

session = get_session()
async with session.create_client("gameliftstreams") as client:  # (1)
    paginator: ListStreamSessionsByAccountPaginator = client.get_paginator("list_stream_sessions_by_account")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamSessionsByAccountOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftStreamsClient](./client.md)
2. paginator: [ListStreamSessionsByAccountPaginator](./paginators.md#liststreamsessionsbyaccountpaginator)
3. item: `AioPageIterator[ListStreamSessionsByAccountOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStreamSessionsByAccountPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Status: StreamSessionStatusType = ...,  # (1)
    ExportFilesStatus: ExportFilesStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListStreamSessionsByAccountOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: StreamSessionStatusType](./literals.md#streamsessionstatustype)
2. See [:material-code-brackets: ExportFilesStatusType](./literals.md#exportfilesstatustype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListStreamSessionsByAccountOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamSessionsByAccountInputPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamSessionsByAccountInputPaginateTypeDef](./type_defs.md#liststreamsessionsbyaccountinputpaginatetypedef)
## ListStreamSessionsPaginator

Type annotations and code completion for `#!python session.create_client("gameliftstreams").get_paginator("list_stream_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/paginator/ListStreamSessions.html#GameLiftStreams.Paginator.ListStreamSessions)

```python
# ListStreamSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gameliftstreams.paginator import ListStreamSessionsPaginator

session = get_session()
async with session.create_client("gameliftstreams") as client:  # (1)
    paginator: ListStreamSessionsPaginator = client.get_paginator("list_stream_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamSessionsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftStreamsClient](./client.md)
2. paginator: [ListStreamSessionsPaginator](./paginators.md#liststreamsessionspaginator)
3. item: `AioPageIterator[ListStreamSessionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStreamSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Identifier: str,
    Status: StreamSessionStatusType = ...,  # (1)
    ExportFilesStatus: ExportFilesStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListStreamSessionsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: StreamSessionStatusType](./literals.md#streamsessionstatustype)
2. See [:material-code-brackets: ExportFilesStatusType](./literals.md#exportfilesstatustype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListStreamSessionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamSessionsInputPaginateTypeDef = {  # (1)
    "Identifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamSessionsInputPaginateTypeDef](./type_defs.md#liststreamsessionsinputpaginatetypedef)
