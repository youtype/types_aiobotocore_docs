# Paginators

> [Index](../README.md) > [RedshiftDataAPIService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RedshiftDataAPIService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#redshiftdataapiservice)
    type annotations stubs module [types-aiobotocore-redshift-data](https://pypi.org/project/types-aiobotocore-redshift-data/).

## DescribeTablePaginator

Type annotations and code completion for `#!python session.create_client("redshift-data").get_paginator("describe_table")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/paginator/DescribeTable.html#RedshiftDataAPIService.Paginator.DescribeTable)

```python
# DescribeTablePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_data.paginator import DescribeTablePaginator

session = get_session()
async with session.create_client("redshift-data") as client:  # (1)
    paginator: DescribeTablePaginator = client.get_paginator("describe_table")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTableResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [DescribeTablePaginator](./paginators.md#describetablepaginator)
3. item: `AioPageIterator[DescribeTableResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTablePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    ConnectedDatabase: str = ...,
    DbUser: str = ...,
    Schema: str = ...,
    SecretArn: str = ...,
    Table: str = ...,
    WorkgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeTableResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeTableResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTableRequestPaginateTypeDef = {  # (1)
    "Database": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTableRequestPaginateTypeDef](./type_defs.md#describetablerequestpaginatetypedef)
## GetStatementResultPaginator

Type annotations and code completion for `#!python session.create_client("redshift-data").get_paginator("get_statement_result")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/paginator/GetStatementResult.html#RedshiftDataAPIService.Paginator.GetStatementResult)

```python
# GetStatementResultPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_data.paginator import GetStatementResultPaginator

session = get_session()
async with session.create_client("redshift-data") as client:  # (1)
    paginator: GetStatementResultPaginator = client.get_paginator("get_statement_result")  # (2)
    async for item in paginator.paginate(...):
        item: GetStatementResultResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [GetStatementResultPaginator](./paginators.md#getstatementresultpaginator)
3. item: `AioPageIterator[GetStatementResultResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetStatementResultPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetStatementResultResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetStatementResultResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetStatementResultRequestPaginateTypeDef = {  # (1)
    "Id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetStatementResultRequestPaginateTypeDef](./type_defs.md#getstatementresultrequestpaginatetypedef)
## GetStatementResultV2Paginator

Type annotations and code completion for `#!python session.create_client("redshift-data").get_paginator("get_statement_result_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/paginator/GetStatementResultV2.html#RedshiftDataAPIService.Paginator.GetStatementResultV2)

```python
# GetStatementResultV2Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_data.paginator import GetStatementResultV2Paginator

session = get_session()
async with session.create_client("redshift-data") as client:  # (1)
    paginator: GetStatementResultV2Paginator = client.get_paginator("get_statement_result_v2")  # (2)
    async for item in paginator.paginate(...):
        item: GetStatementResultV2ResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [GetStatementResultV2Paginator](./paginators.md#getstatementresultv2paginator)
3. item: `AioPageIterator[GetStatementResultV2ResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetStatementResultV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetStatementResultV2ResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetStatementResultV2ResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetStatementResultV2RequestPaginateTypeDef = {  # (1)
    "Id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetStatementResultV2RequestPaginateTypeDef](./type_defs.md#getstatementresultv2requestpaginatetypedef)
## ListDatabasesPaginator

Type annotations and code completion for `#!python session.create_client("redshift-data").get_paginator("list_databases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/paginator/ListDatabases.html#RedshiftDataAPIService.Paginator.ListDatabases)

```python
# ListDatabasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_data.paginator import ListDatabasesPaginator

session = get_session()
async with session.create_client("redshift-data") as client:  # (1)
    paginator: ListDatabasesPaginator = client.get_paginator("list_databases")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatabasesResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [ListDatabasesPaginator](./paginators.md#listdatabasespaginator)
3. item: `AioPageIterator[ListDatabasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDatabasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    DbUser: str = ...,
    SecretArn: str = ...,
    WorkgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDatabasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDatabasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDatabasesRequestPaginateTypeDef = {  # (1)
    "Database": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatabasesRequestPaginateTypeDef](./type_defs.md#listdatabasesrequestpaginatetypedef)
## ListSchemasPaginator

Type annotations and code completion for `#!python session.create_client("redshift-data").get_paginator("list_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/paginator/ListSchemas.html#RedshiftDataAPIService.Paginator.ListSchemas)

```python
# ListSchemasPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_data.paginator import ListSchemasPaginator

session = get_session()
async with session.create_client("redshift-data") as client:  # (1)
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [ListSchemasPaginator](./paginators.md#listschemaspaginator)
3. item: `AioPageIterator[ListSchemasResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSchemasPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    ConnectedDatabase: str = ...,
    DbUser: str = ...,
    SchemaPattern: str = ...,
    SecretArn: str = ...,
    WorkgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSchemasResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemasRequestPaginateTypeDef = {  # (1)
    "Database": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemasRequestPaginateTypeDef](./type_defs.md#listschemasrequestpaginatetypedef)
## ListStatementsPaginator

Type annotations and code completion for `#!python session.create_client("redshift-data").get_paginator("list_statements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/paginator/ListStatements.html#RedshiftDataAPIService.Paginator.ListStatements)

```python
# ListStatementsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_data.paginator import ListStatementsPaginator

session = get_session()
async with session.create_client("redshift-data") as client:  # (1)
    paginator: ListStatementsPaginator = client.get_paginator("list_statements")  # (2)
    async for item in paginator.paginate(...):
        item: ListStatementsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [ListStatementsPaginator](./paginators.md#liststatementspaginator)
3. item: `AioPageIterator[ListStatementsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStatementsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    Database: str = ...,
    RoleLevel: bool = ...,
    StatementName: str = ...,
    Status: StatusStringType = ...,  # (1)
    WorkgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListStatementsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: StatusStringType](./literals.md#statusstringtype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListStatementsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStatementsRequestPaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStatementsRequestPaginateTypeDef](./type_defs.md#liststatementsrequestpaginatetypedef)
## ListTablesPaginator

Type annotations and code completion for `#!python session.create_client("redshift-data").get_paginator("list_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/paginator/ListTables.html#RedshiftDataAPIService.Paginator.ListTables)

```python
# ListTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_data.paginator import ListTablesPaginator

session = get_session()
async with session.create_client("redshift-data") as client:  # (1)
    paginator: ListTablesPaginator = client.get_paginator("list_tables")  # (2)
    async for item in paginator.paginate(...):
        item: ListTablesResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [ListTablesPaginator](./paginators.md#listtablespaginator)
3. item: `AioPageIterator[ListTablesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    ConnectedDatabase: str = ...,
    DbUser: str = ...,
    SchemaPattern: str = ...,
    SecretArn: str = ...,
    TablePattern: str = ...,
    WorkgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTablesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTablesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTablesRequestPaginateTypeDef = {  # (1)
    "Database": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTablesRequestPaginateTypeDef](./type_defs.md#listtablesrequestpaginatetypedef)
