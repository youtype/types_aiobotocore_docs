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
async with session.create_client("athena") as client:
    client: AthenaClient
    paginator: GetQueryResultsPaginator = client.get_paginator("get_query_results")
```


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
async with session.create_client("athena") as client:
    client: AthenaClient
    paginator: ListDataCatalogsPaginator = client.get_paginator("list_data_catalogs")
```


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
async with session.create_client("athena") as client:
    client: AthenaClient
    paginator: ListDatabasesPaginator = client.get_paginator("list_databases")
```


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
async with session.create_client("athena") as client:
    client: AthenaClient
    paginator: ListNamedQueriesPaginator = client.get_paginator("list_named_queries")
```


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
async with session.create_client("athena") as client:
    client: AthenaClient
    paginator: ListQueryExecutionsPaginator = client.get_paginator("list_query_executions")
```


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
async with session.create_client("athena") as client:
    client: AthenaClient
    paginator: ListTableMetadataPaginator = client.get_paginator("list_table_metadata")
```


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
async with session.create_client("athena") as client:
    client: AthenaClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```


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
