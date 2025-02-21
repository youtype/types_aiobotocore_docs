# RDSDataServiceClient

> [Index](../README.md) > [RDSDataService](./README.md) > RDSDataServiceClient

!!! note ""

    Auto-generated documentation for [RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#rdsdataservice)
    type annotations stubs module [types-aiobotocore-rds-data](https://pypi.org/project/types-aiobotocore-rds-data/).

## RDSDataServiceClient

Type annotations and code completion for `#!python session.create_client("rds-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client)

```python
# RDSDataServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_rds_data.client import RDSDataServiceClient

session = get_session()
async with session.create_client("rds-data") as client:
    client: RDSDataServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("rds-data").exceptions` structure.

```python
# RDSDataServiceClient.exceptions usage example

async with session.create_client("rds-data") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.DatabaseErrorException,
        client.DatabaseNotFoundException,
        client.DatabaseResumingException,
        client.DatabaseUnavailableException,
        client.ForbiddenException,
        client.HttpEndpointNotEnabledException,
        client.InternalServerErrorException,
        client.InvalidResourceStateException,
        client.InvalidSecretException,
        client.NotFoundException,
        client.SecretsErrorException,
        client.ServiceUnavailableError,
        client.StatementTimeoutException,
        client.TransactionNotFoundException,
        client.UnsupportedResultException,
    ) as e:
        print(e)
```

```python
# RDSDataServiceClient usage type checking example

from types_aiobotocore_rds_data.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("rds-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("rds-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data/client/generate_presigned_url.html)

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

Runs a batch SQL statement over an array of data.

Type annotations and code completion for `#!python session.create_client("rds-data").batch_execute_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data/client/batch_execute_statement.html)

```python
# batch_execute_statement method definition

await def batch_execute_statement(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    sql: str,
    database: str = ...,
    schema: str = ...,
    parameterSets: Sequence[Sequence[SqlParameterTypeDef]] = ...,  # (1)
    transactionId: str = ...,
) -> BatchExecuteStatementResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
2. See [:material-code-braces: BatchExecuteStatementResponseTypeDef](./type_defs.md#batchexecutestatementresponsetypedef) 


```python
# batch_execute_statement method usage example with argument unpacking

kwargs: BatchExecuteStatementRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
    "sql": ...,
}

parent.batch_execute_statement(**kwargs)
```

1. See [:material-code-braces: BatchExecuteStatementRequestTypeDef](./type_defs.md#batchexecutestatementrequesttypedef) 

### begin\_transaction

Starts a SQL transaction.

Type annotations and code completion for `#!python session.create_client("rds-data").begin_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data/client/begin_transaction.html)

```python
# begin_transaction method definition

await def begin_transaction(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    database: str = ...,
    schema: str = ...,
) -> BeginTransactionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BeginTransactionResponseTypeDef](./type_defs.md#begintransactionresponsetypedef) 


```python
# begin_transaction method usage example with argument unpacking

kwargs: BeginTransactionRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
}

parent.begin_transaction(**kwargs)
```

1. See [:material-code-braces: BeginTransactionRequestTypeDef](./type_defs.md#begintransactionrequesttypedef) 

### commit\_transaction

Ends a SQL transaction started with the <code>BeginTransaction</code> operation
and commits the changes.

Type annotations and code completion for `#!python session.create_client("rds-data").commit_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data/client/commit_transaction.html)

```python
# commit_transaction method definition

await def commit_transaction(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    transactionId: str,
) -> CommitTransactionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CommitTransactionResponseTypeDef](./type_defs.md#committransactionresponsetypedef) 


```python
# commit_transaction method usage example with argument unpacking

kwargs: CommitTransactionRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
    "transactionId": ...,
}

parent.commit_transaction(**kwargs)
```

1. See [:material-code-braces: CommitTransactionRequestTypeDef](./type_defs.md#committransactionrequesttypedef) 

### execute\_sql

Runs one or more SQL statements.

Type annotations and code completion for `#!python session.create_client("rds-data").execute_sql` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data/client/execute_sql.html)

```python
# execute_sql method definition

await def execute_sql(
    self,
    *,
    dbClusterOrInstanceArn: str,
    awsSecretStoreArn: str,
    sqlStatements: str,
    database: str = ...,
    schema: str = ...,
) -> ExecuteSqlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExecuteSqlResponseTypeDef](./type_defs.md#executesqlresponsetypedef) 


```python
# execute_sql method usage example with argument unpacking

kwargs: ExecuteSqlRequestTypeDef = {  # (1)
    "dbClusterOrInstanceArn": ...,
    "awsSecretStoreArn": ...,
    "sqlStatements": ...,
}

parent.execute_sql(**kwargs)
```

1. See [:material-code-braces: ExecuteSqlRequestTypeDef](./type_defs.md#executesqlrequesttypedef) 

### execute\_statement

Runs a SQL statement against a database.

Type annotations and code completion for `#!python session.create_client("rds-data").execute_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data/client/execute_statement.html)

```python
# execute_statement method definition

await def execute_statement(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    sql: str,
    database: str = ...,
    schema: str = ...,
    parameters: Sequence[SqlParameterTypeDef] = ...,  # (1)
    transactionId: str = ...,
    includeResultMetadata: bool = ...,
    continueAfterTimeout: bool = ...,
    resultSetOptions: ResultSetOptionsTypeDef = ...,  # (2)
    formatRecordsAs: RecordsFormatTypeType = ...,  # (3)
) -> ExecuteStatementResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
2. See [:material-code-braces: ResultSetOptionsTypeDef](./type_defs.md#resultsetoptionstypedef) 
3. See [:material-code-brackets: RecordsFormatTypeType](./literals.md#recordsformattypetype) 
4. See [:material-code-braces: ExecuteStatementResponseTypeDef](./type_defs.md#executestatementresponsetypedef) 


```python
# execute_statement method usage example with argument unpacking

kwargs: ExecuteStatementRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
    "sql": ...,
}

parent.execute_statement(**kwargs)
```

1. See [:material-code-braces: ExecuteStatementRequestTypeDef](./type_defs.md#executestatementrequesttypedef) 

### rollback\_transaction

Performs a rollback of a transaction.

Type annotations and code completion for `#!python session.create_client("rds-data").rollback_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data/client/rollback_transaction.html)

```python
# rollback_transaction method definition

await def rollback_transaction(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    transactionId: str,
) -> RollbackTransactionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RollbackTransactionResponseTypeDef](./type_defs.md#rollbacktransactionresponsetypedef) 


```python
# rollback_transaction method usage example with argument unpacking

kwargs: RollbackTransactionRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
    "transactionId": ...,
}

parent.rollback_transaction(**kwargs)
```

1. See [:material-code-braces: RollbackTransactionRequestTypeDef](./type_defs.md#rollbacktransactionrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("rds-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("rds-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client)

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





