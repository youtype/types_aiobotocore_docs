<a id="redshiftdataapiserviceclient-for-aiobotocore-redshiftdataapiservice-module"></a>

# RedshiftDataAPIServiceClient for aiobotocore RedshiftDataAPIService module

> [Index](../README.md) > [RedshiftDataAPIService](./README.md) >
> RedshiftDataAPIServiceClient

Auto-generated documentation for
[RedshiftDataAPIService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
type annotations stubs module
[types-aiobotocore-redshift-data](https://pypi.org/project/types-aiobotocore-redshift-data/).

- [RedshiftDataAPIServiceClient for aiobotocore RedshiftDataAPIService module](#redshiftdataapiserviceclient-for-aiobotocore-redshiftdataapiservice-module)
  - [RedshiftDataAPIServiceClient](#redshiftdataapiserviceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [batch_execute_statement](#batch_execute_statement)
    - [can_paginate](#can_paginate)
    - [cancel_statement](#cancel_statement)
    - [describe_statement](#describe_statement)
    - [describe_table](#describe_table)
    - [execute_statement](#execute_statement)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_statement_result](#get_statement_result)
    - [list_databases](#list_databases)
    - [list_schemas](#list_schemas)
    - [list_statements](#list_statements)
    - [list_tables](#list_tables)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="redshiftdataapiserviceclient"></a>

## RedshiftDataAPIServiceClient

Type annotations for `session.create_client("redshift-data")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_redshift_data.client import RedshiftDataAPIServiceClient

session = get_session()
async with session.create_client("redshift-data") as client:
    client: RedshiftDataAPIServiceClient
```

Boto3 documentation:
[RedshiftDataAPIService.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_redshift_data.client import Exceptions

def handle_error(exc: Exceptions.ActiveStatementsExceededException) -> None:
    ...
```

Exceptions:

- `Exceptions.ActiveStatementsExceededException`
- `Exceptions.BatchExecuteStatementException`
- `Exceptions.ClientError`
- `Exceptions.DatabaseConnectionException`
- `Exceptions.ExecuteStatementException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

RedshiftDataAPIServiceClient exceptions.

Type annotations for `session.create_client("redshift-data").exceptions`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="batch\_execute\_statement"></a>

### batch_execute_statement

Runs one or more SQL statements, which can be data manipulation language (DML)
or data definition language (DDL).

Type annotations for
`session.create_client("redshift-data").batch_execute_statement` method.

Boto3 documentation:
[RedshiftDataAPIService.Client.batch_execute_statement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.batch_execute_statement)

Asynchronous method. Use `await batch_execute_statement(...)` for a synchronous
call.

Arguments mapping described in
[BatchExecuteStatementInputRequestTypeDef](./type_defs.md#batchexecutestatementinputrequesttypedef).

Keyword-only arguments:

- `Database`: `str` *(required)*
- `Sqls`: `Sequence`\[`str`\] *(required)*
- `ClusterIdentifier`: `str`
- `DbUser`: `str`
- `SecretArn`: `str`
- `StatementName`: `str`
- `WithEvent`: `bool`

Returns a `Coroutine` for
[BatchExecuteStatementOutputTypeDef](./type_defs.md#batchexecutestatementoutputtypedef).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("redshift-data").can_paginate`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_statement"></a>

### cancel_statement

Cancels a running query.

Type annotations for `session.create_client("redshift-data").cancel_statement`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.cancel_statement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.cancel_statement)

Asynchronous method. Use `await cancel_statement(...)` for a synchronous call.

Arguments mapping described in
[CancelStatementRequestRequestTypeDef](./type_defs.md#cancelstatementrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[CancelStatementResponseTypeDef](./type_defs.md#cancelstatementresponsetypedef).

<a id="describe\_statement"></a>

### describe_statement

Describes the details about a specific instance when a query was run by the
Amazon Redshift Data API.

Type annotations for
`session.create_client("redshift-data").describe_statement` method.

Boto3 documentation:
[RedshiftDataAPIService.Client.describe_statement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.describe_statement)

Asynchronous method. Use `await describe_statement(...)` for a synchronous
call.

Arguments mapping described in
[DescribeStatementRequestRequestTypeDef](./type_defs.md#describestatementrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[DescribeStatementResponseTypeDef](./type_defs.md#describestatementresponsetypedef).

<a id="describe\_table"></a>

### describe_table

Describes the detailed information about a table from metadata in the cluster.

Type annotations for `session.create_client("redshift-data").describe_table`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.describe_table](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.describe_table)

Asynchronous method. Use `await describe_table(...)` for a synchronous call.

Arguments mapping described in
[DescribeTableRequestRequestTypeDef](./type_defs.md#describetablerequestrequesttypedef).

Keyword-only arguments:

- `Database`: `str` *(required)*
- `ClusterIdentifier`: `str`
- `ConnectedDatabase`: `str`
- `DbUser`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`
- `Schema`: `str`
- `SecretArn`: `str`
- `Table`: `str`

Returns a `Coroutine` for
[DescribeTableResponseTypeDef](./type_defs.md#describetableresponsetypedef).

<a id="execute\_statement"></a>

### execute_statement

Runs an SQL statement, which can be data manipulation language (DML) or data
definition language (DDL).

Type annotations for `session.create_client("redshift-data").execute_statement`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.execute_statement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.execute_statement)

Asynchronous method. Use `await execute_statement(...)` for a synchronous call.

Arguments mapping described in
[ExecuteStatementInputRequestTypeDef](./type_defs.md#executestatementinputrequesttypedef).

Keyword-only arguments:

- `Database`: `str` *(required)*
- `Sql`: `str` *(required)*
- `ClusterIdentifier`: `str`
- `DbUser`: `str`
- `Parameters`:
  `Sequence`\[[SqlParameterTypeDef](./type_defs.md#sqlparametertypedef)\]
- `SecretArn`: `str`
- `StatementName`: `str`
- `WithEvent`: `bool`

Returns a `Coroutine` for
[ExecuteStatementOutputTypeDef](./type_defs.md#executestatementoutputtypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("redshift-data").generate_presigned_url` method.

Boto3 documentation:
[RedshiftDataAPIService.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_statement\_result"></a>

### get_statement_result

Fetches the temporarily cached result of an SQL statement.

Type annotations for
`session.create_client("redshift-data").get_statement_result` method.

Boto3 documentation:
[RedshiftDataAPIService.Client.get_statement_result](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.get_statement_result)

Asynchronous method. Use `await get_statement_result(...)` for a synchronous
call.

Arguments mapping described in
[GetStatementResultRequestRequestTypeDef](./type_defs.md#getstatementresultrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `NextToken`: `str`

Returns a `Coroutine` for
[GetStatementResultResponseTypeDef](./type_defs.md#getstatementresultresponsetypedef).

<a id="list\_databases"></a>

### list_databases

List the databases in a cluster.

Type annotations for `session.create_client("redshift-data").list_databases`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.list_databases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_databases)

Asynchronous method. Use `await list_databases(...)` for a synchronous call.

Arguments mapping described in
[ListDatabasesRequestRequestTypeDef](./type_defs.md#listdatabasesrequestrequesttypedef).

Keyword-only arguments:

- `Database`: `str` *(required)*
- `ClusterIdentifier`: `str`
- `DbUser`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`
- `SecretArn`: `str`

Returns a `Coroutine` for
[ListDatabasesResponseTypeDef](./type_defs.md#listdatabasesresponsetypedef).

<a id="list\_schemas"></a>

### list_schemas

Lists the schemas in a database.

Type annotations for `session.create_client("redshift-data").list_schemas`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.list_schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_schemas)

Asynchronous method. Use `await list_schemas(...)` for a synchronous call.

Arguments mapping described in
[ListSchemasRequestRequestTypeDef](./type_defs.md#listschemasrequestrequesttypedef).

Keyword-only arguments:

- `Database`: `str` *(required)*
- `ClusterIdentifier`: `str`
- `ConnectedDatabase`: `str`
- `DbUser`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`
- `SchemaPattern`: `str`
- `SecretArn`: `str`

Returns a `Coroutine` for
[ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef).

<a id="list\_statements"></a>

### list_statements

List of SQL statements.

Type annotations for `session.create_client("redshift-data").list_statements`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.list_statements](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_statements)

Asynchronous method. Use `await list_statements(...)` for a synchronous call.

Arguments mapping described in
[ListStatementsRequestRequestTypeDef](./type_defs.md#liststatementsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `RoleLevel`: `bool`
- `StatementName`: `str`
- `Status`: [StatusStringType](./literals.md#statusstringtype)

Returns a `Coroutine` for
[ListStatementsResponseTypeDef](./type_defs.md#liststatementsresponsetypedef).

<a id="list\_tables"></a>

### list_tables

List the tables in a database.

Type annotations for `session.create_client("redshift-data").list_tables`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.list_tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_tables)

Asynchronous method. Use `await list_tables(...)` for a synchronous call.

Arguments mapping described in
[ListTablesRequestRequestTypeDef](./type_defs.md#listtablesrequestrequesttypedef).

Keyword-only arguments:

- `Database`: `str` *(required)*
- `ClusterIdentifier`: `str`
- `ConnectedDatabase`: `str`
- `DbUser`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`
- `SchemaPattern`: `str`
- `SecretArn`: `str`
- `TablePattern`: `str`

Returns a `Coroutine` for
[ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("redshift-data").__aenter__`
method.

Boto3 documentation:
[RedshiftDataAPIService.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[RedshiftDataAPIServiceClient](#redshiftdataapiserviceclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("redshift-data").__aexit__` method.

Boto3 documentation:
[RedshiftDataAPIService.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("redshift-data").get_paginator`
method with overloads.

- `client.get_paginator("describe_table")` ->
  [DescribeTablePaginator](./paginators.md#describetablepaginator)
- `client.get_paginator("get_statement_result")` ->
  [GetStatementResultPaginator](./paginators.md#getstatementresultpaginator)
- `client.get_paginator("list_databases")` ->
  [ListDatabasesPaginator](./paginators.md#listdatabasespaginator)
- `client.get_paginator("list_schemas")` ->
  [ListSchemasPaginator](./paginators.md#listschemaspaginator)
- `client.get_paginator("list_statements")` ->
  [ListStatementsPaginator](./paginators.md#liststatementspaginator)
- `client.get_paginator("list_tables")` ->
  [ListTablesPaginator](./paginators.md#listtablespaginator)
