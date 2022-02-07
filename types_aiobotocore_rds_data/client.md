<a id="rdsdataserviceclient-for-aiobotocore-rdsdataservice-module"></a>

# RDSDataServiceClient for aiobotocore RDSDataService module

> [Index](..) > [RDSDataService](.) > RDSDataServiceClient

Auto-generated documentation for
[RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
type annotations stubs module
[types-aiobotocore-rds-data](https://pypi.org/project/types-aiobotocore-rds-data/).

- [RDSDataServiceClient for aiobotocore RDSDataService module](#rdsdataserviceclient-for-aiobotocore-rdsdataservice-module)
  - [RDSDataServiceClient](#rdsdataserviceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [batch_execute_statement](#batch_execute_statement)
    - [begin_transaction](#begin_transaction)
    - [can_paginate](#can_paginate)
    - [commit_transaction](#commit_transaction)
    - [execute_sql](#execute_sql)
    - [execute_statement](#execute_statement)
    - [generate_presigned_url](#generate_presigned_url)
    - [rollback_transaction](#rollback_transaction)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="rdsdataserviceclient"></a>

## RDSDataServiceClient

Type annotations for `session.create_client("rds-data")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_rds_data.client import RDSDataServiceClient

session = get_session()
async with session.create_client("rds-data") as client:
    client: RDSDataServiceClient
```

Boto3 documentation:
[RDSDataService.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_rds_data.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.NotFoundException`
- `Exceptions.ServiceUnavailableError`
- `Exceptions.StatementTimeoutException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

RDSDataServiceClient exceptions.

Type annotations for `session.create_client("rds-data").exceptions` method.

Boto3 documentation:
[RDSDataService.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="batch_execute_statement"></a>

### batch_execute_statement

Runs a batch SQL statement over an array of data.

Type annotations for
`session.create_client("rds-data").batch_execute_statement` method.

Boto3 documentation:
[RDSDataService.Client.batch_execute_statement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.batch_execute_statement)

Asynchronous method. Use `await batch_execute_statement(...)` for a synchronous
call.

Arguments mapping described in
[BatchExecuteStatementRequestRequestTypeDef](./type_defs.md#batchexecutestatementrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `secretArn`: `str` *(required)*
- `sql`: `str` *(required)*
- `database`: `str`
- `parameterSets`:
  `Sequence`\[`Sequence`\[[SqlParameterTypeDef](./type_defs.md#sqlparametertypedef)\]\]
- `schema`: `str`
- `transactionId`: `str`

Returns a `Coroutine` for
[BatchExecuteStatementResponseTypeDef](./type_defs.md#batchexecutestatementresponsetypedef).

<a id="begin_transaction"></a>

### begin_transaction

Starts a SQL transaction.

Type annotations for `session.create_client("rds-data").begin_transaction`
method.

Boto3 documentation:
[RDSDataService.Client.begin_transaction](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.begin_transaction)

Asynchronous method. Use `await begin_transaction(...)` for a synchronous call.

Arguments mapping described in
[BeginTransactionRequestRequestTypeDef](./type_defs.md#begintransactionrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `secretArn`: `str` *(required)*
- `database`: `str`
- `schema`: `str`

Returns a `Coroutine` for
[BeginTransactionResponseTypeDef](./type_defs.md#begintransactionresponsetypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("rds-data").can_paginate` method.

Boto3 documentation:
[RDSDataService.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="commit_transaction"></a>

### commit_transaction

Ends a SQL transaction started with the `BeginTransaction` operation and
commits the changes.

Type annotations for `session.create_client("rds-data").commit_transaction`
method.

Boto3 documentation:
[RDSDataService.Client.commit_transaction](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.commit_transaction)

Asynchronous method. Use `await commit_transaction(...)` for a synchronous
call.

Arguments mapping described in
[CommitTransactionRequestRequestTypeDef](./type_defs.md#committransactionrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `secretArn`: `str` *(required)*
- `transactionId`: `str` *(required)*

Returns a `Coroutine` for
[CommitTransactionResponseTypeDef](./type_defs.md#committransactionresponsetypedef).

<a id="execute_sql"></a>

### execute_sql

Runs one or more SQL statements.

Type annotations for `session.create_client("rds-data").execute_sql` method.

Boto3 documentation:
[RDSDataService.Client.execute_sql](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.execute_sql)

Asynchronous method. Use `await execute_sql(...)` for a synchronous call.

Arguments mapping described in
[ExecuteSqlRequestRequestTypeDef](./type_defs.md#executesqlrequestrequesttypedef).

Keyword-only arguments:

- `awsSecretStoreArn`: `str` *(required)*
- `dbClusterOrInstanceArn`: `str` *(required)*
- `sqlStatements`: `str` *(required)*
- `database`: `str`
- `schema`: `str`

Returns a `Coroutine` for
[ExecuteSqlResponseTypeDef](./type_defs.md#executesqlresponsetypedef).

<a id="execute_statement"></a>

### execute_statement

Runs a SQL statement against a database.

Type annotations for `session.create_client("rds-data").execute_statement`
method.

Boto3 documentation:
[RDSDataService.Client.execute_statement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.execute_statement)

Asynchronous method. Use `await execute_statement(...)` for a synchronous call.

Arguments mapping described in
[ExecuteStatementRequestRequestTypeDef](./type_defs.md#executestatementrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `secretArn`: `str` *(required)*
- `sql`: `str` *(required)*
- `continueAfterTimeout`: `bool`
- `database`: `str`
- `includeResultMetadata`: `bool`
- `parameters`:
  `Sequence`\[[SqlParameterTypeDef](./type_defs.md#sqlparametertypedef)\]
- `resultSetOptions`:
  [ResultSetOptionsTypeDef](./type_defs.md#resultsetoptionstypedef)
- `schema`: `str`
- `transactionId`: `str`

Returns a `Coroutine` for
[ExecuteStatementResponseTypeDef](./type_defs.md#executestatementresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("rds-data").generate_presigned_url`
method.

Boto3 documentation:
[RDSDataService.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="rollback_transaction"></a>

### rollback_transaction

Performs a rollback of a transaction.

Type annotations for `session.create_client("rds-data").rollback_transaction`
method.

Boto3 documentation:
[RDSDataService.Client.rollback_transaction](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.rollback_transaction)

Asynchronous method. Use `await rollback_transaction(...)` for a synchronous
call.

Arguments mapping described in
[RollbackTransactionRequestRequestTypeDef](./type_defs.md#rollbacktransactionrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `secretArn`: `str` *(required)*
- `transactionId`: `str` *(required)*

Returns a `Coroutine` for
[RollbackTransactionResponseTypeDef](./type_defs.md#rollbacktransactionresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("rds-data").__aenter__` method.

Boto3 documentation:
[RDSDataService.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [RDSDataServiceClient](#rdsdataserviceclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("rds-data").__aexit__` method.

Boto3 documentation:
[RDSDataService.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
