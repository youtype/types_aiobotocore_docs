# Examples

> [Index](../README.md) > [DynamoDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#dynamodb)
    type annotations stubs module [types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[dynamodb]` package installed.

Write your `DynamoDB` code as usual,
type checking and code completion should work out of the box.



```python
# DynamoDBClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dynamodb") as client:  # (1)
    result = await client.batch_execute_statement()  # (2)
```

1. client: [DynamoDBClient](./client.md)
2. result: [:material-code-braces: BatchExecuteStatementOutputTypeDef](./type_defs.md#batchexecutestatementoutputtypedef) 



```python
# ListBackupsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dynamodb") as client:  # (1)
    paginator = client.get_paginator("list_backups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DynamoDBClient](./client.md)
2. paginator: [ListBackupsPaginator](./paginators.md#listbackupspaginator)
3. item: [:material-code-braces: ListBackupsOutputTypeDef](./type_defs.md#listbackupsoutputtypedef) 



```python
# TableExistsWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dynamodb") as client:  # (1)
    waiter = client.get_waiter("table_exists")  # (2)
    await waiter.wait()
```

1. client: [DynamoDBClient](./client.md)
2. waiter: [TableExistsWaiter](./waiters.md#tableexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[dynamodb]`
or a standalone `types_aiobotocore_dynamodb` package, you have to explicitly specify
`client: DynamoDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DynamoDBClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.client import DynamoDBClient
from types_aiobotocore_dynamodb.type_defs import BatchExecuteStatementOutputTypeDef
from types_aiobotocore_dynamodb.type_defs import BatchExecuteStatementInputTypeDef


session = get_session()

async with session.create_client("dynamodb") as client:
    client: DynamoDBClient
    kwargs: BatchExecuteStatementInputTypeDef = {...}
    result: BatchExecuteStatementOutputTypeDef = await client.batch_execute_statement(**kwargs)
```



```python
# ListBackupsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.client import DynamoDBClient
from types_aiobotocore_dynamodb.paginator import ListBackupsPaginator
from types_aiobotocore_dynamodb.type_defs import ListBackupsOutputTypeDef


session = get_session()

async with session.create_client("dynamodb") as client:
    client: DynamoDBClient
    paginator: ListBackupsPaginator = client.get_paginator("list_backups")
    async for item in paginator.paginate(...):
        item: ListBackupsOutputTypeDef
        print(item)
```



```python
# TableExistsWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.client import DynamoDBClient
from types_aiobotocore_dynamodb.waiter import TableExistsWaiter


session = get_session()

async with session.create_client("dynamodb") as client:
    client: DynamoDBClient
    waiter: TableExistsWaiter = client.get_waiter("table_exists")
    await waiter.wait()
```
