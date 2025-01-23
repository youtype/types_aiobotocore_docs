# Paginators

> [Index](../README.md) > [SecurityLake](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SecurityLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#securitylake)
    type annotations stubs module [types-aiobotocore-securitylake](https://pypi.org/project/types-aiobotocore-securitylake/).

## GetDataLakeSourcesPaginator

Type annotations and code completion for `#!python session.create_client("securitylake").get_paginator("get_data_lake_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake/paginator/GetDataLakeSources.html#SecurityLake.Paginator.GetDataLakeSources)

```python
# GetDataLakeSourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securitylake.paginator import GetDataLakeSourcesPaginator

session = get_session()
async with session.create_client("securitylake") as client:  # (1)
    paginator: GetDataLakeSourcesPaginator = client.get_paginator("get_data_lake_sources")  # (2)
    async for item in paginator.paginate(...):
        item: GetDataLakeSourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityLakeClient](./client.md)
2. paginator: [GetDataLakeSourcesPaginator](./paginators.md#getdatalakesourcespaginator)
3. item: [:material-code-braces: GetDataLakeSourcesResponseTypeDef](./type_defs.md#getdatalakesourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetDataLakeSourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accounts: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetDataLakeSourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDataLakeSourcesResponseTypeDef](./type_defs.md#getdatalakesourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDataLakeSourcesRequestPaginateTypeDef = {  # (1)
    "accounts": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDataLakeSourcesRequestPaginateTypeDef](./type_defs.md#getdatalakesourcesrequestpaginatetypedef) 
## ListDataLakeExceptionsPaginator

Type annotations and code completion for `#!python session.create_client("securitylake").get_paginator("list_data_lake_exceptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake/paginator/ListDataLakeExceptions.html#SecurityLake.Paginator.ListDataLakeExceptions)

```python
# ListDataLakeExceptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securitylake.paginator import ListDataLakeExceptionsPaginator

session = get_session()
async with session.create_client("securitylake") as client:  # (1)
    paginator: ListDataLakeExceptionsPaginator = client.get_paginator("list_data_lake_exceptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataLakeExceptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityLakeClient](./client.md)
2. paginator: [ListDataLakeExceptionsPaginator](./paginators.md#listdatalakeexceptionspaginator)
3. item: [:material-code-braces: ListDataLakeExceptionsResponseTypeDef](./type_defs.md#listdatalakeexceptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataLakeExceptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    regions: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataLakeExceptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataLakeExceptionsResponseTypeDef](./type_defs.md#listdatalakeexceptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataLakeExceptionsRequestPaginateTypeDef = {  # (1)
    "regions": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataLakeExceptionsRequestPaginateTypeDef](./type_defs.md#listdatalakeexceptionsrequestpaginatetypedef) 
## ListLogSourcesPaginator

Type annotations and code completion for `#!python session.create_client("securitylake").get_paginator("list_log_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake/paginator/ListLogSources.html#SecurityLake.Paginator.ListLogSources)

```python
# ListLogSourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securitylake.paginator import ListLogSourcesPaginator

session = get_session()
async with session.create_client("securitylake") as client:  # (1)
    paginator: ListLogSourcesPaginator = client.get_paginator("list_log_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListLogSourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityLakeClient](./client.md)
2. paginator: [ListLogSourcesPaginator](./paginators.md#listlogsourcespaginator)
3. item: [:material-code-braces: ListLogSourcesResponseTypeDef](./type_defs.md#listlogsourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLogSourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accounts: Sequence[str] = ...,
    regions: Sequence[str] = ...,
    sources: Sequence[LogSourceResourceTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListLogSourcesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLogSourcesResponseTypeDef](./type_defs.md#listlogsourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLogSourcesRequestPaginateTypeDef = {  # (1)
    "accounts": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLogSourcesRequestPaginateTypeDef](./type_defs.md#listlogsourcesrequestpaginatetypedef) 
## ListSubscribersPaginator

Type annotations and code completion for `#!python session.create_client("securitylake").get_paginator("list_subscribers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake/paginator/ListSubscribers.html#SecurityLake.Paginator.ListSubscribers)

```python
# ListSubscribersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securitylake.paginator import ListSubscribersPaginator

session = get_session()
async with session.create_client("securitylake") as client:  # (1)
    paginator: ListSubscribersPaginator = client.get_paginator("list_subscribers")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscribersResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityLakeClient](./client.md)
2. paginator: [ListSubscribersPaginator](./paginators.md#listsubscriberspaginator)
3. item: [:material-code-braces: ListSubscribersResponseTypeDef](./type_defs.md#listsubscribersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscribersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSubscribersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscribersResponseTypeDef](./type_defs.md#listsubscribersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscribersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscribersRequestPaginateTypeDef](./type_defs.md#listsubscribersrequestpaginatetypedef) 
