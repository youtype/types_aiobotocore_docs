# Paginators

> [Index](../README.md) > [Athena](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Athena](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
    type annotations stubs module [types-aiobotocore-athena](https://pypi.org/project/types-aiobotocore-athena/).

## GetQueryResultsPaginator

Type annotations and code completion for `#!python session.create_client("athena").get_paginator("get_query_results")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_athena.paginator import GetQueryResultsPaginator

session = get_session()
async with session.create_client("athena") as client:  # (1)
    paginator: GetQueryResultsPaginator = client.get_paginator("get_query_results")  # (2)
    async for item in paginator.paginate(...):
        item: GetQueryResultsOutputTypeDef
        print(item)  # (3)
```

1. client: [AthenaClient](./client.md)
2. paginator: [GetQueryResultsPaginator](./paginators.md#getqueryresultspaginator)
3. item: [:material-code-braces: GetQueryResultsOutputTypeDef](./type_defs.md#getqueryresultsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python GetQueryResultsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    QueryExecutionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetQueryResultsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetQueryResultsOutputTypeDef](./type_defs.md#getqueryresultsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetQueryResultsInputGetQueryResultsPaginateTypeDef = {  # (1)
    "QueryExecutionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetQueryResultsInputGetQueryResultsPaginateTypeDef](./type_defs.md#getqueryresultsinputgetqueryresultspaginatetypedef) 
## ListDataCatalogsPaginator

Type annotations and code completion for `#!python session.create_client("athena").get_paginator("list_data_catalogs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_athena.paginator import ListDataCatalogsPaginator

session = get_session()
async with session.create_client("athena") as client:  # (1)
    paginator: ListDataCatalogsPaginator = client.get_paginator("list_data_catalogs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataCatalogsOutputTypeDef
        print(item)  # (3)
```

1. client: [AthenaClient](./client.md)
2. paginator: [ListDataCatalogsPaginator](./paginators.md#listdatacatalogspaginator)
3. item: [:material-code-braces: ListDataCatalogsOutputTypeDef](./type_defs.md#listdatacatalogsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDataCatalogsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDataCatalogsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataCatalogsOutputTypeDef](./type_defs.md#listdatacatalogsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListDataCatalogsInputListDataCatalogsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataCatalogsInputListDataCatalogsPaginateTypeDef](./type_defs.md#listdatacatalogsinputlistdatacatalogspaginatetypedef) 
## ListDatabasesPaginator

Type annotations and code completion for `#!python session.create_client("athena").get_paginator("list_databases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_athena.paginator import ListDatabasesPaginator

session = get_session()
async with session.create_client("athena") as client:  # (1)
    paginator: ListDatabasesPaginator = client.get_paginator("list_databases")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatabasesOutputTypeDef
        print(item)  # (3)
```

1. client: [AthenaClient](./client.md)
2. paginator: [ListDatabasesPaginator](./paginators.md#listdatabasespaginator)
3. item: [:material-code-braces: ListDatabasesOutputTypeDef](./type_defs.md#listdatabasesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDatabasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CatalogName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatabasesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatabasesOutputTypeDef](./type_defs.md#listdatabasesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatabasesInputListDatabasesPaginateTypeDef = {  # (1)
    "CatalogName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatabasesInputListDatabasesPaginateTypeDef](./type_defs.md#listdatabasesinputlistdatabasespaginatetypedef) 
## ListNamedQueriesPaginator

Type annotations and code completion for `#!python session.create_client("athena").get_paginator("list_named_queries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_athena.paginator import ListNamedQueriesPaginator

session = get_session()
async with session.create_client("athena") as client:  # (1)
    paginator: ListNamedQueriesPaginator = client.get_paginator("list_named_queries")  # (2)
    async for item in paginator.paginate(...):
        item: ListNamedQueriesOutputTypeDef
        print(item)  # (3)
```

1. client: [AthenaClient](./client.md)
2. paginator: [ListNamedQueriesPaginator](./paginators.md#listnamedqueriespaginator)
3. item: [:material-code-braces: ListNamedQueriesOutputTypeDef](./type_defs.md#listnamedqueriesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListNamedQueriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    WorkGroup: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListNamedQueriesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNamedQueriesOutputTypeDef](./type_defs.md#listnamedqueriesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListNamedQueriesInputListNamedQueriesPaginateTypeDef = {  # (1)
    "WorkGroup": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNamedQueriesInputListNamedQueriesPaginateTypeDef](./type_defs.md#listnamedqueriesinputlistnamedqueriespaginatetypedef) 
## ListQueryExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("athena").get_paginator("list_query_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_athena.paginator import ListQueryExecutionsPaginator

session = get_session()
async with session.create_client("athena") as client:  # (1)
    paginator: ListQueryExecutionsPaginator = client.get_paginator("list_query_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueryExecutionsOutputTypeDef
        print(item)  # (3)
```

1. client: [AthenaClient](./client.md)
2. paginator: [ListQueryExecutionsPaginator](./paginators.md#listqueryexecutionspaginator)
3. item: [:material-code-braces: ListQueryExecutionsOutputTypeDef](./type_defs.md#listqueryexecutionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListQueryExecutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    WorkGroup: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListQueryExecutionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQueryExecutionsOutputTypeDef](./type_defs.md#listqueryexecutionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = {  # (1)
    "WorkGroup": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef](./type_defs.md#listqueryexecutionsinputlistqueryexecutionspaginatetypedef) 
## ListTableMetadataPaginator

Type annotations and code completion for `#!python session.create_client("athena").get_paginator("list_table_metadata")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_athena.paginator import ListTableMetadataPaginator

session = get_session()
async with session.create_client("athena") as client:  # (1)
    paginator: ListTableMetadataPaginator = client.get_paginator("list_table_metadata")  # (2)
    async for item in paginator.paginate(...):
        item: ListTableMetadataOutputTypeDef
        print(item)  # (3)
```

1. client: [AthenaClient](./client.md)
2. paginator: [ListTableMetadataPaginator](./paginators.md#listtablemetadatapaginator)
3. item: [:material-code-braces: ListTableMetadataOutputTypeDef](./type_defs.md#listtablemetadataoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTableMetadataPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CatalogName: str,
    DatabaseName: str,
    Expression: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTableMetadataOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTableMetadataOutputTypeDef](./type_defs.md#listtablemetadataoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListTableMetadataInputListTableMetadataPaginateTypeDef = {  # (1)
    "CatalogName": ...,
    "DatabaseName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTableMetadataInputListTableMetadataPaginateTypeDef](./type_defs.md#listtablemetadatainputlisttablemetadatapaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("athena").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_athena.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("athena") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceOutputTypeDef
        print(item)  # (3)
```

1. client: [AthenaClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceARN: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceInputListTagsForResourcePaginateTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourceinputlisttagsforresourcepaginatetypedef) 
