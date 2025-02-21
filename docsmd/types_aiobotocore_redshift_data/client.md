# RedshiftDataAPIServiceClient

> [Index](../README.md) > [RedshiftDataAPIService](./README.md) > RedshiftDataAPIServiceClient

!!! note ""

    Auto-generated documentation for [RedshiftDataAPIService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#redshiftdataapiservice)
    type annotations stubs module [types-aiobotocore-redshift-data](https://pypi.org/project/types-aiobotocore-redshift-data/).

## RedshiftDataAPIServiceClient

Type annotations and code completion for `#!python session.create_client("redshift-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client)

```python
# RedshiftDataAPIServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_redshift_data.client import RedshiftDataAPIServiceClient

session = get_session()
async with session.create_client("redshift-data") as client:
    client: RedshiftDataAPIServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("redshift-data").exceptions` structure.

```python
# RedshiftDataAPIServiceClient.exceptions usage example

async with session.create_client("redshift-data") as client:
    try:
        do_something(client)
    except (
            client.ActiveSessionsExceededException,
        client.ActiveStatementsExceededException,
        client.BatchExecuteStatementException,
        client.ClientError,
        client.DatabaseConnectionException,
        client.ExecuteStatementException,
        client.InternalServerException,
        client.QueryTimeoutException,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# RedshiftDataAPIServiceClient usage type checking example

from types_aiobotocore_redshift_data.client import Exceptions

def handle_error(exc: Exceptions.ActiveSessionsExceededException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("redshift-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("redshift-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### batch\_execute\_statement

Runs one or more SQL statements, which can be data manipulation language (DML)
or data definition language (DDL).

Type annotations and code completion for `#!python session.create_client("redshift-data").batch_execute_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/batch_execute_statement.html)

```python
# batch_execute_statement method definition

await def batch_execute_statement(
    self,
    *,
    Sqls: Sequence[str],
    ClientToken: str = ...,
    ClusterIdentifier: str = ...,
    Database: str = ...,
    DbUser: str = ...,
    ResultFormat: ResultFormatStringType = ...,  # (1)
    SecretArn: str = ...,
    SessionId: str = ...,
    SessionKeepAliveSeconds: int = ...,
    StatementName: str = ...,
    WithEvent: bool = ...,
    WorkgroupName: str = ...,
) -> BatchExecuteStatementOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResultFormatStringType](./literals.md#resultformatstringtype) 
2. See [:material-code-braces: BatchExecuteStatementOutputTypeDef](./type_defs.md#batchexecutestatementoutputtypedef) 


```python
# batch_execute_statement method usage example with argument unpacking

kwargs: BatchExecuteStatementInputTypeDef = {  # (1)
    "Sqls": ...,
}

parent.batch_execute_statement(**kwargs)
```

1. See [:material-code-braces: BatchExecuteStatementInputTypeDef](./type_defs.md#batchexecutestatementinputtypedef) 

### cancel\_statement

Cancels a running query.

Type annotations and code completion for `#!python session.create_client("redshift-data").cancel_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/cancel_statement.html)

```python
# cancel_statement method definition

await def cancel_statement(
    self,
    *,
    Id: str,
) -> CancelStatementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelStatementResponseTypeDef](./type_defs.md#cancelstatementresponsetypedef) 


```python
# cancel_statement method usage example with argument unpacking

kwargs: CancelStatementRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.cancel_statement(**kwargs)
```

1. See [:material-code-braces: CancelStatementRequestTypeDef](./type_defs.md#cancelstatementrequesttypedef) 

### describe\_statement

Describes the details about a specific instance when a query was run by the
Amazon Redshift Data API.

Type annotations and code completion for `#!python session.create_client("redshift-data").describe_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/describe_statement.html)

```python
# describe_statement method definition

await def describe_statement(
    self,
    *,
    Id: str,
) -> DescribeStatementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStatementResponseTypeDef](./type_defs.md#describestatementresponsetypedef) 


```python
# describe_statement method usage example with argument unpacking

kwargs: DescribeStatementRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.describe_statement(**kwargs)
```

1. See [:material-code-braces: DescribeStatementRequestTypeDef](./type_defs.md#describestatementrequesttypedef) 

### describe\_table

Describes the detailed information about a table from metadata in the cluster.

Type annotations and code completion for `#!python session.create_client("redshift-data").describe_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/describe_table.html)

```python
# describe_table method definition

await def describe_table(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    ConnectedDatabase: str = ...,
    DbUser: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Schema: str = ...,
    SecretArn: str = ...,
    Table: str = ...,
    WorkgroupName: str = ...,
) -> DescribeTableResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTableResponseTypeDef](./type_defs.md#describetableresponsetypedef) 


```python
# describe_table method usage example with argument unpacking

kwargs: DescribeTableRequestTypeDef = {  # (1)
    "Database": ...,
}

parent.describe_table(**kwargs)
```

1. See [:material-code-braces: DescribeTableRequestTypeDef](./type_defs.md#describetablerequesttypedef) 

### execute\_statement

Runs an SQL statement, which can be data manipulation language (DML) or data
definition language (DDL).

Type annotations and code completion for `#!python session.create_client("redshift-data").execute_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/execute_statement.html)

```python
# execute_statement method definition

await def execute_statement(
    self,
    *,
    Sql: str,
    ClientToken: str = ...,
    ClusterIdentifier: str = ...,
    Database: str = ...,
    DbUser: str = ...,
    Parameters: Sequence[SqlParameterTypeDef] = ...,  # (1)
    ResultFormat: ResultFormatStringType = ...,  # (2)
    SecretArn: str = ...,
    SessionId: str = ...,
    SessionKeepAliveSeconds: int = ...,
    StatementName: str = ...,
    WithEvent: bool = ...,
    WorkgroupName: str = ...,
) -> ExecuteStatementOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
2. See [:material-code-brackets: ResultFormatStringType](./literals.md#resultformatstringtype) 
3. See [:material-code-braces: ExecuteStatementOutputTypeDef](./type_defs.md#executestatementoutputtypedef) 


```python
# execute_statement method usage example with argument unpacking

kwargs: ExecuteStatementInputTypeDef = {  # (1)
    "Sql": ...,
}

parent.execute_statement(**kwargs)
```

1. See [:material-code-braces: ExecuteStatementInputTypeDef](./type_defs.md#executestatementinputtypedef) 

### get\_statement\_result

Fetches the temporarily cached result of an SQL statement in JSON format.

Type annotations and code completion for `#!python session.create_client("redshift-data").get_statement_result` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/get_statement_result.html)

```python
# get_statement_result method definition

await def get_statement_result(
    self,
    *,
    Id: str,
    NextToken: str = ...,
) -> GetStatementResultResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStatementResultResponseTypeDef](./type_defs.md#getstatementresultresponsetypedef) 


```python
# get_statement_result method usage example with argument unpacking

kwargs: GetStatementResultRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_statement_result(**kwargs)
```

1. See [:material-code-braces: GetStatementResultRequestTypeDef](./type_defs.md#getstatementresultrequesttypedef) 

### get\_statement\_result\_v2

Fetches the temporarily cached result of an SQL statement in CSV format.

Type annotations and code completion for `#!python session.create_client("redshift-data").get_statement_result_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/get_statement_result_v2.html)

```python
# get_statement_result_v2 method definition

await def get_statement_result_v2(
    self,
    *,
    Id: str,
    NextToken: str = ...,
) -> GetStatementResultV2ResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStatementResultV2ResponseTypeDef](./type_defs.md#getstatementresultv2responsetypedef) 


```python
# get_statement_result_v2 method usage example with argument unpacking

kwargs: GetStatementResultV2RequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_statement_result_v2(**kwargs)
```

1. See [:material-code-braces: GetStatementResultV2RequestTypeDef](./type_defs.md#getstatementresultv2requesttypedef) 

### list\_databases

List the databases in a cluster.

Type annotations and code completion for `#!python session.create_client("redshift-data").list_databases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/list_databases.html)

```python
# list_databases method definition

await def list_databases(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    DbUser: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    SecretArn: str = ...,
    WorkgroupName: str = ...,
) -> ListDatabasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatabasesResponseTypeDef](./type_defs.md#listdatabasesresponsetypedef) 


```python
# list_databases method usage example with argument unpacking

kwargs: ListDatabasesRequestTypeDef = {  # (1)
    "Database": ...,
}

parent.list_databases(**kwargs)
```

1. See [:material-code-braces: ListDatabasesRequestTypeDef](./type_defs.md#listdatabasesrequesttypedef) 

### list\_schemas

Lists the schemas in a database.

Type annotations and code completion for `#!python session.create_client("redshift-data").list_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/list_schemas.html)

```python
# list_schemas method definition

await def list_schemas(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    ConnectedDatabase: str = ...,
    DbUser: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    SchemaPattern: str = ...,
    SecretArn: str = ...,
    WorkgroupName: str = ...,
) -> ListSchemasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python
# list_schemas method usage example with argument unpacking

kwargs: ListSchemasRequestTypeDef = {  # (1)
    "Database": ...,
}

parent.list_schemas(**kwargs)
```

1. See [:material-code-braces: ListSchemasRequestTypeDef](./type_defs.md#listschemasrequesttypedef) 

### list\_statements

List of SQL statements.

Type annotations and code completion for `#!python session.create_client("redshift-data").list_statements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/list_statements.html)

```python
# list_statements method definition

await def list_statements(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    RoleLevel: bool = ...,
    StatementName: str = ...,
    Status: StatusStringType = ...,  # (1)
) -> ListStatementsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatusStringType](./literals.md#statusstringtype) 
2. See [:material-code-braces: ListStatementsResponseTypeDef](./type_defs.md#liststatementsresponsetypedef) 


```python
# list_statements method usage example with argument unpacking

kwargs: ListStatementsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_statements(**kwargs)
```

1. See [:material-code-braces: ListStatementsRequestTypeDef](./type_defs.md#liststatementsrequesttypedef) 

### list\_tables

List the tables in a database.

Type annotations and code completion for `#!python session.create_client("redshift-data").list_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data/client/list_tables.html)

```python
# list_tables method definition

await def list_tables(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    ConnectedDatabase: str = ...,
    DbUser: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    SchemaPattern: str = ...,
    SecretArn: str = ...,
    TablePattern: str = ...,
    WorkgroupName: str = ...,
) -> ListTablesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef) 


```python
# list_tables method usage example with argument unpacking

kwargs: ListTablesRequestTypeDef = {  # (1)
    "Database": ...,
}

parent.list_tables(**kwargs)
```

1. See [:material-code-braces: ListTablesRequestTypeDef](./type_defs.md#listtablesrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("redshift-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("redshift-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("redshift-data").get_paginator` method with overloads.

- `client.get_paginator("describe_table")` -> [DescribeTablePaginator](./paginators.md#describetablepaginator)
- `client.get_paginator("get_statement_result")` -> [GetStatementResultPaginator](./paginators.md#getstatementresultpaginator)
- `client.get_paginator("get_statement_result_v2")` -> [GetStatementResultV2Paginator](./paginators.md#getstatementresultv2paginator)
- `client.get_paginator("list_databases")` -> [ListDatabasesPaginator](./paginators.md#listdatabasespaginator)
- `client.get_paginator("list_schemas")` -> [ListSchemasPaginator](./paginators.md#listschemaspaginator)
- `client.get_paginator("list_statements")` -> [ListStatementsPaginator](./paginators.md#liststatementspaginator)
- `client.get_paginator("list_tables")` -> [ListTablesPaginator](./paginators.md#listtablespaginator)



