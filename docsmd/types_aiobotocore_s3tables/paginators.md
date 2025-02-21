# Paginators

> [Index](../README.md) > [S3Tables](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [S3Tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#s3tables)
    type annotations stubs module [types-aiobotocore-s3tables](https://pypi.org/project/types-aiobotocore-s3tables/).

## ListNamespacesPaginator

Type annotations and code completion for `#!python session.create_client("s3tables").get_paginator("list_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/paginator/ListNamespaces.html#S3Tables.Paginator.ListNamespaces)

```python
# ListNamespacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3tables.paginator import ListNamespacesPaginator

session = get_session()
async with session.create_client("s3tables") as client:  # (1)
    paginator: ListNamespacesPaginator = client.get_paginator("list_namespaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListNamespacesResponseTypeDef
        print(item)  # (3)
```

1. client: [S3TablesClient](./client.md)
2. paginator: [ListNamespacesPaginator](./paginators.md#listnamespacespaginator)
3. item: [:material-code-braces: ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNamespacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    tableBucketARN: str,
    prefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListNamespacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNamespacesRequestPaginateTypeDef = {  # (1)
    "tableBucketARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNamespacesRequestPaginateTypeDef](./type_defs.md#listnamespacesrequestpaginatetypedef) 
## ListTableBucketsPaginator

Type annotations and code completion for `#!python session.create_client("s3tables").get_paginator("list_table_buckets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/paginator/ListTableBuckets.html#S3Tables.Paginator.ListTableBuckets)

```python
# ListTableBucketsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3tables.paginator import ListTableBucketsPaginator

session = get_session()
async with session.create_client("s3tables") as client:  # (1)
    paginator: ListTableBucketsPaginator = client.get_paginator("list_table_buckets")  # (2)
    async for item in paginator.paginate(...):
        item: ListTableBucketsResponseTypeDef
        print(item)  # (3)
```

1. client: [S3TablesClient](./client.md)
2. paginator: [ListTableBucketsPaginator](./paginators.md#listtablebucketspaginator)
3. item: [:material-code-braces: ListTableBucketsResponseTypeDef](./type_defs.md#listtablebucketsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTableBucketsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    prefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTableBucketsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTableBucketsResponseTypeDef](./type_defs.md#listtablebucketsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTableBucketsRequestPaginateTypeDef = {  # (1)
    "prefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTableBucketsRequestPaginateTypeDef](./type_defs.md#listtablebucketsrequestpaginatetypedef) 
## ListTablesPaginator

Type annotations and code completion for `#!python session.create_client("s3tables").get_paginator("list_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables/paginator/ListTables.html#S3Tables.Paginator.ListTables)

```python
# ListTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3tables.paginator import ListTablesPaginator

session = get_session()
async with session.create_client("s3tables") as client:  # (1)
    paginator: ListTablesPaginator = client.get_paginator("list_tables")  # (2)
    async for item in paginator.paginate(...):
        item: ListTablesResponseTypeDef
        print(item)  # (3)
```

1. client: [S3TablesClient](./client.md)
2. paginator: [ListTablesPaginator](./paginators.md#listtablespaginator)
3. item: [:material-code-braces: ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    tableBucketARN: str,
    namespace: str = ...,
    prefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTablesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTablesRequestPaginateTypeDef = {  # (1)
    "tableBucketARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTablesRequestPaginateTypeDef](./type_defs.md#listtablesrequestpaginatetypedef) 
